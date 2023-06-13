# Comparing `tmp/ape-polygon-0.6.3.tar.gz` & `tmp/ape-polygon-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.6.3.tar", last modified: Tue Jun 13 01:26:03 2023, max compression
+gzip compressed data, was "ape-polygon-0.6.4.tar", last modified: Tue Jun 13 14:05:41 2023, max compression
```

## Comparing `ape-polygon-0.6.3.tar` & `ape-polygon-0.6.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.861336 ape-polygon-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.861336 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.658024 ape-polygon-0.6.4/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 14:05:41.000000 ape-polygon-0.6.4/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:05:41.662024 ape-polygon-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 14:04:32.000000 ape-polygon-0.6.4/tests/test_provider.py
```

### Comparing `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.6.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/release-drafter.yml` & `ape-polygon-0.6.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/workflows/commitlint.yaml` & `ape-polygon-0.6.4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/workflows/prtitle.yaml` & `ape-polygon-0.6.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/workflows/publish.yaml` & `ape-polygon-0.6.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.github/workflows/test.yaml` & `ape-polygon-0.6.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.gitignore` & `ape-polygon-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/.pre-commit-config.yaml` & `ape-polygon-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/CONTRIBUTING.md` & `ape-polygon-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/LICENSE` & `ape-polygon-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/PKG-INFO` & `ape-polygon-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-polygon-0.6.3/README.md` & `ape-polygon-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/ape_polygon/__init__.py` & `ape-polygon-0.6.4/ape_polygon/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,9 +27,10 @@
     yield "polygon", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
         yield "polygon", network_name, GethProvider
+        yield "polygon", f"{network_name}-fork", LocalProvider
 
     yield "polygon", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-polygon-0.6.3/ape_polygon/ecosystem.py` & `ape-polygon-0.6.4/ape_polygon/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.6.4/ape_polygon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.3
+Version: 0.6.4
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-polygon-0.6.3/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.6.4/ape_polygon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/ape_polygon.egg-info/requires.txt` & `ape-polygon-0.6.4/ape_polygon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/pyproject.toml` & `ape-polygon-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/setup.py` & `ape-polygon-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.3/tests/test_integration.py` & `ape-polygon-0.6.4/tests/test_integration.py`

 * *Files identical despite different names*

