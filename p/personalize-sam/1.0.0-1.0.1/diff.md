# Comparing `tmp/personalize-sam-1.0.0.tar.gz` & `tmp/personalize-sam-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personalize-sam-1.0.0.tar", last modified: Tue Jun 13 13:04:53 2023, max compression
+gzip compressed data, was "personalize-sam-1.0.1.tar", last modified: Tue Jun 13 14:00:17 2023, max compression
```

## Comparing `personalize-sam-1.0.0.tar` & `personalize-sam-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 13:04:53.886518 personalize-sam-1.0.0/
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     1069 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/LICENSE.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       24 2023-06-13 13:04:50.000000 personalize-sam-1.0.0/MANIFEST.in
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     4698 2023-06-13 13:04:53.886351 personalize-sam-1.0.0/PKG-INFO
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     4224 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/README.md
-drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 13:04:53.883700 personalize-sam-1.0.0/per_segment_anything/
--rw-r--r--   0 nathaliewillems   (501) staff       (20)      427 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/__init__.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)    15148 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/automatic_mask_generator.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     2941 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/build_sam.py
-drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 13:04:53.884613 personalize-sam-1.0.0/per_segment_anything/modeling/
--rw-r--r--   0 nathaliewillems   (501) staff       (20)      385 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/__init__.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     1479 2023-05-26 12:12:52.000000 personalize-sam-1.0.0/per_segment_anything/modeling/common.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)    14420 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/image_encoder.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     6826 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     8594 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     7553 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/sam.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     8831 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/modeling/transformer.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)    12609 2023-05-10 18:32:08.000000 personalize-sam-1.0.0/per_segment_anything/predictor.py
-drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 13:04:53.885129 personalize-sam-1.0.0/per_segment_anything/utils/
--rw-r--r--   0 nathaliewillems   (501) staff       (20)      197 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/utils/__init__.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)    12712 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/utils/amg.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     5812 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/utils/onnx.py
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     3972 2023-05-09 12:24:42.000000 personalize-sam-1.0.0/per_segment_anything/utils/transforms.py
-drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 13:04:53.886083 personalize-sam-1.0.0/personalize_SAM.egg-info/
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     4698 2023-06-13 13:04:53.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/PKG-INFO
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     1134 2023-06-13 13:04:53.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/SOURCES.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       51 2023-06-13 13:04:53.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/dependency_links.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)        1 2023-05-26 11:59:45.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/not-zip-safe
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       43 2023-06-13 13:04:53.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/requires.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       21 2023-06-13 13:04:53.000000 personalize-sam-1.0.0/personalize_SAM.egg-info/top_level.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)      556 2023-06-13 12:57:38.000000 personalize-sam-1.0.0/pyproject.toml
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       61 2023-06-13 12:53:33.000000 personalize-sam-1.0.0/requirements.txt
--rw-r--r--   0 nathaliewillems   (501) staff       (20)       38 2023-06-13 13:04:53.886563 personalize-sam-1.0.0/setup.cfg
--rw-r--r--   0 nathaliewillems   (501) staff       (20)     1344 2023-06-13 13:02:30.000000 personalize-sam-1.0.0/setup.py
+drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 14:00:17.407908 personalize-sam-1.0.1/
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     1069 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/LICENSE.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       24 2023-06-13 13:04:50.000000 personalize-sam-1.0.1/MANIFEST.in
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     4698 2023-06-13 14:00:17.407760 personalize-sam-1.0.1/PKG-INFO
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     4224 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/README.md
+drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 14:00:17.404340 personalize-sam-1.0.1/per_segment_anything/
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)      427 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/__init__.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)    15148 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     2941 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/build_sam.py
+drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 14:00:17.405654 personalize-sam-1.0.1/per_segment_anything/modeling/
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)      385 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/__init__.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     1479 2023-05-26 12:12:52.000000 personalize-sam-1.0.1/per_segment_anything/modeling/common.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)    14420 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     6826 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     8594 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     7553 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/sam.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     8831 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/modeling/transformer.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)    12609 2023-05-10 18:32:08.000000 personalize-sam-1.0.1/per_segment_anything/predictor.py
+drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 14:00:17.406286 personalize-sam-1.0.1/per_segment_anything/utils/
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)      197 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/utils/__init__.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)    12712 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/utils/amg.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     5812 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/utils/onnx.py
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     3972 2023-05-09 12:24:42.000000 personalize-sam-1.0.1/per_segment_anything/utils/transforms.py
+drwxr-xr-x   0 nathaliewillems   (501) staff       (20)        0 2023-06-13 14:00:17.407493 personalize-sam-1.0.1/personalize_SAM.egg-info/
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     4698 2023-06-13 14:00:17.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/PKG-INFO
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     1134 2023-06-13 14:00:17.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/SOURCES.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       51 2023-06-13 14:00:17.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/dependency_links.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)        1 2023-05-26 11:59:45.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/not-zip-safe
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       43 2023-06-13 14:00:17.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/requires.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       21 2023-06-13 14:00:17.000000 personalize-sam-1.0.1/personalize_SAM.egg-info/top_level.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)      556 2023-06-13 13:58:44.000000 personalize-sam-1.0.1/pyproject.toml
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       61 2023-06-13 12:53:33.000000 personalize-sam-1.0.1/requirements.txt
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)       38 2023-06-13 14:00:17.407955 personalize-sam-1.0.1/setup.cfg
+-rw-r--r--   0 nathaliewillems   (501) staff       (20)     1346 2023-06-13 13:45:47.000000 personalize-sam-1.0.1/setup.py
```

### Comparing `personalize-sam-1.0.0/LICENSE.txt` & `personalize-sam-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/PKG-INFO` & `personalize-sam-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personalize-sam
-Version: 1.0.0
+Version: 1.0.1
 Summary: Personalize-SAM package
 Home-page: https://github.com/ZrrSkywalker/Personalize-SAM
 Project-URL: Homepage, https://github.com/ZrrSkywalker/Personalize-SAM
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `personalize-sam-1.0.0/README.md` & `personalize-sam-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/automatic_mask_generator.py` & `personalize-sam-1.0.1/per_segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/build_sam.py` & `personalize-sam-1.0.1/per_segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/common.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/image_encoder.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/mask_decoder.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/prompt_encoder.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/sam.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/modeling/transformer.py` & `personalize-sam-1.0.1/per_segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/predictor.py` & `personalize-sam-1.0.1/per_segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/utils/amg.py` & `personalize-sam-1.0.1/per_segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/utils/onnx.py` & `personalize-sam-1.0.1/per_segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/per_segment_anything/utils/transforms.py` & `personalize-sam-1.0.1/per_segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/personalize_SAM.egg-info/PKG-INFO` & `personalize-sam-1.0.1/personalize_SAM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personalize-sam
-Version: 1.0.0
+Version: 1.0.1
 Summary: Personalize-SAM package
 Home-page: https://github.com/ZrrSkywalker/Personalize-SAM
 Project-URL: Homepage, https://github.com/ZrrSkywalker/Personalize-SAM
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `personalize-sam-1.0.0/personalize_SAM.egg-info/SOURCES.txt` & `personalize-sam-1.0.1/personalize_SAM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personalize-sam-1.0.0/pyproject.toml` & `personalize-sam-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "personalize-sam"
-version = "1.0.0"
+version = "1.0.1"
 description = "Personalize-SAM package"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `personalize-sam-1.0.0/setup.py` & `personalize-sam-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1"
+version = "1.0.0"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

