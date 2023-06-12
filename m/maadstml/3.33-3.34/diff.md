# Comparing `tmp/maadstml-3.33.tar.gz` & `tmp/maadstml-3.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.33.tar", last modified: Mon Jun 12 22:53:12 2023, max compression
+gzip compressed data, was "maadstml-3.34.tar", last modified: Mon Jun 12 22:57:20 2023, max compression
```

## Comparing `maadstml-3.33.tar` & `maadstml-3.34.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 22:53:12.096658 maadstml-3.33/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.33/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.33/MANIFEST.in
--rw-rw-rw-   0        0        0   173473 2023-06-12 22:53:12.096658 maadstml-3.33/PKG-INFO
--rw-rw-rw-   0        0        0   172876 2023-06-12 22:51:47.000000 maadstml-3.33/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 22:53:12.066307 maadstml-3.33/maadstml/
--rw-rw-rw-   0        0        0     2158 2023-06-11 18:45:29.000000 maadstml-3.33/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.33/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    80259 2023-06-12 22:44:41.000000 maadstml-3.33/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.33/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:53:12.096658 maadstml-3.33/maadstml.egg-info/
--rw-rw-rw-   0        0        0   173473 2023-06-12 22:53:11.000000 maadstml-3.33/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-12 22:53:12.000000 maadstml-3.33/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 22:53:11.000000 maadstml-3.33/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-12 22:53:11.000000 maadstml-3.33/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 22:53:11.000000 maadstml-3.33/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      188 2023-06-12 17:35:52.000000 maadstml-3.33/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 22:53:12.096658 maadstml-3.33/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-12 22:52:26.000000 maadstml-3.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.986688 maadstml-3.34/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.34/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.34/MANIFEST.in
+-rw-rw-rw-   0        0        0   173473 2023-06-12 22:57:20.986688 maadstml-3.34/PKG-INFO
+-rw-rw-rw-   0        0        0   172876 2023-06-12 22:51:47.000000 maadstml-3.34/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.970822 maadstml-3.34/maadstml/
+-rw-rw-rw-   0        0        0     2258 2023-06-12 22:57:03.000000 maadstml-3.34/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.34/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    80259 2023-06-12 22:44:41.000000 maadstml-3.34/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.34/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:57:20.986688 maadstml-3.34/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   173473 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 22:57:20.000000 maadstml-3.34/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      188 2023-06-12 17:35:52.000000 maadstml-3.34/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 22:57:20.986688 maadstml-3.34/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-12 22:57:11.000000 maadstml-3.34/setup.py
```

### Comparing `maadstml-3.33/LICENSE.txt` & `maadstml-3.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.33/PKG-INFO` & `maadstml-3.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.33
+Version: 3.34
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.33/README.md` & `maadstml-3.34/README.md`

 * *Files identical despite different names*

### Comparing `maadstml-3.33/maadstml/__init__.py` & `maadstml-3.34/maadstml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,8 +75,12 @@
 
 from .sendfiles import viperhpdepredictprocess
 
 from .sendfiles import vipernlp
 
 from .sendfiles import viperchatgpt
 
+from .sendfiles import viperexractpdffields
+
+from .sendfiles import viperexractpdffieldbylabel
+
 name = "maadstml"
```

### Comparing `maadstml-3.33/maadstml/readpdf.py` & `maadstml-3.34/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.33/maadstml/sendfiles.py` & `maadstml-3.34/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.33/maadstml/tmltextsummary.py` & `maadstml-3.34/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.33/maadstml.egg-info/PKG-INFO` & `maadstml-3.34/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.33
+Version: 3.34
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.33/setup.py` & `maadstml-3.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.33',
+    version='3.34',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

