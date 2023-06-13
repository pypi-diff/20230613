# Comparing `tmp/spade_bdi-0.2.2.tar.gz` & `tmp/spade_bdi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_bdi-0.2.2.tar", last modified: Fri Jun  3 15:56:55 2022, max compression
+gzip compressed data, was "spade_bdi-0.3.0.tar", last modified: Tue Jun 13 14:29:40 2023, max compression
```

## Comparing `spade_bdi-0.2.2.tar` & `spade_bdi-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.615517 spade_bdi-0.2.2/
--rw-r--r--   0 jpalanca   (501) staff       (20)      169 2019-06-13 15:26:28.000000 spade_bdi-0.2.2/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3542 2020-02-24 11:13:27.000000 spade_bdi-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1098 2022-06-03 15:56:21.000000 spade_bdi-0.2.2/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1575 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)      262 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/MANIFEST.in
--rw-r--r--   0 jpalanca   (501) staff       (20)     6787 2022-06-03 15:56:55.615757 spade_bdi-0.2.2/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     3173 2022-06-03 15:56:21.000000 spade_bdi-0.2.2/README.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.603700 spade_bdi-0.2.2/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)      610 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/Makefile
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.592176 spade_bdi-0.2.2/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.592320 spade_bdi-0.2.2/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.610568 spade_bdi-0.2.2/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)      673 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 jpalanca   (501) staff       (20)      756 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      829 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      641 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/comment.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      222 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      202 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/down.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      214 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      203 2019-05-16 16:07:28.000000 spade_bdi-0.2.2/docs/_build/html/_static/up.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/authors.rst
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     4897 2020-02-24 11:13:27.000000 spade_bdi-0.2.2/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/history.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      306 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1142 2020-02-24 11:13:27.000000 spade_bdi-0.2.2/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      771 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/make.bat
--rw-r--r--   0 jpalanca   (501) staff       (20)       64 2020-02-24 11:04:25.000000 spade_bdi-0.2.2/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2019-06-13 15:04:07.000000 spade_bdi-0.2.2/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      312 2020-02-24 11:04:25.000000 spade_bdi-0.2.2/docs/spade_bdi.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1242 2020-02-24 11:13:27.000000 spade_bdi-0.2.2/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      452 2022-06-03 15:56:55.616708 spade_bdi-0.2.2/setup.cfg
--rw-r--r--   0 jpalanca   (501) staff       (20)     1948 2022-06-03 15:56:21.000000 spade_bdi-0.2.2/setup.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.611595 spade_bdi-0.2.2/spade_bdi/
--rw-r--r--   0 jpalanca   (501) staff       (20)      198 2022-06-03 15:56:21.000000 spade_bdi-0.2.2/spade_bdi/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     9057 2022-06-03 15:56:14.000000 spade_bdi-0.2.2/spade_bdi/bdi.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.614568 spade_bdi-0.2.2/spade_bdi.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     6787 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)      966 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)       45 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       10 2022-06-03 15:56:55.000000 spade_bdi-0.2.2/spade_bdi.egg-info/top_level.txt
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2022-06-03 15:56:55.614966 spade_bdi-0.2.2/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)      101 2019-06-13 15:25:36.000000 spade_bdi-0.2.2/tests/test_spade_bdi.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.344498 spade_bdi-0.3.0/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      169 2019-06-13 15:26:28.000000 spade_bdi-0.3.0/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3542 2020-02-24 11:13:27.000000 spade_bdi-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1163 2023-06-13 14:29:31.000000 spade_bdi-0.3.0/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1575 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      262 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6872 2023-06-13 14:29:40.344920 spade_bdi-0.3.0/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3153 2023-06-13 14:29:31.000000 spade_bdi-0.3.0/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.327681 spade_bdi-0.3.0/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      610 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.314242 spade_bdi-0.3.0/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.314371 spade_bdi-0.3.0/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.337415 spade_bdi-0.3.0/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      673 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 jpalanca   (501) staff       (20)      756 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      829 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      641 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/comment.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      222 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      202 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/down.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      214 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      203 2019-05-16 16:07:28.000000 spade_bdi-0.3.0/docs/_build/html/_static/up.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     4897 2020-02-24 11:13:27.000000 spade_bdi-0.3.0/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/contributing.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/history.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      306 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1142 2020-02-24 11:13:27.000000 spade_bdi-0.3.0/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      771 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)       64 2020-02-24 11:04:25.000000 spade_bdi-0.3.0/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2019-06-13 15:04:07.000000 spade_bdi-0.3.0/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      312 2020-02-24 11:04:25.000000 spade_bdi-0.3.0/docs/spade_bdi.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1242 2020-02-24 11:13:27.000000 spade_bdi-0.3.0/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      452 2023-06-13 14:29:40.346147 spade_bdi-0.3.0/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1948 2023-06-13 14:29:31.000000 spade_bdi-0.3.0/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.338847 spade_bdi-0.3.0/spade_bdi/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      198 2023-06-13 14:29:31.000000 spade_bdi-0.3.0/spade_bdi/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     9057 2022-06-03 15:56:14.000000 spade_bdi-0.3.0/spade_bdi/bdi.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.343019 spade_bdi-0.3.0/spade_bdi.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     6872 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)      966 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)       45 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       10 2023-06-13 14:29:40.000000 spade_bdi-0.3.0/spade_bdi.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-13 14:29:40.343707 spade_bdi-0.3.0/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      101 2019-06-13 15:25:36.000000 spade_bdi-0.3.0/tests/test_spade_bdi.py
```

### Comparing `spade_bdi-0.2.2/CONTRIBUTING.rst` & `spade_bdi-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/HISTORY.rst` & `spade_bdi-0.3.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.3.0 (2023-06-13)
+------------------
+
+* Updated to SPADE 3.3.0.
+
 0.2.2 (2022-06-03)
 ------------------
 
 * Added exception when belief is not initialized.
 * Improved examples.
 * Improved documentation.
 
@@ -36,15 +41,15 @@
 * Allow to receive messages with lists of lists.
 * Fixed readme.
 
 0.1.1 (2019-06-18)
 ------------------
 
 * Moved from pyson to python-agentspeak
-* Added some helpers like pause_bdi, resume_bdi. 
+* Added some helpers like pause_bdi, resume_bdi.
 * Now the asl file in the constructor is mandatory.
 * Allow to send tell messages with no args.
 * Allow sending messages with variables.
 * Extended the examples.
 
 0.1.0 (2019-03-09)
 ------------------
```

### Comparing `spade_bdi-0.2.2/LICENSE` & `spade_bdi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/PKG-INFO` & `spade_bdi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spade_bdi
-Version: 0.2.2
+Version: 0.3.0
 Summary: Plugin for SPADE 3 MAS platform to implement BDI Agents.
 Home-page: https://github.com/javipalanca/spade_bdi
 Author: Sergio Frayle Pérez
 Author-email: sfp932705@gmail.com
 License: MIT License v3
 Description: =========
         Spade-BDI
@@ -12,15 +12,15 @@
         
         .. image:: https://img.shields.io/pypi/v/spade_bdi.svg
                 :target: https://pypi.python.org/pypi/spade
         
         .. image:: https://img.shields.io/pypi/pyversions/spade_bdi.svg
             :target: https://pypi.python.org/pypi/spade_bdi
         
-        .. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+        .. image:: https://img.shields.io/pypi/l/spade_bdi
             :target: https://opensource.org/licenses/MIT
             :alt: MIT License
         
         .. image:: https://pepy.tech/badge/spade_bdi
             :target: https://pepy.tech/project/spade_bdi
             :alt: Downloads
         
@@ -106,18 +106,18 @@
             a.start()
         
             a.bdi.set_belief("car", "blue", "big")
             a.bdi.print_beliefs()
         
             print(a.bdi.get_belief("car"))
             a.bdi.print_beliefs()
-            
+        
             a.bdi.remove_belief("car", 'blue', "big")
             a.bdi.print_beliefs()
-            
+        
             print(a.bdi.get_beliefs())
             a.bdi.set_belief("car", 'yellow')
         
         
         basic.asl::
         
             !start.
@@ -127,15 +127,15 @@
                 .a_function(3,W);
                 .print("w =", W);
                 literal_function(red,Y);
                 .print("Y =", Y);
                 .custom_action(8);
                 +truck(blue).
         
-            +car(Color) 
+            +car(Color)
              <- .print("The car is ",Color).
         
         
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
@@ -144,14 +144,19 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.3.0 (2023-06-13)
+        ------------------
+        
+        * Updated to SPADE 3.3.0.
+        
         0.2.2 (2022-06-03)
         ------------------
         
         * Added exception when belief is not initialized.
         * Improved examples.
         * Improved documentation.
         
@@ -182,15 +187,15 @@
         * Allow to receive messages with lists of lists.
         * Fixed readme.
         
         0.1.1 (2019-06-18)
         ------------------
         
         * Moved from pyson to python-agentspeak
-        * Added some helpers like pause_bdi, resume_bdi. 
+        * Added some helpers like pause_bdi, resume_bdi.
         * Now the asl file in the constructor is mandatory.
         * Allow to send tell messages with no args.
         * Allow sending messages with variables.
         * Extended the examples.
         
         0.1.0 (2019-03-09)
         ------------------
```

### Comparing `spade_bdi-0.2.2/README.rst` & `spade_bdi-0.3.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 .. image:: https://img.shields.io/pypi/v/spade_bdi.svg
         :target: https://pypi.python.org/pypi/spade
 
 .. image:: https://img.shields.io/pypi/pyversions/spade_bdi.svg
     :target: https://pypi.python.org/pypi/spade_bdi
 
-.. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+.. image:: https://img.shields.io/pypi/l/spade_bdi
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://pepy.tech/badge/spade_bdi
     :target: https://pepy.tech/project/spade_bdi
     :alt: Downloads
 
@@ -98,18 +98,18 @@
     a.start()
 
     a.bdi.set_belief("car", "blue", "big")
     a.bdi.print_beliefs()
 
     print(a.bdi.get_belief("car"))
     a.bdi.print_beliefs()
-    
+
     a.bdi.remove_belief("car", 'blue', "big")
     a.bdi.print_beliefs()
-    
+
     print(a.bdi.get_beliefs())
     a.bdi.set_belief("car", 'yellow')
 
 
 basic.asl::
 
     !start.
@@ -119,15 +119,15 @@
         .a_function(3,W);
         .print("w =", W);
         literal_function(red,Y);
         .print("Y =", Y);
         .custom_action(8);
         +truck(blue).
 
-    +car(Color) 
+    +car(Color)
      <- .print("The car is ",Color).
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
```

### Comparing `spade_bdi-0.2.2/docs/Makefile` & `spade_bdi-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/_build/html/_static/ajax-loader.gif` & `spade_bdi-0.3.0/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/_build/html/_static/comment-bright.png` & `spade_bdi-0.3.0/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/_build/html/_static/comment-close.png` & `spade_bdi-0.3.0/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/_build/html/_static/comment.png` & `spade_bdi-0.3.0/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/conf.py` & `spade_bdi-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/installation.rst` & `spade_bdi-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/make.bat` & `spade_bdi-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/docs/usage.rst` & `spade_bdi-0.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/setup.py` & `spade_bdi-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     keywords='spade_bdi',
     name='spade_bdi',
     packages=find_packages(include=['spade_bdi']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/javipalanca/spade_bdi',
-    version='0.2.2',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `spade_bdi-0.2.2/spade_bdi/bdi.py` & `spade_bdi-0.3.0/spade_bdi/bdi.py`

 * *Files identical despite different names*

### Comparing `spade_bdi-0.2.2/spade_bdi.egg-info/PKG-INFO` & `spade_bdi-0.3.0/spade_bdi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spade-bdi
-Version: 0.2.2
+Version: 0.3.0
 Summary: Plugin for SPADE 3 MAS platform to implement BDI Agents.
 Home-page: https://github.com/javipalanca/spade_bdi
 Author: Sergio Frayle Pérez
 Author-email: sfp932705@gmail.com
 License: MIT License v3
 Description: =========
         Spade-BDI
@@ -12,15 +12,15 @@
         
         .. image:: https://img.shields.io/pypi/v/spade_bdi.svg
                 :target: https://pypi.python.org/pypi/spade
         
         .. image:: https://img.shields.io/pypi/pyversions/spade_bdi.svg
             :target: https://pypi.python.org/pypi/spade_bdi
         
-        .. image:: https://img.shields.io/apm/l/atomic-design-ui.svg?
+        .. image:: https://img.shields.io/pypi/l/spade_bdi
             :target: https://opensource.org/licenses/MIT
             :alt: MIT License
         
         .. image:: https://pepy.tech/badge/spade_bdi
             :target: https://pepy.tech/project/spade_bdi
             :alt: Downloads
         
@@ -106,18 +106,18 @@
             a.start()
         
             a.bdi.set_belief("car", "blue", "big")
             a.bdi.print_beliefs()
         
             print(a.bdi.get_belief("car"))
             a.bdi.print_beliefs()
-            
+        
             a.bdi.remove_belief("car", 'blue', "big")
             a.bdi.print_beliefs()
-            
+        
             print(a.bdi.get_beliefs())
             a.bdi.set_belief("car", 'yellow')
         
         
         basic.asl::
         
             !start.
@@ -127,15 +127,15 @@
                 .a_function(3,W);
                 .print("w =", W);
                 literal_function(red,Y);
                 .print("Y =", Y);
                 .custom_action(8);
                 +truck(blue).
         
-            +car(Color) 
+            +car(Color)
              <- .print("The car is ",Color).
         
         
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
@@ -144,14 +144,19 @@
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.3.0 (2023-06-13)
+        ------------------
+        
+        * Updated to SPADE 3.3.0.
+        
         0.2.2 (2022-06-03)
         ------------------
         
         * Added exception when belief is not initialized.
         * Improved examples.
         * Improved documentation.
         
@@ -182,15 +187,15 @@
         * Allow to receive messages with lists of lists.
         * Fixed readme.
         
         0.1.1 (2019-06-18)
         ------------------
         
         * Moved from pyson to python-agentspeak
-        * Added some helpers like pause_bdi, resume_bdi. 
+        * Added some helpers like pause_bdi, resume_bdi.
         * Now the asl file in the constructor is mandatory.
         * Allow to send tell messages with no args.
         * Allow sending messages with variables.
         * Extended the examples.
         
         0.1.0 (2019-03-09)
         ------------------
```

### Comparing `spade_bdi-0.2.2/spade_bdi.egg-info/SOURCES.txt` & `spade_bdi-0.3.0/spade_bdi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

