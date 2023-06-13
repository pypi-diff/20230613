# Comparing `tmp/opengraph_writer-0.3.3.tar.gz` & `tmp/opengraph_writer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opengraph_writer-0.3.3.tar", last modified: Fri Mar 26 16:24:12 2021, max compression
+gzip compressed data, was "opengraph_writer-0.4.0.tar", last modified: Tue Jun 13 19:25:54 2023, max compression
```

## Comparing `opengraph_writer-0.3.3.tar` & `opengraph_writer-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1050 2021-03-26 16:21:42.000000 opengraph_writer-0.3.3/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2012-01-13 03:20:13.000000 opengraph_writer-0.3.3/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      183 2021-03-26 16:18:16.000000 opengraph_writer-0.3.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     3027 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-14 19:51:35.000000 opengraph_writer-0.3.3/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)     1878 2020-10-20 22:12:29.000000 opengraph_writer-0.3.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       38 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1639 2021-03-26 16:19:18.000000 opengraph_writer-0.3.3/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/src/opengraph_writer/
--rw-r--r--   0 jvanasco   (501) admin       (80)    31953 2021-03-26 16:18:56.000000 opengraph_writer-0.3.3/src/opengraph_writer/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      360 2019-09-19 22:01:05.000000 opengraph_writer-0.3.3/src/opengraph_writer/pyramid_helpers.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:24:11.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:20:08.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     3027 2021-03-26 16:24:11.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       52 2021-03-26 16:24:11.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      493 2021-03-26 16:24:11.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       17 2021-03-26 16:24:11.000000 opengraph_writer-0.3.3/src/opengraph_writer.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:24:12.000000 opengraph_writer-0.3.3/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:18:24.000000 opengraph_writer-0.3.3/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3752 2019-09-19 22:01:05.000000 opengraph_writer-0.3.3/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1256 2020-10-20 19:22:05.000000 opengraph_writer-0.3.3/tests/test_pyramid_integration.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-13 00:24:20.000000 opengraph_writer-0.3.3/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 19:25:54.608554 opengraph_writer-0.4.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1199 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2012-01-13 03:20:13.000000 opengraph_writer-0.4.0/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      183 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2786 2023-06-13 19:25:54.609067 opengraph_writer-0.4.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1877 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-13 19:25:34.000000 opengraph_writer-0.4.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      325 2023-06-13 19:25:54.611371 opengraph_writer-0.4.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1959 2023-06-13 19:25:34.000000 opengraph_writer-0.4.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 19:25:54.547342 opengraph_writer-0.4.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 19:25:54.564257 opengraph_writer-0.4.0/src/opengraph_writer/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    34523 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/src/opengraph_writer/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/src/opengraph_writer/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)      705 2023-06-13 19:25:34.000000 opengraph_writer-0.4.0/src/opengraph_writer/pyramid_helpers.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 19:25:54.584926 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2786 2023-06-13 19:25:54.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      523 2023-06-13 19:25:54.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-13 19:25:54.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:20:08.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       48 2023-06-13 19:25:54.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       17 2023-06-13 19:25:54.000000 opengraph_writer-0.4.0/src/opengraph_writer.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 19:25:54.588669 opengraph_writer-0.4.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    10653 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1330 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/tests/test_pyramid_integration.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-04-24 21:29:58.000000 opengraph_writer-0.4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opengraph_writer-0.3.3/CHANGES.txt` & `opengraph_writer-0.4.0/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.4.0
+    * typing support
+    * drop PY2
+    * drop PY3.5
+    * og_properties is deprecated in favor of OG_PROPERTIES
+    * redid validation logic
+
 0.3.3
 	packaging fix
 
 0.3.2
 	packaging fix
 
 0.3.1 -
```

### Comparing `opengraph_writer-0.3.3/LICENSE.txt` & `opengraph_writer-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opengraph_writer-0.3.3/PKG-INFO` & `opengraph_writer-0.4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,63 @@
-Metadata-Version: 2.1
-Name: opengraph_writer
-Version: 0.3.3
-Summary: Lightweight OpenGraph support for writing and validating objects.
-Home-page: https://github.com/jvanasco/opengraph_writer
-Author: Jonathan Vanasco
-Author-email: jonathan@findmeon.com
-License: MIT
-Description: opengraph_writer
-        ================
-        
-        ![Python package](https://github.com/jvanasco/opengraph_writer/workflows/Python%20package/badge.svg)
-        
-        About
-        =====
-        
-        This library was created to both manage writing OpenGraph data, and perform
-        lightweight verifications for offline debugging.
-        
-        This library does the following:
-        
-        - CREATE an object to stash OGP data
-        - VALIDATE the data, offering debug information on the object
-        - RENDER the object as html, and optionally include debug data on incorrect elements
-        
-        
-        This is currently aimed at "single object page data". It is not necessarily
-        with multi-value items yet (such as multiple profiles or tracks on a single page).
-        
-        Most of the validation routines were derived from regexing the `https://ogp.me`
-        site into a Python dict, and researching what they are supposed to do.
-        The validation routes themselves are super trivial.
-        
-        At the time of initially writing this library, and several checks ever since, the
-        specification on  the `https://ogp.me` seems out of date. 
-        
-        In practice, Facebook's "premier" partners seem to all be using URLs which point 
-        to certain data , however there aren't any guidelines for this within the
-        public OGP spec.
-        
-        An example would be on the Spotify integration: when looking at a `SONG`, the
-        `ARTIST` and `ALBUM` refer to URLs which contain the relevant data.
-        
-        Documentation
-        =============
-        
-        The Python file contains extensive inline documentation.
-        
-        
-        Contributions Welcome!
-        ======================
-        
-        If anyone wants to fork and tackle the multiple value problem, please do.
-        
-        
-        Framework Support: Pyramid
-        ==========================
-        
-        This package offers an includeme for Pyramid to set up an `opengraph_item`
-        as a `@reify` request method.
-        
-        Simply update your application:
-        
-        	config.include("opengraph_writer.pyramid_helpers")
-        
-        And your `Request` objects will be extended as such:
-        
-            request.opengraph_item
-            
-            
-            
-        
-        
-Keywords: facebook opengraph open graph web pyramid
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Framework :: Pyramid
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+opengraph_writer
+================
+
+![Python package](https://github.com/jvanasco/opengraph_writer/workflows/Python%20package/badge.svg)
+
+About
+=====
+
+This library was created to both manage writing OpenGraph data, and perform
+lightweight verifications for offline debugging.
+
+This library does the following:
+
+- CREATE an object to stash OGP data
+- VALIDATE the data, offering debug information on the object
+- RENDER the object as html, and optionally include debug data on incorrect elements
+
+This is currently aimed at "single object page data". It is not necessarily
+with multi-value items yet (such as multiple profiles or tracks on a single page).
+
+Most of the validation routines were derived from regexing the `https://ogp.me`
+site into a Python dict, and researching what they are supposed to do.
+The validation routes themselves are super trivial.
+
+At the time of initially writing this library, and several checks ever since, the
+specification on  the `https://ogp.me` seems out of date. 
+
+In practice, Facebook's "premier" partners seem to all be using URLs which point 
+to certain data , however there aren't any guidelines for this within the
+public OGP spec.
+
+An example would be on the Spotify integration: when looking at a `SONG`, the
+`ARTIST` and `ALBUM` refer to URLs which contain the relevant data.
+
+Documentation
+=============
+
+The Python file contains extensive inline documentation.
+
+
+Contributions Welcome!
+======================
+
+If anyone wants to fork and tackle the multiple value problem, please do.
+
+
+Framework Support: Pyramid
+==========================
+
+This package offers an includeme for Pyramid to set up an `opengraph_item`
+as a `@reify` request method.
+
+Simply update your application:
+
+	config.include("opengraph_writer.pyramid_helpers")
+
+And your `Request` objects will be extended as such:
+
+    request.opengraph_item
+    
+    
+    
+
```

### Comparing `opengraph_writer-0.3.3/README.md` & `opengraph_writer-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: opengraph_writer
+Version: 0.4.0
+Summary: Lightweight OpenGraph support for writing and validating objects.
+Home-page: https://github.com/jvanasco/opengraph_writer
+Author: Jonathan Vanasco
+Author-email: jonathan@findmeon.com
+License: MIT
+Keywords: facebook opengraph open graph web pyramid
+Classifier: Intended Audience :: Developers
+Classifier: Framework :: Pyramid
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 opengraph_writer
 ================
 
 ![Python package](https://github.com/jvanasco/opengraph_writer/workflows/Python%20package/badge.svg)
 
 About
 =====
@@ -11,15 +35,14 @@
 
 This library does the following:
 
 - CREATE an object to stash OGP data
 - VALIDATE the data, offering debug information on the object
 - RENDER the object as html, and optionally include debug data on incorrect elements
 
-
 This is currently aimed at "single object page data". It is not necessarily
 with multi-value items yet (such as multiple profiles or tracks on a single page).
 
 Most of the validation routines were derived from regexing the `https://ogp.me`
 site into a Python dict, and researching what they are supposed to do.
 The validation routes themselves are super trivial.
```

### Comparing `opengraph_writer-0.3.3/setup.py` & `opengraph_writer-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """opengraph_writer installation script.
 """
 import os
 import re
 
-from setuptools import setup
 from setuptools import find_packages
+from setuptools import setup
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 long_description = (
     description
 ) = "Lightweight OpenGraph support for writing and validating objects."
 with open(os.path.join(HERE, "README.md")) as r_file:
     long_description = r_file.read()
 
 # store version in the init.py
 with open(os.path.join(HERE, "src", "opengraph_writer", "__init__.py")) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
 requires = [
-    "metadata_utils>=0.1.1",
-    "six",
+    "metadata_utils>=0.2.0",
 ]
 tests_require = [
     "pytest",
     "pyramid",
 ]
 testing_extras = tests_require + []
 setup(
@@ -33,28 +32,35 @@
     author="Jonathan Vanasco",
     author_email="jonathan@findmeon.com",
     version=VERSION,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
+    python_requires=">=3.6",
     keywords="facebook opengraph open graph web pyramid",
     install_requires=requires,
     tests_require=requires,
     extras_require={
         "testing": testing_extras,
     },
     test_suite="tests",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"opengraph_writer": ["py.typed"]},
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     license="MIT",
 )
```

### Comparing `opengraph_writer-0.3.3/src/opengraph_writer/__init__.py` & `opengraph_writer-0.4.0/src/opengraph_writer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
     https://developers.facebook.com/docs/opengraphprotocol/
 
     Example:
 
          <meta property="og:title" content="The Rock"/>
 
-
     The Open Graph protocol defines four required properties:
 
         og:title - The title of your object as it should appear within the graph, e.g., "The Rock".
         og:type - The type of your object, e.g., "movie". See the complete list of supported types.
         og:image - An image URL which should represent your object within the graph. The image must be at least 50px by 50px and have a maximum aspect ratio of 3:1. We support PNG, JPEG and GIF formats. You may include multiple og:image tags to associate multiple images with your page.
         og:url - The canonical URL of your object that will be used as its permanent ID in the graph, e.g., http://www.imdb.com/title/tt0117500/.
 
@@ -41,23 +40,29 @@
 
         <meta property="og:image" content="http://example.com/rock.jpg" />
         <meta property="og:image" content="http://example.com/rock2.jpg" />
 
     Put structured properties after you declare their root tag. Whenever another root element is parsed, that structured property is considered to be done and another one is started.
 """
 
-__VERSION__ = "0.3.3"
+__VERSION__ = "0.4.0"
 
 # stdlib
 import datetime
 import re
+import typing
 
 # pypi
 from metadata_utils import html_attribute_escape
-import six
+
+# typing
+_OG_KV = typing.Tuple[str, str]
+_OG_KV_MANY = typing.List[_OG_KV]
+_OG_SET = typing.Tuple[str, typing.Any]
+_OG_DATA = typing.Dict[str, typing.Any]
 
 
 # http://en.wikipedia.org/wiki/ISO_8601
 regex_dates = {
     #  Date    2012-02-02
     "date": re.compile("^([0-9]{4})-(1[0-2]|0[1-9])-(3[0-1]|0[1-9]|[1-2][0-9])$"),
     # Ordinal date:    2012-033
@@ -70,18 +75,18 @@
     "datetime, UTC": re.compile(
         "^(-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[0-1]|0[1-9]|[1-2][0-9])T(2[0-3]|[0-1][0-9]):([0-5][0-9]):([0-5][0-9])(.[0-9]+)?(Z|[+-](?:2[0-3]|[0-1][0-9]):[0-5][0-9])?$"
     ),
 }
 
 
 # basically just testing that the string starts with http/https, and has some resemeblence of a domain on it.  after an optional trailing slash, i don't need to make this super accurate
-regex_url = re.compile("""^http[s]?:\/\/[a-z0-9.\-]+[.][a-z]{2,4}\/?""")
+regex_url = re.compile(r"""^http[s]?:\/\/[a-z0-9.\-]+[.][a-z]{2,4}\/?""")
 
 
-og_properties = {
+OG_PROPERTIES: typing.Dict[str, dict] = {
     "og:title": {
         "required": True,
         "description": 'The title of your object as it should appear within the graph, e.g., "The Rock".',
         "type": "string",
     },
     "og:type": {
         "required": True,
@@ -561,31 +566,44 @@
     },
     "fb:app_id": {
         "required": False,
         "description": "A Facebook Platform application ID that administers this page.",
     },
 }
 
+# deprecated
+og_properties = OG_PROPERTIES
+
+
+class OGErrors(dict):
+    def __init__(self):
+        self["critical"] = {}
+        self["recommended"] = {}
+        self["not_validated"] = []
+
 
-def validate_item(info_dict, value):
+def validate_item(
+    info_dict: typing.Dict[str, typing.Any],
+    value: typing.Any,
+) -> bool:
     if info_dict["type"] == "string":
-        if isinstance(value, six.string_types):
+        if isinstance(value, str):
             return True
         return False
 
     elif info_dict["type"] == "boolean":
         try:
-            success = (0, 1, "true", "false").index(value)
+            _success = (0, 1, "true", "false").index(value)  # noqa: F841
             return True
         except ValueError:
             return False
 
     elif info_dict["type"] == "enum":
         try:
-            success = info_dict.enums.index(value)
+            _success = info_dict["enums"].index(value)  # noqa: F841
             return True
         except ValueError:
             return False
 
     elif info_dict["type"] == "integer":
         try:
             if isinstance(value, int):
@@ -597,184 +615,241 @@
                     return True
         except ValueError:
             return False
 
     elif info_dict["type"] == "datetime":
         if isinstance(value, (datetime.date, datetime.datetime)):
             return True
-        if isinstance(value, six.string_types):
+        if isinstance(value, str):
             for test in regex_dates:
                 if re.match(regex_dates[test], value):
                     return True
             return False
 
     elif info_dict["type"] == "url":
         if re.match(regex_url, value):
             return True
         return False
 
     elif info_dict["type"] == "profile":
-        # TO DO
+        # TODO
         # this involves looking for other fields.
         return True
 
     return False
 
 
+def stringify(value: typing.Any) -> str:
+    """turns a value into a string if needed"""
+    if isinstance(value, bool):
+        if value:
+            return "true"
+        return "false"
+    elif isinstance(value, datetime.datetime):
+        return value.isoformat()
+    elif isinstance(value, datetime.date):
+        return value.isoformat()
+    return value
+
+
 class OpenGraphItem(object):
-    _data = None
-    _errors = None
+    _data: _OG_DATA = {}
+    _errors: typing.Optional[OGErrors] = None
 
-    def __init__(self, sets=None):
+    def __init__(
+        self,
+        sets: typing.Optional[_OG_KV_MANY] = None,
+    ) -> None:
         self._data = {}
-        self._errors = {}
         if sets:
             self.set_many(sets)
 
-    def set_many(self, pairs):
+    def set_many(
+        self,
+        pairs: _OG_KV_MANY,
+    ) -> None:
         for pair in pairs:
             (f, v) = pair
             self.set(f, v)
 
-    def set(self, field, value, append=False):
+    def set(
+        self,
+        field: str,
+        value: str,
+        append: bool = False,
+    ) -> None:
         if not append:
             self._data[field] = value
         else:
             if field not in self._data:
                 self._data[field] = []
             else:
                 if not isinstance(self._data[field], list):
                     self._data[field] = [self._data[field]]
             self._data[field].append(value)
 
-    def validate(self, facebook=False, schema1=False, schema2=True):
-        errors = {"critical": {}, "recommended": {}}
-
-        def _errror(level, item, message):
+    def validate(
+        self,
+        facebook: bool = False,
+        schema1: bool = False,
+        schema2: bool = True,
+    ) -> bool:
+        """
+        Validate the object
+
+        :param facebook: validate against the facebook extensions?
+        :type resp: bool
+        :param schema1: validate against schema1? Default: `False`.
+            This is likely the schema before opengraph was open sourced.
+            It is very basic, and only checks for a supported "og:type"
+        :type resp: bool
+        :param schema2: validate against schema2? Default: `True`
+            This appears to be the current opengraph protocol.
+            This will process both the og:type and the subtypes.
+        :type resp: bool
+
+        :rtype: bool
+        """
+        if facebook is True:
+            raise ValueError("Support for Facebook Extensions is not built yet")
+        if schema1 and schema2:
+            raise ValueError("Validate against either schema1 or schema2")
+
+        errors = OGErrors()
+
+        def _set_error(
+            level: str,
+            item: str,
+            message: str,
+        ) -> None:
             # if level not in errors:
             #    errors[level]= {}
             errors[level][item] = message
 
-        for i in og_properties:
-            # make sure that everything in og_properties which is required is present
-            if og_properties[i]["required"] and (i not in self._data):
-                _errror("critical", i, "Missing Required Element")
-            elif og_properties[i]["required"] and (i in self._data):
-                if not validate_item(og_properties[i], self._data[i]):
-                    _errror("critical", i, "Required Element does not validate")
+        validate_fields = set(self._data.keys())
+
+        # make sure that everything in OG_PROPERTIES:
+        # 1) is present if required
+        # 2) is valid if not required
+        # 3) is valid if not required
+        for i in OG_PROPERTIES:
+            if OG_PROPERTIES[i]["required"]:
+                if i not in self._data:
+                    _set_error("critical", i, "Missing Required Element")
+                else:
+                    # required; check validity
+                    validate_fields.remove(i)
+                    if not validate_item(OG_PROPERTIES[i], self._data[i]):
+                        _set_error("critical", i, "Required Element does not validate")
             else:
+                # not required; check validity
                 if i in self._data:
-                    if not validate_item(og_properties[i], self._data[i]):
-                        _errror(
+                    validate_fields.remove(i)
+                    if not validate_item(OG_PROPERTIES[i], self._data[i]):
+                        _set_error(
                             "recommended", i, "non-required Element does not validate"
                         )
 
-        if (
-            "og:type" not in errors["critical"]
-            and "og:type" not in errors["recommended"]
-        ):
-            _error = None
-            if schema1:
-                if (
-                    self._data["og:type"]
-                    not in og_properties["og:type"]["valid_types-1"]
-                ):
-                    _errror("critical", "og:type", "Invalid og:type")
-            elif schema2:
-                if (
-                    self._data["og:type"]
-                    not in og_properties["og:type"]["valid_types-2"]
-                ):
-                    _errror("critical", "og:type", "Invalid og:type")
-                for subtype in og_properties["og:type"]["valid_types-2"][
-                    self._data["og:type"]
-                ]["properties"]:
-                    info = og_properties["og:type"]["valid_types-2"][
-                        self._data["og:type"]
-                    ]
-                    info_dict = info["properties"][subtype]
-                    error = None
-                    value = None
-                    if subtype in self._data:
-                        value = self._data[subtype]
-                    if "required" in info and info["required"]:
-                        if subtype not in og_properties:
-                            _errror(
-                                "critical", "%s" % subtype, "Missing required subtype"
-                            )
-                        elif not validate_item(info_dict, value):
-                            _errror(
-                                "critical",
-                                "%s" % subtype,
-                                "Required subtype does not validate correctly",
-                            )
-                    else:
-                        if subtype not in self._data:
-                            _errror(
-                                "recommended",
-                                "%s" % subtype,
-                                "non-required subtype not included",
-                            )
+        og_type = self._data.get("og:type")
+
+        if schema1:
+            # schema1 only checks for validity of the valid type
+            if not og_type:
+                _set_error("critical", "og:type", "Missing og:type")
+            else:
+                if og_type not in OG_PROPERTIES["og:type"]["valid_types-1"]:
+                    _set_error("critical", "og:type", "Invalid og:type")
+
+        if schema2:
+            if not og_type:
+                _set_error("critical", "og:type", "Missing og:type")
+            else:
+                if og_type not in OG_PROPERTIES["og:type"]["valid_types-2"]:
+                    _set_error("critical", "og:type", "Invalid og:type")
+                else:
+                    # validate all the likely subtypes
+                    og_type_dict = OG_PROPERTIES["og:type"]["valid_types-2"][og_type]
+                    for subtype in OG_PROPERTIES["og:type"]["valid_types-2"][og_type][
+                        "properties"
+                    ]:
+                        subtype_dict = og_type_dict["properties"][subtype]
+                        value = None
+                        if subtype in self._data:
+                            value = self._data[subtype]
+                        if "required" in og_type_dict and og_type_dict["required"]:
+                            if subtype not in OG_PROPERTIES:
+                                _set_error(
+                                    "critical",
+                                    "%s" % subtype,
+                                    "Missing required subtype",
+                                )
+                            else:
+                                validate_fields.remove(subtype)
+                                if not validate_item(subtype_dict, value):
+                                    _set_error(
+                                        "critical",
+                                        "%s" % subtype,
+                                        "Required subtype does not validate correctly",
+                                    )
                         else:
-                            if not validate_item(info_dict, value):
-                                _errror(
+                            if subtype not in self._data:
+                                _set_error(
                                     "recommended",
                                     "%s" % subtype,
-                                    "non-required subtype does not validate correctly",
+                                    "non-required subtype not included",
                                 )
+                            else:
+                                validate_fields.remove(subtype)
+                                if not validate_item(subtype_dict, value):
+                                    _set_error(
+                                        "recommended",
+                                        "%s" % subtype,
+                                        "non-required subtype does not validate correctly",
+                                    )
 
+        if validate_fields:
+            errors["not_validated"] = list(validate_fields)
         self._errors = errors
         if errors["critical"]:
             return False
         return True
 
-    def errors(self):
+    def errors(self) -> OGErrors:
+        if self._errors is None:
+            raise ValueError("You must call `.validate()` first")
         return self._errors
 
-    def as_html(self, debug=False):
-        output = []
+    def as_html(
+        self,
+        debug: bool = False,
+    ) -> str:
+        _output = []
         _keys = sorted(self._data.keys())
+        if self._errors is None:
+            return ""
         for k in _keys:
             v = self._data[k]
-            _error = u""
+            _error = ""
             if debug:
                 if k in self._errors["critical"]:
-                    _error = u' critical-error="%s"' % html_attribute_escape(
+                    _error = ' critical-error="%s"' % html_attribute_escape(
                         self._errors["critical"][k]
                     )
                 elif k in self._errors["recommended"]:
-                    _error = u' recommended-error="%s"' % html_attribute_escape(
+                    _error = ' recommended-error="%s"' % html_attribute_escape(
                         self._errors["recommended"][k]
                     )
             if isinstance(v, list):
                 for i in v:
-                    output.append(
-                        u"""<meta property="%s" content="%s"%s/>"""
+                    i = stringify(i)
+                    _output.append(
+                        """<meta property="%s" content="%s"%s/>"""
                         % (html_attribute_escape(k), html_attribute_escape(i), _error)
                     )
             else:
-                output.append(
-                    u"""<meta property="%s" content="%s"%s/>"""
+                v = stringify(v)
+                _output.append(
+                    """<meta property="%s" content="%s"%s/>"""
                     % (html_attribute_escape(k), html_attribute_escape(v), _error)
                 )
-        output = u"\n".join(output)
+        output = "\n".join(_output)
         return output
-
-
-if __name__ == "__main__":
-    a = OpenGraphItem()
-    a.set("og:title", "MyWebsite")
-    a.set("og:type", "article")
-    a.set_many(
-        (
-            ("og:url", "http://f.me"),
-            ("og:image", "http://f.me/a.png"),
-            ("article:author", "abc"),
-            ("article:published_time", "2012-01-10"),
-        )
-    )
-    status = a.validate()
-    if status:
-        print("object ok")
-    else:
-        print("object not ok")
-    print(a.as_html(debug=True))
```

### Comparing `opengraph_writer-0.3.3/src/opengraph_writer.egg-info/PKG-INFO` & `opengraph_writer-0.4.0/src/opengraph_writer.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,87 @@
 Metadata-Version: 2.1
 Name: opengraph-writer
-Version: 0.3.3
+Version: 0.4.0
 Summary: Lightweight OpenGraph support for writing and validating objects.
 Home-page: https://github.com/jvanasco/opengraph_writer
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: opengraph_writer
-        ================
-        
-        ![Python package](https://github.com/jvanasco/opengraph_writer/workflows/Python%20package/badge.svg)
-        
-        About
-        =====
-        
-        This library was created to both manage writing OpenGraph data, and perform
-        lightweight verifications for offline debugging.
-        
-        This library does the following:
-        
-        - CREATE an object to stash OGP data
-        - VALIDATE the data, offering debug information on the object
-        - RENDER the object as html, and optionally include debug data on incorrect elements
-        
-        
-        This is currently aimed at "single object page data". It is not necessarily
-        with multi-value items yet (such as multiple profiles or tracks on a single page).
-        
-        Most of the validation routines were derived from regexing the `https://ogp.me`
-        site into a Python dict, and researching what they are supposed to do.
-        The validation routes themselves are super trivial.
-        
-        At the time of initially writing this library, and several checks ever since, the
-        specification on  the `https://ogp.me` seems out of date. 
-        
-        In practice, Facebook's "premier" partners seem to all be using URLs which point 
-        to certain data , however there aren't any guidelines for this within the
-        public OGP spec.
-        
-        An example would be on the Spotify integration: when looking at a `SONG`, the
-        `ARTIST` and `ALBUM` refer to URLs which contain the relevant data.
-        
-        Documentation
-        =============
-        
-        The Python file contains extensive inline documentation.
-        
-        
-        Contributions Welcome!
-        ======================
-        
-        If anyone wants to fork and tackle the multiple value problem, please do.
-        
-        
-        Framework Support: Pyramid
-        ==========================
-        
-        This package offers an includeme for Pyramid to set up an `opengraph_item`
-        as a `@reify` request method.
-        
-        Simply update your application:
-        
-        	config.include("opengraph_writer.pyramid_helpers")
-        
-        And your `Request` objects will be extended as such:
-        
-            request.opengraph_item
-            
-            
-            
-        
-        
 Keywords: facebook opengraph open graph web pyramid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+opengraph_writer
+================
+
+![Python package](https://github.com/jvanasco/opengraph_writer/workflows/Python%20package/badge.svg)
+
+About
+=====
+
+This library was created to both manage writing OpenGraph data, and perform
+lightweight verifications for offline debugging.
+
+This library does the following:
+
+- CREATE an object to stash OGP data
+- VALIDATE the data, offering debug information on the object
+- RENDER the object as html, and optionally include debug data on incorrect elements
+
+This is currently aimed at "single object page data". It is not necessarily
+with multi-value items yet (such as multiple profiles or tracks on a single page).
+
+Most of the validation routines were derived from regexing the `https://ogp.me`
+site into a Python dict, and researching what they are supposed to do.
+The validation routes themselves are super trivial.
+
+At the time of initially writing this library, and several checks ever since, the
+specification on  the `https://ogp.me` seems out of date. 
+
+In practice, Facebook's "premier" partners seem to all be using URLs which point 
+to certain data , however there aren't any guidelines for this within the
+public OGP spec.
+
+An example would be on the Spotify integration: when looking at a `SONG`, the
+`ARTIST` and `ALBUM` refer to URLs which contain the relevant data.
+
+Documentation
+=============
+
+The Python file contains extensive inline documentation.
+
+
+Contributions Welcome!
+======================
+
+If anyone wants to fork and tackle the multiple value problem, please do.
+
+
+Framework Support: Pyramid
+==========================
+
+This package offers an includeme for Pyramid to set up an `opengraph_item`
+as a `@reify` request method.
+
+Simply update your application:
+
+	config.include("opengraph_writer.pyramid_helpers")
+
+And your `Request` objects will be extended as such:
+
+    request.opengraph_item
+    
+    
+    
+
```

### Comparing `opengraph_writer-0.3.3/tests/test_pyramid_integration.py` & `opengraph_writer-0.4.0/tests/test_pyramid_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # stdlib
 import unittest
 
-# local package to test
-import opengraph_writer
-
-# pyramid testing requirements
+# pyramid testing requirements; pypi
 from pyramid import testing
 from pyramid.interfaces import IRequestExtensions
-from webob.multidict import MultiDict
 
+# from webob.multidict import MultiDict
+
+# local package
+import opengraph_writer
 
 # ==============================================================================
 
 
 class TestSetupSimple(unittest.TestCase):
     def setUp(self):
         self.config = testing.setUp()
 
         # grab the config object, then modify in place
         settings = self.config.get_settings()
+        # mare sure we have it...
+        self.assertIsNotNone(settings)
+
         self.config.include("opengraph_writer.pyramid_helpers")
         self.context = testing.DummyResource()
         self.request = testing.DummyRequest()
 
         # mare sure we have it...
         exts = self.config.registry.getUtility(IRequestExtensions)
         self.assertTrue("opengraph_item" in exts.descriptors)
```

