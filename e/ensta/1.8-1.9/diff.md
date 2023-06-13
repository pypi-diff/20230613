# Comparing `tmp/ensta-1.8.tar.gz` & `tmp/ensta-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.8.tar", last modified: Tue Jun 13 14:12:31 2023, max compression
+gzip compressed data, was "ensta-1.9.tar", last modified: Tue Jun 13 14:23:46 2023, max compression
```

## Comparing `ensta-1.8.tar` & `ensta-1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     6730 2023-06-13 14:12:31.667818 ensta-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5965 2023-06-13 10:14:35.000000 ensta-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.636442 ensta-1.8/ensta/
--rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.8/ensta/Guest.py
--rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.8/ensta/Host.py
--rw-rw-rw-   0        0        0    14438 2023-06-13 09:23:10.000000 ensta-1.8/ensta/Stream.py
--rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.8/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.8/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.8/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.8/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.8/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.8/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/ensta/lib/
--rw-rw-rw-   0        0        0     2457 2023-06-13 14:11:09.000000 ensta-1.8/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.8/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.8/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.652065 ensta-1.8/ensta.egg-info/
--rw-rw-rw-   0        0        0     6730 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 14:12:31.683318 ensta-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-13 14:12:13.000000 ensta-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:23:46.563021 ensta-1.9/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     6730 2023-06-13 14:23:46.563021 ensta-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5965 2023-06-13 10:14:35.000000 ensta-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 14:23:46.528735 ensta-1.9/ensta/
+-rw-rw-rw-   0        0        0    11194 2023-06-13 14:18:20.000000 ensta-1.9/ensta/Guest.py
+-rw-rw-rw-   0        0        0    12566 2023-06-13 14:18:02.000000 ensta-1.9/ensta/Host.py
+-rw-rw-rw-   0        0        0    14438 2023-06-13 09:23:10.000000 ensta-1.9/ensta/Stream.py
+-rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.9/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:23:46.555026 ensta-1.9/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.9/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.9/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.9/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.9/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.9/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:23:46.563021 ensta-1.9/ensta/lib/
+-rw-rw-rw-   0        0        0     2457 2023-06-13 14:11:09.000000 ensta-1.9/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.9/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.9/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:23:46.547017 ensta-1.9/ensta.egg-info/
+-rw-rw-rw-   0        0        0     6730 2023-06-13 14:23:46.000000 ensta-1.9/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-06-13 14:23:46.000000 ensta-1.9/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:23:46.000000 ensta-1.9/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 14:23:46.000000 ensta-1.9/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 14:23:46.000000 ensta-1.9/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 14:23:46.563021 ensta-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-13 14:20:53.000000 ensta-1.9/setup.py
```

### Comparing `ensta-1.8/LICENSE.txt` & `ensta-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.8/PKG-INFO` & `ensta-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.8
+Version: 1.9
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-1.8/README.md` & `ensta-1.9/README.md`

 * *Files identical despite different names*

### Comparing `ensta-1.8/ensta/Guest.py` & `ensta-1.9/ensta/Guest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 class Guest:
     request_session: requests.Session = None
     homepage_source: str = None
     insta_app_id: str = None
     csrf_token: str = None
 
-    def __init__(self, homepage_source: str = None, insta_app_id: str = None) -> None:
+    def __init__(self, homepage_source: str = None, app_id: str | int = None) -> None:
         update_session(self)
 
         if homepage_source is not None:
             self.homepage_source = homepage_source
         else:
             update_homepage_source(self)
 
-        if insta_app_id is not None:
-            self.insta_app_id = insta_app_id
+        if app_id is not None:
+            self.insta_app_id = str(app_id)
         else:
             update_app_id(self)
 
     def username_availability(self, username: str) -> bool | None:
         username = format_username(username)
         refresh_csrf_token(self)
         body_json = {
```

### Comparing `ensta-1.8/ensta/Host.py` & `ensta-1.9/ensta/Host.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,27 @@
     homepage_source: str = None
     insta_app_id: str = None
     preferred_color_scheme: str = "dark"
     x_ig_www_claim: str = None
     csrf_token: str = None
     guest: Guest = None
 
-    def __init__(self, session_id: str) -> None:
+    def __init__(self, session_id: str, app_id: str | int = None) -> None:
         self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
         update_session(self)
         update_homepage_source(self)
-        update_app_id(self)
+
+        if app_id is not None:
+            self.insta_app_id = str(app_id)
+        else:
+            update_app_id(self)
+
         self.guest = Guest(
             homepage_source=self.homepage_source,
-            insta_app_id=self.insta_app_id
+            app_id=self.insta_app_id
         )
 
         self.request_session.cookies.set("sessionid", session_id)
 
         if not self.authenticated():
             raise AuthenticationError("Either User ID or Session ID is not valid.")
```

### Comparing `ensta-1.8/ensta/Stream.py` & `ensta-1.9/ensta/Stream.py`

 * *Files identical despite different names*

### Comparing `ensta-1.8/ensta/containers/Profile.py` & `ensta-1.9/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-1.8/ensta/lib/Commons.py` & `ensta-1.9/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-1.8/ensta/lib/Exceptions.py` & `ensta-1.9/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-1.8/ensta.egg-info/PKG-INFO` & `ensta-1.9/ensta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.8
+Version: 1.9
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
```

### Comparing `ensta-1.8/setup.py` & `ensta-1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="1.8",
+    version="1.9",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

