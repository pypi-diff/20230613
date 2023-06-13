# Comparing `tmp/pyncraft-0.2.0.tar.gz` & `tmp/pyncraft-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncraft-0.2.0.tar", last modified: Sun Jun 11 03:08:48 2023, max compression
+gzip compressed data, was "pyncraft-0.2.1.tar", last modified: Tue Jun 13 20:46:52 2023, max compression
```

## Comparing `pyncraft-0.2.0.tar` & `pyncraft-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.364900 pyncraft-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1334 2023-06-11 03:08:48.363909 pyncraft-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-06-07 01:53:06.000000 pyncraft-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.318065 pyncraft-0.2.0/pyncraft/
--rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/__init__.py
--rw-rw-rw-   0        0        0     2993 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/block.py
--rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.2.0/pyncraft/connection.py
--rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.2.0/pyncraft/entity.py
--rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.2.0/pyncraft/event.py
--rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.2.0/pyncraft/logger.py
--rw-rw-rw-   0        0        0    14748 2023-06-10 03:53:51.000000 pyncraft-0.2.0/pyncraft/minecraft.py
--rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.2.0/pyncraft/settings.py
--rw-rw-rw-   0        0        0      487 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/util.py
--rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.2.0/pyncraft/vec3.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:08:48.360463 pyncraft-0.2.0/pyncraft.egg-info/
--rw-rw-rw-   0        0        0     1334 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-11 03:08:48.000000 pyncraft-0.2.0/pyncraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 03:08:47.000000 pyncraft-0.2.0/pyncraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 03:08:48.366954 pyncraft-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     9508 2023-06-11 02:56:37.000000 pyncraft-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:46:52.429607 pyncraft-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-06 03:05:16.000000 pyncraft-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1295 2023-06-13 20:46:52.428606 pyncraft-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-07 01:53:06.000000 pyncraft-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 20:46:52.392294 pyncraft-0.2.1/pyncraft/
+-rw-rw-rw-   0        0        0        0 2023-06-02 17:29:00.000000 pyncraft-0.2.1/pyncraft/__init__.py
+-rw-rw-rw-   0        0        0     4019 2023-06-13 03:27:26.000000 pyncraft-0.2.1/pyncraft/block.py
+-rw-rw-rw-   0        0        0     1956 2023-06-03 02:32:24.000000 pyncraft-0.2.1/pyncraft/connection.py
+-rw-rw-rw-   0        0        0     3404 2023-06-02 17:29:01.000000 pyncraft-0.2.1/pyncraft/entity.py
+-rw-rw-rw-   0        0        0     1807 2023-06-02 17:29:01.000000 pyncraft-0.2.1/pyncraft/event.py
+-rw-rw-rw-   0        0        0      777 2023-06-02 18:21:46.000000 pyncraft-0.2.1/pyncraft/logger.py
+-rw-rw-rw-   0        0        0    14748 2023-06-10 03:53:51.000000 pyncraft-0.2.1/pyncraft/minecraft.py
+-rw-rw-rw-   0        0        0    42041 2023-06-12 15:13:47.000000 pyncraft-0.2.1/pyncraft/minecraftstuff.py
+-rw-rw-rw-   0        0        0      159 2023-06-02 18:22:17.000000 pyncraft-0.2.1/pyncraft/settings.py
+-rw-rw-rw-   0        0        0      559 2023-06-13 20:35:31.000000 pyncraft-0.2.1/pyncraft/util.py
+-rw-rw-rw-   0        0        0     2458 2023-06-02 17:29:00.000000 pyncraft-0.2.1/pyncraft/vec3.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:46:52.426607 pyncraft-0.2.1/pyncraft.egg-info/
+-rw-rw-rw-   0        0        0     1295 2023-06-13 20:46:52.000000 pyncraft-0.2.1/pyncraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-06-13 20:46:52.000000 pyncraft-0.2.1/pyncraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 20:46:52.000000 pyncraft-0.2.1/pyncraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-13 20:46:52.000000 pyncraft-0.2.1/pyncraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 20:46:52.000000 pyncraft-0.2.1/pyncraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 20:46:52.431606 pyncraft-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     9508 2023-06-13 20:36:22.000000 pyncraft-0.2.1/setup.py
```

### Comparing `pyncraft-0.2.0/LICENSE` & `pyncraft-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/PKG-INFO` & `pyncraft-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pyncraft
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to minecraft + pyncraft bukkit plugin
 Home-page: https://github.com/jdeast/pyncraft
 Author: Jason Eastman
 Author-email: jdeast@gmail.com
-License: UNKNOWN
 Keywords: minecraft,plugin,scratch,java,bukkit
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -22,8 +20,7 @@
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python API to Minecraft that works with the [FruitJuice](https://github.com/jdeast/FruitJuice) Bukkit plugin to enable a python and/or scratch programming interface.
 
 See [FruitJuice/README_server_setup.md](https://github.com/jdeast/FruitJuice/blob/master/README_server_setup.md) for instructions to set up your own python/scratch server that works on java or bedrock.
-
```

### Comparing `pyncraft-0.2.0/pyncraft/connection.py` & `pyncraft-0.2.1/pyncraft/connection.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft/entity.py` & `pyncraft-0.2.1/pyncraft/entity.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft/event.py` & `pyncraft-0.2.1/pyncraft/event.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft/logger.py` & `pyncraft-0.2.1/pyncraft/logger.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft/minecraft.py` & `pyncraft-0.2.1/pyncraft/minecraft.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft/vec3.py` & `pyncraft-0.2.1/pyncraft/vec3.py`

 * *Files identical despite different names*

### Comparing `pyncraft-0.2.0/pyncraft.egg-info/PKG-INFO` & `pyncraft-0.2.1/pyncraft.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pyncraft
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to minecraft + pyncraft bukkit plugin
 Home-page: https://github.com/jdeast/pyncraft
 Author: Jason Eastman
 Author-email: jdeast@gmail.com
-License: UNKNOWN
 Keywords: minecraft,plugin,scratch,java,bukkit
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -22,8 +20,7 @@
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A Python API to Minecraft that works with the [FruitJuice](https://github.com/jdeast/FruitJuice) Bukkit plugin to enable a python and/or scratch programming interface.
 
 See [FruitJuice/README_server_setup.md](https://github.com/jdeast/FruitJuice/blob/master/README_server_setup.md) for instructions to set up your own python/scratch server that works on java or bedrock.
-
```

### Comparing `pyncraft-0.2.0/setup.py` & `pyncraft-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.2.0',  # Required
+    version='0.2.1',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python interface to minecraft + pyncraft bukkit plugin',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

