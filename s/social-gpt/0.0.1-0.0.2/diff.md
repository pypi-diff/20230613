# Comparing `tmp/social_gpt-0.0.1.tar.gz` & `tmp/social_gpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_gpt-0.0.1.tar", last modified: Tue Jun 13 14:50:37 2023, max compression
+gzip compressed data, was "social_gpt-0.0.2.tar", last modified: Tue Jun 13 14:51:45 2023, max compression
```

## Comparing `social_gpt-0.0.1.tar` & `social_gpt-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.068015 social_gpt-0.0.1/
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.1/LICENSE
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:50:37.067859 social_gpt-0.0.1/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.1/README.md
--rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.1/pyproject.toml
--rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-13 14:50:37.068055 social_gpt-0.0.1/setup.cfg
--rw-r--r--   0 dineshsingh   (501) staff       (20)      597 2023-06-13 14:48:25.000000 social_gpt-0.0.1/setup.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.065069 social_gpt-0.0.1/social-gpt2/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.1/social-gpt2/__init__.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.065717 social_gpt-0.0.1/social-gpt2/ingestion/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.1/social-gpt2/ingestion/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.1/social-gpt2/ingestion/indexer.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.1/social-gpt2/ingestion/ingestion.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.066809 social_gpt-0.0.1/social-gpt2/ingestion/scraper/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.1/social-gpt2/ingestion/scraper/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.1/social-gpt2/ingestion/scraper/scraper_factory.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.1/social-gpt2/ingestion/scraper/social_scraper.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.1/social-gpt2/ingestion/scraper/youtube_scraper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.067141 social_gpt-0.0.1/social-gpt2/query/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.1/social-gpt2/query/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.1/social-gpt2/query/query_helper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:50:37.067684 social_gpt-0.0.1/social_gpt.egg-info/
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:50:37.000000 social_gpt-0.0.1/social_gpt.egg-info/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)      555 2023-06-13 14:50:37.000000 social_gpt-0.0.1/social_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-13 14:50:37.000000 social_gpt-0.0.1/social_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:50:37.000000 social_gpt-0.0.1/social_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.737402 social_gpt-0.0.2/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.2/LICENSE
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:51:45.737274 social_gpt-0.0.2/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.2/README.md
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.2/pyproject.toml
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-13 14:51:45.737439 social_gpt-0.0.2/setup.cfg
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      597 2023-06-13 14:51:34.000000 social_gpt-0.0.2/setup.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.735146 social_gpt-0.0.2/social-gpt2/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.2/social-gpt2/__init__.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.735546 social_gpt-0.0.2/social-gpt2/ingestion/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.2/social-gpt2/ingestion/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.2/social-gpt2/ingestion/indexer.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/ingestion.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.736299 social_gpt-0.0.2/social-gpt2/ingestion/scraper/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/scraper_factory.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/social_scraper.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/youtube_scraper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.736564 social_gpt-0.0.2/social-gpt2/query/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.2/social-gpt2/query/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.2/social-gpt2/query/query_helper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.737122 social_gpt-0.0.2/social_gpt.egg-info/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      555 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/top_level.txt
```

### Comparing `social_gpt-0.0.1/LICENSE` & `social_gpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.1/setup.py` & `social_gpt-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="social_gpt",
-    version="0.0.1",
+    version="0.0.2",
     author="dinesh1301",
     author_email="dinesh@topmate.io",
     description="Social gpt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dinesh1301/social-gpt2",
     packages=setuptools.find_packages(),
```

### Comparing `social_gpt-0.0.1/social-gpt2/ingestion/indexer.py` & `social_gpt-0.0.2/social-gpt2/ingestion/indexer.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.1/social-gpt2/ingestion/ingestion.py` & `social_gpt-0.0.2/social-gpt2/ingestion/ingestion.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.1/social-gpt2/ingestion/scraper/youtube_scraper.py` & `social_gpt-0.0.2/social-gpt2/ingestion/scraper/youtube_scraper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.1/social-gpt2/query/query_helper.py` & `social_gpt-0.0.2/social-gpt2/query/query_helper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.1/social_gpt.egg-info/SOURCES.txt` & `social_gpt-0.0.2/social_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

