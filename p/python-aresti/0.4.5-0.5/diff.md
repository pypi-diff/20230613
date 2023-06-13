# Comparing `tmp/python-aresti-0.4.5.tar.gz` & `tmp/python-aresti-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aresti-0.4.5.tar", last modified: Mon Jun 12 06:14:48 2023, max compression
+gzip compressed data, was "python-aresti-0.5.tar", last modified: Tue Jun 13 09:27:30 2023, max compression
```

## Comparing `python-aresti-0.4.5.tar` & `python-aresti-0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:14:48.511728 python-aresti-0.4.5/
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-12 06:14:48.511541 python-aresti-0.4.5/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.4.5/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:14:48.508499 python-aresti-0.4.5/aresti/
--rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.4.5/aresti/__init__.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:14:48.509999 python-aresti-0.4.5/aresti/rajapinta/
--rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.4.5/aresti/rajapinta/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.4.5/aresti/rajapinta/meta.py
--rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.4.5/aresti/rajapinta/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.4.5/aresti/rajapinta/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.4.5/aresti/rajapinta/vierasavain.py
--rw-r--r--   0 aha        (501) staff       (20)     3387 2023-06-08 10:10:22.000000 python-aresti-0.4.5/aresti/rest.py
--rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.4.5/aresti/sanoma.py
--rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.4.5/aresti/testi.py
--rw-r--r--   0 aha        (501) staff       (20)     2345 2023-06-05 08:50:11.000000 python-aresti-0.4.5/aresti/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.4.5/aresti/yhteys.py
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:17:11.000000 python-aresti-0.4.5/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:14:48.511321 python-aresti-0.4.5/python_aresti.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     4022 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-12 06:14:48.000000 python-aresti-0.4.5/python_aresti.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-12 06:14:48.511769 python-aresti-0.4.5/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.4.5/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.502029 python-aresti-0.5/
+-rw-r--r--   0 aha        (501) staff       (20)      245 2023-06-13 09:27:30.501866 python-aresti-0.5/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.5/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.498959 python-aresti-0.5/aresti/
+-rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.5/aresti/__init__.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.500658 python-aresti-0.5/aresti/rajapinta/
+-rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.5/aresti/rajapinta/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.5/aresti/rajapinta/meta.py
+-rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.5/aresti/rajapinta/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.5/aresti/rajapinta/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.5/aresti/rajapinta/vierasavain.py
+-rw-r--r--   0 aha        (501) staff       (20)     3387 2023-06-08 10:10:22.000000 python-aresti-0.5/aresti/rest.py
+-rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.5/aresti/sanoma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.5/aresti/testi.py
+-rw-r--r--   0 aha        (501) staff       (20)     2345 2023-06-05 08:50:11.000000 python-aresti-0.5/aresti/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.5/aresti/yhteys.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:17:11.000000 python-aresti-0.5/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.501690 python-aresti-0.5/python_aresti.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      245 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     4020 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-13 09:27:30.502082 python-aresti-0.5/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.5/setup.py
```

### Comparing `python-aresti-0.4.5/aresti/rajapinta/__init__.py` & `python-aresti-0.5/aresti/rajapinta/__init__.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/rajapinta/meta.py` & `python-aresti-0.5/aresti/rajapinta/meta.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/rajapinta/nakyma.py` & `python-aresti-0.5/aresti/rajapinta/nakyma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/rajapinta/tyokalut.py` & `python-aresti-0.5/aresti/rajapinta/tyokalut.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/rajapinta/vierasavain.py` & `python-aresti-0.5/aresti/rajapinta/vierasavain.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/rest.py` & `python-aresti-0.5/aresti/rest.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/sanoma.py` & `python-aresti-0.5/aresti/sanoma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/testi.py` & `python-aresti-0.5/aresti/testi.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/tyokalut.py` & `python-aresti-0.5/aresti/tyokalut.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/aresti/yhteys.py` & `python-aresti-0.5/aresti/yhteys.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.4.5/python_aresti.egg-info/historia.json` & `python-aresti-0.5/python_aresti.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927536231884059%*

 * *Differences: {'0': "{'versio': '0.5'}"}*

```diff
@@ -1,12 +1,12 @@
 [
     {
         "kuvaus": "Korjattu `nouda_sivutettu_data`",
         "revisio": "abb9fe3f792cf12027d91034c6a08245641f0eb2",
-        "versio": "0.4.5"
+        "versio": "0.5"
     },
     {
         "kuvaus": "PEP 517 -yhteensopivuus",
         "revisio": "4b7cbfd6b7bfe7efe2ff036abe2569aea0f2d281",
         "versio": "0.4.4"
     },
     {
```

