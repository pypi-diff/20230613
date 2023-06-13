# Comparing `tmp/streamlit-image-coordinates-0.1.4.tar.gz` & `tmp/streamlit-image-coordinates-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-image-coordinates-0.1.4.tar", last modified: Tue Jun 13 14:19:22 2023, max compression
+gzip compressed data, was "streamlit-image-coordinates-0.1.5.tar", last modified: Tue Jun 13 14:47:53 2023, max compression
```

## Comparing `streamlit-image-coordinates-0.1.4.tar` & `streamlit-image-coordinates-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.319159 streamlit-image-coordinates-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.323159 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.331160 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:01.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:22.323159 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 14:19:22.000000 streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/top_level.txt
```

### Comparing `streamlit-image-coordinates-0.1.4/LICENSE` & `streamlit-image-coordinates-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.4/PKG-INFO` & `streamlit-image-coordinates-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.4/README.md` & `streamlit-image-coordinates-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.4/setup.py` & `streamlit-image-coordinates-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-image-coordinates",
-    version="0.1.4",
+    version="0.1.5",
     author="Zachary Blackwood",
     author_email="zachary@streamlit.io",
     description=(
         "Streamlit component that displays an image and returns the coordinates when "
         "you click on it"
     ),
     long_description=long_description,
```

### Comparing `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/__init__.py` & `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import base64
 from io import BytesIO
 from pathlib import Path
 
+import numpy as np
 import streamlit as st
 import streamlit.components.v1 as components
+from PIL import Image
 
 # Tell streamlit that there is a component called streamlit_image_coordinates,
 # and that the code to display that component is in the "frontend" folder
 frontend_dir = (Path(__file__).parent / "frontend").absolute()
 _component_func = components.declare_component(
     "streamlit_image_coordinates", path=str(frontend_dir)
 )
 
 
 # Create the python function that will be called
 def streamlit_image_coordinates(
-    source: str | Path | object,
+    source: str | Path | np.ndarray | object,
     height: int | None = None,
     width: int | None = None,
     key: str | None = None,
 ):
     """
     Take an image source and return the coordinates of the image clicked
 
@@ -42,16 +44,24 @@
         else:
             src = str(source)
     elif hasattr(source, "save"):
         buffered = BytesIO()
         source.save(buffered, format="PNG")  # type: ignore
         src = "data:image/png;base64,"
         src += base64.b64encode(buffered.getvalue()).decode("utf-8")  # type: ignore
+    elif isinstance(source, np.ndarray):
+        image = Image.fromarray(source)
+        buffered = BytesIO()
+        image.save(buffered, format="PNG")  # type: ignore
+        src = "data:image/png;base64,"
+        src += base64.b64encode(buffered.getvalue()).decode("utf-8")  # type: ignore
     else:
-        raise ValueError("Must pass a string, Path, or object with a save method")
+        raise ValueError(
+            "Must pass a string, Path, numpy array or object with a save method"
+        )
 
     component_value = _component_func(
         src=src,
         height=height,
         width=width,
         key=key,
     )
```

### Comparing `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/main.js` & `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js` & `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/PKG-INFO` & `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.4/src/streamlit_image_coordinates.egg-info/SOURCES.txt` & `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

