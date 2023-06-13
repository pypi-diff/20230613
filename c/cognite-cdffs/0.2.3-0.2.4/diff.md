# Comparing `tmp/cognite_cdffs-0.2.3.tar.gz` & `tmp/cognite_cdffs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_cdffs-0.2.3.tar", max compression
+gzip compressed data, was "cognite_cdffs-0.2.4.tar", max compression
```

## Comparing `cognite_cdffs-0.2.3.tar` & `cognite_cdffs-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2423 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/README.md
--rw-r--r--   0        0        0      205 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/__init__.py
--rw-r--r--   0        0        0     3907 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/credentials.py
--rw-r--r--   0        0        0     3134 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/file_handler.py
--rw-r--r--   0        0        0    26358 2023-05-25 10:04:47.537252 cognite_cdffs-0.2.3/cognite/cdffs/spec.py
--rw-r--r--   0        0        0     1638 2023-05-25 10:04:47.541252 cognite_cdffs-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.3/setup.py
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2423 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/README.md
+-rw-r--r--   0        0        0      205 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/__init__.py
+-rw-r--r--   0        0        0     3907 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/credentials.py
+-rw-r--r--   0        0        0     3134 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/file_handler.py
+-rw-r--r--   0        0        0    28003 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/spec.py
+-rw-r--r--   0        0        0     1663 2023-06-13 10:14:31.999285 cognite_cdffs-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.4/setup.py
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.4/PKG-INFO
```

### Comparing `cognite_cdffs-0.2.3/README.md` & `cognite_cdffs-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.3/cognite/cdffs/credentials.py` & `cognite_cdffs-0.2.4/cognite/cdffs/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.3/cognite/cdffs/file_handler.py` & `cognite_cdffs-0.2.4/cognite/cdffs/file_handler.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.3/cognite/cdffs/spec.py` & `cognite_cdffs-0.2.4/cognite/cdffs/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     Attributes:
         protocol (str): (class attribute) Protocol name to use when interacting with CDF Files.
         cdf_list_cache (Dict): Cache the file list results from CDF.
         cdf_list_expiry_time (int): Expiry time in seconds to invalidate the file list cache.
         file_metadata (FileMetadata): File Metadata that a user can use when reading/writing the files to CDF.
         file_cache (Dict): Cache the contents of the files.
         file_handler (FileHandler): File handler to manage the requests to a cloud storage.
+        max_download_retries (int): Maximum number of download retries allowed before exhausting.
+        download_retries (bool): Flag to indicate enable/disable download retries.
     """
 
     protocol: str = "cdffs"
 
     def __init__(
         self,
         connection_config: Optional[ClientConfig] = None,
@@ -68,14 +70,16 @@
         super().__init__(**kwargs)
         if isinstance(file_metadata, FileMetadata):
             self.file_metadata: FileMetadata = file_metadata
         else:
             raise ValueError("User must provide a valid 'file_metadata' in storage_options")
         self.cdf_list_cache: Dict[str, float] = {}
         self.cdf_list_expiry_time: int = kwargs.get("cdf_list_expiry_time", 60)  # type: ignore
+        self.max_download_retries: int = kwargs.get("max_download_retries", 5)  # type: ignore
+        self.download_retries: bool = kwargs.get("download_retries", True)  # type: ignore
         self.file_cache: Dict[str, Dict[str, Any]] = {}
         self.file_handler: FileHandler = FileHandler()
 
         # Create a connection to Cdf
         self.do_connect(connection_config, **kwargs)
 
     @classmethod
@@ -328,23 +332,58 @@
     def rm_file(self, path: str) -> None:
         """Remove the file at a given path.
 
         Args:
             path (str): Path to use to remove the file.
 
         Raises:
-            NotImplementedError: Error as it is not supported.
+            FileNotFoundError: When a file is not found.
         """
         _, external_id_prefix, _ = self.split_path(path, validate_suffix=False)
         if external_id_prefix:
             try:
                 self.cognite_client.files.delete(external_id=external_id_prefix)
             except CogniteNotFoundError as cognite_exp:
                 raise FileNotFoundError from cognite_exp
 
+    def rm_files(self, paths: List) -> None:
+        """Remove the list of files.
+
+        Args:
+            paths (List): List of files to remove.
+
+        Raises:
+            FileNotFoundError: When a file is not found.
+        """
+        validated_external_ids = []
+        # Validate the external ids before attempting to remove them
+        for path in paths:
+            _, external_id_prefix, _ = self.split_path(path, validate_suffix=False)
+            if external_id_prefix:
+                validated_external_ids.append(external_id_prefix)
+
+        # Delete only if the external ids are valid.
+        if validated_external_ids:
+            try:
+                self.cognite_client.files.delete(external_id=validated_external_ids)
+            except CogniteNotFoundError as cognite_exp:
+                raise FileNotFoundError from cognite_exp
+
+    def exists(self, path: str) -> bool:
+        """Check if the file exists at the given path.
+
+        Args:
+            path (str): Absolute path to check.
+
+        Returns:
+            bool: True/False to indicate if the file exists.
+        """
+        _, _, external_id = self.split_path(path, validate_suffix=False)
+        return bool(self.cognite_client.files.retrieve(external_id=external_id)) if external_id else False
+
     def mv(
         self,
         source_path: str,
         destination_path: str,
         recursive: bool = False,
         maxdepth: Union[int, None] = None,
         **kwargs: Optional[Any],
@@ -424,26 +463,25 @@
             bytes: File contents as is from a cloud storage.
 
         Raises:
             FileNotFoundError: When there is no file matching the external_id given.
         """
         _download_retries = 0
         _retry_wait_seconds = 0.5
-        _download_max_retries = 5
         while True:
             try:
                 if not (download_url := self.file_handler.get_url(external_id)):
                     url_dict = self.cognite_client.files.retrieve_download_urls(external_id=external_id)
                     download_url = url_dict[external_id]
                     self.file_handler.add_or_update_url(external_id, download_url)
 
                 return self.file_handler.download_file(download_url, start_byte, end_byte)
 
             except (CogniteAPIError, FileException) as cognite_exp:
-                if _download_retries < _download_max_retries:
+                if self.download_retries and _download_retries < self.max_download_retries:
                     _download_retries += 1
                     time.sleep(_retry_wait_seconds)
                     _retry_wait_seconds *= 2
                     continue
 
                 raise FileNotFoundError from cognite_exp
 
@@ -625,8 +663,9 @@
             bytes: Subset of file contents.
         """
         if self.all_bytes_caching:
             cache = self.fs._fetch_file(self.external_id)
             file_contents = cache._fetch(start, end)
         else:
             file_contents = self.fs.read_file(self.external_id, start_byte=start, end_byte=end)
+
         return file_contents
```

### Comparing `cognite_cdffs-0.2.3/pyproject.toml` & `cognite_cdffs-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "cognite-cdffs"
-version = "0.2.3"
+version = "0.2.4"
 description = "File System Interface for CDF Files"
 license = "Apache-2.0"
 authors = ["Infant Alex <infant.alex@cognite.com>"]
 readme = "README.md"
 packages = [
     { include="cognite", from="." },
 ]
 [tool.poetry.group.test.dependencies]
 pandas = "^1.5.1"
-geopandas = "^0.13.0"
 pyarrow = "^12.0.0"
 zarr = "^2.13.3"
-dask = "^2023.5.0"
+dask = "^2023.6.0"
 xarray = "^2023.5.0"
+geodatasets = "^2023.3.0"
+geopandas = "^0.13.2"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.28.11.5"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 responses = "^0.23.1"
 flake8 = "6.0.0"
 pre-commit = "^3.2.2"
 flake8-pyproject = "^1.2.3"
 twine = "^4.0.2"
 toml = "^0.10.2"
-sphinx-rtd-theme = "^1.2.1"
+sphinx-rtd-theme = "^1.2.2"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
 include = '\.py$'
 
 [tool.flake8]
@@ -63,19 +64,19 @@
 commands =
     coverage run --source cognite -m pytest -v tests
     coverage xml
 """
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
-cognite-sdk = "^6.1.10"
-fsspec = "^2023.5.0"
+cognite-sdk = "^6.4.0"
+fsspec = "^2023.6.0"
 requests = "^2.31.0"
 twine = "^4.0.2"
-pydantic = "^1.10.8"
+pydantic = "^1.10.9"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cognite_cdffs-0.2.3/setup.py` & `cognite_cdffs-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 packages = \
 ['cognite', 'cognite.cdffs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cognite-sdk>=6.1.10,<7.0.0',
- 'fsspec>=2023.5.0,<2024.0.0',
- 'pydantic>=1.10.8,<2.0.0',
+['cognite-sdk>=6.4.0,<7.0.0',
+ 'fsspec>=2023.6.0,<2024.0.0',
+ 'pydantic>=1.10.9,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'requests>=2.31.0,<3.0.0',
  'twine>=4.0.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'cognite-cdffs',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'File System Interface for CDF Files',
     'long_description': '<a href="https://cognite.com/">\n  <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">\n</a>\n\n[![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/badge.svg)](https://codecov.io/gh/cognitedata/cdffs)\n![PyPI](https://img.shields.io/pypi/v/cognite-cdffs)\n\n# cdffs\n\nA file system interface (`cdffs`) to allow users to work with CDF Files using the [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) supported/compatible python packages (`pandas`, `xarray` etc).\n\n`fsspec` provides an abstract file system interface to work with local/cloud storages and based on the protocol name (example, `s3` or `abfs`) provided in the path, `fsspec` translates the incoming requests to storage specific implementations and send the responses back to the upstream package to work with the desired data.\n\nRefer [fsspec documentation](https://filesystem-spec.readthedocs.io/en/latest/#who-uses-fsspec) to get the list of all supported/compatible python packages.\n\n## Installation\n\n`cdffs` is available on PyPI. Install using,\n\n```shell\npip install cognite-cdffs\n```\n\n## Usage\n\nImportant steps to follow when working with CDF Files using the `fsspec` supported python packages.\n\n1) Import `cdffs` package\n```python\n  from cognite import cdffs  # noqa\n```\n\n2) Follow instructions from [Authentication](https://cdffs.readthedocs.io/en/latest/authentication.html) to authenticate.\n\n3) Read/write the files from/to CDF using `fsspec` supported packages. Example,\n\n    * Read `zarr` files using using `xarray`.\n\n    ```python\n    ds = xarray.open_zarr("cdffs://sample_data/test.zarr")\n    ```\n    * Write `zarr` files using `xarray`.\n\n    ```python\n    ds.to_zarr("cdffs://sample_data/test.zarr", storage_options={"file_metadata": metadata})\n    ```\n\nRefer [cdffs.readthedocs.io](https://cdffs.readthedocs.io) for more details.\n\n## Contributing\nWant to contribute? Check out [CONTRIBUTING](CONTRIBUTING.md).\n',
     'author': 'Infant Alex',
     'author_email': 'infant.alex@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
 packages = \ ['cognite', 'cognite.cdffs'] package_data = \ {'': ['*']}
-install_requires = \ ['cognite-sdk>=6.1.10,<7.0.0',
-'fsspec>=2023.5.0,<2024.0.0', 'pydantic>=1.10.8,<2.0.0', 'python-
+install_requires = \ ['cognite-sdk>=6.4.0,<7.0.0',
+'fsspec>=2023.6.0,<2024.0.0', 'pydantic>=1.10.9,<2.0.0', 'python-
 dotenv>=1.0.0,<2.0.0', 'requests>=2.31.0,<3.0.0', 'twine>=4.0.2,<5.0.0']
-setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.3', 'description':
+setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.4', 'description':
 'File System Interface for CDF Files', 'long_description': '\n_[Cognite]\n\n\n
 [![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://
 github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status]
 (https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

### Comparing `cognite_cdffs-0.2.3/PKG-INFO` & `cognite_cdffs-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cognite-cdffs
-Version: 0.2.3
+Version: 0.2.4
 Summary: File System Interface for CDF Files
 License: Apache-2.0
 Author: Infant Alex
 Author-email: infant.alex@cognite.com
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cognite-sdk (>=6.1.10,<7.0.0)
-Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: cognite-sdk (>=6.4.0,<7.0.0)
+Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://cognite.com/">
   <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.3 Summary: File System
+Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.4 Summary: File System
 Interface for CDF Files License: Apache-2.0 Author: Infant Alex Author-email:
 infant.alex@cognite.com Requires-Python: >=3.9.10,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: cognite-sdk
-(>=6.1.10,<7.0.0) Requires-Dist: fsspec (>=2023.5.0,<2024.0.0) Requires-Dist:
-pydantic (>=1.10.8,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+(>=6.4.0,<7.0.0) Requires-Dist: fsspec (>=2023.6.0,<2024.0.0) Requires-Dist:
+pydantic (>=1.10.9,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: twine (>=4.0.2,<5.0.0)
 Description-Content-Type: text/markdown [Cognite] [![GitHub](https://
 img.shields.io/github/license/cognitedata/cdffs)](https://github.com/
 cognitedata/cdffs/blob/main/LICENSE) [![Documentation Status](https://
 readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
```

