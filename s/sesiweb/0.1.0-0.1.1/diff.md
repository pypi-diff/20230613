# Comparing `tmp/sesiweb-0.1.0.tar.gz` & `tmp/sesiweb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesiweb-0.1.0.tar", last modified: Mon Apr  3 02:04:07 2023, max compression
+gzip compressed data, was "sesiweb-0.1.1.tar", last modified: Tue Jun 13 12:41:15 2023, max compression
```

## Comparing `sesiweb-0.1.0.tar` & `sesiweb-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.489387 sesiweb-0.1.0/
--rw-r--r--   0 aaronsmith   (501) staff       (20)     1067 2023-04-02 16:45:28.000000 sesiweb-0.1.0/LICENSE
--rw-r--r--   0 aaronsmith   (501) staff       (20)     4873 2023-04-03 02:04:07.489169 sesiweb-0.1.0/PKG-INFO
--rw-r--r--   0 aaronsmith   (501) staff       (20)     2846 2023-04-03 01:56:15.000000 sesiweb-0.1.0/README.md
--rw-r--r--   0 aaronsmith   (501) staff       (20)     1078 2023-04-03 01:58:03.000000 sesiweb-0.1.0/pyproject.toml
--rw-r--r--   0 aaronsmith   (501) staff       (20)       38 2023-04-03 02:04:07.489450 sesiweb-0.1.0/setup.cfg
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.484605 sesiweb-0.1.0/src/
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.486373 sesiweb-0.1.0/src/sesiweb/
--rw-r--r--   0 aaronsmith   (501) staff       (20)       50 2023-04-03 01:30:18.000000 sesiweb-0.1.0/src/sesiweb/__init__.py
--rw-r--r--   0 aaronsmith   (501) staff       (20)      736 2023-04-02 20:12:11.000000 sesiweb-0.1.0/src/sesiweb/exceptions.py
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.488313 sesiweb-0.1.0/src/sesiweb/model/
--rw-r--r--   0 aaronsmith   (501) staff       (20)        0 2023-04-02 16:56:16.000000 sesiweb-0.1.0/src/sesiweb/model/__init__.py
--rw-r--r--   0 aaronsmith   (501) staff       (20)      511 2023-04-02 20:11:12.000000 sesiweb-0.1.0/src/sesiweb/model/file.py
--rw-r--r--   0 aaronsmith   (501) staff       (20)     3915 2023-04-02 23:30:43.000000 sesiweb-0.1.0/src/sesiweb/model/service.py
--rw-r--r--   0 aaronsmith   (501) staff       (20)    10332 2023-04-03 01:41:08.000000 sesiweb-0.1.0/src/sesiweb/webapi.py
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.487579 sesiweb-0.1.0/src/sesiweb.egg-info/
--rw-r--r--   0 aaronsmith   (501) staff       (20)     4873 2023-04-03 02:04:07.000000 sesiweb-0.1.0/src/sesiweb.egg-info/PKG-INFO
--rw-r--r--   0 aaronsmith   (501) staff       (20)      385 2023-04-03 02:04:07.000000 sesiweb-0.1.0/src/sesiweb.egg-info/SOURCES.txt
--rw-r--r--   0 aaronsmith   (501) staff       (20)        1 2023-04-03 02:04:07.000000 sesiweb-0.1.0/src/sesiweb.egg-info/dependency_links.txt
--rw-r--r--   0 aaronsmith   (501) staff       (20)       72 2023-04-03 02:04:07.000000 sesiweb-0.1.0/src/sesiweb.egg-info/requires.txt
--rw-r--r--   0 aaronsmith   (501) staff       (20)        8 2023-04-03 02:04:07.000000 sesiweb-0.1.0/src/sesiweb.egg-info/top_level.txt
-drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-04-03 02:04:07.488668 sesiweb-0.1.0/tests/
--rw-r--r--   0 aaronsmith   (501) staff       (20)     1569 2023-04-03 01:38:11.000000 sesiweb-0.1.0/tests/test_sesiweb.py
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.483338 sesiweb-0.1.1/
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     1067 2023-04-02 16:45:28.000000 sesiweb-0.1.1/LICENSE
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     5792 2023-06-13 12:41:15.483141 sesiweb-0.1.1/PKG-INFO
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     3770 2023-04-03 17:30:28.000000 sesiweb-0.1.1/README.md
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     1113 2023-06-13 12:27:55.000000 sesiweb-0.1.1/pyproject.toml
+-rw-r--r--   0 aaronsmith   (501) staff       (20)       38 2023-06-13 12:41:15.483400 sesiweb-0.1.1/setup.cfg
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.479242 sesiweb-0.1.1/src/
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.480551 sesiweb-0.1.1/src/sesiweb/
+-rw-r--r--   0 aaronsmith   (501) staff       (20)       51 2023-04-08 19:58:01.000000 sesiweb-0.1.1/src/sesiweb/__init__.py
+-rw-r--r--   0 aaronsmith   (501) staff       (20)      738 2023-04-08 19:58:01.000000 sesiweb-0.1.1/src/sesiweb/exceptions.py
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.482479 sesiweb-0.1.1/src/sesiweb/model/
+-rw-r--r--   0 aaronsmith   (501) staff       (20)        0 2023-04-02 16:56:16.000000 sesiweb-0.1.1/src/sesiweb/model/__init__.py
+-rw-r--r--   0 aaronsmith   (501) staff       (20)      512 2023-04-08 19:58:01.000000 sesiweb-0.1.1/src/sesiweb/model/file.py
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     3926 2023-06-13 12:00:37.000000 sesiweb-0.1.1/src/sesiweb/model/service.py
+-rw-r--r--   0 aaronsmith   (501) staff       (20)    10378 2023-06-13 12:00:37.000000 sesiweb-0.1.1/src/sesiweb/webapi.py
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.481843 sesiweb-0.1.1/src/sesiweb.egg-info/
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     5792 2023-06-13 12:41:15.000000 sesiweb-0.1.1/src/sesiweb.egg-info/PKG-INFO
+-rw-r--r--   0 aaronsmith   (501) staff       (20)      385 2023-06-13 12:41:15.000000 sesiweb-0.1.1/src/sesiweb.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronsmith   (501) staff       (20)        1 2023-06-13 12:41:15.000000 sesiweb-0.1.1/src/sesiweb.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronsmith   (501) staff       (20)       80 2023-06-13 12:41:15.000000 sesiweb-0.1.1/src/sesiweb.egg-info/requires.txt
+-rw-r--r--   0 aaronsmith   (501) staff       (20)        8 2023-06-13 12:41:15.000000 sesiweb-0.1.1/src/sesiweb.egg-info/top_level.txt
+drwxr-xr-x   0 aaronsmith   (501) staff       (20)        0 2023-06-13 12:41:15.482817 sesiweb-0.1.1/tests/
+-rw-r--r--   0 aaronsmith   (501) staff       (20)     1507 2023-04-08 19:58:01.000000 sesiweb-0.1.1/tests/test_sesiweb.py
```

### Comparing `sesiweb-0.1.0/LICENSE` & `sesiweb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sesiweb-0.1.0/PKG-INFO` & `sesiweb-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesiweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unofficial driver for the SideFX Web API
 Author-email: Aaron Smith <aaron@aaronsmith.tv>
 License: MIT License
         
         Copyright (c) 2023 Aaron Smith
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/aaronsmithtv/sesiweb
-Project-URL: Bug Reports, https://github.com/pypa/aaronsmithtv/issues
+Project-URL: Bug Reports, https://github.com/aaronsmithtv/issues
 Project-URL: Source, https://github.com/aaronsmithtv/sesiweb/
 Keywords: sidefx,houdini,sesi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # <img src="https://static.sidefx.com/images/apple-touch-icon.png" width="25" height="25" alt="Hbuild Logo"> sesiweb
 
+[![](https://img.shields.io/pypi/v/sesiweb.svg?maxAge=3600)](https://pypi.org/project/sesiweb/)
 ![Test](https://github.com/aaronsmithtv/sesiweb/actions/workflows/test.yml/badge.svg)
 
 sesiweb is a Python module used as a synchronous driver for the SideFX Web API. It provides a simple interface to interact with the API and obtain data about Houdini product builds.
 
 Inputs are validated with Pydantic, and methods in sesiweb provide additional lookup functionality, exceptions, and models.
 
 ## Table of Contents
@@ -106,21 +107,32 @@
 )
 ```
 
 For more information on the SideFX Web API and the returned results you can filter by, refer to the [SideFX Web API documentation](https://www.sidefx.com/docs/api/).
 
 ## Acquiring a Build Download
 
-Using sesiweb, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
+Using sesiweb and Pydantic, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
 
-In the script below, 
+In the script below, the single latest daily development build (irrespective of version number) is acquired using `get_latest_build`. `get_build_download` is then used to return the download metadata for that build:
 
 ```python
-# Get the latest Houdini build (filtered)
-build = sw.get_latest_build(prodinfo=build, prodfilter=buildfilter)
+from sesiweb import SesiWeb
+from sesiweb.model.service import ProductBuild
+
+sesi_secret = "your_secret_key"
+sesi_id = "your_client_id"
+
+sw = SesiWeb(sesi_secret, sesi_id)
+
+# Get the most recent Houdini product builds
+build = {"product": "houdini", "platform": "linux"}
+
+# Get the latest Houdini build
+build = sw.get_latest_build(prodinfo=build, only_production=False)
 
 # Get the download URL, filename and hash of the build
 build_dl = sw.get_build_download(
 	prodinfo=ProductBuild(**build.dict())
 )
 
 print(build_dl)
@@ -128,10 +140,12 @@
 
 This will return a `BuildDownloadModel` object containing a download URL, build filename, and hash:
 
 ```shell
 download_url=AnyUrl('https://gjvnth38g.cloudfront.net/download/download-build/456223/cdn/?Expires=166636236...
 ```
 
+For an example of using this metadata in a purpose suitable for a production environment, see [autobuild.py](https://github.com/aaronsmithtv/Houdini-Docker/blob/main/hbuild/autobuild.py) in [Houdini-Docker](https://github.com/aaronsmithtv/Houdini-Docker); Where sesiweb build data is used to construct a Docker image using a custom Houdini installation process.
+
 ## License
 
 sesiweb is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `sesiweb-0.1.0/README.md` & `sesiweb-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # <img src="https://static.sidefx.com/images/apple-touch-icon.png" width="25" height="25" alt="Hbuild Logo"> sesiweb
 
+[![](https://img.shields.io/pypi/v/sesiweb.svg?maxAge=3600)](https://pypi.org/project/sesiweb/)
 ![Test](https://github.com/aaronsmithtv/sesiweb/actions/workflows/test.yml/badge.svg)
 
 sesiweb is a Python module used as a synchronous driver for the SideFX Web API. It provides a simple interface to interact with the API and obtain data about Houdini product builds.
 
 Inputs are validated with Pydantic, and methods in sesiweb provide additional lookup functionality, exceptions, and models.
 
 ## Table of Contents
@@ -64,21 +65,32 @@
 )
 ```
 
 For more information on the SideFX Web API and the returned results you can filter by, refer to the [SideFX Web API documentation](https://www.sidefx.com/docs/api/).
 
 ## Acquiring a Build Download
 
-Using sesiweb, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
+Using sesiweb and Pydantic, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
 
-In the script below, 
+In the script below, the single latest daily development build (irrespective of version number) is acquired using `get_latest_build`. `get_build_download` is then used to return the download metadata for that build:
 
 ```python
-# Get the latest Houdini build (filtered)
-build = sw.get_latest_build(prodinfo=build, prodfilter=buildfilter)
+from sesiweb import SesiWeb
+from sesiweb.model.service import ProductBuild
+
+sesi_secret = "your_secret_key"
+sesi_id = "your_client_id"
+
+sw = SesiWeb(sesi_secret, sesi_id)
+
+# Get the most recent Houdini product builds
+build = {"product": "houdini", "platform": "linux"}
+
+# Get the latest Houdini build
+build = sw.get_latest_build(prodinfo=build, only_production=False)
 
 # Get the download URL, filename and hash of the build
 build_dl = sw.get_build_download(
 	prodinfo=ProductBuild(**build.dict())
 )
 
 print(build_dl)
@@ -86,10 +98,12 @@
 
 This will return a `BuildDownloadModel` object containing a download URL, build filename, and hash:
 
 ```shell
 download_url=AnyUrl('https://gjvnth38g.cloudfront.net/download/download-build/456223/cdn/?Expires=166636236...
 ```
 
+For an example of using this metadata in a purpose suitable for a production environment, see [autobuild.py](https://github.com/aaronsmithtv/Houdini-Docker/blob/main/hbuild/autobuild.py) in [Houdini-Docker](https://github.com/aaronsmithtv/Houdini-Docker); Where sesiweb build data is used to construct a Docker image using a custom Houdini installation process.
+
 ## License
 
 sesiweb is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `sesiweb-0.1.0/pyproject.toml` & `sesiweb-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sesiweb"
-version = "0.1.0"
+version = "0.1.1"
 description = "Unofficial driver for the SideFX Web API"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["sidefx", "houdini", "sesi"]
 
 authors = [
@@ -18,29 +18,32 @@
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "requests",
-    "urllib3",
+    "urllib3==1.26.5",
     "pydantic"
 ]
 
 [project.optional-dependencies]
 dev = ["check-manifest"]
 test = [
     "pytest",
     "coverage",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/aaronsmithtv/sesiweb"
-"Bug Reports" = "https://github.com/pypa/aaronsmithtv/issues"
+"Bug Reports" = "https://github.com/aaronsmithtv/issues"
 "Source" = "https://github.com/aaronsmithtv/sesiweb/"
 
 [tool.setuptools]
 package-data = {"sample" = ["*.dat"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.isort]
+profile = "black"
```

### Comparing `sesiweb-0.1.0/src/sesiweb/exceptions.py` & `sesiweb-0.1.1/src/sesiweb/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class APIError(Exception):
     """SideFX Web API error
 
     Raised from the client if the server generated an error while calling
     into the API.
     """
+
     def __init__(self, http_code, message, response=None):
         super(APIError, self).__init__(message)
         self.http_code = http_code
         self.response = response
 
     def __str__(self):
         return "%s %s" % (self.http_code, self.args[0])
@@ -15,10 +16,11 @@
 
 class AuthorizationError(Exception):
     """SideFX client authentication error
 
     Raised from the client if the server generated an error while generating
     an access token.
     """
+
     def __init__(self, http_code, message):
         super(AuthorizationError, self).__init__(message)
         self.http_code = http_code
```

### Comparing `sesiweb-0.1.0/src/sesiweb/model/service.py` & `sesiweb-0.1.1/src/sesiweb/model/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 
 from pydantic import AnyUrl, BaseModel
 
 
 class ProductModel(BaseModel):
     """Base product build class for SideFX Web API.
 
@@ -11,27 +11,29 @@
             following values: `'houdini', 'houdini-py3', 'houdini-py37',
             'houdini-py2', 'docker', 'sidefxlabs', 'houdini-launcher',
             'houdini-launcher-py3', 'houdini-launcher-py37', 'launcher-iso',
             'launcher-iso-py3', 'launcher-iso-py37', 'launcher-iso-py2'`
         platform (str): The operating system to install Houdini on: `'win64', 'macos',
             'macosx_arm64', 'linux'`. Does not effect Docker and SideFXLabs builds.
     """
+
     product: str
     platform: str
 
 
 class ProductBuild(ProductModel):
     """A full product with build and version num, based on ProductModel.
 
     Attributes:
         product (str): The product name, e.g. `'houdini'`.
         platform (str): The platform name, e.g. `'linux'`.
         version (Optional[str]): A product version, e.g. `'17.0'`.
         build (Optional[str]): A product build, e.g. `'382'`.
     """
+
     version: Optional[str]
     build: Optional[str]
 
 
 class DailyBuild(ProductBuild):
     """A web API return model, with date, release, status metadata appended.
 
@@ -40,14 +42,15 @@
         platform (str): The platform name, e.g. `'linux'`.
         version (Optional[str]): A product version, e.g. `'17.0'`.
         build (Optional[str]): A product build, e.g. `'382'`.
         date (str): The date the build was introduced, in `'YYYY/MM/DD'` format.
         release (str): The type of release the build is tagged with, e.g.`'gold'`.
         status (str): The condition of the build, e.g. `'good'`.
     """
+
     date: str
     release: str
     status: str
 
     class Config:
         schema_extra = {
             "example": {
@@ -66,14 +69,15 @@
     """Download & installation metadata for a returned build.
 
     Attributes:
         download_url (AnyUrl): A cloudfront URL to download the build from.
         filename (str): A filename for the downloadable binary.
         hash (str): A hash for the downloadable binary.
     """
+
     download_url: AnyUrl
     filename: str
     hash: str
 
 
 class BuildDownloadModel(InstallBuild):
     """Full download metadata with build status, size and date introduced
@@ -83,14 +87,15 @@
         filename (str): A filename for the downloadable binary.
         hash (str): A hash for the downloadable binary.
         date (str): The date the build was introduced, in `'YYYY/MM/DD'` format.
         releases_list (str): The type of release the build is tagged with, e.g.`'gold'`.
         status (str): The condition of the build, e.g. `'good'`.
         size (int): The integer filesize of the download in bytes.
     """
+
     date: str
     releases_list: str
     status: str
     size: int
 
     class Config:
         schema_extra = {
@@ -110,9 +115,9 @@
     server_name: str
     server_code: str
     version: str
     products: str
 
 
 class LicenseModel(BaseModel):
-    license_keys: list[str]
+    license_keys: List[str]
     server_key: str
```

### Comparing `sesiweb-0.1.0/src/sesiweb/webapi.py` & `sesiweb-0.1.1/src/sesiweb/webapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import base64
 import html
 import json
 import time
-from typing import Any, AnyStr, Optional
+from typing import Any, AnyStr, Dict, List, Optional, Union
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .exceptions import APIError, AuthorizationError
 from .model.file import ResponseFile
-from .model.service import (BuildDownloadModel, DailyBuild, HServerModel,
-                            LicenseModel, ProductBuild, ProductModel)
+from .model.service import (
+    BuildDownloadModel,
+    DailyBuild,
+    HServerModel,
+    LicenseModel,
+    ProductBuild,
+    ProductModel,
+)
 
 
 class SesiWeb:
     """Http client for SideFX Web API
 
     Opens a synchronous requests http session for the SideFX Web API. A full
     length access token is created in the __init__ method, from the input
@@ -30,68 +36,73 @@
         access_token_url (str): The oauth2 application token url, default:
             `https://www.sidefx.com/oauth2/application_token`
         access_token (str): The constructed access token from client_id and
             client_secret, for the SideFX Web API app oauth2 process.
         expiry_time (str): The expiration time of the access token.
 
     """
-    def __init__(self, client_id: str, client_secret: str):
+
+    def __init__(self, client_id: str, client_secret: str) -> None:
         """Construct http session and access token
 
         Args:
             client_id (str): SideFX Application client id
             client_secret (str): SideFX Application secret key
         """
         self.session = get_session()
         self.endpoint_url = "https://www.sidefx.com/api/"
         self.access_token_url = "https://www.sidefx.com/oauth2/application_token"
         self.access_token, self.expiry_time = get_access_token(
             access_token_url=self.access_token_url,
             client_secret_key=client_secret,
-            client_id=client_id
+            client_id=client_id,
         )
 
     def get_latest_builds(
-            self, prodinfo: ProductModel | dict,
-            only_production: Optional[bool] = True,
-            prodfilter: Optional[dict] = None) -> list[DailyBuild]:
+        self,
+        prodinfo: Union[ProductModel, dict],
+        only_production: bool = True,
+        prodfilter: Optional[dict] = None,
+    ) -> List[DailyBuild]:
         """List all latest SideFX product builds, with metadata
 
         Args:
             prodinfo (ProductModel | dict): The input product and platform data,
                 (e.g houdini & linux).
-            only_production (Optional[bool]): Whether builds are daily (False)
-                or production (True), default: True
+            only_production (bool): Whether builds are daily (False) or production
+                (True), default: True
             prodfilter (Optional[dict]): An optional filter for the results of
                 latest builds. Accepted keys are `'build', 'date',
                 'release', 'status', 'version'`.
 
         Returns:
             list[DailyBuild]: A list of builds, with returned metadata for each
                 build.
         """
         api_command = "download.get_daily_builds_list"
 
         build_dict = dict(prodinfo)
-        build_dict.update({'only_production': only_production})
+        build_dict.update({"only_production": only_production})
 
-        post_data = dict(json=json.dumps([api_command, [], build_dict]))
+        post_data = {"json": json.dumps([api_command, [], build_dict])}
         resp_builds = self.get_session_response(post_data)
 
-        if prodfilter:
+        if prodfilter is not None:
             resp_builds = filter_list_response(resp_builds, prodfilter)
 
         builds = [DailyBuild.parse_obj(resp_build) for resp_build in resp_builds]
 
         return builds
 
     def get_latest_build(
-            self, prodinfo: ProductModel | dict,
-            only_production: Optional[bool] = True,
-            prodfilter: Optional[dict] = None) -> DailyBuild:
+        self,
+        prodinfo: Union[ProductModel, dict],
+        only_production: bool = True,
+        prodfilter: Optional[dict] = None,
+    ) -> DailyBuild:
         """Single return method for get_latest_builds
 
         Args:
             prodinfo (ProductModel | dict): The input product and platform data,
                 (e.g houdini & linux).
             only_production (Optional[bool]): Whether builds are daily (False)
                 or production (True), default: True
@@ -101,28 +112,29 @@
 
         Returns:
             list[DailyBuild]: A list of builds
         """
         return self.get_latest_builds(prodinfo, only_production, prodfilter)[0]
 
     def get_build_download(
-            self, prodinfo: ProductBuild | dict) -> BuildDownloadModel:
+        self, prodinfo: Union[ProductBuild, dict]
+    ) -> BuildDownloadModel:
         """Using ProductBuild object data, get download info for the build
 
         Args:
             prodinfo (ProductBuild | dict): Info based on the appropriate
                 product, build and version.
 
         Returns:
             BuildDownloadModel: Download, hash and filename data.
         """
         api_command = "download.get_daily_build_download"
 
         build_dict = dict(prodinfo)
-        post_data = dict(json=json.dumps([api_command, [], build_dict]))
+        post_data = {"json": json.dumps([api_command, [], build_dict])}
         resp_build = self.get_session_response(post_data)
         build_dl = BuildDownloadModel.parse_obj(resp_build)
         return build_dl
 
     def get_nc_license(self, srvinfo: HServerModel):
         """Generate a non-commercial license key
 
@@ -138,64 +150,64 @@
         build_dict = dict(srvinfo)
         post_data = dict(json=json.dumps([api_command, [], build_dict]))
         resp_build = self.get_session_response(post_data)
         build_dl = LicenseModel.parse_obj(resp_build)
         return build_dl
 
     def get_session_response(
-            self, post_data: dict[str, Any],
-            timeout: Optional[int] = None) -> Any:
+        self, post_data: Dict[str, Any], timeout: Optional[int] = None
+    ) -> Any:
         """Get an appropriate response from constructed requests session.
 
         Args:
             post_data (dict[str, Any]): SideFX Web API POST request data
             timeout (Optional[int]): Optional timeout length, default: None
 
         Returns:
             Any: Session response.
         """
         response = self.session.post(
             self.endpoint_url,
-            headers={"Authorization": "Bearer " + self.access_token},
+            headers={"Authorization": f"Bearer {self.access_token}"},
             data=post_data,
-            timeout=timeout)
+            timeout=timeout,
+        )
         if response.status_code == 200:
             if response.headers.get("Content-Type") == "application/octet-stream":
                 return ResponseFile(response)
             return response.json()
 
-        raise APIError(
-            response.status_code,
-            extract_traceback(response))
+        raise APIError(response.status_code, extract_traceback(response))
 
 
 def get_session() -> requests.Session:
     """Get a requests http session
 
     Returns:
         requests.Session: A http session
     """
     retry_strategy = Retry(
         total=3,
-        status_forcelist=[429, ],
+        status_forcelist=[429],
         method_whitelist=["GET", "POST"],
         backoff_factor=1,
     )
     adapter = HTTPAdapter(max_retries=retry_strategy)
     http = requests.Session()
     http.mount("https://", adapter)
     http.mount("http://", adapter)
     return http
 
 
 def get_access_token(
-        client_id: str,
-        client_secret_key: str,
-        access_token_url: str,
-        timeout: Optional[int] = None) -> (AnyStr, AnyStr):
+    client_id: str,
+    client_secret_key: str,
+    access_token_url: str,
+    timeout: Optional[int] = None,
+) -> (AnyStr, AnyStr):
     """Construct the access token for API requests
 
     Given an API client (id and secret key) that is allowed to make API
     calls, return an access token that can be used to make calls.
 
     If request is made using the /token URL directly then assume the app a
     client-credentials based application.
@@ -219,15 +231,16 @@
 
     response = requests.post(
         access_token_url,
         headers={
             "Authorization": f"Basic {base64.b64encode(auth_header).decode('utf-8')}",
         },
         data=post_data,
-        timeout=timeout)
+        timeout=timeout,
+    )
 
     if response.status_code != 200:
         status_msg = f"{response.status_code}: {extract_traceback(response)}"
         raise AuthorizationError(response.status_code, status_msg)
 
     response_json = response.json()
     access_token_expiry_time = time.time() - 2 + response_json["expires_in"]
@@ -261,36 +274,35 @@
 
     if traceback:
         traceback = error_message
 
     return html.unescape(traceback)
 
 
-def without_keys(d: dict, keys: list[str]) -> dict:
+def without_keys(dictionary: dict, keys_to_remove: List[str]) -> dict:
     """Return a dict without keys specified in list
 
     Args:
-        d (dict): Dict to remove keys from
-        keys (list[str]): Keys to remove
+        dictionary (dict): Dict to remove keys from
+        keys_to_remove (list[str]): Keys to remove
 
     Returns:
         dict: Original dict with removed keys
     """
-    return {k: d[k] for k in d.keys() - keys}
+    return {key: dictionary[key] for key in dictionary.keys() - keys_to_remove}
 
 
-def filter_list_response(results: list[dict], resfilter: dict) -> list[dict]:
+def filter_list_response(results: List[dict], resfilter: dict) -> List[dict]:
     """Returns a filtered dict array
 
     Args:
         results (list[dict]): A list of dict objects to filter
         resfilter (dict): Key/value pairs to filter by
 
     Returns:
         list[dict]:
     """
+
     def filter_func(d):
-        return all(
-            d[k] == v if k in d else KeyError() for k, v in resfilter.items()
-        )
+        return all(d[k] == v if k in d else KeyError() for k, v in resfilter.items())
 
     return list(filter(filter_func, results))
```

### Comparing `sesiweb-0.1.0/src/sesiweb.egg-info/PKG-INFO` & `sesiweb-0.1.1/src/sesiweb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesiweb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unofficial driver for the SideFX Web API
 Author-email: Aaron Smith <aaron@aaronsmith.tv>
 License: MIT License
         
         Copyright (c) 2023 Aaron Smith
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/aaronsmithtv/sesiweb
-Project-URL: Bug Reports, https://github.com/pypa/aaronsmithtv/issues
+Project-URL: Bug Reports, https://github.com/aaronsmithtv/issues
 Project-URL: Source, https://github.com/aaronsmithtv/sesiweb/
 Keywords: sidefx,houdini,sesi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # <img src="https://static.sidefx.com/images/apple-touch-icon.png" width="25" height="25" alt="Hbuild Logo"> sesiweb
 
+[![](https://img.shields.io/pypi/v/sesiweb.svg?maxAge=3600)](https://pypi.org/project/sesiweb/)
 ![Test](https://github.com/aaronsmithtv/sesiweb/actions/workflows/test.yml/badge.svg)
 
 sesiweb is a Python module used as a synchronous driver for the SideFX Web API. It provides a simple interface to interact with the API and obtain data about Houdini product builds.
 
 Inputs are validated with Pydantic, and methods in sesiweb provide additional lookup functionality, exceptions, and models.
 
 ## Table of Contents
@@ -106,21 +107,32 @@
 )
 ```
 
 For more information on the SideFX Web API and the returned results you can filter by, refer to the [SideFX Web API documentation](https://www.sidefx.com/docs/api/).
 
 ## Acquiring a Build Download
 
-Using sesiweb, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
+Using sesiweb and Pydantic, you can also transform a `DailyBuild` object into a `ProductBuild` object, which is a required input for acquiring a download URL.
 
-In the script below, 
+In the script below, the single latest daily development build (irrespective of version number) is acquired using `get_latest_build`. `get_build_download` is then used to return the download metadata for that build:
 
 ```python
-# Get the latest Houdini build (filtered)
-build = sw.get_latest_build(prodinfo=build, prodfilter=buildfilter)
+from sesiweb import SesiWeb
+from sesiweb.model.service import ProductBuild
+
+sesi_secret = "your_secret_key"
+sesi_id = "your_client_id"
+
+sw = SesiWeb(sesi_secret, sesi_id)
+
+# Get the most recent Houdini product builds
+build = {"product": "houdini", "platform": "linux"}
+
+# Get the latest Houdini build
+build = sw.get_latest_build(prodinfo=build, only_production=False)
 
 # Get the download URL, filename and hash of the build
 build_dl = sw.get_build_download(
 	prodinfo=ProductBuild(**build.dict())
 )
 
 print(build_dl)
@@ -128,10 +140,12 @@
 
 This will return a `BuildDownloadModel` object containing a download URL, build filename, and hash:
 
 ```shell
 download_url=AnyUrl('https://gjvnth38g.cloudfront.net/download/download-build/456223/cdn/?Expires=166636236...
 ```
 
+For an example of using this metadata in a purpose suitable for a production environment, see [autobuild.py](https://github.com/aaronsmithtv/Houdini-Docker/blob/main/hbuild/autobuild.py) in [Houdini-Docker](https://github.com/aaronsmithtv/Houdini-Docker); Where sesiweb build data is used to construct a Docker image using a custom Houdini installation process.
+
 ## License
 
 sesiweb is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `sesiweb-0.1.0/tests/test_sesiweb.py` & `sesiweb-0.1.1/tests/test_sesiweb.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,42 +13,34 @@
 
 
 def test_get_latest_builds():
     sesiweb = SesiWeb(client_id, client_secret)
     prodinfo = ProductModel(product="houdini", platform="linux")
     prodfilter = {"status": "good", "release": "gold"}
     latest_builds = sesiweb.get_latest_builds(
-        prodinfo=prodinfo,
-        only_production=False,
-        prodfilter=prodfilter
+        prodinfo=prodinfo, only_production=False, prodfilter=prodfilter
     )
     assert latest_builds is not None
     assert len(latest_builds) > 0
 
 
 def test_get_latest_build():
     sesiweb = SesiWeb(client_id, client_secret)
     prodinfo = ProductModel(product="houdini", platform="linux")
     prodfilter = {"status": "good", "release": "gold"}
     latest_builds = sesiweb.get_latest_build(
-        prodinfo=prodinfo,
-        only_production=False,
-        prodfilter=prodfilter
+        prodinfo=prodinfo, only_production=False, prodfilter=prodfilter
     )
     assert latest_builds is not None
 
 
 def test_get_dl():
     sesiweb = SesiWeb(client_id, client_secret)
     prodinfo = ProductModel(product="houdini", platform="linux")
     prodfilter = {"status": "good", "release": "gold"}
     latest_build = sesiweb.get_latest_build(
-        prodinfo=prodinfo,
-        only_production=False,
-        prodfilter=prodfilter
+        prodinfo=prodinfo, only_production=False, prodfilter=prodfilter
     )
 
-    build_dl = sesiweb.get_build_download(
-        prodinfo=ProductBuild(**latest_build.dict())
-    )
+    build_dl = sesiweb.get_build_download(prodinfo=ProductBuild(**latest_build.dict()))
 
     assert build_dl is not None
```

