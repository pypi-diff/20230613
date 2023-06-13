# Comparing `tmp/hayloft-0.1.2.tar.gz` & `tmp/hayloft-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.2.tar", max compression
+gzip compressed data, was "hayloft-0.1.3.tar", max compression
```

## Comparing `hayloft-0.1.2.tar` & `hayloft-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.2/LICENSE
--rw-r--r--   0        0        0      119 2023-06-13 15:27:19.792693 hayloft-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.2/hayloft/__init__.py
--rw-r--r--   0        0        0     3185 2023-06-13 17:03:36.638281 hayloft-0.1.2/hayloft/app.py
--rw-r--r--   0        0        0      455 2023-06-13 17:02:40.814396 hayloft-0.1.2/hayloft/logger.py
--rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.2/hayloft/public/assets/index-144454fa.css
--rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.2/hayloft/public/assets/index-efbd5a31.js
--rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.2/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.2/hayloft/schema.py
--rw-r--r--   0        0        0      430 2023-06-13 17:03:43.625017 hayloft-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 hayloft-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.3/LICENSE
+-rw-r--r--   0        0        0      293 2023-06-13 17:37:06.188148 hayloft-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.3/hayloft/__init__.py
+-rw-r--r--   0        0        0     3185 2023-06-13 17:03:36.638281 hayloft-0.1.3/hayloft/app.py
+-rw-r--r--   0        0        0      455 2023-06-13 17:02:40.814396 hayloft-0.1.3/hayloft/logger.py
+-rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.3/hayloft/public/assets/index-144454fa.css
+-rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.3/hayloft/public/assets/index-efbd5a31.js
+-rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.3/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.3/hayloft/schema.py
+-rw-r--r--   0        0        0      430 2023-06-13 17:46:13.723561 hayloft-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 hayloft-0.1.3/PKG-INFO
```

### Comparing `hayloft-0.1.2/LICENSE` & `hayloft-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.2/hayloft/app.py` & `hayloft-0.1.3/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.2/hayloft/public/assets/index-144454fa.css` & `hayloft-0.1.3/hayloft/public/assets/index-144454fa.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.2/hayloft/public/assets/index-efbd5a31.js` & `hayloft-0.1.3/hayloft/public/assets/index-efbd5a31.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.2/hayloft/schema.py` & `hayloft-0.1.3/hayloft/schema.py`

 * *Files identical despite different names*

