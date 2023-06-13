# Comparing `tmp/streamlit-image-coordinates-0.1.3.tar.gz` & `tmp/streamlit-image-coordinates-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-image-coordinates-0.1.3.tar", last modified: Mon Jan  9 21:27:56 2023, max compression
+gzip compressed data, was "streamlit-image-coordinates-0.1.4.tar", last modified: Tue Jun 13 14:19:22 2023, max compression
```

## Comparing `streamlit-image-coordinates-0.1.3.tar` & `streamlit-image-coordinates-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:56.493697 streamlit-image-coordinates-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-09 21:27:56.493697 streamlit-image-coordinates-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 21:27:56.493697 streamlit-image-coordinates-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:56.485697 streamlit-image-coordinates-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:56.489697 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:56.493697 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:37.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 21:27:56.489697 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-09 21:27:56.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-09 21:27:56.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 21:27:56.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 21:27:56.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-09 21:27:56.000000 streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.319159 streamlit-image-coordinates-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.323159 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.323159 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/top_level.txt
```

### Comparing `streamlit-image-coordinates-0.1.3/LICENSE` & `streamlit-image-coordinates-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.3/PKG-INFO` & `streamlit-image-coordinates-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.3/README.md` & `streamlit-image-coordinates-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.3/setup.py` & `streamlit-image-coordinates-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-image-coordinates",
-    version="0.1.3",
+    version="0.1.4",
     author="Zachary Blackwood",
     author_email="zachary@streamlit.io",
     description=(
         "Streamlit component that displays an image and returns the coordinates when "
         "you click on it"
     ),
     long_description=long_description,
```

### Comparing `streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/__init__.py` & `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         if not str(source).startswith("http"):
             content = Path(source).read_bytes()
             src = "data:image/png;base64," + base64.b64encode(content).decode("utf-8")
         else:
             src = str(source)
     elif hasattr(source, "save"):
         buffered = BytesIO()
-        source.save(buffered, format="JPEG")  # type: ignore
+        source.save(buffered, format="PNG")  # type: ignore
         src = "data:image/png;base64,"
         src += base64.b64encode(buffered.getvalue()).decode("utf-8")  # type: ignore
     else:
         raise ValueError("Must pass a string, Path, or object with a save method")
 
     component_value = _component_func(
         src=src,
```

### Comparing `streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/main.js` & `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js` & `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/PKG-INFO` & `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.3/src/streamlit_image_coordinates.egg-info/SOURCES.txt` & `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

