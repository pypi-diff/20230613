# Comparing `tmp/coveo_testing_extras-2.1.2.tar.gz` & `tmp/coveo_testing_extras-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo_testing_extras-2.1.2.tar", max compression
+gzip compressed data, was "coveo_testing_extras-2.1.3.tar", max compression
```

## Comparing `coveo_testing_extras-2.1.2.tar` & `coveo_testing_extras-2.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1709 2023-02-16 21:12:17.524925 coveo_testing_extras-2.1.2/README.md
--rw-r--r--   0        0        0        0 2023-02-16 21:12:17.524925 coveo_testing_extras-2.1.2/coveo_testing_extras/__init__.py
--rw-r--r--   0        0        0        0 2023-02-16 21:12:17.524925 coveo_testing_extras-2.1.2/coveo_testing_extras/py.typed
--rw-r--r--   0        0        0        0 2023-02-16 21:12:17.524925 coveo_testing_extras-2.1.2/coveo_testing_extras/temporary_resource/__init__.py
--rw-r--r--   0        0        0    10759 2023-02-16 21:12:17.524925 coveo_testing_extras-2.1.2/coveo_testing_extras/temporary_resource/docker_container.py
--rw-r--r--   0        0        0     1093 2023-02-16 21:12:57.927515 coveo_testing_extras-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2548 1970-01-01 00:00:00.000000 coveo_testing_extras-2.1.2/setup.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 coveo_testing_extras-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1709 2023-06-13 15:50:46.473093 coveo_testing_extras-2.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:50:46.473093 coveo_testing_extras-2.1.3/coveo_testing_extras/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:50:46.473093 coveo_testing_extras-2.1.3/coveo_testing_extras/py.typed
+-rw-r--r--   0        0        0        0 2023-06-13 15:50:46.473093 coveo_testing_extras-2.1.3/coveo_testing_extras/temporary_resource/__init__.py
+-rw-r--r--   0        0        0    10759 2023-06-13 15:50:46.473093 coveo_testing_extras-2.1.3/coveo_testing_extras/temporary_resource/docker_container.py
+-rw-r--r--   0        0        0     1093 2023-06-13 15:51:13.829573 coveo_testing_extras-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 coveo_testing_extras-2.1.3/PKG-INFO
```

### Comparing `coveo_testing_extras-2.1.2/README.md` & `coveo_testing_extras-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `coveo_testing_extras-2.1.2/coveo_testing_extras/temporary_resource/docker_container.py` & `coveo_testing_extras-2.1.3/coveo_testing_extras/temporary_resource/docker_container.py`

 * *Files identical despite different names*

### Comparing `coveo_testing_extras-2.1.2/pyproject.toml` & `coveo_testing_extras-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-testing-extras"
-version = "2.1.2"
+version = "2.1.3"
 description = "Dependency-hungry testing helpers"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `coveo_testing_extras-2.1.2/setup.py` & `coveo_testing_extras-2.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,74 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coveo-testing-extras
+Version: 2.1.3
+Summary: Dependency-hungry testing helpers
+Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras
+License: Apache-2.0
+Author: Jonathan Piché
+Author-email: tools@coveo.com
+Requires-Python: >=3.8,<3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: coveo-functools
+Requires-Dist: coveo-settings
+Requires-Dist: coveo-systools
+Requires-Dist: coveo-testing
+Requires-Dist: docker
+Project-URL: Repository, https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras
+Description-Content-Type: text/markdown
+
+# coveo-testing-extras
+
+Contains extra testing tools without dependency restrictions.
+
+
+## temporary resource implementation: Docker Container
+
+The docker container temporary resource can be used to prepare short-lived containers.
+
+- Supports building from a dockerfile
+- Supports pulling images
+- Can signal on AWS ECR logout
+- Dynamic port mapping retrieval
+- Saves log output before removing the container
+
+
+### Automatic AWS ECR login example
+
+Here's how you can enhance `TemporaryDockerContainerResource` with automatic ECR login:
+
+```python
+from base64 import b64decode
+
+import boto3
+from coveo_testing_extras.temporary_resource.docker_container import (
+    TemporaryDockerContainerResource, 
+    ECRLogoutException,
+    get_docker_client
+)
+
+class WithECR(TemporaryDockerContainerResource):
+    def obtain_image(self) -> None:
+        try:
+            super().obtain_image()
+        except ECRLogoutException:
+            self._do_ecr_login()
+            super().obtain_image()
+
+    def _do_ecr_login(self) -> None:
+        """ Performs an ecr login through awscli. """
+        assert self.ecr_region
+        ecr = boto3.client('ecr')
+        account_id, *_ = self.image_name.split('.')
+        assert account_id.isdigit()
+        authorization_data = ecr.get_authorization_token(registryIds=[account_id])['authorizationData'][0]
+        username, password = b64decode(authorization_data['authorizationToken']).decode().split(':')
+        with get_docker_client() as client:
+            login = client.login(username=username, password=password, registry=authorization_data['proxyEndpoint'])
+        assert login['Status'] == 'Login Succeeded'
+```
 
-packages = \
-['coveo_testing_extras', 'coveo_testing_extras.temporary_resource']
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['coveo-functools',
- 'coveo-settings',
- 'coveo-systools',
- 'coveo-testing',
- 'docker']
-
-setup_kwargs = {
-    'name': 'coveo-testing-extras',
-    'version': '2.1.2',
-    'description': 'Dependency-hungry testing helpers',
-    'long_description': '# coveo-testing-extras\n\nContains extra testing tools without dependency restrictions.\n\n\n## temporary resource implementation: Docker Container\n\nThe docker container temporary resource can be used to prepare short-lived containers.\n\n- Supports building from a dockerfile\n- Supports pulling images\n- Can signal on AWS ECR logout\n- Dynamic port mapping retrieval\n- Saves log output before removing the container\n\n\n### Automatic AWS ECR login example\n\nHere\'s how you can enhance `TemporaryDockerContainerResource` with automatic ECR login:\n\n```python\nfrom base64 import b64decode\n\nimport boto3\nfrom coveo_testing_extras.temporary_resource.docker_container import (\n    TemporaryDockerContainerResource, \n    ECRLogoutException,\n    get_docker_client\n)\n\nclass WithECR(TemporaryDockerContainerResource):\n    def obtain_image(self) -> None:\n        try:\n            super().obtain_image()\n        except ECRLogoutException:\n            self._do_ecr_login()\n            super().obtain_image()\n\n    def _do_ecr_login(self) -> None:\n        """ Performs an ecr login through awscli. """\n        assert self.ecr_region\n        ecr = boto3.client(\'ecr\')\n        account_id, *_ = self.image_name.split(\'.\')\n        assert account_id.isdigit()\n        authorization_data = ecr.get_authorization_token(registryIds=[account_id])[\'authorizationData\'][0]\n        username, password = b64decode(authorization_data[\'authorizationToken\']).decode().split(\':\')\n        with get_docker_client() as client:\n            login = client.login(username=username, password=password, registry=authorization_data[\'proxyEndpoint\'])\n        assert login[\'Status\'] == \'Login Succeeded\'\n```\n\n\n',
-    'author': 'Jonathan Piché',
-    'author_email': 'tools@coveo.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
-}
-
-
-setup(**setup_kwargs)
```

