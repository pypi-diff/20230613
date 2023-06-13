# Comparing `tmp/dft2kp-0.0.1.tar.gz` & `tmp/dft2kp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dft2kp-0.0.1.tar", last modified: Tue Jun 13 19:59:59 2023, max compression
+gzip compressed data, was "dft2kp-0.0.2.tar", last modified: Tue Jun 13 21:34:00 2023, max compression
```

## Comparing `dft2kp-0.0.1.tar` & `dft2kp-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 19:59:59.931478 dft2kp-0.0.1/
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      539 2023-06-13 19:42:05.000000 dft2kp-0.0.1/AUTHORS.md
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    35060 2023-06-13 19:42:08.000000 dft2kp-0.0.1/LICENSE
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1357 2023-06-13 19:59:59.931478 dft2kp-0.0.1/PKG-INFO
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1017 2023-06-13 19:42:08.000000 dft2kp-0.0.1/README.md
-drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 19:59:59.931478 dft2kp-0.0.1/dft2kp.egg-info/
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1357 2023-06-13 19:59:59.000000 dft2kp-0.0.1/dft2kp.egg-info/PKG-INFO
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      380 2023-06-13 19:59:59.000000 dft2kp-0.0.1/dft2kp.egg-info/SOURCES.txt
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)        1 2023-06-13 19:59:59.000000 dft2kp-0.0.1/dft2kp.egg-info/dependency_links.txt
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       82 2023-06-13 19:59:59.000000 dft2kp-0.0.1/dft2kp.egg-info/requires.txt
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)        9 2023-06-13 19:59:59.000000 dft2kp-0.0.1/dft2kp.egg-info/top_level.txt
-drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 19:59:59.931478 dft2kp-0.0.1/pydft2kp/
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      349 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/__init__.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       21 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/__version.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1652 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/constants.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    26892 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/irrepwrapper.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    24083 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/lowdin.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    13560 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/qe_aux.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     5596 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/qsymmwrapper.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    17404 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/rotatebasis.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     5698 2023-06-13 19:42:08.000000 dft2kp-0.0.1/pydft2kp/util.py
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       38 2023-06-13 19:59:59.931478 dft2kp-0.0.1/setup.cfg
--rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      844 2023-06-13 19:48:50.000000 dft2kp-0.0.1/setup.py
+drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 21:34:00.762756 dft2kp-0.0.2/
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      539 2023-06-13 19:42:05.000000 dft2kp-0.0.2/AUTHORS.md
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    35060 2023-06-13 19:42:08.000000 dft2kp-0.0.2/LICENSE
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1357 2023-06-13 21:34:00.762756 dft2kp-0.0.2/PKG-INFO
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1017 2023-06-13 19:42:08.000000 dft2kp-0.0.2/README.md
+drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 21:34:00.762756 dft2kp-0.0.2/dft2kp.egg-info/
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1357 2023-06-13 21:34:00.000000 dft2kp-0.0.2/dft2kp.egg-info/PKG-INFO
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      380 2023-06-13 21:34:00.000000 dft2kp-0.0.2/dft2kp.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)        1 2023-06-13 21:34:00.000000 dft2kp-0.0.2/dft2kp.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       82 2023-06-13 21:34:00.000000 dft2kp-0.0.2/dft2kp.egg-info/requires.txt
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)        9 2023-06-13 21:34:00.000000 dft2kp-0.0.2/dft2kp.egg-info/top_level.txt
+drwxrwxr-x   0 joao.cassiano  (1001) joao.cassiano  (1001)        0 2023-06-13 21:34:00.762756 dft2kp-0.0.2/pydft2kp/
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      349 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/__init__.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       22 2023-06-13 21:33:30.000000 dft2kp-0.0.2/pydft2kp/__version.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     1652 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/constants.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    26892 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/irrepwrapper.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    24083 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/lowdin.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    13560 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/qe_aux.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     5596 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/qsymmwrapper.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)    17404 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/rotatebasis.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)     5698 2023-06-13 19:42:08.000000 dft2kp-0.0.2/pydft2kp/util.py
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)       38 2023-06-13 21:34:00.762756 dft2kp-0.0.2/setup.cfg
+-rw-rw-r--   0 joao.cassiano  (1001) joao.cassiano  (1001)      844 2023-06-13 19:48:50.000000 dft2kp-0.0.2/setup.py
```

### Comparing `dft2kp-0.0.1/AUTHORS.md` & `dft2kp-0.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/LICENSE` & `dft2kp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/PKG-INFO` & `dft2kp-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dft2kp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculates kp model and coefficients from DFT ab initio data.
 Home-page: https://gitlab.com/dft2kp/dft2kp
 Author: Gerson J. Ferreira
 Author-email: gersonjferreira@ufu.br
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dft2kp-0.0.1/README.md` & `dft2kp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/dft2kp.egg-info/PKG-INFO` & `dft2kp-0.0.2/dft2kp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dft2kp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculates kp model and coefficients from DFT ab initio data.
 Home-page: https://gitlab.com/dft2kp/dft2kp
 Author: Gerson J. Ferreira
 Author-email: gersonjferreira@ufu.br
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dft2kp-0.0.1/pydft2kp/constants.py` & `dft2kp-0.0.2/pydft2kp/constants.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/irrepwrapper.py` & `dft2kp-0.0.2/pydft2kp/irrepwrapper.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/lowdin.py` & `dft2kp-0.0.2/pydft2kp/lowdin.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/qe_aux.py` & `dft2kp-0.0.2/pydft2kp/qe_aux.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/qsymmwrapper.py` & `dft2kp-0.0.2/pydft2kp/qsymmwrapper.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/rotatebasis.py` & `dft2kp-0.0.2/pydft2kp/rotatebasis.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/pydft2kp/util.py` & `dft2kp-0.0.2/pydft2kp/util.py`

 * *Files identical despite different names*

### Comparing `dft2kp-0.0.1/setup.py` & `dft2kp-0.0.2/setup.py`

 * *Files identical despite different names*

