# Comparing `tmp/ensta-1.5.tar.gz` & `tmp/ensta-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.5.tar", last modified: Mon Jun 12 16:04:13 2023, max compression
+gzip compressed data, was "ensta-1.6.tar", last modified: Tue Jun 13 08:46:10 2023, max compression
```

## Comparing `ensta-1.5.tar` & `ensta-1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.225485 ensta-1.5/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     6100 2023-06-12 16:04:13.225485 ensta-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5365 2023-06-12 15:53:10.000000 ensta-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.162726 ensta-1.5/ensta/
--rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.5/ensta/Guest.py
--rw-rw-rw-   0        0        0    12446 2023-06-12 15:23:46.000000 ensta-1.5/ensta/Host.py
--rw-rw-rw-   0        0        0    14411 2023-06-12 15:13:54.000000 ensta-1.5/ensta/Stream.py
--rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.5/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.209656 ensta-1.5/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.5/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.5/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.5/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.5/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.5/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.225485 ensta-1.5/ensta/lib/
--rw-rw-rw-   0        0        0     1424 2023-06-09 09:01:13.000000 ensta-1.5/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.5/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.5/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:04:13.192954 ensta-1.5/ensta.egg-info/
--rw-rw-rw-   0        0        0     6100 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 16:04:13.000000 ensta-1.5/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 16:04:13.240008 ensta-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-06-12 16:04:02.000000 ensta-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.821377 ensta-1.6/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     6728 2023-06-13 08:46:10.821377 ensta-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5963 2023-06-13 08:34:59.000000 ensta-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.732075 ensta-1.6/ensta/
+-rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.6/ensta/Guest.py
+-rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.6/ensta/Host.py
+-rw-rw-rw-   0        0        0    14411 2023-06-13 08:32:24.000000 ensta-1.6/ensta/Stream.py
+-rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.6/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.798033 ensta-1.6/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.6/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.6/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.6/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.6/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.6/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.818002 ensta-1.6/ensta/lib/
+-rw-rw-rw-   0        0        0     1477 2023-06-13 08:32:05.000000 ensta-1.6/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.6/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.6/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.764659 ensta-1.6/ensta.egg-info/
+-rw-rw-rw-   0        0        0     6728 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 08:46:10.826738 ensta-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-13 08:45:55.000000 ensta-1.6/setup.py
```

### Comparing `ensta-1.5/LICENSE.txt` & `ensta-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.5/PKG-INFO` & `ensta-1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.5
-Summary: Simple & Up-to-date Instagram API
+Version: 1.6
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Ensta - Instagram Automation 🤖
+# 🤖 Ensta - Simple Instagram API
 This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
 
 It supports three types of classes - *Guest*, *Host*, *Stream*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
@@ -115,14 +115,23 @@
         print("Something went wrong.")
         break
 
     print(user.username)
     print(user.full_name)
 ```
 
+## Considerations
+Here are some key points to consider when using this library in production:
+- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
+- Functions should return *None* on failure. So, add clauses for the same.
+
+- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
+  - The argument **Identifier** means you can pass either Username or UserID.
+  - The argument **Username** means you must pass the Username only, and not the UserID.
+
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
```

### Comparing `ensta-1.5/README.md` & `ensta-1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ensta - Instagram Automation 🤖
+# 🤖 Ensta - Simple Instagram API
 This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
 
 It supports three types of classes - *Guest*, *Host*, *Stream*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
@@ -96,14 +96,23 @@
         print("Something went wrong.")
         break
 
     print(user.username)
     print(user.full_name)
 ```
 
+## Considerations
+Here are some key points to consider when using this library in production:
+- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
+- Functions should return *None* on failure. So, add clauses for the same.
+
+- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
+  - The argument **Identifier** means you can pass either Username or UserID.
+  - The argument **Username** means you must pass the Username only, and not the UserID.
+
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
```

### Comparing `ensta-1.5/ensta/Guest.py` & `ensta-1.6/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-1.5/ensta/Host.py` & `ensta-1.6/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-1.5/ensta/Stream.py` & `ensta-1.6/ensta/Stream.py`

 * *Files identical despite different names*

### Comparing `ensta-1.5/ensta/containers/Profile.py` & `ensta-1.6/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-1.5/ensta/lib/Commons.py` & `ensta-1.6/ensta/lib/Commons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import string
 import requests
 import requests.cookies
 import random
 from .Exceptions import NetworkError
 
 
-def update_app_id(self):
+def update_app_id(self) -> None:
     app_id_occurrence_string = "\"APP_ID\":\""
     app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
     app_id_raw_text = self.homepage_source[
                       app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
     self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
 
 
-def refresh_csrf_token(self):
+def refresh_csrf_token(self) -> None:
     self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
     cookie_object = requests.cookies.create_cookie(domain="instagram.com", name="csrftoken", value=self.csrf_token)
     self.request_session.cookies.set_cookie(cookie_object)
 
 
-def update_session(self):
+def update_session(self) -> None:
     self.request_session = requests.Session()
 
 
-def update_homepage_source(self):
+def update_homepage_source(self) -> None:
     temp_homepage_source = requests.get("https://www.instagram.com").text.strip()
 
     if temp_homepage_source != "":
         self.homepage_source = temp_homepage_source
     else:
         raise NetworkError("Couldn't load instagram homepage.")
 
 
-def format_username(username: str):
+def format_username(username: str) -> str:
     return username.replace(" ", "").lower()
 
 
-def format_uid(uid: str):
+def format_uid(uid: str) -> str:
     return uid.replace(" ", "")
 
 
-def format_identifier(identifier: str | int):
+def format_identifier(identifier: str | int) -> str:
     return str(identifier).lower().replace(" ", "")
```

### Comparing `ensta-1.5/ensta/lib/Exceptions.py` & `ensta-1.6/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-1.5/ensta.egg-info/PKG-INFO` & `ensta-1.6/ensta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.5
-Summary: Simple & Up-to-date Instagram API
+Version: 1.6
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Ensta - Instagram Automation 🤖
+# 🤖 Ensta - Simple Instagram API
 This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
 
 It supports three types of classes - *Guest*, *Host*, *Stream*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
@@ -115,14 +115,23 @@
         print("Something went wrong.")
         break
 
     print(user.username)
     print(user.full_name)
 ```
 
+## Considerations
+Here are some key points to consider when using this library in production:
+- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
+- Functions should return *None* on failure. So, add clauses for the same.
+
+- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
+  - The argument **Identifier** means you can pass either Username or UserID.
+  - The argument **Username** means you must pass the Username only, and not the UserID.
+
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
```

### Comparing `ensta-1.5/setup.py` & `ensta-1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="1.5",
+    version="1.6",
     license="MIT",
-    description="Simple & Up-to-date Instagram API",
+    description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
     download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

