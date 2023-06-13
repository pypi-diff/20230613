# Comparing `tmp/streetview-0.0.2.tar.gz` & `tmp/streetview-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetview-0.0.2.tar", last modified: Sun May 14 20:35:26 2023, max compression
+gzip compressed data, was "streetview-0.0.4.tar", last modified: Tue Jun 13 16:39:43 2023, max compression
```

## Comparing `streetview-0.0.2.tar` & `streetview-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.965448 streetview-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 20:35:08.000000 streetview-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-14 20:35:26.961448 streetview-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-14 20:35:08.000000 streetview-0.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:35:26.965448 streetview-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 20:35:08.000000 streetview-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/streetview/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 20:35:08.000000 streetview-0.0.2/streetview/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/streetview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 20:35:26.000000 streetview-0.0.2/streetview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:35:26.961448 streetview-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-14 20:35:08.000000 streetview-0.0.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 20:35:09.000000 streetview-0.0.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 16:39:26.000000 streetview-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-13 16:39:43.483541 streetview-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-13 16:39:26.000000 streetview-0.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:39:43.483541 streetview-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:39:26.000000 streetview-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.479541 streetview-0.0.4/streetview/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 16:39:26.000000 streetview-0.0.4/streetview/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/streetview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 16:39:43.000000 streetview-0.0.4/streetview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:39:43.483541 streetview-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-13 16:39:26.000000 streetview-0.0.4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 16:39:26.000000 streetview-0.0.4/version.py
```

### Comparing `streetview-0.0.2/PKG-INFO` & `streetview-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.2
+Version: 0.0.4
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `streetview-0.0.2/readme.md` & `streetview-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `streetview-0.0.2/setup.py` & `streetview-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import setup
+
 from version import VERSION
 
 
 def readme():
     with open("readme.md") as f:
         return f.read()
```

### Comparing `streetview-0.0.2/streetview/api.py` & `streetview-0.0.4/streetview/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from io import BytesIO
+from typing import Dict, Union
 
 import requests
 from PIL import Image
 from pydantic import BaseModel
 
 
 class Location(BaseModel):
@@ -58,15 +59,15 @@
         width (int): Image width (max 640 for non-premium downloads).
         height (int): Image height (max 640 for non-premium downloads).
         fov (int): Image field-of-view.
         pitch (int): Image pitch.
     """
 
     url = "https://maps.googleapis.com/maps/api/streetview"
-    params: dict[str, str | int] = {
+    params: Dict[str, Union[str, int]] = {
         "size": "%dx%d" % (width, height),
         "fov": fov,
         "pitch": pitch,
         "heading": heading,
         "pano": pano_id,
         "key": api_key,
     }
```

### Comparing `streetview-0.0.2/streetview/download.py` & `streetview-0.0.4/streetview/download.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.2/streetview/search.py` & `streetview-0.0.4/streetview/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import re
+from typing import List, Optional
 
 import requests
 from pydantic import BaseModel
 from requests.models import Response
 
 
 class Panorama(BaseModel):
     pano_id: str
     lat: float
     lon: float
     heading: float
     pitch: float
     roll: float
-    date: str | None
+    date: Optional[str]
 
 
 def make_search_url(lat: float, lon: float) -> str:
     """
     Builds the URL of the script on Google's servers that returns the closest
     panoramas (ids) to a give GPS coordinate.
     """
@@ -37,15 +38,15 @@
     Gets the response of the script on Google's servers that returns the
     closest panoramas (ids) to a give GPS coordinate.
     """
     url = make_search_url(lat, lon)
     return requests.get(url)
 
 
-def extract_panoramas(text: str) -> list[Panorama]:
+def extract_panoramas(text: str) -> List[Panorama]:
     """
     Given a valid response from the panoids endpoint, return a list of all the
     panoids.
     """
 
     # The response is actually javascript code. It's a function with a single
     # input which is a huge deeply nested array of items.
@@ -82,15 +83,15 @@
             roll=pano[2][2][2],
             date=dates[i] if i < len(dates) else None,
         )
         for i, pano in enumerate(raw_panos)
     ]
 
 
-def search_panoramas(lat: float, lon: float) -> list[Panorama]:
+def search_panoramas(lat: float, lon: float) -> List[Panorama]:
     """
     Gets the closest panoramas (ids) to the GPS coordinates.
     """
 
     resp = search_request(lat, lon)
     pans = extract_panoramas(resp.text)
     return pans
```

### Comparing `streetview-0.0.2/streetview.egg-info/PKG-INFO` & `streetview-0.0.4/streetview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetview
-Version: 0.0.2
+Version: 0.0.4
 Summary: Retrieve current and historical photos from Google Street View
 Home-page: https://github.com/robolyst/streetview
 Author: Adrian Letchford
 Author-email: me@dradrian.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `streetview-0.0.2/tests/test_api.py` & `streetview-0.0.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.2/tests/test_download.py` & `streetview-0.0.4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `streetview-0.0.2/tests/test_search.py` & `streetview-0.0.4/tests/test_search.py`

 * *Files identical despite different names*

