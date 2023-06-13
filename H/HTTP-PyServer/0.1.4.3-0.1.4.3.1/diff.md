# Comparing `tmp/HTTP-PyServer-0.1.4.3.tar.gz` & `tmp/HTTP-PyServer-0.1.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.4.3.tar", last modified: Mon Jun 12 00:05:29 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.3.1.tar", last modified: Tue Jun 13 18:45:01 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.4.3.tar` & `HTTP-PyServer-0.1.4.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.343387 HTTP-PyServer-0.1.4.3/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.3/LICENSE
--rw-rw-rw-   0        0        0     2106 2023-06-12 00:05:29.342388 HTTP-PyServer-0.1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.3/README.md
--rw-rw-rw-   0        0        0      643 2023-06-12 00:05:06.000000 HTTP-PyServer-0.1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 00:05:29.344383 HTTP-PyServer-0.1.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.282549 HTTP-PyServer-0.1.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.306484 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2106 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.340394 HTTP-PyServer-0.1.4.3/src/server/
--rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.3/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.3/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.3/src/server/render.py
--rw-rw-rw-   0        0        0     4667 2023-06-12 00:04:01.000000 HTTP-PyServer-0.1.4.3/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.3/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.3/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.3/src/server/response_messages.py
--rw-rw-rw-   0        0        0     8866 2023-06-11 23:42:15.000000 HTTP-PyServer-0.1.4.3/src/server/routes.py
--rw-rw-rw-   0        0        0     7406 2023-06-11 23:52:43.000000 HTTP-PyServer-0.1.4.3/src/server/server.py
--rw-rw-rw-   0        0        0     3588 2023-06-11 23:50:14.000000 HTTP-PyServer-0.1.4.3/src/server/sessions.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.3/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.073362 HTTP-PyServer-0.1.4.3.1/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2108 2023-06-13 18:45:01.072364 HTTP-PyServer-0.1.4.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.3.1/README.md
+-rw-rw-rw-   0        0        0      645 2023-06-13 18:44:48.000000 HTTP-PyServer-0.1.4.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:45:01.073362 HTTP-PyServer-0.1.4.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 18:45:00.987591 HTTP-PyServer-0.1.4.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.017510 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2108 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 18:45:00.000000 HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:45:01.069373 HTTP-PyServer-0.1.4.3.1/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.3.1/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.3.1/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.3.1/src/server/render.py
+-rw-rw-rw-   0        0        0     4667 2023-06-12 00:04:01.000000 HTTP-PyServer-0.1.4.3.1/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.3.1/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.3.1/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.3.1/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8866 2023-06-11 23:42:15.000000 HTTP-PyServer-0.1.4.3.1/src/server/routes.py
+-rw-rw-rw-   0        0        0     7390 2023-06-13 18:43:49.000000 HTTP-PyServer-0.1.4.3.1/src/server/server.py
+-rw-rw-rw-   0        0        0     3588 2023-06-11 23:50:14.000000 HTTP-PyServer-0.1.4.3.1/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.3.1/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.4.3/LICENSE` & `HTTP-PyServer-0.1.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/PKG-INFO` & `HTTP-PyServer-0.1.4.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.3
+Version: 0.1.4.3.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.3/README.md` & `HTTP-PyServer-0.1.4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/pyproject.toml` & `HTTP-PyServer-0.1.4.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.4.3"
+version = "0.1.4.3.1"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4.3.1/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.3
+Version: 0.1.4.3.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.3/src/server/cache.py` & `HTTP-PyServer-0.1.4.3.1/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/render.py` & `HTTP-PyServer-0.1.4.3.1/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/request.py` & `HTTP-PyServer-0.1.4.3.1/src/server/request.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/response.py` & `HTTP-PyServer-0.1.4.3.1/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/response_codes.py` & `HTTP-PyServer-0.1.4.3.1/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/response_messages.py` & `HTTP-PyServer-0.1.4.3.1/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/routes.py` & `HTTP-PyServer-0.1.4.3.1/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/server.py` & `HTTP-PyServer-0.1.4.3.1/src/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,23 +173,24 @@
 
                     connection.close()
 
                     return None
 
                 if content_length:=parsed_request.headers.get('Content-Length'):
 
-                    if (length_recieved:=len(raw_request.split(b'\r\n\r\n')[1])) < \
-                    (length_to_recieve:=int(content_length)):
-
-                        raw_request += connection.recv(length_to_recieve - \
-                                                       length_recieved)
-
-                        parsed_request = request.Request.from_bytestring(
-                                        address = address,
-                                        request = raw_request)
+                    content_length = int(content_length)
+                        
+                    while (body_length:=len(raw_request.split(b'\r\n\r\n', 1)[1]))\
+                    < (content_length):
+
+                        raw_request += connection.recv(content_length - body_length)
+
+                    parsed_request = request.Request.from_bytestring(
+                                    address = address,
+                                    request = raw_request)
 
                 if self._logger:
 
                     self._logger.debug(f'Recieved {parsed_request.method} request from \
 {address[0]}:{address[1]} for {parsed_request.path if parsed_request.path else "/"}')
 
                 connection.send(self._get_route(path = parsed_request.path,
```

### Comparing `HTTP-PyServer-0.1.4.3/src/server/sessions.py` & `HTTP-PyServer-0.1.4.3.1/src/server/sessions.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.3/src/server/template.py` & `HTTP-PyServer-0.1.4.3.1/src/server/template.py`

 * *Files identical despite different names*

