# Comparing `tmp/jhsingle-native-proxy-0.8.0.tar.gz` & `tmp/jhsingle-native-proxy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhsingle-native-proxy-0.8.0.tar", last modified: Mon Nov  8 12:06:55 2021, max compression
+gzip compressed data, was "jhsingle-native-proxy-0.8.1.tar", last modified: Tue Jun 13 08:24:59 2023, max compression
```

## Comparing `jhsingle-native-proxy-0.8.0.tar` & `jhsingle-native-proxy-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-11-08 12:06:55.871347 jhsingle-native-proxy-0.8.0/
--rw-r--r--   0 dan        (501) staff       (20)    11358 2020-02-27 15:35:06.000000 jhsingle-native-proxy-0.8.0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     1705 2020-02-27 15:41:33.000000 jhsingle-native-proxy-0.8.0/LICENSE-jupyter-server-proxy
--rw-r--r--   0 dan        (501) staff       (20)      128 2020-07-18 10:22:20.000000 jhsingle-native-proxy-0.8.0/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)    13212 2021-11-08 12:06:55.870683 jhsingle-native-proxy-0.8.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)    10703 2021-11-08 12:06:10.000000 jhsingle-native-proxy-0.8.0/README.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-11-08 12:06:55.862938 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/
--rw-r--r--   0 dan        (501) staff       (20)        0 2020-02-11 10:12:14.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3035 2020-08-04 09:07:59.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/activity.py
--rw-r--r--   0 dan        (501) staff       (20)     1858 2020-07-22 09:45:53.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/conda_runner.py
--rw-r--r--   0 dan        (501) staff       (20)     1832 2020-09-03 12:15:54.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/gitwrapper.py
--rw-r--r--   0 dan        (501) staff       (20)     9411 2021-11-08 12:01:13.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/main.py
--rw-r--r--   0 dan        (501) staff       (20)    35811 2021-04-20 12:45:15.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/proxyhandlers.py
--rw-r--r--   0 dan        (501) staff       (20)     9471 2020-11-12 10:41:01.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/pull.py
--rw-r--r--   0 dan        (501) staff       (20)      492 2020-02-27 14:17:17.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/util.py
--rw-r--r--   0 dan        (501) staff       (20)     4058 2021-04-20 12:44:43.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/websocket.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2021-11-08 12:06:55.869817 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    13212 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      706 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       74 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2020-06-01 14:54:28.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       69 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       22 2021-11-08 12:06:55.000000 jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2021-01-06 09:08:58.000000 jhsingle-native-proxy-0.8.0/requirements.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2021-11-08 12:06:55.871498 jhsingle-native-proxy-0.8.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1097 2021-11-08 12:05:17.000000 jhsingle-native-proxy-0.8.0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-13 08:24:59.019775 jhsingle-native-proxy-0.8.1/
+-rw-r--r--   0 dan        (501) staff       (20)    11358 2020-02-27 15:35:06.000000 jhsingle-native-proxy-0.8.1/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     1705 2020-02-27 15:41:33.000000 jhsingle-native-proxy-0.8.1/LICENSE-jupyter-server-proxy
+-rw-r--r--   0 dan        (501) staff       (20)      128 2020-07-18 10:22:20.000000 jhsingle-native-proxy-0.8.1/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)    13530 2023-06-13 08:24:59.019120 jhsingle-native-proxy-0.8.1/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)    10981 2023-06-13 08:24:16.000000 jhsingle-native-proxy-0.8.1/README.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-13 08:24:59.013634 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2020-02-11 10:12:14.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3035 2020-08-04 09:07:59.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/activity.py
+-rw-r--r--   0 dan        (501) staff       (20)     1858 2020-07-22 09:45:53.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/conda_runner.py
+-rw-r--r--   0 dan        (501) staff       (20)     1832 2020-09-03 12:15:54.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/gitwrapper.py
+-rw-r--r--   0 dan        (501) staff       (20)     9411 2022-04-08 09:42:12.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/main.py
+-rw-r--r--   0 dan        (501) staff       (20)    35811 2022-04-08 12:44:18.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/proxyhandlers.py
+-rw-r--r--   0 dan        (501) staff       (20)     9471 2020-11-12 10:41:01.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/pull.py
+-rw-r--r--   0 dan        (501) staff       (20)      492 2020-02-27 14:17:17.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/util.py
+-rw-r--r--   0 dan        (501) staff       (20)     4058 2021-04-20 12:44:43.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/websocket.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-13 08:24:59.018268 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)    13530 2023-06-13 08:24:57.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      706 2023-06-13 08:24:58.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-13 08:24:57.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       74 2023-06-13 08:24:57.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2020-06-01 14:54:28.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-13 08:24:57.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       22 2023-06-13 08:24:57.000000 jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/top_level.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-13 08:21:44.000000 jhsingle-native-proxy-0.8.1/requirements.txt
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-13 08:24:59.019892 jhsingle-native-proxy-0.8.1/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1097 2023-06-13 08:23:08.000000 jhsingle-native-proxy-0.8.1/setup.py
```

### Comparing `jhsingle-native-proxy-0.8.0/LICENSE` & `jhsingle-native-proxy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/LICENSE-jupyter-server-proxy` & `jhsingle-native-proxy-0.8.1/LICENSE-jupyter-server-proxy`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/PKG-INFO` & `jhsingle-native-proxy-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhsingle-native-proxy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Wrap an arbitrary webapp so it can be used in place of jupyter-singleuser in a JupyterHub setting
 Home-page: https://github.com/ideonate/jhsingle-native-proxy
 Author: Dan Lester
 Author-email: dan@ideonate.com
 License: UNKNOWN
 Description: # jhsingle-native-proxy
         
@@ -133,17 +133,22 @@
         
         --query-user-info - add a GET query param named CDSDASHBOARDS_JH_USER when calling underlying process containing JupyterHub user info as JSON-encoded string
         
         --ready-timeout - integer timeout for period of checking the process is running at startup (default 10). Increase if your process is not able to return anything at --ready-check-path until a longer time after it first starts up. Be aware that the process must (once ready) return its HTTP response within 1 second. Note this argument is different from --request-timeout which applies to individual HTTP proxy calls during normal operation (not just at startup).
         
         --websocket-max-message-size - message size in bytes allowed by websocket connections made to the underlying process (default is to rely on the tornado library defaults).
         
+         --progressive - flush buffer from underlying service whenever chunks appear (this is useful to see results from Voila sooner)
         
         ## Changelog
         
+        ### v0.8.1 released 13 Jun 2023
+        
+        - Pin simpervisor version to avoid conflict with version 1.0. Thanks to [dangercrow](https://github.com/dangercrow).
+        
         ### v0.8.0 released 8 Nov 2021
         
         - Change to work with JupyterHub 2 (detects port from JUPYTERHUB_SERVICE_URL env var if no --port set)
         
         ### v0.7.6 released 20 Apr 2021
         
         - New command-line options --ready-timeout and --websocket-max-message-size
```

### Comparing `jhsingle-native-proxy-0.8.0/README.md` & `jhsingle-native-proxy-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,22 @@
 
 --query-user-info - add a GET query param named CDSDASHBOARDS_JH_USER when calling underlying process containing JupyterHub user info as JSON-encoded string
 
 --ready-timeout - integer timeout for period of checking the process is running at startup (default 10). Increase if your process is not able to return anything at --ready-check-path until a longer time after it first starts up. Be aware that the process must (once ready) return its HTTP response within 1 second. Note this argument is different from --request-timeout which applies to individual HTTP proxy calls during normal operation (not just at startup).
 
 --websocket-max-message-size - message size in bytes allowed by websocket connections made to the underlying process (default is to rely on the tornado library defaults).
 
+ --progressive - flush buffer from underlying service whenever chunks appear (this is useful to see results from Voila sooner)
 
 ## Changelog
 
+### v0.8.1 released 13 Jun 2023
+
+- Pin simpervisor version to avoid conflict with version 1.0. Thanks to [dangercrow](https://github.com/dangercrow).
+
 ### v0.8.0 released 8 Nov 2021
 
 - Change to work with JupyterHub 2 (detects port from JUPYTERHUB_SERVICE_URL env var if no --port set)
 
 ### v0.7.6 released 20 Apr 2021
 
 - New command-line options --ready-timeout and --websocket-max-message-size
```

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/activity.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/activity.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/conda_runner.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/conda_runner.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/gitwrapper.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/gitwrapper.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/main.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/main.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/proxyhandlers.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/proxyhandlers.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/pull.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/pull.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy/websocket.py` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy/websocket.py`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/PKG-INFO` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhsingle-native-proxy
-Version: 0.8.0
+Version: 0.8.1
 Summary: Wrap an arbitrary webapp so it can be used in place of jupyter-singleuser in a JupyterHub setting
 Home-page: https://github.com/ideonate/jhsingle-native-proxy
 Author: Dan Lester
 Author-email: dan@ideonate.com
 License: UNKNOWN
 Description: # jhsingle-native-proxy
         
@@ -133,17 +133,22 @@
         
         --query-user-info - add a GET query param named CDSDASHBOARDS_JH_USER when calling underlying process containing JupyterHub user info as JSON-encoded string
         
         --ready-timeout - integer timeout for period of checking the process is running at startup (default 10). Increase if your process is not able to return anything at --ready-check-path until a longer time after it first starts up. Be aware that the process must (once ready) return its HTTP response within 1 second. Note this argument is different from --request-timeout which applies to individual HTTP proxy calls during normal operation (not just at startup).
         
         --websocket-max-message-size - message size in bytes allowed by websocket connections made to the underlying process (default is to rely on the tornado library defaults).
         
+         --progressive - flush buffer from underlying service whenever chunks appear (this is useful to see results from Voila sooner)
         
         ## Changelog
         
+        ### v0.8.1 released 13 Jun 2023
+        
+        - Pin simpervisor version to avoid conflict with version 1.0. Thanks to [dangercrow](https://github.com/dangercrow).
+        
         ### v0.8.0 released 8 Nov 2021
         
         - Change to work with JupyterHub 2 (detects port from JUPYTERHUB_SERVICE_URL env var if no --port set)
         
         ### v0.7.6 released 20 Apr 2021
         
         - New command-line options --ready-timeout and --websocket-max-message-size
```

### Comparing `jhsingle-native-proxy-0.8.0/jhsingle_native_proxy.egg-info/SOURCES.txt` & `jhsingle-native-proxy-0.8.1/jhsingle_native_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jhsingle-native-proxy-0.8.0/setup.py` & `jhsingle-native-proxy-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open('requirements.txt', 'r') as f:
     content = f.read()
 li_req = content.split('\n')
 install_requires = [e.strip() for e in li_req if len(e)]
 
 setuptools.setup(
     name="jhsingle-native-proxy",
-    version="0.8.0",
+    version="0.8.1",
     author="Dan Lester",
     author_email="dan@ideonate.com",
     description="Wrap an arbitrary webapp so it can be used in place of jupyter-singleuser in a JupyterHub setting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ideonate/jhsingle-native-proxy",
     packages=setuptools.find_packages(),
```

