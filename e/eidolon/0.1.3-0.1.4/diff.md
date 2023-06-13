# Comparing `tmp/eidolon-0.1.3.tar.gz` & `tmp/eidolon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon-0.1.3.tar", max compression
+gzip compressed data, was "eidolon-0.1.4.tar", max compression
```

## Comparing `eidolon-0.1.3.tar` & `eidolon-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1053 2023-06-06 20:22:19.935316 eidolon-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     1344 2023-06-06 20:18:33.530135 eidolon-0.1.3/README.md
--rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.3/eidolon/__init__.py
--rw-r--r--   0        0        0     3174 2023-06-06 20:01:33.035631 eidolon-0.1.3/eidolon/api_request.py
--rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.3/eidolon/tracker.py
--rw-r--r--   0        0        0      791 2023-06-06 20:35:21.376600 eidolon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 eidolon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-06-06 20:22:19.935316 eidolon-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     1344 2023-06-06 20:18:33.530135 eidolon-0.1.4/README.md
+-rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.4/eidolon/__init__.py
+-rw-r--r--   0        0        0     3316 2023-06-13 06:57:55.039584 eidolon-0.1.4/eidolon/api_request.py
+-rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.4/eidolon/tracker.py
+-rw-r--r--   0        0        0      791 2023-06-13 06:58:03.387668 eidolon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 eidolon-0.1.4/PKG-INFO
```

### Comparing `eidolon-0.1.3/LICENSE.md` & `eidolon-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.3/README.md` & `eidolon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.3/eidolon/__init__.py` & `eidolon-0.1.4/eidolon/__init__.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.3/eidolon/api_request.py` & `eidolon-0.1.4/eidolon/api_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         logging.info(f"Starting request #{self.task_id}")
         error = None
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.request(
                     method=self.request_method,
                     url=self.request_url,
+                    params=self.request_params,
+                    headers=self.request_headers,
+                    json=self.request_json,
                 ) as response:
                     if response.status == 429:
                         logging.warning(
                             f"Request {self.task_id} failed with status 429"
                         )
                         status_tracker.num_rate_limit_errors += 1
                         status_tracker.time_of_last_rate_limit_error = time.time()
```

### Comparing `eidolon-0.1.3/eidolon/tracker.py` & `eidolon-0.1.4/eidolon/tracker.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.3/pyproject.toml` & `eidolon-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon"
-version = "0.1.3"
+version = "0.1.4"
 description = "A utility to concurrently make HTTP requests, with an optional rate limit. Powered by asyncio and aiohttp"
 authors = ["Sphericalkat <amolele@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SphericalKat/eidolon"
 repository = "https://github.com/SphericalKat/eidolon"
 documentation = "https://github.com/SphericalKat/eidolon/blob/main/README.md"
```

### Comparing `eidolon-0.1.3/PKG-INFO` & `eidolon-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon
-Version: 0.1.3
+Version: 0.1.4
 Summary: A utility to concurrently make HTTP requests, with an optional rate limit. Powered by asyncio and aiohttp
 Home-page: https://github.com/SphericalKat/eidolon
 License: MIT
 Keywords: asyncio,aiohttp,http,requests,concurrency,rate-limit
 Author: Sphericalkat
 Author-email: amolele@gmail.com
 Requires-Python: >=3.7
```

