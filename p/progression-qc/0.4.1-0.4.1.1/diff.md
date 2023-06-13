# Comparing `tmp/progression_qc-0.4.1.tar.gz` & `tmp/progression_qc-0.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progression_qc-0.4.1.tar", last modified: Tue Jun 13 05:36:59 2023, max compression
+gzip compressed data, was "progression_qc-0.4.1.1.tar", last modified: Tue Jun 13 06:15:36 2023, max compression
```

## Comparing `progression_qc-0.4.1.tar` & `progression_qc-0.4.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:36:59.061009 progression_qc-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35074 2023-06-13 05:16:01.000000 progression_qc-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 05:36:59.061009 progression_qc-0.4.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:36:59.061009 progression_qc-0.4.1/progression_qc/
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7864 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/progression_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:36:59.061009 progression_qc-0.4.1/progression_qc/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 05:36:49.000000 progression_qc-0.4.1/progression_qc/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-13 05:36:49.000000 progression_qc-0.4.1/progression_qc/schemas/question_base.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/schemas/question_bd.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/schemas/question_prog.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/schemas/question_sys.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/schemas/question_vcs.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-13 05:16:01.000000 progression_qc-0.4.1/progression_qc/schemas/rétroactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:36:59.061009 progression_qc-0.4.1/progression_qc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 05:36:59.000000 progression_qc-0.4.1/progression_qc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2023-06-13 05:36:59.000000 progression_qc-0.4.1/progression_qc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:36:59.000000 progression_qc-0.4.1/progression_qc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 05:36:59.000000 progression_qc-0.4.1/progression_qc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 05:36:59.000000 progression_qc-0.4.1/progression_qc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 05:36:59.061009 progression_qc-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-13 05:16:01.000000 progression_qc-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:36:59.061009 progression_qc-0.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9214 2023-06-13 05:16:01.000000 progression_qc-0.4.1/tests/test_progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35074 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-06-13 06:15:26.000000 progression_qc-0.4.1.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/progression_qc/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7864 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/progression_qc/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 06:15:26.000000 progression_qc-0.4.1.1/progression_qc/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-13 05:36:49.000000 progression_qc-0.4.1.1/progression_qc/schemas/question_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/schemas/question_bd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/schemas/question_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/schemas/question_sys.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/schemas/question_vcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/progression_qc/schemas/rétroactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/progression_qc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-13 06:15:36.000000 progression_qc-0.4.1.1/progression_qc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 06:15:36.000000 progression_qc-0.4.1.1/progression_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 06:15:36.000000 progression_qc-0.4.1.1/progression_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 06:15:36.000000 progression_qc-0.4.1.1/progression_qc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 06:15:36.000000 progression_qc-0.4.1.1/progression_qc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-13 06:15:26.000000 progression_qc-0.4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:15:36.075420 progression_qc-0.4.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9214 2023-06-13 05:16:01.000000 progression_qc-0.4.1.1/tests/test_progression_qc.py
```

### Comparing `progression_qc-0.4.1/LICENSE` & `progression_qc-0.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/PKG-INFO` & `progression_qc-0.4.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression_qc
-Version: 0.4.1
+Version: 0.4.1.1
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-0.4.1/progression_qc/__main__.py` & `progression_qc-0.4.1.1/progression_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/progression_qc/progression_qc.py` & `progression_qc-0.4.1.1/progression_qc/progression_qc.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/progression_qc/schemas/question_base.py` & `progression_qc-0.4.1.1/progression_qc/schemas/question_base.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/progression_qc/schemas/question_prog.py` & `progression_qc-0.4.1.1/progression_qc/schemas/question_prog.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/progression_qc/schemas/question_sys.py` & `progression_qc-0.4.1.1/progression_qc/schemas/question_sys.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.4.1/progression_qc.egg-info/PKG-INFO` & `progression_qc-0.4.1.1/progression_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression-qc
-Version: 0.4.1
+Version: 0.4.1.1
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-0.4.1/progression_qc.egg-info/SOURCES.txt` & `progression_qc-0.4.1.1/progression_qc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+VERSION
 setup.py
 progression_qc/__init__.py
 progression_qc/__main__.py
 progression_qc/progression_qc.py
 progression_qc.egg-info/PKG-INFO
 progression_qc.egg-info/SOURCES.txt
 progression_qc.egg-info/dependency_links.txt
```

### Comparing `progression_qc-0.4.1/setup.py` & `progression_qc-0.4.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,9 +11,10 @@
     description="progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.",
     url="https://git.dti.crosemont.quebec/progression/validateur",
     author="Patrick Lafrance",
     author_email="plafrance@crosemont.qc.ca",
     license='GPLv3+',
     packages=["progression_qc", "progression_qc/schemas"],
     install_requires=["cerberus", "pyyaml-include", "werkzeug"],
+    data_files=["VERSION"],
     classifiers=['Programming Language :: Python :: 3'],
 )
```

### Comparing `progression_qc-0.4.1/tests/test_progression_qc.py` & `progression_qc-0.4.1.1/tests/test_progression_qc.py`

 * *Files identical despite different names*

