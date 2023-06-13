# Comparing `tmp/coveo_arnparse-1.0.4.tar.gz` & `tmp/coveo_arnparse-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo_arnparse-1.0.4.tar", max compression
+gzip compressed data, was "coveo_arnparse-1.0.5.tar", max compression
```

## Comparing `coveo_arnparse-1.0.4.tar` & `coveo_arnparse-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1087 2023-02-16 21:11:39.496866 coveo_arnparse-1.0.4/README.md
--rw-r--r--   0        0        0     2927 2023-02-16 21:11:39.496866 coveo_arnparse-1.0.4/coveo_arnparse/__init__.py
--rw-r--r--   0        0        0        0 2023-02-16 21:11:39.496866 coveo_arnparse-1.0.4/coveo_arnparse/py.typed
--rw-r--r--   0        0        0      847 2023-02-16 21:12:10.841681 coveo_arnparse-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 coveo_arnparse-1.0.4/setup.py
--rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 coveo_arnparse-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-13 15:50:38.980067 coveo_arnparse-1.0.5/README.md
+-rw-r--r--   0        0        0     2927 2023-06-13 15:50:38.980067 coveo_arnparse-1.0.5/coveo_arnparse/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:50:38.980067 coveo_arnparse-1.0.5/coveo_arnparse/py.typed
+-rw-r--r--   0        0        0      847 2023-06-13 15:51:04.804448 coveo_arnparse-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 coveo_arnparse-1.0.5/PKG-INFO
```

### Comparing `coveo_arnparse-1.0.4/README.md` & `coveo_arnparse-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `coveo_arnparse-1.0.4/coveo_arnparse/__init__.py` & `coveo_arnparse-1.0.5/coveo_arnparse/__init__.py`

 * *Files identical despite different names*

### Comparing `coveo_arnparse-1.0.4/pyproject.toml` & `coveo_arnparse-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-arnparse"
-version = "1.0.4"
+version = "1.0.5"
 description = "Parse an arn in multiple components."
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-arnparse"
 authors = ["Jonathan Piché <tools@coveo.com>"]
```

### Comparing `coveo_arnparse-1.0.4/setup.py` & `coveo_arnparse-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,62 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coveo-arnparse
+Version: 1.0.5
+Summary: Parse an arn in multiple components.
+Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-arnparse
+License: Apache-2.0
+Author: Jonathan Piché
+Author-email: tools@coveo.com
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/coveooss/coveo-python-oss/tree/main/coveo-arnparse
+Description-Content-Type: text/markdown
 
-packages = \
-['coveo_arnparse']
+# coveo-arnparse
 
-package_data = \
-{'': ['*']}
+Simple dataclass and parser around Amazon Resource Names (ARNs).
 
-setup_kwargs = {
-    'name': 'coveo-arnparse',
-    'version': '1.0.4',
-    'description': 'Parse an arn in multiple components.',
-    'long_description': '# coveo-arnparse\n\nSimple dataclass and parser around Amazon Resource Names (ARNs).\n\nRef: https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\n\n## Usage\n\n### Parse from a string\n```python\n>>> from coveo_arnparse import arnparse\n>>> arn = arnparse("arn:aws:sns:us-east-1:123456789012:my_topic")\n>>> repr(arn)\nArn(partition=\'aws\', service=\'sns\', region=\'us-east-1\', account=\'123456789012\', resource=\'my_topic\')\n>>> str(arn)\n"arn:aws:sns:us-east-1:123456789012:my_topic"\n>>> arn.resource_type\n\'\'\n>>> arn.resource_id\n\'\'\n```\n\nWhen a `:` or a `/` is in the resource, you can also obtain either parts:\n\n```python\n>>> from coveo_arnparse import arnparse\n>>> arn = arnparse("arn:aws:ssm:us-east-1:123456789012:parameter/path/key")\n>>> arn.resource_type\n\'parameter\'\n>>> arn.resource_id\n\'path/key\'\n>>> arn.resource\n\'parameter/path/key\'\n```\n\n\n### Create an instance directly\n\n```python\n>>> from coveo_arnparse import Arn\n>>> Arn(service="s3", resource="my_bucket/path/file.jpg")\nArn(partition=\'aws\', service=\'s3\', region=\'\', account=\'\', resource=\'my_bucket/path/file.jpg\')\n```\n ',
-    'author': 'Jonathan Piché',
-    'author_email': 'tools@coveo.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/coveooss/coveo-python-oss/tree/main/coveo-arnparse',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8',
-}
+Ref: https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html
 
+## Usage
 
-setup(**setup_kwargs)
+### Parse from a string
+```python
+>>> from coveo_arnparse import arnparse
+>>> arn = arnparse("arn:aws:sns:us-east-1:123456789012:my_topic")
+>>> repr(arn)
+Arn(partition='aws', service='sns', region='us-east-1', account='123456789012', resource='my_topic')
+>>> str(arn)
+"arn:aws:sns:us-east-1:123456789012:my_topic"
+>>> arn.resource_type
+''
+>>> arn.resource_id
+''
+```
+
+When a `:` or a `/` is in the resource, you can also obtain either parts:
+
+```python
+>>> from coveo_arnparse import arnparse
+>>> arn = arnparse("arn:aws:ssm:us-east-1:123456789012:parameter/path/key")
+>>> arn.resource_type
+'parameter'
+>>> arn.resource_id
+'path/key'
+>>> arn.resource
+'parameter/path/key'
+```
+
+
+### Create an instance directly
+
+```python
+>>> from coveo_arnparse import Arn
+>>> Arn(service="s3", resource="my_bucket/path/file.jpg")
+Arn(partition='aws', service='s3', region='', account='', resource='my_bucket/path/file.jpg')
+```
+
```

