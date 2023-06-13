# Comparing `tmp/social_gpt-0.0.2.tar.gz` & `tmp/social_gpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_gpt-0.0.2.tar", last modified: Tue Jun 13 14:51:45 2023, max compression
+gzip compressed data, was "social_gpt-0.0.3.tar", last modified: Tue Jun 13 19:28:58 2023, max compression
```

## Comparing `social_gpt-0.0.2.tar` & `social_gpt-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.737402 social_gpt-0.0.2/
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.2/LICENSE
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:51:45.737274 social_gpt-0.0.2/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.2/README.md
--rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.2/pyproject.toml
--rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-13 14:51:45.737439 social_gpt-0.0.2/setup.cfg
--rw-r--r--   0 dineshsingh   (501) staff       (20)      597 2023-06-13 14:51:34.000000 social_gpt-0.0.2/setup.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.735146 social_gpt-0.0.2/social-gpt2/
--rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.2/social-gpt2/__init__.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.735546 social_gpt-0.0.2/social-gpt2/ingestion/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.2/social-gpt2/ingestion/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.2/social-gpt2/ingestion/indexer.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/ingestion.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.736299 social_gpt-0.0.2/social-gpt2/ingestion/scraper/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/scraper_factory.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/social_scraper.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.2/social-gpt2/ingestion/scraper/youtube_scraper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.736564 social_gpt-0.0.2/social-gpt2/query/
--rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.2/social-gpt2/query/__init__.py
--rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.2/social-gpt2/query/query_helper.py
-drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 14:51:45.737122 social_gpt-0.0.2/social_gpt.egg-info/
--rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/PKG-INFO
--rw-r--r--   0 dineshsingh   (501) staff       (20)      555 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:51:45.000000 social_gpt-0.0.2/social_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.992659 social_gpt-0.0.3/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1072 2023-06-13 14:09:04.000000 social_gpt-0.0.3/LICENSE
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 19:28:58.992518 social_gpt-0.0.3/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       12 2023-06-13 14:08:39.000000 social_gpt-0.0.3/README.md
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       99 2023-06-13 14:09:35.000000 social_gpt-0.0.3/pyproject.toml
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       38 2023-06-13 19:28:58.992696 social_gpt-0.0.3/setup.cfg
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      597 2023-06-13 19:28:43.000000 social_gpt-0.0.3/setup.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.989466 social_gpt-0.0.3/social_gpt/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       21 2023-06-13 14:49:17.000000 social_gpt-0.0.3/social_gpt/__init__.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.990498 social_gpt-0.0.3/social_gpt/ingestion/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-07 11:16:57.000000 social_gpt-0.0.3/social_gpt/ingestion/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1650 2023-06-13 10:34:27.000000 social_gpt-0.0.3/social_gpt/ingestion/indexer.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      515 2023-06-13 14:23:25.000000 social_gpt-0.0.3/social_gpt/ingestion/ingestion.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.991877 social_gpt-0.0.3/social_gpt/ingestion/scraper/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-12 18:55:48.000000 social_gpt-0.0.3/social_gpt/ingestion/scraper/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      306 2023-06-13 14:23:25.000000 social_gpt-0.0.3/social_gpt/ingestion/scraper/scraper_factory.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      258 2023-06-13 07:48:49.000000 social_gpt-0.0.3/social_gpt/ingestion/scraper/social_scraper.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)     1708 2023-06-13 14:23:25.000000 social_gpt-0.0.3/social_gpt/ingestion/scraper/youtube_scraper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.992234 social_gpt-0.0.3/social_gpt/query/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        0 2023-06-13 09:26:30.000000 social_gpt-0.0.3/social_gpt/query/__init__.py
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      586 2023-06-13 10:15:48.000000 social_gpt-0.0.3/social_gpt/query/query_helper.py
+drwxr-xr-x   0 dineshsingh   (501) staff       (20)        0 2023-06-13 19:28:58.990006 social_gpt-0.0.3/social_gpt.egg-info/
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      400 2023-06-13 19:28:58.000000 social_gpt-0.0.3/social_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 dineshsingh   (501) staff       (20)      545 2023-06-13 19:28:58.000000 social_gpt-0.0.3/social_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)        1 2023-06-13 19:28:58.000000 social_gpt-0.0.3/social_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 dineshsingh   (501) staff       (20)       11 2023-06-13 19:28:58.000000 social_gpt-0.0.3/social_gpt.egg-info/top_level.txt
```

### Comparing `social_gpt-0.0.2/LICENSE` & `social_gpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.2/setup.py` & `social_gpt-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="social_gpt",
-    version="0.0.2",
+    version="0.0.3",
     author="dinesh1301",
     author_email="dinesh@topmate.io",
     description="Social gpt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dinesh1301/social-gpt2",
     packages=setuptools.find_packages(),
```

### Comparing `social_gpt-0.0.2/social-gpt2/ingestion/indexer.py` & `social_gpt-0.0.3/social_gpt/ingestion/indexer.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.2/social-gpt2/ingestion/ingestion.py` & `social_gpt-0.0.3/social_gpt/ingestion/ingestion.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.2/social-gpt2/ingestion/scraper/youtube_scraper.py` & `social_gpt-0.0.3/social_gpt/ingestion/scraper/youtube_scraper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.2/social-gpt2/query/query_helper.py` & `social_gpt-0.0.3/social_gpt/query/query_helper.py`

 * *Files identical despite different names*

### Comparing `social_gpt-0.0.2/social_gpt.egg-info/SOURCES.txt` & `social_gpt-0.0.3/social_gpt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-social-gpt2/__init__.py
-social-gpt2/ingestion/__init__.py
-social-gpt2/ingestion/indexer.py
-social-gpt2/ingestion/ingestion.py
-social-gpt2/ingestion/scraper/__init__.py
-social-gpt2/ingestion/scraper/scraper_factory.py
-social-gpt2/ingestion/scraper/social_scraper.py
-social-gpt2/ingestion/scraper/youtube_scraper.py
-social-gpt2/query/__init__.py
-social-gpt2/query/query_helper.py
+social_gpt/__init__.py
 social_gpt.egg-info/PKG-INFO
 social_gpt.egg-info/SOURCES.txt
 social_gpt.egg-info/dependency_links.txt
-social_gpt.egg-info/top_level.txt
+social_gpt.egg-info/top_level.txt
+social_gpt/ingestion/__init__.py
+social_gpt/ingestion/indexer.py
+social_gpt/ingestion/ingestion.py
+social_gpt/ingestion/scraper/__init__.py
+social_gpt/ingestion/scraper/scraper_factory.py
+social_gpt/ingestion/scraper/social_scraper.py
+social_gpt/ingestion/scraper/youtube_scraper.py
+social_gpt/query/__init__.py
+social_gpt/query/query_helper.py
```

