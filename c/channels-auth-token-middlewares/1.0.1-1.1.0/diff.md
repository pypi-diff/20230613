# Comparing `tmp/channels_auth_token_middlewares-1.0.1.tar.gz` & `tmp/channels_auth_token_middlewares-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "channels_auth_token_middlewares-1.0.1.tar", last modified: Mon Apr 17 19:25:11 2023, max compression
+gzip compressed data, was "channels_auth_token_middlewares-1.1.0.tar", last modified: Tue Jun 13 21:26:28 2023, max compression
```

## Comparing `channels_auth_token_middlewares-1.0.1.tar` & `channels_auth_token_middlewares-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1038 2023-04-17 18:28:46.000000 channels_auth_token_middlewares-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.456685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      764 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/
--rw-rw-r--   0 root         (0) root         (0)      788 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5746 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/base.py
--rw-rw-r--   0 root         (0) root         (0)     2291 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/drf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.456685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1290 2023-04-17 19:08:37.000000 channels_auth_token_middlewares-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:26:28.123777 channels_auth_token_middlewares-1.1.0/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2022-02-24 20:17:02.000000 channels_auth_token_middlewares-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-06-13 21:26:28.123777 channels_auth_token_middlewares-1.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1038 2023-05-08 20:55:08.000000 channels_auth_token_middlewares-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:26:28.119777 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-27 19:09:51.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      764 2022-02-24 20:19:56.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:26:28.123777 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/
+-rw-rw-r--   0 root         (0) root         (0)      949 2023-06-13 21:18:52.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5746 2023-06-13 21:18:52.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/base.py
+-rw-rw-r--   0 root         (0) root         (0)     4085 2023-06-13 21:18:52.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/drf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:26:28.123777 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-06-13 21:26:28.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-06-13 21:26:28.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 21:26:28.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-13 21:26:28.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-13 21:26:28.000000 channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 21:26:28.123777 channels_auth_token_middlewares-1.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1290 2023-06-13 21:18:52.000000 channels_auth_token_middlewares-1.1.0/setup.py
```

### Comparing `channels_auth_token_middlewares-1.0.1/LICENSE` & `channels_auth_token_middlewares-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.1/PKG-INFO` & `channels_auth_token_middlewares-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channels_auth_token_middlewares
-Version: 1.0.1
+Version: 1.1.0
 Summary: Django Channels auth token middlewares
 Home-page: https://github.com/YegorDB/django-channels-auth-token-middlewares
 Author: Yegor Bitensky
 Keywords: django channels middleware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `channels_auth_token_middlewares-1.0.1/README.md` & `channels_auth_token_middlewares-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/apps.py` & `channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/apps.py`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/__init__.py` & `channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,13 @@
 # limitations under the License.
 
 
 from .base import (
     BaseAuthTokenMiddleware, CookieAuthTokenMiddleware,
     HeaderAuthTokenMiddleware, QueryStringAuthTokenMiddleware,
 )
-from .drf import DRFAuthTokenMiddleware, SimpleJWTAuthTokenMiddleware
+from .drf import (
+    DRFAuthTokenMiddleware, QueryStringDRFAuthTokenMiddleware,
+    DRFAuthTokenMiddlewareStack,
+    SimpleJWTAuthTokenMiddleware, QueryStringSimpleJWTAuthTokenMiddleware,
+    SimpleJWTAuthTokenMiddlewareStack,
+)
```

### Comparing `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/base.py` & `channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares/middleware/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def __init__(self, *args, cookie_name=None, **kwargs):
         self.cookie_name = str(cookie_name or self.cookie_name)
 
         super().__init__(*args, **kwargs)
 
     def get_token_key_string(self, scope):
         header_name = "Cookie"
-        cookie_raw_data = self.get_scope_header_value(scope, header_name) or ''
+        cookie_raw_data = self.get_scope_header_value(scope, header_name) or ""
         cookie = BaseCookie()
         cookie.load(cookie_raw_data)
         cookie_item = cookie.get(self.cookie_name)
         if not cookie_item:
             return None
         return cookie_item.value
```

### Comparing `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/PKG-INFO` & `channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: channels-auth-token-middlewares
-Version: 1.0.1
+Version: 1.1.0
 Summary: Django Channels auth token middlewares
 Home-page: https://github.com/YegorDB/django-channels-auth-token-middlewares
 Author: Yegor Bitensky
 Keywords: django channels middleware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/SOURCES.txt` & `channels_auth_token_middlewares-1.1.0/channels_auth_token_middlewares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.1/setup.py` & `channels_auth_token_middlewares-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="channels_auth_token_middlewares",
-    version="1.0.1",
+    version="1.1.0",
     description="Django Channels auth token middlewares",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YegorDB/django-channels-auth-token-middlewares",
     author="Yegor Bitensky",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

