# Comparing `tmp/ape-base-0.1.1.tar.gz` & `tmp/ape-base-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-base-0.1.1.tar", last modified: Tue Jun 13 00:41:39 2023, max compression
+gzip compressed data, was "ape-base-0.6.0.tar", last modified: Tue Jun 13 03:41:31 2023, max compression
```

## Comparing `ape-base-0.1.1.tar` & `ape-base-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 00:40:27.000000 ape-base-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 00:40:27.000000 ape-base-0.1.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 00:40:27.000000 ape-base-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-13 00:40:27.000000 ape-base-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 00:40:27.000000 ape-base-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 00:41:39.412399 ape-base-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-13 00:40:27.000000 ape-base-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/ape_base/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/ape_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 00:40:27.000000 ape-base-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 00:41:39.412399 ape-base-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-13 00:40:27.000000 ape-base-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.830806 ape-base-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.826806 ape-base-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.826806 ape-base-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.826806 ape-base-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 03:40:06.000000 ape-base-0.6.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 03:40:06.000000 ape-base-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 03:40:06.000000 ape-base-0.6.0/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 03:40:06.000000 ape-base-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-13 03:40:06.000000 ape-base-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 03:40:06.000000 ape-base-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 03:41:31.830806 ape-base-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-13 03:40:06.000000 ape-base-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.826806 ape-base-0.6.0/ape_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 03:40:06.000000 ape-base-0.6.0/ape_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-13 03:40:06.000000 ape-base-0.6.0/ape_base/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:40:06.000000 ape-base-0.6.0/ape_base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.826806 ape-base-0.6.0/ape_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 03:41:31.000000 ape-base-0.6.0/ape_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 03:40:06.000000 ape-base-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 03:41:31.830806 ape-base-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-13 03:40:06.000000 ape-base-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:41:31.830806 ape-base-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:40:06.000000 ape-base-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 03:40:06.000000 ape-base-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 03:40:06.000000 ape-base-0.6.0/tests/test_provider.py
```

### Comparing `ape-base-0.1.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-base-0.6.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-base-0.6.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-base-0.6.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/release-drafter.yml` & `ape-base-0.6.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/workflows/codeql.yaml` & `ape-base-0.6.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/workflows/commitlint.yaml` & `ape-base-0.6.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/workflows/prtitle.yaml` & `ape-base-0.6.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/workflows/publish.yaml` & `ape-base-0.6.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.github/workflows/test.yaml` & `ape-base-0.6.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.gitignore` & `ape-base-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/.pre-commit-config.yaml` & `ape-base-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/CONTRIBUTING.md` & `ape-base-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/LICENSE` & `ape-base-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/PKG-INFO` & `ape-base-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.1.1
+Version: 0.6.0
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-base-0.1.1/README.md` & `ape-base-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/ape_base/__init__.py` & `ape-base-0.6.0/ape_base/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/ape_base/ecosystem.py` & `ape-base-0.6.0/ape_base/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/ape_base.egg-info/PKG-INFO` & `ape-base-0.6.0/ape_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.1.1
+Version: 0.6.0
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-base-0.1.1/ape_base.egg-info/SOURCES.txt` & `ape-base-0.6.0/ape_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/ape_base.egg-info/requires.txt` & `ape-base-0.6.0/ape_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/pyproject.toml` & `ape-base-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/setup.py` & `ape-base-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.1/tests/test_provider.py` & `ape-base-0.6.0/tests/test_provider.py`

 * *Files identical despite different names*

