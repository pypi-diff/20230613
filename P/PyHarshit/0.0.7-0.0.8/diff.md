# Comparing `tmp/PyHarshit-0.0.7.tar.gz` & `tmp/PyHarshit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHarshit-0.0.7.tar", last modified: Thu Jun  1 15:13:59 2023, max compression
+gzip compressed data, was "PyHarshit-0.0.8.tar", last modified: Tue Jun 13 04:53:37 2023, max compression
```

## Comparing `PyHarshit-0.0.7.tar` & `PyHarshit-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/PKG-INFO
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/__init__.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit/tg/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     4125 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/Control.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)    12360 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/FasterTg.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1803 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/Functions.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3009 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/extractor.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      478 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/tools.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     2761 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/uploader.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      174 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tg/utils.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/PyHarshit/tools/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/anim.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/boolset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/charset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1301 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/fiverr.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/maths.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      887 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/PyHarshit/tools/utils.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-01 15:13:59.104886 PyHarshit-0.0.7/PyHarshit.egg-info/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/PKG-INFO
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      581 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/SOURCES.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/dependency_links.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      119 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/requires.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-06-01 15:13:59.000000 PyHarshit-0.0.7/PyHarshit.egg-info/top_level.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      564 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/README.md
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-06-01 15:13:59.108886 PyHarshit-0.0.7/setup.cfg
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-06-01 15:13:13.000000 PyHarshit-0.0.7/setup.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.792955 PyHarshit-0.0.8/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      963 2023-06-13 04:53:37.792955 PyHarshit-0.0.8/PKG-INFO
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.788955 PyHarshit-0.0.8/PyHarshit/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/__init__.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.788955 PyHarshit-0.0.8/PyHarshit/db/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     9064 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/db/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     9065 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/db/save.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3226 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/db/tests.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.792955 PyHarshit-0.0.8/PyHarshit/tg/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     4125 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/Control.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)    12360 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/FasterTg.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1803 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/Functions.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3009 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/extractor.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      478 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/tools.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     2761 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/uploader.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      174 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tg/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.792955 PyHarshit-0.0.8/PyHarshit/tools/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/anim.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/boolset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/charset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1301 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/fiverr.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/maths.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      887 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/PyHarshit/tools/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-06-13 04:53:37.788955 PyHarshit-0.0.8/PyHarshit.egg-info/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      963 2023-06-13 04:53:37.000000 PyHarshit-0.0.8/PyHarshit.egg-info/PKG-INFO
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      649 2023-06-13 04:53:37.000000 PyHarshit-0.0.8/PyHarshit.egg-info/SOURCES.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-06-13 04:53:37.000000 PyHarshit-0.0.8/PyHarshit.egg-info/dependency_links.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      209 2023-06-13 04:53:37.000000 PyHarshit-0.0.8/PyHarshit.egg-info/requires.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-06-13 04:53:37.000000 PyHarshit-0.0.8/PyHarshit.egg-info/top_level.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      749 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/README.md
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-06-13 04:53:37.792955 PyHarshit-0.0.8/setup.cfg
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-06-13 04:53:06.000000 PyHarshit-0.0.8/setup.py
```

### Comparing `PyHarshit-0.0.7/PKG-INFO` & `PyHarshit-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHarshit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utlity file for my codes
 Author: Harshit Shrivastav
 Author-email: itsharshit@yandex.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # just a utility files for my codes
@@ -44,7 +44,20 @@
 
 For using tg functions 
 ```
 from PyHarshit.tg import tgFunctions 
 
 tgFunctions.copy_msg(arguments_here)
 ```
+For using database
+```python
+>>> import PyHarshit.db as database
+>>> db = database.load('test.db', False)
+
+>>> db.set('key', 'value')
+
+>>> db.get('key')
+'value'
+
+>>> db.dump()
+True
+```
```

### Comparing `PyHarshit-0.0.7/PyHarshit/tg/Control.py` & `PyHarshit-0.0.8/PyHarshit/tg/Control.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tg/FasterTg.py` & `PyHarshit-0.0.8/PyHarshit/tg/FasterTg.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tg/Functions.py` & `PyHarshit-0.0.8/PyHarshit/tg/Functions.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tg/extractor.py` & `PyHarshit-0.0.8/PyHarshit/tg/extractor.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tg/uploader.py` & `PyHarshit-0.0.8/PyHarshit/tg/uploader.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tools/fiverr.py` & `PyHarshit-0.0.8/PyHarshit/tools/fiverr.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit/tools/utils.py` & `PyHarshit-0.0.8/PyHarshit/tools/utils.py`

 * *Files identical despite different names*

### Comparing `PyHarshit-0.0.7/PyHarshit.egg-info/PKG-INFO` & `PyHarshit-0.0.8/PyHarshit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHarshit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utlity file for my codes
 Author: Harshit Shrivastav
 Author-email: itsharshit@yandex.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # just a utility files for my codes
@@ -44,7 +44,20 @@
 
 For using tg functions 
 ```
 from PyHarshit.tg import tgFunctions 
 
 tgFunctions.copy_msg(arguments_here)
 ```
+For using database
+```python
+>>> import PyHarshit.db as database
+>>> db = database.load('test.db', False)
+
+>>> db.set('key', 'value')
+
+>>> db.get('key')
+'value'
+
+>>> db.dump()
+True
+```
```

### Comparing `PyHarshit-0.0.7/PyHarshit.egg-info/SOURCES.txt` & `PyHarshit-0.0.8/PyHarshit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 setup.py
 PyHarshit/__init__.py
 PyHarshit.egg-info/PKG-INFO
 PyHarshit.egg-info/SOURCES.txt
 PyHarshit.egg-info/dependency_links.txt
 PyHarshit.egg-info/requires.txt
 PyHarshit.egg-info/top_level.txt
+PyHarshit/db/__init__.py
+PyHarshit/db/save.py
+PyHarshit/db/tests.py
 PyHarshit/tg/Control.py
 PyHarshit/tg/FasterTg.py
 PyHarshit/tg/Functions.py
 PyHarshit/tg/__init__.py
 PyHarshit/tg/extractor.py
 PyHarshit/tg/tools.py
 PyHarshit/tg/uploader.py
```

### Comparing `PyHarshit-0.0.7/README.md` & `PyHarshit-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -35,7 +35,20 @@
 
 For using tg functions 
 ```
 from PyHarshit.tg import tgFunctions 
 
 tgFunctions.copy_msg(arguments_here)
 ```
+For using database
+```python
+>>> import PyHarshit.db as database
+>>> db = database.load('test.db', False)
+
+>>> db.set('key', 'value')
+
+>>> db.get('key')
+'value'
+
+>>> db.dump()
+True
+```
```

### Comparing `PyHarshit-0.0.7/setup.py` & `PyHarshit-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="PyHarshit",
-    version="0.0.7",
+    version="0.0.8",
     author="Harshit Shrivastav",
     author_email="itsharshit@yandex.com",
     description="Utlity file for my codes",
     long_description=page_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

