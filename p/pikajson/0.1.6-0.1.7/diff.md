# Comparing `tmp/pikajson-0.1.6.tar.gz` & `tmp/pikajson-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikajson-0.1.6.tar", last modified: Thu Apr 27 08:12:41 2023, max compression
+gzip compressed data, was "pikajson-0.1.7.tar", last modified: Tue Jun 13 06:38:26 2023, max compression
```

## Comparing `pikajson-0.1.6.tar` & `pikajson-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.572249 pikajson-0.1.6/
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)      329 2023-04-27 08:12:45.570299 pikajson-0.1.6/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      114 2022-12-05 04:08:07.000000 pikajson-0.1.6/README.rst
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.467127 pikajson-0.1.6/pikajson/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)       23 2023-04-27 08:11:54.000000 pikajson-0.1.6/pikajson/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     6162 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/client.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.526123 pikajson-0.1.6/pikajson/exceptions/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2023-04-03 09:52:49.000000 pikajson-0.1.6/pikajson/exceptions/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      203 2023-04-03 09:52:49.000000 pikajson-0.1.6/pikajson/exceptions/need_retry_exception.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     9760 2023-04-27 08:11:54.000000 pikajson-0.1.6/pikajson/server.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.560966 pikajson-0.1.6/pikajson/tests/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        0 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/tests/__init__.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     3492 2022-12-05 04:08:07.000000 pikajson-0.1.6/pikajson/tests/performance_test.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)     7153 2023-04-03 09:07:19.000000 pikajson-0.1.6/pikajson/tests/test_client.py
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)    12488 2023-04-05 08:35:42.000000 pikajson-0.1.6/pikajson/tests/test_server.py
-drwxrwxrwx   0 vagrant   (1000) vagrant   (1000)        0 2023-04-27 08:12:45.510368 pikajson-0.1.6/pikajson.egg-info/
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      329 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/PKG-INFO
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      435 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/SOURCES.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        1 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/dependency_links.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        5 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/requires.txt
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)        9 2023-04-27 08:12:45.000000 pikajson-0.1.6/pikajson.egg-info/top_level.txt
--rwxrwxrwx   0 vagrant   (1000) vagrant   (1000)       38 2023-04-27 08:12:45.573229 pikajson-0.1.6/setup.cfg
--rw-rw-rw-   0 vagrant   (1000) vagrant   (1000)      372 2022-12-05 04:52:49.000000 pikajson-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.641131 pikajson-0.1.7/
+-rw-rw-rw-   0        0        0      222 2023-06-13 06:38:26.641131 pikajson-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-04 13:53:18.000000 pikajson-0.1.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.632129 pikajson-0.1.7/pikajson/
+-rw-rw-rw-   0        0        0       23 2023-06-13 06:14:17.000000 pikajson-0.1.7/pikajson/__init__.py
+-rw-rw-rw-   0        0        0     6162 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.636130 pikajson-0.1.7/pikajson/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/exceptions/need_retry_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.637130 pikajson-0.1.7/pikajson/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:14:17.000000 pikajson-0.1.7/pikajson/helpers/__init__.py
+-rw-rw-rw-   0        0        0      507 2023-06-13 06:14:17.000000 pikajson-0.1.7/pikajson/helpers/helpers.py
+-rw-rw-rw-   0        0        0     9728 2023-06-13 06:14:17.000000 pikajson-0.1.7/pikajson/server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.640131 pikajson-0.1.7/pikajson/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/tests/__init__.py
+-rw-rw-rw-   0        0        0     3492 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/tests/performance_test.py
+-rw-rw-rw-   0        0        0     7153 2023-04-04 13:53:18.000000 pikajson-0.1.7/pikajson/tests/test_client.py
+-rw-rw-rw-   0        0        0    12488 2023-06-13 06:14:17.000000 pikajson-0.1.7/pikajson/tests/test_server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:38:26.635132 pikajson-0.1.7/pikajson.egg-info/
+-rw-rw-rw-   0        0        0      222 2023-06-13 06:38:26.000000 pikajson-0.1.7/pikajson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-06-13 06:38:26.000000 pikajson-0.1.7/pikajson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:38:26.000000 pikajson-0.1.7/pikajson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 06:38:26.000000 pikajson-0.1.7/pikajson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 06:38:26.000000 pikajson-0.1.7/pikajson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:38:26.641131 pikajson-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      372 2023-04-04 13:53:18.000000 pikajson-0.1.7/setup.py
```

### Comparing `pikajson-0.1.6/pikajson/client.py` & `pikajson-0.1.7/pikajson/client.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.6/pikajson/server.py` & `pikajson-0.1.7/pikajson/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,18 +134,16 @@
         logging.info("rabbit consumer terminated on host %s queue %s" % (self._host, self._queue))
 
     def _consuming(self):
         for message in self._channel.consume(queue=self._queue, inactivity_timeout=5):
 
             method, properties, body = message
             
-            if body is None:
-                continue
-            
-            self._callback(ch=self._channel, method=method, properties=properties, body=body)
+            if body is not None:
+                self._callback(ch=self._channel, method=method, properties=properties, body=body)
 
             if self._terminate:
                 break
 
     def _retry(self, body, timeout):
         if self._wait_queue is not None:
             body['retry'] = body.get('retry', 0) + 1
```

### Comparing `pikajson-0.1.6/pikajson/tests/performance_test.py` & `pikajson-0.1.7/pikajson/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.6/pikajson/tests/test_client.py` & `pikajson-0.1.7/pikajson/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pikajson-0.1.6/pikajson/tests/test_server.py` & `pikajson-0.1.7/pikajson/tests/test_server.py`

 * *Files identical despite different names*

