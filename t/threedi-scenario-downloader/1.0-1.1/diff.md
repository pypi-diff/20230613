# Comparing `tmp/threedi-scenario-downloader-1.0.tar.gz` & `tmp/threedi-scenario-downloader-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-scenario-downloader-1.0.tar", last modified: Mon May 15 08:33:00 2023, max compression
+gzip compressed data, was "threedi-scenario-downloader-1.1.tar", last modified: Tue Jun 13 11:22:20 2023, max compression
```

## Comparing `threedi-scenario-downloader-1.0.tar` & `threedi-scenario-downloader-1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.304116 threedi-scenario-downloader-1.0/
--rw-r--r--   0 reinout    (501) staff       (20)     2371 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/CHANGES.rst
--rw-r--r--   0 reinout    (501) staff       (20)     1111 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/LICENSE
--rw-r--r--   0 reinout    (501) staff       (20)      203 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)     6466 2023-05-15 08:33:00.304167 threedi-scenario-downloader-1.0/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     3698 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      159 2023-05-15 08:33:00.304352 threedi-scenario-downloader-1.0/setup.cfg
--rw-r--r--   0 reinout    (501) staff       (20)      974 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/setup.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.302578 threedi-scenario-downloader-1.0/threedi_scenario_downloader/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)    27513 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/downloader.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.303767 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     1379 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_batch.py
--rw-r--r--   0 reinout    (501) staff       (20)     2070 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader.py
--rw-r--r--   0 reinout    (501) staff       (20)     4819 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader_manual.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.304008 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/
--rw-r--r--   0 reinout    (501) staff       (20)       31 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/README.rst
--rw-r--r--   0 reinout    (501) staff       (20)      366 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/testdata/batch.csv
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-05-15 08:33:00.303327 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)     6466 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      761 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/not-zip-safe
--rw-r--r--   0 reinout    (501) staff       (20)       67 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)       28 2023-05-15 08:33:00.000000 threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350441 threedi-scenario-downloader-1.1/
+-rw-r--r--   0 reinout    (501) staff       (20)     2655 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/CHANGES.rst
+-rw-r--r--   0 reinout    (501) staff       (20)     1111 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)      203 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)     6799 2023-06-13 11:22:20.350497 threedi-scenario-downloader-1.1/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     3747 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      159 2023-06-13 11:22:20.350701 threedi-scenario-downloader-1.1/setup.cfg
+-rw-r--r--   0 reinout    (501) staff       (20)      974 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/setup.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.348892 threedi-scenario-downloader-1.1/threedi_scenario_downloader/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)    29227 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/downloader.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350083 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     1379 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_batch.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2070 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4819 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader_manual.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.350329 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/
+-rw-r--r--   0 reinout    (501) staff       (20)       31 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/README.rst
+-rw-r--r--   0 reinout    (501) staff       (20)      366 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/testdata/batch.csv
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2023-06-13 11:22:20.349643 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)     6799 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      761 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/not-zip-safe
+-rw-r--r--   0 reinout    (501) staff       (20)       67 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       28 2023-06-13 11:22:20.000000 threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/top_level.txt
```

### Comparing `threedi-scenario-downloader-1.0/CHANGES.rst` & `threedi-scenario-downloader-1.1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.1 (2023-06-13)
+----------------
+
+- Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
+- Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
+- Bugfix with width and height
+
+
 1.0 (2023-05-15)
 ----------------
 
 - Changed functions to support the Lizard API v4 (v3 is not supported with this release)
 - Added error statements for faulty API requests
```

### Comparing `threedi-scenario-downloader-1.0/LICENSE` & `threedi-scenario-downloader-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.0/PKG-INFO` & `threedi-scenario-downloader-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-scenario-downloader
-Version: 1.0
+Version: 1.1
 Summary: Tools for downloading results for 3Di scenarios
 Home-page: https://github.com/nens/threedi-scenario-downloader
 Author: Emiel Verstegen
 Author-email: emiel.verstegen@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -61,18 +61,18 @@
 
   >>> dl.download_raw_results("scenario_uuid",pathname="save_under_different_name.nc")
   >>> dl.download_grid_administration("scenario_uuid",pathname="save_under_different_name.h5")
 
 Downloading (temporal) rasters of specific scenarios can be done using the
 following methods::
 
-  >>> dl.download_maximum_waterdepth_raster("scenario_uuid","EPSG:28992",10)
+  >>> dl.download_maximum_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10)
   #download the full extent of the maximum waterdepth of the given scenario_uuid with a 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
-  >>> dl.download_waterdepth_raster("scenario_uuid","EPSG:28992",10,"2019-01-01T02:00")
+  >>> dl.download_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10,time="2019-01-01T02:00")
   #download the full extend of the waterdepth at the supplied timestamp given scenario_uuid, on 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
 The raster download methods creates a task for the API. Depending on the size
 and resolution it takes some time for the raster to be prepared. These methods
 will keep on checking if the raster is ready to be downloaded.  When a raster
 is ready to be downloaded a message in the Lizard portal is created as
 well. If you want to delete these messages (due to bulk downloading for
@@ -117,14 +117,22 @@
 
   $ bin/pip install -r requirements.txt
 
 
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.1 (2023-06-13)
+----------------
+
+- Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
+- Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
+- Bugfix with width and height
+
+
 1.0 (2023-05-15)
 ----------------
 
 - Changed functions to support the Lizard API v4 (v3 is not supported with this release)
 - Added error statements for faulty API requests
```

### Comparing `threedi-scenario-downloader-1.0/README.rst` & `threedi-scenario-downloader-1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 
   >>> dl.download_raw_results("scenario_uuid",pathname="save_under_different_name.nc")
   >>> dl.download_grid_administration("scenario_uuid",pathname="save_under_different_name.h5")
 
 Downloading (temporal) rasters of specific scenarios can be done using the
 following methods::
 
-  >>> dl.download_maximum_waterdepth_raster("scenario_uuid","EPSG:28992",10)
+  >>> dl.download_maximum_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10)
   #download the full extent of the maximum waterdepth of the given scenario_uuid with a 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
-  >>> dl.download_waterdepth_raster("scenario_uuid","EPSG:28992",10,"2019-01-01T02:00")
+  >>> dl.download_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10,time="2019-01-01T02:00")
   #download the full extend of the waterdepth at the supplied timestamp given scenario_uuid, on 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
 The raster download methods creates a task for the API. Depending on the size
 and resolution it takes some time for the raster to be prepared. These methods
 will keep on checking if the raster is ready to be downloaded.  When a raster
 is ready to be downloaded a message in the Lizard portal is created as
 well. If you want to delete these messages (due to bulk downloading for
```

### Comparing `threedi-scenario-downloader-1.0/setup.py` & `threedi-scenario-downloader-1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "1.0"
+version = "1.1"
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 install_requires = ["requests"]
 tests_require = ["pytest", "mock", "pytest-cov", "pytest-flakes", "pytest-black"]
 setup(
     name="threedi-scenario-downloader",
     version=version,
     description="Tools for downloading results for 3Di scenarios",
```

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader/downloader.py` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,24 @@
     "model_name": "model_name__icontains",
     "organisation": "organisation__icontains",
     "organisation__unique_id": "organisation__unique_id",
     "username": "username__icontains",
     "offset": "offset",
 }
 
+WATER_DEPTH = "depth-dtri"
+MAX_WATER_DEPTH = "depth-max-dtri"
+
+WATER_LEVEL = "s1-dtri"
+MAX_WATER_LEVEL = "s1-max-dtri"
+
+ARRIVAL_TIME = "depth-first-dtri"
+TOTAL_DAMAGE = "total-damage"
+PRECIPITATION = "rain-quad"
+
 
 def set_logging_level(level):
     """set logging level to the supplied level"""
 
     log.level = level
 
 
@@ -98,24 +108,34 @@
         auth=("__key__", get_api_key()),
     )
     r.raise_for_status()
     scenario_instance = r.json()
     return scenario_instance
 
 
-def get_scenario_instance_results(scenario_uuid):
-    """check if scenario exist"""
+def get_scenario_instance_results(scenario_uuid, subendpoint=None):
+    """get the scenario instance results, either from basic raster results, or specific results by using a subendpoint (damage and arrival time)"""
     get_scenario_instance(scenario_uuid)
 
-    """return request response with all raster results"""
-    r = requests.get(
-        url="{}scenarios/{}/results".format(LIZARD_URL, scenario_uuid),
-        auth=("__key__", get_api_key()),
-    )
+    if subendpoint:
+        url = "{}scenarios/{}/results/{}".format(LIZARD_URL, scenario_uuid, subendpoint)
+    else:
+        url = "{}scenarios/{}/results".format(LIZARD_URL, scenario_uuid)
+
+    r = requests.get(url=url, auth=("__key__", get_api_key()))
     r.raise_for_status()
+
+    if not r.json()["results"]:
+        logging.debug(
+            "The result data you request is non-existent, or your user account does not have the rights to request this data"
+        )
+        raise ValueError(
+            "The result data you request is non-existent, or your user account does not have the rights to request this data"
+        )
+
     return r.json()["results"]
 
 
 def get_netcdf_link(scenario_uuid):
     """return url to raw 3Di results"""
     result_list = get_scenario_instance_results(scenario_uuid)
 
@@ -151,37 +171,37 @@
 
     for result in result_list:
         if result["code"] == "logfiles":
             url = result["attachment_url"]
             return url
 
 
-def get_raster_url(scenario_uuid, raster_code):
-    result_list = get_scenario_instance_results(scenario_uuid)
+def get_raster_url(scenario_uuid, raster_code, subendpoint=None):
+    result_list = get_scenario_instance_results(scenario_uuid, subendpoint)
 
     for result in result_list:
         if result["code"] == raster_code:
             raster_url = result["raster"]
             return raster_url
 
 
-def get_raster(scenario_uuid, raster_code):
+def get_raster(scenario_uuid, raster_code, subendpoint=None):
     """return json of raster based on scenario uuid and raster type"""
 
-    raster_url = get_raster_url(scenario_uuid, raster_code)
+    raster_url = get_raster_url(scenario_uuid, raster_code, subendpoint)
 
     r = requests.get(url=raster_url, auth=("__key__", get_api_key()),)
     r.raise_for_status()
 
     raster = r.json()
     return raster
 
 
 def create_raster_task(
-    raster, scenario_instance, resolution=None, projection=None, bbox=None, time=None
+    raster, scenario_instance, projection=None, resolution=None, bbox=None, time=None
 ):
     """create Lizard raster task"""
     x1 = scenario_instance["origin_x"]
     y1 = scenario_instance["origin_y"]
     x2 = scenario_instance["upper_bound_x"]
     y2 = scenario_instance["upper_bound_y"]
 
@@ -193,28 +213,29 @@
     if resolution is None:
         pixelsize_x = abs(scenario_instance["pixelsize_x"])
         pixelsize_y = abs(scenario_instance["pixelsize_y"])
     else:
         pixelsize_x = resolution
         pixelsize_y = resolution
 
-    height = math.ceil((x2 - x1) / pixelsize_x)
-    width = math.ceil((y2 - y1) / pixelsize_y)
+    width = math.ceil((x2 - x1) / pixelsize_x)
+    height = math.ceil((y2 - y1) / pixelsize_y)
 
     url = "{}rasters/{}/data/".format(LIZARD_URL, raster["uuid"])
 
     # non temporal raster
     payload = {
         "width": width,
         "height": height,
         "bbox": bbox,
         "projection": projection,
         "format": "geotiff",
         "async": "true",
     }
+
     if time is not None:
         # temporal rasters
         payload["start"] = time
 
     r = requests.get(url=url, auth=("__key__", get_api_key()), params=payload)
     print_negative_response(r)
 
@@ -307,14 +328,20 @@
     )
 
     # Helper parameters.
     processed_list = transform_to_list(var=False, length=len(scenario_list))
     task_id_list = transform_to_list(var=None, length=len(scenario_list))
     task_url_list = transform_to_list(var=None, length=len(scenario_list))
 
+    # Helper for subendpoints
+    subendpoint_per_raster_code = {
+        ARRIVAL_TIME: "arrival",
+        TOTAL_DAMAGE: "damage",
+    }
+
     # Wrong input error
     if len(scenario_list) != len(pathname_list):
         logging.debug("Scenarios and output should be of same length")
         raise ValueError("scenario_list and pathname_list are of different length")
 
     tasks = []
     # Create tasks
@@ -332,22 +359,30 @@
         projection_list,
         bbox_list,
         resolution_list,
         time_list,
         is_threedi_scenario_list,
     ):
         if is_threedi_scenario:
+
             if type(scenario) is str:
-                # assume uuid
+                # assume 'scenario' is an uuid
                 scenario_instance = get_scenario_instance(scenario)
-                raster = get_raster(scenario, raster_code)
+                subendpoint = subendpoint_per_raster_code.get(raster_code)
+
+                raster = get_raster(scenario, raster_code, subendpoint=subendpoint)
+
             elif type(scenario) is dict:
-                # assume json object
+                # assume 'scenario' is a json object
                 scenario_instance = scenario
-                raster = get_raster_from_json(scenario, raster_code)
+
+                subendpoint = subendpoint_per_raster_code.get(raster_code)
+                raster = get_raster_from_json(
+                    scenario, raster_code, subendpoint=subendpoint
+                )
             else:
                 logging.debug("Invalid scenario: supply a json object or uuid string")
                 raise ValueError(
                     "Invalid scenario: supply a json object or uuid string"
                 )
         else:
             # If no bbox are passed the function will probably crash.
@@ -446,89 +481,103 @@
 
 def download_maximum_waterdepth_raster(
     scenario_uuid, projection, resolution, bbox=None, pathname=None
 ):
     """download Maximum waterdepth raster"""
     download_raster(
         scenario_uuid,
-        "depth-max-dtri",
-        projection,
-        resolution,
+        MAX_WATER_DEPTH,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_maximum_waterlevel_raster(
     scenario_uuid, projection, resolution, bbox=None, pathname=None
 ):
-    """download Maximum waterdepth raster"""
+    """download Maximum waterlevel raster"""
     download_raster(
         scenario_uuid,
-        "s1-max-dtri",
-        projection,
-        resolution,
+        MAX_WATER_LEVEL,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_total_damage_raster(
     scenario_uuid, projection, resolution, bbox=None, pathname=None
 ):
     """download Total Damage raster"""
     download_raster(
         scenario_uuid,
-        "total-damage",
-        projection,
-        resolution,
+        TOTAL_DAMAGE,
+        projection=projection,
+        resolution=resolution,
+        bbox=bbox,
+        pathname=pathname,
+    )
+
+
+def download_arrival_time_raster(
+    scenario_uuid, projection, resolution, bbox=None, pathname=None
+):
+    """download arrival time raster"""
+    download_raster(
+        scenario_uuid,
+        ARRIVAL_TIME,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         pathname=pathname,
     )
 
 
 def download_waterdepth_raster(
     scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
 ):
     """download snapshot of Waterdepth raster"""
     download_raster(
         scenario_uuid,
-        "depth-dtri",
-        projection,
-        resolution,
+        WATER_DEPTH,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         time=time,
         pathname=pathname,
     )
 
 
 def download_waterlevel_raster(
     scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
 ):
-    """download snapshot of Waterdepth raster"""
+    """download snapshot of Waterlevel raster"""
     download_raster(
         scenario_uuid,
-        "s1-dtri",
-        projection,
-        resolution,
+        WATER_LEVEL,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         time=time,
         pathname=pathname,
     )
 
 
 def download_precipitation_raster(
     scenario_uuid, projection, resolution, time, bbox=None, pathname=None,
 ):
-    """download snapshot of Waterdepth raster"""
+    """download snapshot of precipitation raster"""
     download_raster(
         scenario_uuid,
-        "rain-quad",
-        projection,
-        resolution,
+        PRECIPITATION,
+        projection=projection,
+        resolution=resolution,
         bbox=bbox,
         time=time,
         pathname=pathname,
     )
 
 
 def download_raw_results(scenario_uuid, pathname=None):
@@ -745,15 +794,15 @@
         timesteps = [
             timestep_obj.strftime("%Y-%m-%dT%H:%M:%S")
             for timestep_obj in timestep_obj_list
         ]
     return timesteps
 
 
-def get_raster_from_json(scenario_json, raster_code):
+def get_raster_from_json(scenario_json, raster_code, subendpoint=None):
     """return raster json object from scenario"""
     scenario_uuid = scenario_json["uuid"]
     raster_url = get_raster_url(scenario_uuid, raster_code)
 
     r = requests.get(url=raster_url, auth=("__key__", get_api_key()),)
 
     r.raise_for_status()
```

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_batch.py` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader.py` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader/tests/test_downloader_manual.py` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader/tests/test_downloader_manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     assert static_rasters is not None and temporal_rasters is not None
 
 
 def test_get_raster_download_link():
     raster = downloader.get_raster(SCENARIO_UUID, "depth-max-dtri")
     scenario_instance = downloader.get_scenario_instance(SCENARIO_UUID)
     download_url = downloader.get_raster_download_link(
-        raster, scenario_instance, 10, "EPSG:4326", bbox=None, time=None
+        raster, scenario_instance, "EPSG:4326", 10, bbox=None, time=None
     )
     assert download_url is not None
 
 
 def test_download_raster():
     file_path = "threedi_scenario_downloader/tests/testdata/max_wd.tif"
```

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/PKG-INFO` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-scenario-downloader
-Version: 1.0
+Version: 1.1
 Summary: Tools for downloading results for 3Di scenarios
 Home-page: https://github.com/nens/threedi-scenario-downloader
 Author: Emiel Verstegen
 Author-email: emiel.verstegen@nelen-schuurmans.nl
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
@@ -61,18 +61,18 @@
 
   >>> dl.download_raw_results("scenario_uuid",pathname="save_under_different_name.nc")
   >>> dl.download_grid_administration("scenario_uuid",pathname="save_under_different_name.h5")
 
 Downloading (temporal) rasters of specific scenarios can be done using the
 following methods::
 
-  >>> dl.download_maximum_waterdepth_raster("scenario_uuid","EPSG:28992",10)
+  >>> dl.download_maximum_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10)
   #download the full extent of the maximum waterdepth of the given scenario_uuid with a 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
-  >>> dl.download_waterdepth_raster("scenario_uuid","EPSG:28992",10,"2019-01-01T02:00")
+  >>> dl.download_waterdepth_raster("scenario_uuid",projection="EPSG:28992",resolution=10,time="2019-01-01T02:00")
   #download the full extend of the waterdepth at the supplied timestamp given scenario_uuid, on 10 meter resolution in the RD New/Amersfoort projection (EPSG:28992)
 
 The raster download methods creates a task for the API. Depending on the size
 and resolution it takes some time for the raster to be prepared. These methods
 will keep on checking if the raster is ready to be downloaded.  When a raster
 is ready to be downloaded a message in the Lizard portal is created as
 well. If you want to delete these messages (due to bulk downloading for
@@ -117,14 +117,22 @@
 
   $ bin/pip install -r requirements.txt
 
 
 Changelog of threedi-scenario-downloader
 ===================================================
 
+1.1 (2023-06-13)
+----------------
+
+- Added support for sub-endpoints "/api/v4/scenarios/{uuid}/results/damage/" and "/api/v4/scenarios/{uuid}/results/arrival/"
+- Now added the use of keyword arguments for "resolution", "projection","bbox" and "time".
+- Bugfix with width and height
+
+
 1.0 (2023-05-15)
 ----------------
 
 - Changed functions to support the Lizard API v4 (v3 is not supported with this release)
 - Added error statements for faulty API requests
```

### Comparing `threedi-scenario-downloader-1.0/threedi_scenario_downloader.egg-info/SOURCES.txt` & `threedi-scenario-downloader-1.1/threedi_scenario_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

