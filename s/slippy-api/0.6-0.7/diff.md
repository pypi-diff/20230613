# Comparing `tmp/slippy_api-0.6.tar.gz` & `tmp/slippy_api-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippy_api-0.6.tar", last modified: Tue Jun 13 14:09:25 2023, max compression
+gzip compressed data, was "slippy_api-0.7.tar", last modified: Tue Jun 13 14:17:09 2023, max compression
```

## Comparing `slippy_api-0.6.tar` & `slippy_api-0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.308989 slippy_api-0.6/
--rw-rw-rw-   0        0        0     1088 2023-05-27 00:29:32.000000 slippy_api-0.6/LICENSE
--rw-rw-rw-   0        0        0      142 2023-05-27 00:29:32.000000 slippy_api-0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      486 2023-06-13 14:09:25.307989 slippy_api-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-06-13 14:04:11.000000 slippy_api-0.6/README.md
--rw-rw-rw-   0        0        0       88 2023-05-27 00:29:32.000000 slippy_api-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       57 2023-05-27 00:29:32.000000 slippy_api-0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:09:25.308989 slippy_api-0.6/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-06-13 13:43:53.000000 slippy_api-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.283988 slippy_api-0.6/slippi/
--rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-06-12 08:13:01.000000 slippy_api-0.6/slippi/custom_logging.py
--rw-rw-rw-   0        0        0      522 2023-06-12 08:05:15.000000 slippy_api-0.6/slippi/main.py
--rw-rw-rw-   0        0        0     5479 2023-06-13 12:41:58.000000 slippy_api-0.6/slippi/slippi_api.py
--rw-rw-rw-   0        0        0     3170 2023-06-13 12:48:50.000000 slippy_api-0.6/slippi/slippi_characters.py
--rw-rw-rw-   0        0        0     2014 2023-06-13 12:55:21.000000 slippy_api-0.6/slippi/slippi_ranks.py
--rw-rw-rw-   0        0        0     5562 2023-06-13 13:34:53.000000 slippy_api-0.6/slippi/slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.291989 slippy_api-0.6/slippi/tests/
--rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/__init__.py
--rw-rw-rw-   0        0        0     2039 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_api.py
--rw-rw-rw-   0        0        0      671 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_characters.py
--rw-rw-rw-   0        0        0      885 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_ranks.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 00:29:32.000000 slippy_api-0.6/slippi/tests/test_slippi_user.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:09:25.306987 slippy_api-0.6/slippy_api.egg-info/
--rw-rw-rw-   0        0        0      486 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 14:09:25.000000 slippy_api-0.6/slippy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:17:09.611427 slippy_api-0.7/
+-rw-rw-rw-   0        0        0     1088 2023-05-27 00:29:32.000000 slippy_api-0.7/LICENSE
+-rw-rw-rw-   0        0        0      142 2023-05-27 00:29:32.000000 slippy_api-0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1031 2023-06-13 14:17:09.611427 slippy_api-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-06-13 14:04:11.000000 slippy_api-0.7/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-27 00:29:32.000000 slippy_api-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2023-05-27 00:29:32.000000 slippy_api-0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:17:09.611427 slippy_api-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-13 14:14:25.000000 slippy_api-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:17:09.591428 slippy_api-0.7/slippi/
+-rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-06-12 08:13:01.000000 slippy_api-0.7/slippi/custom_logging.py
+-rw-rw-rw-   0        0        0      522 2023-06-12 08:05:15.000000 slippy_api-0.7/slippi/main.py
+-rw-rw-rw-   0        0        0     5479 2023-06-13 12:41:58.000000 slippy_api-0.7/slippi/slippi_api.py
+-rw-rw-rw-   0        0        0     3170 2023-06-13 12:48:50.000000 slippy_api-0.7/slippi/slippi_characters.py
+-rw-rw-rw-   0        0        0     2014 2023-06-13 12:55:21.000000 slippy_api-0.7/slippi/slippi_ranks.py
+-rw-rw-rw-   0        0        0     5562 2023-06-13 13:34:53.000000 slippy_api-0.7/slippi/slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:17:09.596427 slippy_api-0.7/slippi/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/tests/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/tests/test_slippi_api.py
+-rw-rw-rw-   0        0        0      671 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/tests/test_slippi_characters.py
+-rw-rw-rw-   0        0        0      885 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/tests/test_slippi_ranks.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 00:29:32.000000 slippy_api-0.7/slippi/tests/test_slippi_user.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:17:09.609427 slippy_api-0.7/slippy_api.egg-info/
+-rw-rw-rw-   0        0        0     1031 2023-06-13 14:17:09.000000 slippy_api-0.7/slippy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-06-13 14:17:09.000000 slippy_api-0.7/slippy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:17:09.000000 slippy_api-0.7/slippy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-13 14:17:09.000000 slippy_api-0.7/slippy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 14:17:09.000000 slippy_api-0.7/slippy_api.egg-info/top_level.txt
```

### Comparing `slippy_api-0.6/LICENSE` & `slippy_api-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/README.md` & `slippy_api-0.7/README.md`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/custom_logging.py` & `slippy_api-0.7/slippi/custom_logging.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/main.py` & `slippy_api-0.7/slippi/main.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/slippi_api.py` & `slippy_api-0.7/slippi/slippi_api.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/slippi_characters.py` & `slippy_api-0.7/slippi/slippi_characters.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/slippi_ranks.py` & `slippy_api-0.7/slippi/slippi_ranks.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/slippi_user.py` & `slippy_api-0.7/slippi/slippi_user.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/tests/test_slippi_api.py` & `slippy_api-0.7/slippi/tests/test_slippi_api.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/tests/test_slippi_characters.py` & `slippy_api-0.7/slippi/tests/test_slippi_characters.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/tests/test_slippi_ranks.py` & `slippy_api-0.7/slippi/tests/test_slippi_ranks.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippi/tests/test_slippi_user.py` & `slippy_api-0.7/slippi/tests/test_slippi_user.py`

 * *Files identical despite different names*

### Comparing `slippy_api-0.6/slippy_api.egg-info/SOURCES.txt` & `slippy_api-0.7/slippy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

