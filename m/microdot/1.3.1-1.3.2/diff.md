# Comparing `tmp/microdot-1.3.1.tar.gz` & `tmp/microdot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdot-1.3.1.tar", last modified: Sun May 21 22:37:39 2023, max compression
+gzip compressed data, was "microdot-1.3.2.tar", last modified: Tue Jun 13 13:45:09 2023, max compression
```

## Comparing `microdot-1.3.1.tar` & `microdot-1.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.925662 microdot-1.3.1/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.1/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-05-21 22:37:39.925885 microdot-1.3.1/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.1/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.1/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-05-21 22:37:39.926865 microdot-1.3.1/setup.cfg
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.1/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.906470 microdot-1.3.1/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.909988 microdot-1.3.1/src/microdot.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.1/src/microdot.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/top_level.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)    46254 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4912 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asgi_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_utemplate.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_websocket_alt.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_wsgi.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.925071 microdot-1.3.1/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_cors.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5072 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_wsgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-03-23 00:04:52.000000 microdot-1.3.1/tests/test_multidict.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-04-08 16:16:17.000000 microdot-1.3.1/tests/test_request.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_request_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-03-21 00:28:33.000000 microdot-1.3.1/tests/test_response.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_response_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4188 2023-05-21 22:22:15.000000 microdot-1.3.1/tests/test_url_pattern.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2022-09-24 18:55:50.000000 microdot-1.3.1/tests/test_urlencode.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_utemplate.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.783913 microdot-1.3.2/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.2/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-06-13 13:45:09.784158 microdot-1.3.2/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.2/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.2/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-06-13 13:45:09.785465 microdot-1.3.2/setup.cfg
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.2/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.759444 microdot-1.3.2/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.763285 microdot-1.3.2/src/microdot.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.2/src/microdot.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-06-13 13:45:09.000000 microdot-1.3.2/src/microdot.egg-info/top_level.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    46254 2023-06-07 23:27:49.000000 microdot-1.3.2/src/microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4952 2023-06-07 22:50:44.000000 microdot-1.3.2/src/microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_asgi_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-06-07 23:27:49.000000 microdot-1.3.2/src/microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_asyncio_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-06-06 22:20:32.000000 microdot-1.3.2/src/microdot_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_utemplate.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-06-06 22:21:28.000000 microdot-1.3.2/src/microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-06-06 22:19:56.000000 microdot-1.3.2/src/microdot_websocket_alt.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-06-06 22:20:32.000000 microdot-1.3.2/src/microdot_wsgi.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-06-13 13:45:09.783067 microdot-1.3.2/tests/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_cors.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5088 2023-06-07 22:50:44.000000 microdot-1.3.2/tests/test_microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_microdot_wsgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_multidict.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_request.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_request_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_response.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_response_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-06-06 22:20:36.000000 microdot-1.3.2/tests/test_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4188 2023-06-06 22:21:28.000000 microdot-1.3.2/tests/test_url_pattern.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2023-06-06 22:20:32.000000 microdot-1.3.2/tests/test_urlencode.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-06-06 22:19:56.000000 microdot-1.3.2/tests/test_utemplate.py
```

### Comparing `microdot-1.3.1/LICENSE` & `microdot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/PKG-INFO` & `microdot-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.1
+Version: 1.3.2
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.3.1/README.md` & `microdot-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/setup.cfg` & `microdot-1.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = microdot
-version = 1.3.1
+version = 1.3.2
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = The impossibly small web framework for MicroPython
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/microdot
 project_urls =
```

### Comparing `microdot-1.3.1/src/microdot.egg-info/PKG-INFO` & `microdot-1.3.2/src/microdot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.1
+Version: 1.3.2
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.3.1/src/microdot.egg-info/SOURCES.txt` & `microdot-1.3.2/src/microdot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot.py` & `microdot-1.3.2/src/microdot.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_asgi.py` & `microdot-1.3.2/src/microdot_asgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,17 @@
             return
         path = scope['path']
         if 'query_string' in scope and scope['query_string']:
             path += '?' + scope['query_string'].decode()
         headers = NoCaseDict()
         content_length = 0
         for key, value in scope.get('headers', []):
-            headers[key] = value
-            if key.lower() == 'content-length':
+            key = key.decode().title()
+            headers[key] = value.decode()
+            if key == 'Content-Length':
                 content_length = int(value)
 
         if content_length and content_length <= Request.max_body_length:
             body = b''
             more = True
             while more:
                 packet = await receive()
```

### Comparing `microdot-1.3.1/src/microdot_asgi_websocket.py` & `microdot-1.3.2/src/microdot_asgi_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_asyncio.py` & `microdot-1.3.2/src/microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_asyncio_test_client.py` & `microdot-1.3.2/src/microdot_asyncio_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_asyncio_websocket.py` & `microdot-1.3.2/src/microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_jinja.py` & `microdot-1.3.2/src/microdot_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_session.py` & `microdot-1.3.2/src/microdot_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_test_client.py` & `microdot-1.3.2/src/microdot_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_utemplate.py` & `microdot-1.3.2/src/microdot_utemplate.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_websocket.py` & `microdot-1.3.2/src/microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_websocket_alt.py` & `microdot-1.3.2/src/microdot_websocket_alt.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/src/microdot_wsgi.py` & `microdot-1.3.2/src/microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_cors.py` & `microdot-1.3.2/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_jinja.py` & `microdot-1.3.2/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_microdot.py` & `microdot-1.3.2/tests/test_microdot.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_microdot_asgi.py` & `microdot-1.3.2/tests/test_microdot_asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,17 @@
             res.set_cookie('foo', 'foo')
             res.set_cookie('bar', 'bar', http_only=True)
 
         scope = {
             'type': 'http',
             'path': '/foo/bar',
             'query_string': b'baz=1',
-            'headers': [('Authorization', 'Bearer 123'),
-                        ('Cookie', 'session=xyz'),
-                        ('Content-Length', 4)],
+            'headers': [(b'Authorization', b'Bearer 123'),
+                        (b'Cookie', b'session=xyz'),
+                        (b'Content-Length', b'4')],
             'client': ['1.2.3.4', 1234],
             'method': 'POST',
             'http_version': '1.1',
         }
 
         event_index = 0
 
@@ -110,17 +110,17 @@
             self.assertEqual(req.path, '/foo/bar')
             self.assertEqual(req.args, {})
             return 'response'
 
         scope = {
             'type': 'http',
             'path': '/foo/bar',
-            'headers': [('Authorization', 'Bearer 123'),
-                        ('Cookie', 'session=xyz'),
-                        ('Content-Length', 4)],
+            'headers': [(b'Authorization', b'Bearer 123'),
+                        (b'Cookie', b'session=xyz'),
+                        (b'Content-Length', b'4')],
             'client': ['1.2.3.4', 1234],
             'method': 'POST',
             'http_version': '1.1',
         }
 
         event_index = 0
```

### Comparing `microdot-1.3.1/tests/test_microdot_asyncio.py` & `microdot-1.3.2/tests/test_microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_microdot_asyncio_websocket.py` & `microdot-1.3.2/tests/test_microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_microdot_websocket.py` & `microdot-1.3.2/tests/test_microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_microdot_wsgi.py` & `microdot-1.3.2/tests/test_microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_multidict.py` & `microdot-1.3.2/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_request.py` & `microdot-1.3.2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_request_asyncio.py` & `microdot-1.3.2/tests/test_request_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_response.py` & `microdot-1.3.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_response_asyncio.py` & `microdot-1.3.2/tests/test_response_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_session.py` & `microdot-1.3.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_url_pattern.py` & `microdot-1.3.2/tests/test_url_pattern.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.1/tests/test_utemplate.py` & `microdot-1.3.2/tests/test_utemplate.py`

 * *Files identical despite different names*

