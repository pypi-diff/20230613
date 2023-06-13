# Comparing `tmp/bunkatopics-0.7.tar.gz` & `tmp/bunkatopics-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunkatopics-0.7.tar", last modified: Tue May 24 07:07:56 2022, max compression
+gzip compressed data, was "bunkatopics-0.8.tar", last modified: Tue May 24 11:06:02 2022, max compression
```

## Comparing `bunkatopics-0.7.tar` & `bunkatopics-0.8.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 charlesdedampierre   (501) staff       (20)        0 2022-05-24 07:07:56.814589 bunkatopics-0.7/
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)      704 2022-05-24 07:07:56.814655 bunkatopics-0.7/PKG-INFO
-drwxr-xr-x   0 charlesdedampierre   (501) staff       (20)        0 2022-05-24 07:07:56.814465 bunkatopics-0.7/bunkatopics/
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)       32 2022-05-23 21:16:59.253616 bunkatopics-0.7/bunkatopics/__init__.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     6244 2022-05-24 07:03:56.229512 bunkatopics-0.7/bunkatopics/basic_class.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     6538 2022-05-24 07:01:28.604635 bunkatopics-0.7/bunkatopics/extract_terms.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)      429 2022-05-20 11:51:22.526183 bunkatopics-0.7/bunkatopics/indexer.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1242 2022-05-23 20:23:17.023575 bunkatopics-0.7/bunkatopics/multiprocess_embeddings.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)      473 2022-05-24 07:01:55.720701 bunkatopics-0.7/bunkatopics/sent_multiprocessing.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1510 2022-05-20 07:21:16.569860 bunkatopics-0.7/bunkatopics/specificity.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     7541 2022-05-24 06:06:34.647594 bunkatopics-0.7/bunkatopics/topics.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)      301 2022-05-24 07:06:48.794791 bunkatopics-0.7/bunkatopics/utils.py
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)        0 2022-05-23 19:34:13.103285 bunkatopics-0.7/setup.cfg
--rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1447 2022-05-24 07:07:51.467324 bunkatopics-0.7/setup.py
+drwxr-xr-x   0 charlesdedampierre   (501) staff       (20)        0 2022-05-24 11:06:02.160123 bunkatopics-0.8/
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)        0 2022-05-20 13:16:16.000000 bunkatopics-0.8/LICENSE.txt
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      719 2022-05-24 11:06:02.160199 bunkatopics-0.8/PKG-INFO
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     2238 2022-05-24 11:05:32.000000 bunkatopics-0.8/README.md
+drwxr-xr-x   0 charlesdedampierre   (501) staff       (20)        0 2022-05-24 11:06:02.159392 bunkatopics-0.8/bunkatopics/
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)       32 2022-05-23 21:16:59.000000 bunkatopics-0.8/bunkatopics/__init__.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     6244 2022-05-24 07:03:56.000000 bunkatopics-0.8/bunkatopics/basic_class.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     6538 2022-05-24 07:01:28.000000 bunkatopics-0.8/bunkatopics/extract_terms.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      429 2022-05-20 11:51:22.000000 bunkatopics-0.8/bunkatopics/indexer.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1242 2022-05-23 20:23:17.000000 bunkatopics-0.8/bunkatopics/multiprocess_embeddings.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      473 2022-05-24 07:01:55.000000 bunkatopics-0.8/bunkatopics/sent_multiprocessing.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1510 2022-05-20 07:21:16.000000 bunkatopics-0.8/bunkatopics/specificity.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     7541 2022-05-24 06:06:34.000000 bunkatopics-0.8/bunkatopics/topics.py
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      301 2022-05-24 07:06:48.000000 bunkatopics-0.8/bunkatopics/utils.py
+drwxr-xr-x   0 charlesdedampierre   (501) staff       (20)        0 2022-05-24 11:06:02.160012 bunkatopics-0.8/bunkatopics.egg-info/
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      719 2022-05-24 11:06:01.000000 bunkatopics-0.8/bunkatopics.egg-info/PKG-INFO
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      462 2022-05-24 11:06:02.000000 bunkatopics-0.8/bunkatopics.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)        1 2022-05-24 11:06:01.000000 bunkatopics-0.8/bunkatopics.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)      162 2022-05-24 11:06:02.000000 bunkatopics-0.8/bunkatopics.egg-info/requires.txt
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)       12 2022-05-24 11:06:02.000000 bunkatopics-0.8/bunkatopics.egg-info/top_level.txt
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)       38 2022-05-24 11:06:02.160418 bunkatopics-0.8/setup.cfg
+-rw-r--r--   0 charlesdedampierre   (501) staff       (20)     1447 2022-05-24 11:05:49.000000 bunkatopics-0.8/setup.py
```

### Comparing `bunkatopics-0.7/PKG-INFO` & `bunkatopics-0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bunkatopics
-Version: 0.7
+Version: 0.8
 Summary: Advanced Topic Modeling Using Transformers
 Home-page: https://github.com/charlesdedampierre/BunkaTopics
+Download-URL: https://github.com/charlesdedampierre/BunkaTopics/archive/v_01.tar.gz
 Author: Charles de Dampierre
 Author-email: charles.de-dampierre@hec.edu
 License: MIT
-Download-URL: https://github.com/charlesdedampierre/BunkaTopics/archive/v_01.tar.gz
-Description: UNKNOWN
 Keywords: Topic Modeling,NLP,Search
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `bunkatopics-0.7/bunkatopics/basic_class.py` & `bunkatopics-0.8/bunkatopics/basic_class.py`

 * *Files identical despite different names*

### Comparing `bunkatopics-0.7/bunkatopics/extract_terms.py` & `bunkatopics-0.8/bunkatopics/extract_terms.py`

 * *Files identical despite different names*

### Comparing `bunkatopics-0.7/bunkatopics/multiprocess_embeddings.py` & `bunkatopics-0.8/bunkatopics/multiprocess_embeddings.py`

 * *Files identical despite different names*

### Comparing `bunkatopics-0.7/bunkatopics/specificity.py` & `bunkatopics-0.8/bunkatopics/specificity.py`

 * *Files identical despite different names*

### Comparing `bunkatopics-0.7/bunkatopics/topics.py` & `bunkatopics-0.8/bunkatopics/topics.py`

 * *Files identical despite different names*

### Comparing `bunkatopics-0.7/setup.py` & `bunkatopics-0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name="bunkatopics",
     packages=["bunkatopics"],
-    version="0.7",
+    version="0.8",
     license="MIT",
     description="Advanced Topic Modeling Using Transformers",
     author="Charles de Dampierre",
     author_email="charles.de-dampierre@hec.edu",
     url="https://github.com/charlesdedampierre/BunkaTopics",
     download_url="https://github.com/charlesdedampierre/BunkaTopics/archive/v_01.tar.gz",
     keywords=[
```

