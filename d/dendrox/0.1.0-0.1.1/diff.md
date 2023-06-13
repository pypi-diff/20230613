# Comparing `tmp/dendrox-0.1.0.tar.gz` & `tmp/dendrox-0.1.1.tar.gz`

## Comparing `dendrox-0.1.0.tar` & `dendrox-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 dendrox-0.1.0/src/dendrox/__init__.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dendrox-0.1.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 dendrox-0.1.0/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dendrox-0.1.0/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 dendrox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendrox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 dendrox-0.1.1/src/dendrox/__init__.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dendrox-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 dendrox-0.1.1/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dendrox-0.1.1/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dendrox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 dendrox-0.1.1/PKG-INFO
```

### Comparing `dendrox-0.1.0/src/dendrox/__init__.py` & `dendrox-0.1.1/src/dendrox/__init__.py`

 * *Files identical despite different names*

### Comparing `dendrox-0.1.0/LICENSE` & `dendrox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dendrox-0.1.0/pyproject.toml` & `dendrox-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dendrox"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Qiaonan Duan", email="geonann@gmail.com" },
 ]
 description = "Utility functions to create JSON input for the DendroX app"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy",
-    "seaborn"
+    "numpy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/frlender/dendrox-util"
 "DendroX app" = "https://github.com/frlender/DendroX"
```

### Comparing `dendrox-0.1.0/PKG-INFO` & `dendrox-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dendrox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility functions to create JSON input for the DendroX app
 Project-URL: Homepage, https://github.com/frlender/dendrox-util
 Project-URL: DendroX app, https://github.com/frlender/DendroX
 Author-email: Qiaonan Duan <geonann@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
-Requires-Dist: seaborn
 Description-Content-Type: text/markdown
 
 DendroX
 
 Utility functions to create JSON input for the online DendroX app
```

