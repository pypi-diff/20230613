# Comparing `tmp/impmagic-0.1.2.tar.gz` & `tmp/impmagic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impmagic-0.1.2.tar", last modified: Fri Mar 24 11:09:56 2023, max compression
+gzip compressed data, was "impmagic-0.1.3.tar", last modified: Tue Jun 13 08:04:48 2023, max compression
```

## Comparing `impmagic-0.1.2.tar` & `impmagic-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 11:09:56.197000 impmagic-0.1.2/
--rw-rw-rw-   0        0        0     1106 2023-02-22 09:09:50.000000 impmagic-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3084 2023-03-24 11:09:56.187000 impmagic-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2435 2023-02-22 09:43:02.000000 impmagic-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 11:09:56.103000 impmagic-0.1.2/impmagic/
--rw-rw-rw-   0        0        0       23 2023-02-13 18:26:53.000000 impmagic-0.1.2/impmagic/__init__.py
--rw-rw-rw-   0        0        0     5618 2023-03-24 11:09:20.000000 impmagic-0.1.2/impmagic/impmagic.py
-drwxrwxrwx   0        0        0        0 2023-03-24 11:09:56.173000 impmagic-0.1.2/impmagic.egg-info/
--rw-rw-rw-   0        0        0     3084 2023-03-24 11:09:55.000000 impmagic-0.1.2/impmagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-03-24 11:09:55.000000 impmagic-0.1.2/impmagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 11:09:55.000000 impmagic-0.1.2/impmagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-24 11:09:55.000000 impmagic-0.1.2/impmagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 11:09:56.194000 impmagic-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:48.969000 impmagic-0.1.3/
+-rw-rw-rw-   0        0        0     1106 2023-02-22 09:09:50.000000 impmagic-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3057 2023-06-13 08:04:48.965000 impmagic-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2435 2023-02-22 09:43:02.000000 impmagic-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:48.930000 impmagic-0.1.3/impmagic/
+-rw-rw-rw-   0        0        0       23 2023-03-07 21:49:54.000000 impmagic-0.1.3/impmagic/__init__.py
+-rw-rw-rw-   0        0        0     6226 2023-06-07 15:31:31.000000 impmagic-0.1.3/impmagic/impmagic.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:48.960000 impmagic-0.1.3/impmagic.egg-info/
+-rw-rw-rw-   0        0        0     3057 2023-06-13 08:04:48.000000 impmagic-0.1.3/impmagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-06-13 08:04:48.000000 impmagic-0.1.3/impmagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:04:48.000000 impmagic-0.1.3/impmagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 08:04:48.000000 impmagic-0.1.3/impmagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:04:48.968000 impmagic-0.1.3/setup.cfg
```

### Comparing `impmagic-0.1.2/LICENSE` & `impmagic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `impmagic-0.1.2/PKG-INFO` & `impmagic-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: impmagic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Librairie pour l'importation optimisé de module python
 Home-page: https://github.com/ZephyrOff/impmagic
-Author: ZephyrOff <contact@apajak.fr>
+Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/impmagic
 Keywords: import module zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -75,7 +75,8 @@
 
 ### Utiliser un module sans l'importer
 Il est possible d'utiliser un module sans avoir besoin de l'importer grâce à la méthode get.
 ```python
 module = impmagic.get('os')
 module.mkdir(dir)
 ```
+
```

### Comparing `impmagic-0.1.2/README.md` & `impmagic-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `impmagic-0.1.2/impmagic/impmagic.py` & `impmagic-0.1.3/impmagic/impmagic.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,34 @@
 import inspect
 import sys
 
 if 'imp_cache' not in __main__.__dict__:
     __main__.__dict__['imp_cache'] = {}
 CACHE = __main__.__dict__['imp_cache']
 
+
 #Importation de module à partir d'un tuple ou d'une liste ou d'un str
-def load(data, func=None, globals=None):
+def load(data, func=None, globals_val=None):
+    #Pour supporter l'import des modules locaux
+    if "path" not in globals():
+        if not func:
+            frame = inspect.currentframe()
+            frame = frame.f_back # remonte d'un niveau dans la pile d'appels
+            path = frame.f_globals["__file__"] # récupère le chemin du fichier appelant
+            del frame
+        else:
+            path = inspect.getfile(func)
+
+        globals()['path'] = getattr(__import__('os', fromlist=['object']), 'path').dirname(path)
+        if globals()['path'] not in sys.path:
+            sys.path.append(globals()['path'])
+
     if not func:
-        if globals:
-            func = globals
+        if globals_val:
+            func = globals_val
         else:
             current_frame = inspect.currentframe()
             calling_frame = current_frame.f_back
             calling_globals = calling_frame.f_globals
             func = calling_globals
     else:
         func = func.__globals__
```

### Comparing `impmagic-0.1.2/impmagic.egg-info/PKG-INFO` & `impmagic-0.1.3/impmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: impmagic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Librairie pour l'importation optimisé de module python
 Home-page: https://github.com/ZephyrOff/impmagic
-Author: ZephyrOff <contact@apajak.fr>
+Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/impmagic
 Keywords: import module zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -75,7 +75,8 @@
 
 ### Utiliser un module sans l'importer
 Il est possible d'utiliser un module sans avoir besoin de l'importer grâce à la méthode get.
 ```python
 module = impmagic.get('os')
 module.mkdir(dir)
 ```
+
```

