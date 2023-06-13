# Comparing `tmp/lentille-0.1.0.tar.gz` & `tmp/lentille-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lentille-0.1.0.tar", max compression
+gzip compressed data, was "lentille-0.2.0.tar", max compression
```

## Comparing `lentille-0.1.0.tar` & `lentille-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      410 2023-04-29 12:37:00.012703 lentille-0.1.0/README.md
--rw-r--r--   0        0        0      344 2023-04-29 12:37:21.853220 lentille-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-04-29 12:37:00.012703 lentille-0.1.0/src/lentille/__init__.py
--rw-r--r--   0        0        0      384 2023-04-29 12:37:00.012703 lentille-0.1.0/src/lentille/base_embedder.py
--rw-r--r--   0        0        0      908 2023-04-29 12:37:00.012703 lentille-0.1.0/src/lentille/embedders/vision/Resnet50Embedder.py
--rw-r--r--   0        0        0     1707 2023-04-29 12:37:00.012703 lentille-0.1.0/src/lentille/utils/resnet50_preprocess.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lentille-0.1.0/setup.py
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 lentille-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-06-13 15:21:58.763681 lentille-0.2.0/README.md
+-rw-r--r--   0        0        0      344 2023-06-13 15:22:22.251615 lentille-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-13 15:21:58.767681 lentille-0.2.0/src/lentille/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-13 15:21:58.767681 lentille-0.2.0/src/lentille/base_embedder.py
+-rw-r--r--   0        0        0      908 2023-06-13 15:21:58.767681 lentille-0.2.0/src/lentille/embedders/vision/Resnet50Embedder.py
+-rw-r--r--   0        0        0     1707 2023-06-13 15:21:58.767681 lentille-0.2.0/src/lentille/utils/resnet50_preprocess.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lentille-0.2.0/setup.py
+-rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 lentille-0.2.0/PKG-INFO
```

### Comparing `lentille-0.1.0/src/lentille/embedders/vision/Resnet50Embedder.py` & `lentille-0.2.0/src/lentille/embedders/vision/Resnet50Embedder.py`

 * *Files identical despite different names*

### Comparing `lentille-0.1.0/src/lentille/utils/resnet50_preprocess.py` & `lentille-0.2.0/src/lentille/utils/resnet50_preprocess.py`

 * *Files identical despite different names*

### Comparing `lentille-0.1.0/setup.py` & `lentille-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.3,<2.0.0', 'onnxruntime>=1.14.1,<2.0.0', 'pillow>=9.5.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'lentille',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# Lentille\nLibrary that wraps various embedders. For now it only wraps a Resnet50 model.\n\n## Installation\n``` bash\npip install lentille\n```\n\n## Example usage\n``` python\nfrom lentille import Resnet50Embedder\n\nembedder = Resnet50Embedder.from_file(\n    "resnet50-v1-12-int8.onnx" # ONNX model from: https://github.com/onnx/models/tree/main/vision/classification/resnet\n)\n\nprint(embedder.classify("cat.jpg"))\n```\n',
     'author': 'Alex',
     'author_email': '46456279+the-alex-b@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lentille-0.1.0/PKG-INFO` & `lentille-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lentille
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Alex
 Author-email: 46456279+the-alex-b@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

