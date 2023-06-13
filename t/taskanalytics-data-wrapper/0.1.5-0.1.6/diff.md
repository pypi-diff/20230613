# Comparing `tmp/taskanalytics-data-wrapper-0.1.5.tar.gz` & `tmp/taskanalytics-data-wrapper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskanalytics-data-wrapper-0.1.5.tar", last modified: Fri Jun  2 19:16:57 2023, max compression
+gzip compressed data, was "taskanalytics-data-wrapper-0.1.6.tar", last modified: Tue Jun 13 13:21:54 2023, max compression
```

## Comparing `taskanalytics-data-wrapper-0.1.5.tar` & `taskanalytics-data-wrapper-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.812790 taskanalytics-data-wrapper-0.1.5/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      357 2023-06-02 19:16:57.812936 taskanalytics-data-wrapper-0.1.5/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3362 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/README.md
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      478 2023-06-02 19:16:57.814629 taskanalytics-data-wrapper-0.1.5/setup.cfg
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:04:15.000000 taskanalytics-data-wrapper-0.1.5/setup.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.808730 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:58:55.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/taskanalytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:16:57.812186 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      357 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      323 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       27 2023-06-02 19:16:57.000000 taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.562163 taskanalytics-data-wrapper-0.1.6/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.6/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3837 2023-06-13 13:21:54.562317 taskanalytics-data-wrapper-0.1.6/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3438 2023-06-02 19:20:01.000000 taskanalytics-data-wrapper-0.1.6/README.md
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      559 2023-06-13 13:21:54.563893 taskanalytics-data-wrapper-0.1.6/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.6/setup.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.558067 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:20:43.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5217 2023-05-21 17:59:37.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/taskanalytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:21:54.561502 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     3837 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      323 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       27 2023-06-13 13:21:54.000000 taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper.egg-info/top_level.txt
```

### Comparing `taskanalytics-data-wrapper-0.1.5/LICENSE` & `taskanalytics-data-wrapper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taskanalytics-data-wrapper-0.1.5/README.md` & `taskanalytics-data-wrapper-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,28 @@
 ```
 
 ### Download Survey responses
 
 You can download survey responses for a Top Task survey using the survey ID, email, password and setting a path for where to store the file.
 
 ```python
-get_survey = download_survey(
+import taskanalytics_data_wrapper.taskanalytics_api as task
+
+get_survey = task.download_survey(
     username=email, password=password, survey_id="03324", filename="data/survey.csv"
 )
 get_survey.status_code
 ```
 
 ### Download Survey metadata
 
 You can download the survey metadata which includes the questions and response options for each survey using the survey ID, email and password.
 
 ```python
-survey_metadata = get_survey_metadata(
+survey_metadata = task.get_survey_metadata(
     username=email, password=password, survey_id="03324"
 )
 survey_metadata.status_code
 ```
 
 The object can be easily inspected transformed into a dictionary for analysis
 
@@ -52,15 +54,15 @@
 ```
 
 ### Download Discovery survey responses
 
 You can download responses from open ended task discovery surveys as well
 
 ```python
-get_openended_survey = download_discovery_survey(
+get_openended_survey = task.download_discovery_survey(
     username=email, password=password, organization_id=organization, survey_id="03230"
 )
 ```
 See how to turn this into csv in the code example below by expanding
 
 <details>
 <summary>Expandable example</summary>
```

### Comparing `taskanalytics-data-wrapper-0.1.5/taskanalytics_data_wrapper/taskanalytics_api.py` & `taskanalytics-data-wrapper-0.1.6/taskanalytics_data_wrapper/taskanalytics_api.py`

 * *Files identical despite different names*

