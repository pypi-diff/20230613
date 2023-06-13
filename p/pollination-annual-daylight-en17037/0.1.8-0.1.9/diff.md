# Comparing `tmp/pollination-annual-daylight-en17037-0.1.8.tar.gz` & `tmp/pollination-annual-daylight-en17037-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.8.tar", last modified: Fri May 26 11:01:02 2023, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.9.tar", last modified: Fri May 26 11:37:25 2023, max compression
```

## Comparing `pollination-annual-daylight-en17037-0.1.8.tar` & `pollination-annual-daylight-en17037-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_process_epw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:00:17.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/_process_epw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:36:41.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:37:25.000000 pollination-annual-daylight-en17037-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 11:36:18.000000 pollination-annual-daylight-en17037-0.1.9/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-en17037-0.1.8/.github/workflows/ci.yaml` & `pollination-annual-daylight-en17037-0.1.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/.github/workflows/tests.yaml` & `pollination-annual-daylight-en17037-0.1.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/LICENSE` & `pollination-annual-daylight-en17037-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.8
+Version: 0.1.9
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_postprocess.py` & `pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/_postprocess.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_process_epw.py` & `pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/_process_epw.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/entry.py` & `pollination-annual-daylight-en17037-0.1.9/pollination/annual_daylight_en17037/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.8
+Version: 0.1.9
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/SOURCES.txt` & `pollination-annual-daylight-en17037-0.1.9/pollination_annual_daylight_en17037.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.8/setup.py` & `pollination-annual-daylight-en17037-0.1.9/setup.py`

 * *Files identical despite different names*

