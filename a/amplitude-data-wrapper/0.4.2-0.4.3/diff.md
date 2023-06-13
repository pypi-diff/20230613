# Comparing `tmp/amplitude-data-wrapper-0.4.2.tar.gz` & `tmp/amplitude-data-wrapper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude-data-wrapper-0.4.2.tar", last modified: Fri Jun  2 18:55:24 2023, max compression
+gzip compressed data, was "amplitude-data-wrapper-0.4.3.tar", last modified: Tue Jun 13 13:12:36 2023, max compression
```

## Comparing `amplitude-data-wrapper-0.4.2.tar` & `amplitude-data-wrapper-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.509167 amplitude-data-wrapper-0.4.2/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      343 2023-06-02 18:55:24.509325 amplitude-data-wrapper-0.4.2/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/README.md
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.504127 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-01 19:50:54.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/__init__.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/analytics_api.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.508505 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      343 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      295 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      464 2023-06-02 18:55:24.510942 amplitude-data-wrapper-0.4.2/setup.cfg
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 18:31:26.000000 amplitude-data-wrapper-0.4.2/setup.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:12:36.567867 amplitude-data-wrapper-0.4.3/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.3/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4663 2023-06-13 13:12:36.568004 amplitude-data-wrapper-0.4.3/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4278 2023-06-02 19:23:15.000000 amplitude-data-wrapper-0.4.3/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:12:36.563934 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 19:08:45.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper/analytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-13 13:12:36.567295 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4663 2023-06-13 13:12:36.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      295 2023-06-13 13:12:36.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-13 13:12:36.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-06-13 13:12:36.000000 amplitude-data-wrapper-0.4.3/amplitude_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      545 2023-06-13 13:12:36.571229 amplitude-data-wrapper-0.4.3/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 19:08:45.000000 amplitude-data-wrapper-0.4.3/setup.py
```

### Comparing `amplitude-data-wrapper-0.4.2/LICENSE` & `amplitude-data-wrapper-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.2/README.md` & `amplitude-data-wrapper-0.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,91 +33,89 @@
 ### Dashboard Rest API
 
 [Results from an existing chart](https://developers.amplitude.com/docs/dashboard-rest-api#results-from-an-existing-chart)
 
 Get data from EU account by setting `region=1`.
 
 ```python
-from amplitude_data_wrapper import get_chart
+import amplitude_data_wrapper.analytics_api as amp
 
-r = get_chart(chart_id, api_key, api_secret, region=1)
+r = amp.get_chart(chart_id, api_key, api_secret, region=1)
 r.status_code  # 200
 r.text # print data
 ```
 
 Get data from US account by setting `region=2`.
 
 ```python
-from amplitude_data_wrapper import get_chart
 
-r = get_chart(chart_id, api_key, api_secret, region=2)
+r = amp.get_chart(chart_id, api_key, api_secret, region=2)
 r.status_code  # 200
 r.text # print data
 ```
 
 Get data from EU account with a proxy by setting region and proxy using a dictionary.
 
 ```python
-from amplitude_data_wrapper import get_chart
 
 proxies = {"http": "http://myproxy.domain.org/path"}
-r = get_chart(chart_id, api_key, api_secret, region=1, proxy=proxies)
+r = amp.get_chart(chart_id, api_key, api_secret, region=1, proxy=proxies)
 r.status_code  # 200
 r.text # print data
 ```
 
 [Event segmentation](https://developers.amplitude.com/docs/dashboard-rest-api#event-segmentation) lets you export events with segments and filters.
 
 ```python
 our_event_dict = {
     "event_type": "pageview",
     "group_by": [{"type": "event", "value": "app"}, {"type": "event", "value": "team"}],
 }
-data = get_event_segmentation(
+data = amp.get_event_segmentation(
     api_key=api_key,
     secret=api_secret,
     start="20220601",
     end="20220602",
     event=our_event_dict,
     metrics="uniques",
     interval=1,
     limit=1000,
 )
 ```
 
 [User search](https://developers.amplitude.com/docs/dashboard-rest-api#user-search) lets you search for a user with a specific Amplitude ID, Device ID, User ID, or User ID prefix.
 
 ```python
-user = find_user(
+user = amp.find_user(
     user=example_id_eu, 
     api_key=api_key, 
     secret=api_secret,
     region=1)
 ```
 
 ### Privacy API
 
 Delete user data with a [deletion job](https://developers.amplitude.com/docs/user-deletion#deletion-job)
 
 ```python
-deleteme = delete_user_data(
+deleteme = amp.delete_user_data(
     user["matches"][0]["amplitude_id"],
     email=email,
     api_key=api_key,
     secret=api_secret,
     region=1,
     ignore_invalid_id=True,
     delete_from_org=False,
 )
 ```
 
 [Get a list of deletion jobs](https://developers.amplitude.com/docs/user-deletion#get)
 
 ```python
-tobe_deleted = get_deletion_jobs(
+tobe_deleted = amp.get_deletion_jobs(
     start="2022-06-01",
     end="2022-07-01",
     api_key=api_key,
     secret=api_secret,
     region=1,
 )
 ```
@@ -125,15 +123,15 @@
 ### Cohort API
 
 [Getting one cohort](https://developers.amplitude.com/docs/behavioral-cohorts-api#getting-one-cohort)
 
 ```python
 proxies = {"http": "http://myproxy.domain.org/path"}
 file_path = "path-to/cohortdata.csv"
-kull = get_cohort(
+kull = amp.get_cohort(
     api_key,
     api_secret,
     cohort_id,
     filename=file_path,
     props=1,
     region=1,
     proxy=proxies,
@@ -143,27 +141,27 @@
 ### Export API
 
 [Export API - Export your project's event data](https://developers.amplitude.com/docs/export-api#export-api---export-your-projects-event-data)
 
 ```python
 start = "20220601T00"
 end = "20220601T01"
-data = export_project_data(
+data = amp.export_project_data(
     start=start,
     end=end,
     api_key=api_key,
     secret=api_secret,
     filename="path-to/projectdata_eu.zip",
     region=1,
 )
 ```
 
 ### Taxonomy API
 
 [Get all event types](https://developers.amplitude.com/docs/taxonomy-api#get-all-event-types)
 
 ```python
-types = get_all_event_types(
+types = amp.get_all_event_types(
     api_key=api_key, 
     secret=api_secret, 
     region=1)
 ```
```

### Comparing `amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/analytics_api.py` & `amplitude-data-wrapper-0.4.3/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

