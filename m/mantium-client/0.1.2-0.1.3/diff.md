# Comparing `tmp/mantium_client-0.1.2.tar.gz` & `tmp/mantium_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantium_client-0.1.2.tar", max compression
+gzip compressed data, was "mantium_client-0.1.3.tar", max compression
```

## Comparing `mantium_client-0.1.2.tar` & `mantium_client-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-08 22:23:13.931547 mantium_client-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1030 2023-06-08 22:23:13.931547 mantium_client-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/__init__.py
--rw-r--r--   0        0        0      894 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/build.py
--rw-r--r--   0        0        0      176 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/test.py
--rw-r--r--   0        0        0     1324 2023-06-08 22:23:13.931547 mantium_client-0.1.2/mantium/client/invoke_tasks/utils.py
--rw-r--r--   0        0        0     1665 2023-06-08 22:23:13.931547 mantium_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 mantium_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 19:47:52.127222 mantium_client-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1338 2023-06-13 19:47:52.127222 mantium_client-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/api_client.py
+-rw-r--r--   0        0        0      894 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/__init__.py
+-rw-r--r--   0        0        0     1447 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/build.py
+-rw-r--r--   0        0        0      176 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/test.py
+-rw-r--r--   0        0        0     1324 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/invoke_tasks/utils.py
+-rw-r--r--   0        0        0       22 2023-06-13 19:47:52.127222 mantium_client-0.1.3/mantium_client/version.py
+-rw-r--r--   0        0        0     1775 2023-06-13 19:47:52.127222 mantium_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 mantium_client-0.1.3/PKG-INFO
```

### Comparing `mantium_client-0.1.2/LICENSE.txt` & `mantium_client-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.2/README.md` & `mantium_client-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # Mantium Client
-
+[![Mantium logo](https://avatars.githubusercontent.com/u/82233875?s=20&v=4)](https://mantiumai.com/)
 [![CI status](https://github.com/mantiumai/mantium-client-py/actions/workflows/test.yml/badge.svg)](https://github.com/mantiumai/mantium-client-py/actions)
+[![PyPI](https://img.shields.io/pypi/v/mantium-client?color=green)](https://pypi.org/project/mantium-client/)
 [![License](https://img.shields.io/github/license/mantiumai/mantium-client-py)](https://github.com/mantiumai/mantium-client-py/blob/main/LICENSE.txt)
 
-A Python client library for [Mantium services](https://mantiumai.com/).
+
+A Python client library for [Mantium](https://mantiumai.com/) services.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install this client.
 
 ```bash
 pip install mantium-client
 ```
 
 ## Usage
 
 ```python
-from mantium import ApiClient
-from mantium.openapi_client.api.applications_api import ApplicationsApi
-
+from mantium_client.api_client import ApiClient
+from mantium_spec.api.applications_api import ApplicationsApi
 
 client = ApiClient(client_id=CLIENT_ID, client_secret=CLIENT_SECRET)
 apps_api = ApplicationsApi(api_client=client)
 
 # returns a list of applications
 apps_api.list_applications()
 ```
 
 ## License
 
 [Apache-2.0](https://choosealicense.com/licenses/apache-2.0/)
 
 ## Development
 
+This is only necessary if you want to develop in this project.
+
 We use `poetry` for dependency management.
 ```shell
 pip install poetry
-poetry install
+poetry install --with dev,test --verbose
 ```
```

### Comparing `mantium_client-0.1.2/mantium/client/invoke_tasks/__init__.py` & `mantium_client-0.1.3/mantium_client/invoke_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.2/mantium/client/invoke_tasks/build.py` & `mantium_client-0.1.3/mantium_client/invoke_tasks/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Invoke commands for all things build!"""
 from invoke import Runner, task
 
 # Name of the repository
-REPO_NAME = 'core-client-py'
+REPO_NAME = 'core-mantium-py'
 
 
 @task
 def publish_dev_build(cmd: Runner, token_name: str, token: str) -> None:
     """Publish a development build."""
     # The first step is to build the sdist and wheel
     cmd.run('poetry build')
```

### Comparing `mantium_client-0.1.2/mantium/client/invoke_tasks/utils.py` & `mantium_client-0.1.3/mantium_client/invoke_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `mantium_client-0.1.2/pyproject.toml` & `mantium_client-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tool.poetry]
 name = "mantium-client"
-version = "0.1.2"
+version = "0.1.3"
 license = "Apache-2.0"
 description = "Python client for the Mantium API"
 authors = ["Mantium <support@mantiumai.com>"]
 readme = "README.md"
-packages = [{include = "mantium"}]
 repository = "https://github.com/mantiumai/mantium-client-py"
 homepage = "https://github.com/mantiumai/mantium-client-py"
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'License :: OSI Approved :: Apache Software License',
@@ -25,29 +24,34 @@
     'Topic :: Software Development :: Pre-processors',
     'Operating System :: OS Independent'
 ]
 keywords = ["mantium", "ChatGPT", "AI"]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pydantic = "^1.10.2"
+fastapi = "^0.97.0"
+mantium-spec = "1.0.332"
 pre-commit = "2.20.0"
+pydantic = "^1.10.2"
+python = "^3.10"
+requests = "^2.31.0"
+tenacity = "^8.2.2"
+types-requests = "^2.31.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 invoke = "^1.7.3"
 pre-commit = "^2.20.0"
 mypy = "^0.982"
 types-invoke = "^1.7.3.3"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
-validate-pyproject = "^0.13"
+validate-pyproject = {version = "^0.13", extras = ["all"]}
 flake8 = "^6.0.0"
 
 [[tool.poetry.source]]
 name = "dugong"
 url = "https://git.mantiumai.com/api/v4/groups/278/-/packages/pypi/simple"
 default = false
 secondary = true
```

### Comparing `mantium_client-0.1.2/PKG-INFO` & `mantium_client-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantium-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for the Mantium API
 Home-page: https://github.com/mantiumai/mantium-client-py
 License: Apache-2.0
 Keywords: mantium,ChatGPT,AI
 Author: Mantium
 Author-email: support@mantiumai.com
 Requires-Python: >=3.10,<4.0
@@ -19,53 +19,61 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
+Requires-Dist: fastapi (>=0.97.0,<0.98.0)
+Requires-Dist: mantium-spec (==1.0.332)
 Requires-Dist: pre-commit (==2.20.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: types-requests (>=2.31.0.1,<3.0.0.0)
 Project-URL: Repository, https://github.com/mantiumai/mantium-client-py
 Description-Content-Type: text/markdown
 
 # Mantium Client
-
+[![Mantium logo](https://avatars.githubusercontent.com/u/82233875?s=20&v=4)](https://mantiumai.com/)
 [![CI status](https://github.com/mantiumai/mantium-client-py/actions/workflows/test.yml/badge.svg)](https://github.com/mantiumai/mantium-client-py/actions)
+[![PyPI](https://img.shields.io/pypi/v/mantium-client?color=green)](https://pypi.org/project/mantium-client/)
 [![License](https://img.shields.io/github/license/mantiumai/mantium-client-py)](https://github.com/mantiumai/mantium-client-py/blob/main/LICENSE.txt)
 
-A Python client library for [Mantium services](https://mantiumai.com/).
+
+A Python client library for [Mantium](https://mantiumai.com/) services.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install this client.
 
 ```bash
 pip install mantium-client
 ```
 
 ## Usage
 
 ```python
-from mantium import ApiClient
-from mantium.openapi_client.api.applications_api import ApplicationsApi
-
+from mantium_client.api_client import ApiClient
+from mantium_spec.api.applications_api import ApplicationsApi
 
 client = ApiClient(client_id=CLIENT_ID, client_secret=CLIENT_SECRET)
 apps_api = ApplicationsApi(api_client=client)
 
 # returns a list of applications
 apps_api.list_applications()
 ```
 
 ## License
 
 [Apache-2.0](https://choosealicense.com/licenses/apache-2.0/)
 
 ## Development
 
+This is only necessary if you want to develop in this project.
+
 We use `poetry` for dependency management.
 ```shell
 pip install poetry
-poetry install
+poetry install --with dev,test --verbose
 ```
```

