# Comparing `tmp/progression_qc-0.3.1.2.tar.gz` & `tmp/progression_qc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progression_qc-0.3.1.2.tar", last modified: Mon Apr  3 00:52:58 2023, max compression
+gzip compressed data, was "progression_qc-0.4.0.tar", last modified: Tue Jun 13 05:16:10 2023, max compression
```

## Comparing `progression_qc-0.3.1.2.tar` & `progression_qc-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 00:52:58.580480 progression_qc-0.3.1.2/
--rw-rw-rw-   0 root         (0) root         (0)    35074 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-03 00:52:58.580480 progression_qc-0.3.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 00:52:58.576480 progression_qc-0.3.1.2/progression_qc/
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-04-02 23:27:37.000000 progression_qc-0.3.1.2/progression_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7864 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/progression_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 00:52:58.580480 progression_qc-0.3.1.2/progression_qc/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/question_base.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/question_bd.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/question_prog.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/question_sys.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/question_vcs.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/progression_qc/schemas/rétroactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 00:52:58.576480 progression_qc-0.3.1.2/progression_qc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-03 00:52:58.000000 progression_qc-0.3.1.2/progression_qc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2023-04-03 00:52:58.000000 progression_qc-0.3.1.2/progression_qc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 00:52:58.000000 progression_qc-0.3.1.2/progression_qc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-03 00:52:58.000000 progression_qc-0.3.1.2/progression_qc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 00:52:58.000000 progression_qc-0.3.1.2/progression_qc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 00:52:58.580480 progression_qc-0.3.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-02 23:55:17.000000 progression_qc-0.3.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 00:52:58.580480 progression_qc-0.3.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8960 2023-04-02 21:38:01.000000 progression_qc-0.3.1.2/tests/test_progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:16:10.905340 progression_qc-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35074 2023-06-13 05:16:01.000000 progression_qc-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 05:16:10.905340 progression_qc-0.4.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:16:10.905340 progression_qc-0.4.0/progression_qc/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7864 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:16:10.905340 progression_qc-0.4.0/progression_qc/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/question_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/question_bd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/question_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/question_sys.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/question_vcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-13 05:16:01.000000 progression_qc-0.4.0/progression_qc/schemas/rétroactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:16:10.905340 progression_qc-0.4.0/progression_qc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-13 05:16:10.000000 progression_qc-0.4.0/progression_qc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2023-06-13 05:16:10.000000 progression_qc-0.4.0/progression_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:16:10.000000 progression_qc-0.4.0/progression_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 05:16:10.000000 progression_qc-0.4.0/progression_qc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 05:16:10.000000 progression_qc-0.4.0/progression_qc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 05:16:10.905340 progression_qc-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-13 05:16:01.000000 progression_qc-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:16:10.905340 progression_qc-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9214 2023-06-13 05:16:01.000000 progression_qc-0.4.0/tests/test_progression_qc.py
```

### Comparing `progression_qc-0.3.1.2/LICENSE` & `progression_qc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/progression_qc/__main__.py` & `progression_qc-0.4.0/progression_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/progression_qc/progression_qc.py` & `progression_qc-0.4.0/progression_qc/progression_qc.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/progression_qc/schemas/question_prog.py` & `progression_qc-0.4.0/progression_qc/schemas/question_prog.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/progression_qc/schemas/question_sys.py` & `progression_qc-0.4.0/progression_qc/schemas/question_sys.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/progression_qc.egg-info/PKG-INFO` & `progression_qc-0.4.0/progression_qc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression-qc
-Version: 0.3.1.2
+Version: 0.4.0
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-0.3.1.2/progression_qc.egg-info/SOURCES.txt` & `progression_qc-0.4.0/progression_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/setup.py` & `progression_qc-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `progression_qc-0.3.1.2/tests/test_progression_qc.py` & `progression_qc-0.4.0/tests/test_progression_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,21 @@
 def test_valider_question_prog_complète():
     from question_prog_complète_valide import question
 
     résultat = progression_qc.valider_schema_yaml_infos_question(question)
 
     assert résultat == {"avertissements": {}, "erreurs": {}}
 
+def test_valider_question_avec_dict_pour_énoncés():
+    from question_avec_dict_pour_énoncés import question
+
+    résultat = progression_qc.valider_schema_yaml_infos_question(question)
+
+    assert résultat == {"avertissements": {}, "erreurs": {}}
+
 def test_valider_question_prog_minimale():
     from question_prog_minimale_valide import question
 
     résultat = progression_qc.valider_schema_yaml_infos_question(question)
 
     assert résultat == {"avertissements": {}, "erreurs": {}}
```

