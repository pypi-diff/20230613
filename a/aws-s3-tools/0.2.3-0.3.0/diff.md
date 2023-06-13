# Comparing `tmp/aws_s3_tools-0.2.3.tar.gz` & `tmp/aws_s3_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_s3_tools-0.2.3.tar", max compression
+gzip compressed data, was "aws_s3_tools-0.3.0.tar", max compression
```

## Comparing `aws_s3_tools-0.2.3.tar` & `aws_s3_tools-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1071 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/LICENSE
--rw-r--r--   0        0        0     3898 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/README.md
--rw-r--r--   0        0        0     1491 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1267 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/__init__.py
--rw-r--r--   0        0        0        0 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/buckets/__init__.py
--rw-r--r--   0        0        0      979 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/buckets/check.py
--rw-r--r--   0        0        0      871 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/buckets/create.py
--rw-r--r--   0        0        0     1029 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/buckets/delete.py
--rw-r--r--   0        0        0     1101 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/buckets/list.py
--rw-r--r--   0        0        0        0 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/__init__.py
--rw-r--r--   0        0        0     2533 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/check.py
--rw-r--r--   0        0        0     5380 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/copy.py
--rw-r--r--   0        0        0     2806 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/delete.py
--rw-r--r--   0        0        0     9309 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/download.py
--rw-r--r--   0        0        0     2433 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/list.py
--rw-r--r--   0        0        0     3273 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/move.py
--rw-r--r--   0        0        0     4954 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/presigned_url.py
--rw-r--r--   0        0        0     2483 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/read.py
--rw-r--r--   0        0        0     8950 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/upload.py
--rw-r--r--   0        0        0     3393 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/objects/write.py
--rw-r--r--   0        0        0     1676 2022-11-21 14:54:24.664002 aws_s3_tools-0.2.3/s3_tools/utils.py
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 aws_s3_tools-0.2.3/setup.py
--rw-r--r--   0        0        0     5349 1970-01-01 00:00:00.000000 aws_s3_tools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 10:11:35.086314 aws_s3_tools-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3898 2023-06-13 10:11:35.086314 aws_s3_tools-0.3.0/README.md
+-rw-r--r--   0        0        0     1579 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1267 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/buckets/__init__.py
+-rw-r--r--   0        0        0      979 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/buckets/check.py
+-rw-r--r--   0        0        0      871 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/buckets/create.py
+-rw-r--r--   0        0        0     1029 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/buckets/delete.py
+-rw-r--r--   0        0        0     1101 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/buckets/list.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/check.py
+-rw-r--r--   0        0        0     5380 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/copy.py
+-rw-r--r--   0        0        0     2806 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/delete.py
+-rw-r--r--   0        0        0     9309 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/download.py
+-rw-r--r--   0        0        0     2433 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/list.py
+-rw-r--r--   0        0        0     3273 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/move.py
+-rw-r--r--   0        0        0     4954 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/presigned_url.py
+-rw-r--r--   0        0        0     2483 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/read.py
+-rw-r--r--   0        0        0     8950 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/upload.py
+-rw-r--r--   0        0        0     3393 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/objects/write.py
+-rw-r--r--   0        0        0     1676 2023-06-13 10:11:35.090314 aws_s3_tools-0.3.0/s3_tools/utils.py
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 aws_s3_tools-0.3.0/PKG-INFO
```

### Comparing `aws_s3_tools-0.2.3/LICENSE` & `aws_s3_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/README.md` & `aws_s3_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/pyproject.toml` & `aws_s3_tools-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-s3-tools"
-version = "0.2.3"
+version = "0.3.0"
 description = "AWS S3 tools package"
 authors = ["Daniel Ferrari"]
 maintainers = ["Daniel Ferrari, Carlos Alves, Tomás Osório"]
 license = "MIT"
 
 readme = "README.md"
 
@@ -23,41 +23,42 @@
     "Intended Audience :: Developers",
     "License :: Freely Distributable",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-
-boto3 = "^1"
+python = "^3.8"
+boto3 = "^1.25"
 ujson = "^5"
-rich = {version = "^11", optional = true}
-types-ujson = "^4"
+rich = {version = "^13", optional = true}
 
 [tool.poetry.extras]
 progress = ["rich"]
 
-[tool.poetry.dev-dependencies]
-flake8 = "^4"
-moto = "^3"
-mypy = "^0"
-pydocstyle = "^6"
-pytest = "^6"
-pytest-cov = "^3"
-toml = "^0"
-sphinx-rtd-theme = "^0"
-sphinx = "^3"
-requests = "^2"
-types-requests = "^2"
+[tool.poetry.group.dev.dependencies]
+flake8 = "*"
+moto = "*"
+mypy = "*"
+pydocstyle = "*"
+pytest = "*"
+pytest-cov = "*"
+toml = "*"
+sphinx-rtd-theme = "*"
+sphinx = "*"
+requests = "*"
+types-requests = "*"
+types-ujson = "*"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.aws-s3-tools]
 copyright = "2021, Daniel Ferrari"
```

### Comparing `aws_s3_tools-0.2.3/s3_tools/__init__.py` & `aws_s3_tools-0.3.0/s3_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/buckets/check.py` & `aws_s3_tools-0.3.0/s3_tools/buckets/check.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/buckets/create.py` & `aws_s3_tools-0.3.0/s3_tools/buckets/create.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/buckets/delete.py` & `aws_s3_tools-0.3.0/s3_tools/buckets/delete.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/buckets/list.py` & `aws_s3_tools-0.3.0/s3_tools/buckets/list.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/check.py` & `aws_s3_tools-0.3.0/s3_tools/objects/check.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/copy.py` & `aws_s3_tools-0.3.0/s3_tools/objects/copy.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/delete.py` & `aws_s3_tools-0.3.0/s3_tools/objects/delete.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/download.py` & `aws_s3_tools-0.3.0/s3_tools/objects/download.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/list.py` & `aws_s3_tools-0.3.0/s3_tools/objects/list.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/move.py` & `aws_s3_tools-0.3.0/s3_tools/objects/move.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/presigned_url.py` & `aws_s3_tools-0.3.0/s3_tools/objects/presigned_url.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/read.py` & `aws_s3_tools-0.3.0/s3_tools/objects/read.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/upload.py` & `aws_s3_tools-0.3.0/s3_tools/objects/upload.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/objects/write.py` & `aws_s3_tools-0.3.0/s3_tools/objects/write.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/s3_tools/utils.py` & `aws_s3_tools-0.3.0/s3_tools/utils.py`

 * *Files identical despite different names*

### Comparing `aws_s3_tools-0.2.3/setup.py` & `aws_s3_tools-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,159 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aws-s3-tools
+Version: 0.3.0
+Summary: AWS S3 tools package
+Home-page: https://github.com/dlite-tools/aws-s3-tools
+License: MIT
+Keywords: aws,s3,tools,package
+Author: Daniel Ferrari
+Maintainer: Daniel Ferrari, Carlos Alves, Tomás Osório
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Freely Distributable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Provides-Extra: progress
+Requires-Dist: boto3 (>=1.25,<2.0)
+Requires-Dist: rich (>=13,<14) ; extra == "progress"
+Requires-Dist: ujson (>=5,<6)
+Project-URL: Documentation, https://aws-s3-tools.readthedocs.io/en/latest/index.html
+Project-URL: Repository, https://github.com/dlite-tools/aws-s3-tools
+Description-Content-Type: text/markdown
+
+# AWS S3 Tools
+
+![MIT License](https://img.shields.io/pypi/l/aws-s3-tools)
+[![Test](https://github.com/dlite-tools/aws-s3-tools/actions/workflows/test.yml/badge.svg)](https://github.com/dlite-tools/aws-s3-tools/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/dlite-tools/aws-s3-tools/branch/main/graph/badge.svg?token=YRM26tZexs)](https://codecov.io/gh/dlite-tools/aws-s3-tools)
+![Documentation Status](https://readthedocs.org/projects/aws-s3-tools/badge/?version=latest)
+![Package Version](https://img.shields.io/pypi/v/aws-s3-tools)
+![Python Version](https://img.shields.io/pypi/pyversions/aws-s3-tools)
+
+AWS S3 Tools is a Python package to make it easier to interact with S3 objects, where you can:
+
+- List S3 bucket content
+- Check if an S3 object exists
+- Download/upload S3 objects to/from local files
+- Read/write S3 objects into/from Python variables
+- Delete/move/copy S3 objects
+
+The AWS S3 authentication is done via boto3 package, via environment variables, aws config file, or parameters.
+All S3 objects functions, in this package, have the option to set AWS Session authentication by passing the following dictionary on the `aws_auth` parameter, with the schema below (not all field are required).
+To understand more about AWS authentication mechanism, [read boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html).
+
+```python
+aws_auth = {
+    'region_name': 'REGION',
+    'aws_access_key_id': 'ACCESS_KEY',
+    'aws_secret_access_key': 'SECRET_KEY',
+    'aws_session_token': 'SESSION_TOKEN',
+    'profile_name': 'PROFILE_NAME'
+}
+```
 
-packages = \
-['s3_tools', 's3_tools.buckets', 's3_tools.objects']
+---
 
-package_data = \
-{'': ['*']}
+## Installation
 
-install_requires = \
-['boto3>=1,<2', 'types-ujson>=4,<5', 'ujson>=5,<6']
-
-extras_require = \
-{'progress': ['rich>=11,<12']}
-
-setup_kwargs = {
-    'name': 'aws-s3-tools',
-    'version': '0.2.3',
-    'description': 'AWS S3 tools package',
-    'long_description': '# AWS S3 Tools\n\n![MIT License](https://img.shields.io/pypi/l/aws-s3-tools)\n[![Test](https://github.com/dlite-tools/aws-s3-tools/actions/workflows/test.yml/badge.svg)](https://github.com/dlite-tools/aws-s3-tools/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/dlite-tools/aws-s3-tools/branch/main/graph/badge.svg?token=YRM26tZexs)](https://codecov.io/gh/dlite-tools/aws-s3-tools)\n![Documentation Status](https://readthedocs.org/projects/aws-s3-tools/badge/?version=latest)\n![Package Version](https://img.shields.io/pypi/v/aws-s3-tools)\n![Python Version](https://img.shields.io/pypi/pyversions/aws-s3-tools)\n\nAWS S3 Tools is a Python package to make it easier to interact with S3 objects, where you can:\n\n- List S3 bucket content\n- Check if an S3 object exists\n- Download/upload S3 objects to/from local files\n- Read/write S3 objects into/from Python variables\n- Delete/move/copy S3 objects\n\nThe AWS S3 authentication is done via boto3 package, via environment variables, aws config file, or parameters.\nAll S3 objects functions, in this package, have the option to set AWS Session authentication by passing the following dictionary on the `aws_auth` parameter, with the schema below (not all field are required).\nTo understand more about AWS authentication mechanism, [read boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html).\n\n```python\naws_auth = {\n    \'region_name\': \'REGION\',\n    \'aws_access_key_id\': \'ACCESS_KEY\',\n    \'aws_secret_access_key\': \'SECRET_KEY\',\n    \'aws_session_token\': \'SESSION_TOKEN\',\n    \'profile_name\': \'PROFILE_NAME\'\n}\n```\n\n---\n\n## Installation\n\nYou can install AWS S3 Tools from PyPi with `pip` or your favorite package manager:\n\n```shell\npip install aws-s3-tools\n```\n\nAdd the ``-U`` switch to update to the current version, if AWS S3 Tools is already installed.\n\nIf you want to use the **progress bar** feature when downloading or uploading,\nyou need to install an extra dependency.\n\n```shell\npip install aws-s3-tools[progress]\n```\n\n---\n\n## Usage\n\n[The full documentation can be found here](https://aws-s3-tools.readthedocs.io/en/latest/index.html).\n\n```python\nfrom s3_tools import object_exists\n\nif object_exists("my-bucket", "s3-prefix/object.data"):\n    # Your code goes here\nelse:\n    print("Object not found")\n```\n\nExample to use the progress bar:\n\n```python\nfrom s3_tools import upload_folder_to_prefix\n\nresult = upload_folder_to_prefix(\n    bucket=\'dlite-tools\',\n    prefix=\'aws-s3-tools\',\n    search_str=\'*.py\',\n    threads=2,\n    folder=\'s3_tools\',\n    show_progress=True\n)\n```\n\nProgress bar when running the code above:\n\n![Progress bar gif](docs/source/demo.gif)\n\n---\n\n## Contributions\n\nAll contributions, bug reports, bug fixes, documentation improvements,\nenhancements and ideas are welcome.\n\nA detailed overview on how to contribute can be found in the\n[contributing guide](CONTRIBUTING.md)\non GitHub.\n\n---\n\n## Issues\n\nGo [here](https://github.com/dlite-tools/aws-s3-tools/issues) to submit feature\nrequests or bugfixes.\n\n---\n\n## License and Credits\n\n`AWS S3 Tools` is licensed under the [MIT license](LICENSE) and is written and\nmaintained by:\n\n- Daniel Ferrari ([@FerrariDG](https://github.com/FerrariDG))\n- Carlos Alves ([@cmalves](https://github.com/cmalves))\n- Tomás Osório ([@tomassosorio](https://github.com/tomassosorio/))\n\n---\n\n## Acknowledgement\n\nThe idea from these functions come from an amazing team that I worked with. This repo is a refactor and documentation to make this public to everyone.\n\nMany thanks to:\n\n- [Anabela Nogueira](https://www.linkedin.com/in/abnogueira/)\n- [Carlos Alves](https://www.linkedin.com/in/carlosmalves/)\n- [João Machado](https://www.linkedin.com/in/machadojpf/)\n- [Renato Dantas](https://www.linkedin.com/in/renatomoura/)\n- [Ricardo Garcia](https://www.linkedin.com/in/ricardo-g-oliveira/)\n- [Tomás Osório](https://www.linkedin.com/in/tomas-osorio/)\n',
-    'author': 'Daniel Ferrari',
-    'author_email': 'None',
-    'maintainer': 'Daniel Ferrari, Carlos Alves, Tomás Osório',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dlite-tools/aws-s3-tools',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+You can install AWS S3 Tools from PyPi with `pip` or your favorite package manager:
+
+```shell
+pip install aws-s3-tools
+```
+
+Add the ``-U`` switch to update to the current version, if AWS S3 Tools is already installed.
+
+If you want to use the **progress bar** feature when downloading or uploading,
+you need to install an extra dependency.
+
+```shell
+pip install aws-s3-tools[progress]
+```
+
+---
+
+## Usage
+
+[The full documentation can be found here](https://aws-s3-tools.readthedocs.io/en/latest/index.html).
+
+```python
+from s3_tools import object_exists
+
+if object_exists("my-bucket", "s3-prefix/object.data"):
+    # Your code goes here
+else:
+    print("Object not found")
+```
+
+Example to use the progress bar:
+
+```python
+from s3_tools import upload_folder_to_prefix
+
+result = upload_folder_to_prefix(
+    bucket='dlite-tools',
+    prefix='aws-s3-tools',
+    search_str='*.py',
+    threads=2,
+    folder='s3_tools',
+    show_progress=True
+)
+```
+
+Progress bar when running the code above:
+
+![Progress bar gif](docs/source/demo.gif)
+
+---
+
+## Contributions
+
+All contributions, bug reports, bug fixes, documentation improvements,
+enhancements and ideas are welcome.
+
+A detailed overview on how to contribute can be found in the
+[contributing guide](CONTRIBUTING.md)
+on GitHub.
+
+---
+
+## Issues
+
+Go [here](https://github.com/dlite-tools/aws-s3-tools/issues) to submit feature
+requests or bugfixes.
+
+---
+
+## License and Credits
+
+`AWS S3 Tools` is licensed under the [MIT license](LICENSE) and is written and
+maintained by:
+
+- Daniel Ferrari ([@FerrariDG](https://github.com/FerrariDG))
+- Carlos Alves ([@cmalves](https://github.com/cmalves))
+- Tomás Osório ([@tomassosorio](https://github.com/tomassosorio/))
+
+---
+
+## Acknowledgement
+
+The idea from these functions come from an amazing team that I worked with. This repo is a refactor and documentation to make this public to everyone.
+
+Many thanks to:
 
+- [Anabela Nogueira](https://www.linkedin.com/in/abnogueira/)
+- [Carlos Alves](https://www.linkedin.com/in/carlosmalves/)
+- [João Machado](https://www.linkedin.com/in/machadojpf/)
+- [Renato Dantas](https://www.linkedin.com/in/renatomoura/)
+- [Ricardo Garcia](https://www.linkedin.com/in/ricardo-g-oliveira/)
+- [Tomás Osório](https://www.linkedin.com/in/tomas-osorio/)
 
-setup(**setup_kwargs)
```

