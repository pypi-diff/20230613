# Comparing `tmp/hotjar-data-wrapper-0.1.3.tar.gz` & `tmp/hotjar-data-wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotjar-data-wrapper-0.1.3.tar", last modified: Fri Jun  2 19:31:35 2023, max compression
+gzip compressed data, was "hotjar-data-wrapper-0.1.4.tar", last modified: Tue Jun 13 13:08:08 2023, max compression
```

## Comparing `hotjar-data-wrapper-0.1.3.tar` & `hotjar-data-wrapper-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.594656 hotjar-data-wrapper-0.1.3/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      302 2023-06-02 19:31:35.594845 hotjar-data-wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1517 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/README.md
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.588717 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:27:46.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/hotjar_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:31:35.593960 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      302 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      274 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       20 2023-06-02 19:31:35.000000 hotjar-data-wrapper-0.1.3/hotjar_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      423 2023-06-02 19:31:35.597125 hotjar-data-wrapper-0.1.3/setup.cfg
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:25:41.000000 hotjar-data-wrapper-0.1.3/setup.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.770820 hotjar-data-wrapper-0.1.4/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.4/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1923 2023-06-13 13:08:08.771067 hotjar-data-wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1579 2023-06-02 19:34:25.000000 hotjar-data-wrapper-0.1.4/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.765394 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:33:47.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     6077 2023-05-21 18:16:12.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/hotjar_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:08:08.769715 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1923 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      274 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       20 2023-06-13 13:08:08.000000 hotjar-data-wrapper-0.1.4/hotjar_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      504 2023-06-13 13:08:08.774797 hotjar-data-wrapper-0.1.4/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:33:47.000000 hotjar-data-wrapper-0.1.4/setup.py
```

### Comparing `hotjar-data-wrapper-0.1.3/LICENSE` & `hotjar-data-wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hotjar-data-wrapper-0.1.3/README.md` & `hotjar-data-wrapper-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,43 +14,45 @@
     - [Get all survey metadata](#get-all-survey-metadata)
 
 ### Get survey metadata
 
 Login and download metadata for a specific survey.
 
 ```python
-meta = get_survey_metadata(survey_id=survey_id, site_id=site_id, username=username, password=password)
+import hotjar_data_wrapper.hotjar_api as hot
+
+meta = hot.get_survey_metadata(survey_id=survey_id, site_id=site_id, username=username, password=password)
 meta.status_code # 200
 meta.content # prints content
 ```
 
 ### Get survey questions
 
 Login and download questions for a specific survey.
 
 ```python
-questions = get_survey_questions(survey_id=survey_id, site_id=site_id, username=username, password=password)
+questions = hot.get_survey_questions(survey_id=survey_id, site_id=site_id, username=username, password=password)
 questions.content 
 ```
 
 ### List all surveys
 
 Login and download list of all surveys for a given site ID.
 
 ```python
-all_surveys = get_list_all_surveys(site_id=site_id, username=username, password=password)
+all_surveys = hot.get_list_all_surveys(site_id=site_id, username=username, password=password)
 all_surveys.content
 ```
 
 ### Get all survey metadata
 
 Login and download metadata for a list of surveys with survey IDs.
 
 ```python
-get_all_surveys_metadata(
+hot.get_all_surveys_metadata(
     path="data/hotjar surveys",
     surveys_list=ids,
     site_id=site_id,
     username=username,
     password=password,
 )
 ```
```

### Comparing `hotjar-data-wrapper-0.1.3/hotjar_data_wrapper/hotjar_api.py` & `hotjar-data-wrapper-0.1.4/hotjar_data_wrapper/hotjar_api.py`

 * *Files identical despite different names*

