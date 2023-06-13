# Comparing `tmp/ensta-2.0.tar.gz` & `tmp/ensta-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.0.tar", last modified: Tue Jun 13 14:44:04 2023, max compression
+gzip compressed data, was "ensta-2.1.tar", last modified: Tue Jun 13 17:45:25 2023, max compression
```

## Comparing `ensta-2.0.tar` & `ensta-2.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:04.612121 ensta-2.0/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6730 2023-06-13 14:44:04.612121 ensta-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5965 2023-06-13 10:14:35.000000 ensta-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:04.581005 ensta-2.0/ensta/
--rw-rw-rw-   0        0        0    11194 2023-06-13 14:18:20.000000 ensta-2.0/ensta/Guest.py
--rw-rw-rw-   0        0        0    12442 2023-06-13 14:42:32.000000 ensta-2.0/ensta/Host.py
--rw-rw-rw-   0        0        0    14432 2023-06-13 14:43:07.000000 ensta-2.0/ensta/Stream.py
--rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-2.0/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:04.596497 ensta-2.0/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-2.0/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-2.0/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-2.0/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-2.0/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-2.0/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:04.596497 ensta-2.0/ensta/lib/
--rw-rw-rw-   0        0        0     2483 2023-06-13 14:40:57.000000 ensta-2.0/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-2.0/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-2.0/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:04.596497 ensta-2.0/ensta.egg-info/
--rw-rw-rw-   0        0        0     6730 2023-06-13 14:44:04.000000 ensta-2.0/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-06-13 14:44:04.000000 ensta-2.0/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:44:04.000000 ensta-2.0/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 14:44:04.000000 ensta-2.0/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:44:04.000000 ensta-2.0/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 14:44:04.612121 ensta-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-13 14:43:38.000000 ensta-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.192557 ensta-2.1/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5889 2023-06-13 17:45:25.192557 ensta-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5124 2023-06-13 17:23:39.000000 ensta-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.116706 ensta-2.1/ensta/
+-rw-rw-rw-   0        0        0    11194 2023-06-13 14:18:20.000000 ensta-2.1/ensta/Guest.py
+-rw-rw-rw-   0        0        0    22543 2023-06-13 16:38:17.000000 ensta-2.1/ensta/Host.py
+-rw-rw-rw-   0        0        0       60 2023-06-13 16:38:34.000000 ensta-2.1/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.176938 ensta-2.1/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-2.1/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-2.1/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-2.1/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-2.1/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-2.1/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.192557 ensta-2.1/ensta/lib/
+-rw-rw-rw-   0        0        0     2483 2023-06-13 14:40:57.000000 ensta-2.1/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-2.1/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-2.1/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.145657 ensta-2.1/ensta.egg-info/
+-rw-rw-rw-   0        0        0     5889 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 17:45:25.192557 ensta-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-13 17:45:04.000000 ensta-2.1/setup.py
```

### Comparing `ensta-2.0/LICENSE.txt` & `ensta-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-2.0/PKG-INFO` & `ensta-2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 2.0
+Version: 2.1
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
@@ -14,41 +14,44 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 🤖 Ensta - Simple Instagram API
-This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
 
-It supports three types of classes - *Guest*, *Host*, *Stream*.
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+
+It supports three two of classes - *Guest* & *Host*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
-It's recommended to install this package using [Python's PIP](https://pypi.org/project/pip/), as the GitHub versions may be unstable and may require testing before being used in production.
-
-To install this library, run this command in a terminal window:
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
 ```shell
 pip install ensta
 ```
 
-To upgrade the installed version of this library, run:
+To upgrade to the latest version, run:
 ```shell
 pip install ensta --upgrade
 ```
 
-## Guest Mode
+## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available
-- Fetch someone's profile information
+- Check if username is available for registration
+- Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -56,26 +59,25 @@
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
-## Host Mode
-This mode requires the user to login through their [SessionID](https://github.com/diezo/ensta#session-id). SessionID shall be passed as an argument while initializing this class. It can be used to fetch data that's available only when the user is logged in. Additionally, the user can perform several actions on their profile.
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
 
-Methods supported till now are listed below:
+These are the methods supported till now:
 - Check authentication status of the user
-- Follow someone's account
-- Unfollow someone's account
-- Get someone's follower list of specified size
-- Get someone's following list of specified size
-- Toggle account privacy - 'Private' or 'Public'
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile:
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
 from ensta import Host
 
 sessionid = "123456:abcdefg"  # Place your SessionId here
 
 host = Host(sessionid)
@@ -87,51 +89,28 @@
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Stream Mode
-This mode pulls data at realtime, so the program can process it simultaneously. It requires login through [SessionID](https://github.com/diezo/ensta#session-id).
-
-In a situation where you might need to fetch someone's entire follower list, this mode comes handy.
-
-These are the methods supported till now:
-- Fetch someone's follower list
-- Fetch someone's following list
-
-Here's an example where an instance of *Stream* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) first 100 followers:
-
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
 ```python
-from ensta import Stream
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-stream = Stream(sessionid)
-followers = stream.followers("cristiano")
+from ensta import Guest
 
-for user in followers:
-    if user is None:
-        print("Something went wrong.")
-        break
+guest = Guest()
+available = guest.username_availability("cristiano")
 
-    print(user.username)
-    print(user.full_name)
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
 ```
 
-## Considerations
-Here are some key points to consider when using this library in production:
-- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
-- Functions should return *None* on failure. So, add clauses for the same.
-
-- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
-  - The argument **Identifier** means you can pass either Username or UserID.
-  - The argument **Username** means you must pass the Username only, and not the UserID.
-
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
```

### Comparing `ensta-2.0/README.md` & `ensta-2.1/ensta.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,57 @@
+Metadata-Version: 2.1
+Name: ensta
+Version: 2.1
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
+Author: Deepak Soni
+Author-email: lonelycube@proton.me
+License: MIT
+Keywords: instagram,web,private,api,scraper,easy,download,upload
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # 🤖 Ensta - Simple Instagram API
-This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
 
-It supports three types of classes - *Guest*, *Host*, *Stream*.
+It supports three two of classes - *Guest* & *Host*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
-It's recommended to install this package using [Python's PIP](https://pypi.org/project/pip/), as the GitHub versions may be unstable and may require testing before being used in production.
-
-To install this library, run this command in a terminal window:
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
 ```shell
 pip install ensta
 ```
 
-To upgrade the installed version of this library, run:
+To upgrade to the latest version, run:
 ```shell
 pip install ensta --upgrade
 ```
 
-## Guest Mode
+## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available
-- Fetch someone's profile information
+- Check if username is available for registration
+- Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -37,26 +59,25 @@
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
-## Host Mode
-This mode requires the user to login through their [SessionID](https://github.com/diezo/ensta#session-id). SessionID shall be passed as an argument while initializing this class. It can be used to fetch data that's available only when the user is logged in. Additionally, the user can perform several actions on their profile.
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
 
-Methods supported till now are listed below:
+These are the methods supported till now:
 - Check authentication status of the user
-- Follow someone's account
-- Unfollow someone's account
-- Get someone's follower list of specified size
-- Get someone's following list of specified size
-- Toggle account privacy - 'Private' or 'Public'
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile:
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
 from ensta import Host
 
 sessionid = "123456:abcdefg"  # Place your SessionId here
 
 host = Host(sessionid)
@@ -68,51 +89,28 @@
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Stream Mode
-This mode pulls data at realtime, so the program can process it simultaneously. It requires login through [SessionID](https://github.com/diezo/ensta#session-id).
-
-In a situation where you might need to fetch someone's entire follower list, this mode comes handy.
-
-These are the methods supported till now:
-- Fetch someone's follower list
-- Fetch someone's following list
-
-Here's an example where an instance of *Stream* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) first 100 followers:
-
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
 ```python
-from ensta import Stream
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-stream = Stream(sessionid)
-followers = stream.followers("cristiano")
+from ensta import Guest
 
-for user in followers:
-    if user is None:
-        print("Something went wrong.")
-        break
+guest = Guest()
+available = guest.username_availability("cristiano")
 
-    print(user.username)
-    print(user.full_name)
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
 ```
 
-## Considerations
-Here are some key points to consider when using this library in production:
-- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
-- Functions should return *None* on failure. So, add clauses for the same.
-
-- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
-  - The argument **Identifier** means you can pass either Username or UserID.
-  - The argument **Username** means you must pass the Username only, and not the UserID.
-
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
@@ -124,8 +122,8 @@
 
 ## Donate ❤️
 If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
```

### Comparing `ensta-2.0/ensta/Guest.py` & `ensta-2.1/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-2.0/ensta/Host.py` & `ensta-2.1/ensta/Host.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import requests
 from json import JSONDecodeError
 import random
 import string
+from collections.abc import Generator
 from .Guest import Guest
 from .lib.Commons import (
     refresh_csrf_token,
     update_app_id,
     update_homepage_source,
     update_session,
     format_identifier
 )
 from .lib import (
     AuthenticationError,
     NetworkError,
     IdentifierError,
     CodeError
 )
-from .containers import (FollowedStatus, UnfollowedStatus)
+from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
 from .containers.Profile import Profile
 
 USERNAME = 0
 UID = 1
 
 
 class Host:
@@ -188,14 +189,242 @@
                         return UnfollowedStatus(
                             unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
                             is_my_follower=response_json["friendship_status"]["followed_by"]
                         )
         except JSONDecodeError:
             return None
 
+    def followers(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
+            return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        current_max_id = ""
+        generated_count = 0
+
+        while True:
+            current_max_id_text = ""
+
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
+
+            try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
+                response_json = http_response.json()
+
+                if "status" not in response_json or "users" not in response_json:
+                    yield None
+                    return None
+
+                if response_json["status"] != "ok":
+                    yield None
+                    return None
+
+                for each_item in response_json["users"]:
+                    if generated_count < count or count == 0:
+
+                        prop_has_anonymous_profile_picture = None
+                        prop_user_id = None
+                        prop_username = None
+                        prop_full_name = None
+                        prop_is_private = None
+                        prop_is_verified = None
+                        prop_profile_picture_url = None
+                        prop_is_possible_scammer = None
+
+                        if "has_anonymous_profile_picture" in each_item:
+                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
+
+                        if "pk" in each_item:
+                            prop_user_id = each_item["pk"]
+
+                        if "username" in each_item:
+                            prop_username = each_item["username"]
+
+                        if "full_name" in each_item:
+                            prop_full_name = each_item["full_name"]
+
+                        if "is_private" in each_item:
+                            prop_is_private = each_item["is_private"]
+
+                        if "is_verified" in each_item:
+                            prop_is_verified = each_item["is_verified"]
+
+                        if "profile_pic_url" in each_item:
+                            prop_profile_picture_url = each_item["profile_pic_url"]
+
+                        if "is_possible_scammer" in each_item:
+                            prop_is_possible_scammer = each_item["is_possible_scammer"]
+
+                        yield FollowPerson(
+                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
+                            user_id=prop_user_id,
+                            username=prop_username,
+                            full_name=prop_full_name,
+                            is_private=prop_is_private,
+                            is_verified=prop_is_verified,
+                            profile_picture_url=prop_profile_picture_url,
+                            is_possible_scammer=prop_is_possible_scammer
+                        )
+
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
+                else:
+                    return None
+            except JSONDecodeError:
+                yield None
+                return None
+
+    def followings(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success:
+            yield None
+            return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
+            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "\"Windows\"",
+            "sec-ch-ua-platform-version": "\"15.0.0\"",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "viewport-width": "1475",
+            "x-asbd-id": "198387",
+            "x-csrftoken": self.csrf_token,
+            "x-ig-app-id": self.insta_app_id,
+            "x-ig-www-claim": self.x_ig_www_claim,
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        current_max_id = ""
+        generated_count = 0
+
+        while True:
+            current_max_id_text = ""
+
+            if current_max_id != "":
+                current_max_id_text = f"&max_id={current_max_id}"
+
+            try:
+                count_text = 35
+
+                if count < 35:
+                    count_text = count
+
+                http_response = self.request_session.get(
+                    f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}",
+                    headers=request_headers)
+                response_json = http_response.json()
+
+                if "status" not in response_json or "users" not in response_json:
+                    yield None
+                    return None
+
+                if response_json["status"] != "ok":
+                    yield None
+                    return None
+
+                for each_item in response_json["users"]:
+                    if generated_count < count or count == 0:
+
+                        prop_has_anonymous_profile_picture = None
+                        prop_user_id = None
+                        prop_username = None
+                        prop_full_name = None
+                        prop_is_private = None
+                        prop_is_verified = None
+                        prop_profile_picture_url = None
+                        prop_is_possible_scammer = None
+
+                        if "has_anonymous_profile_picture" in each_item:
+                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
+
+                        if "pk" in each_item:
+                            prop_user_id = each_item["pk"]
+
+                        if "username" in each_item:
+                            prop_username = each_item["username"]
+
+                        if "full_name" in each_item:
+                            prop_full_name = each_item["full_name"]
+
+                        if "is_private" in each_item:
+                            prop_is_private = each_item["is_private"]
+
+                        if "is_verified" in each_item:
+                            prop_is_verified = each_item["is_verified"]
+
+                        if "profile_pic_url" in each_item:
+                            prop_profile_picture_url = each_item["profile_pic_url"]
+
+                        if "is_possible_scammer" in each_item:
+                            prop_is_possible_scammer = each_item["is_possible_scammer"]
+
+                        yield FollowPerson(
+                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
+                            user_id=prop_user_id,
+                            username=prop_username,
+                            full_name=prop_full_name,
+                            is_private=prop_is_private,
+                            is_verified=prop_is_verified,
+                            profile_picture_url=prop_profile_picture_url,
+                            is_possible_scammer=prop_is_possible_scammer
+                        )
+
+                        generated_count += 1
+
+                if (generated_count < count or count == 0) and "next_max_id" in response_json:
+                    current_max_id = response_json["next_max_id"]
+                else:
+                    return None
+            except JSONDecodeError:
+                yield None
+                return None
+
     def _identifier(self, identifier: str | int, required: str | int):
         identifier = format_identifier(identifier)
 
         if len(identifier) <= 0:
             raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
 
         # Identifier: Username or UID?
```

### Comparing `ensta-2.0/ensta/containers/Profile.py` & `ensta-2.1/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-2.0/ensta/lib/Commons.py` & `ensta-2.1/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-2.0/ensta/lib/Exceptions.py` & `ensta-2.1/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-2.0/ensta.egg-info/PKG-INFO` & `ensta-2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,38 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.0
-Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
-Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
-Author: Deepak Soni
-Author-email: lonelycube@proton.me
-License: MIT
-Keywords: instagram,web,private,api,scraper,easy,download,upload
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # 🤖 Ensta - Simple Instagram API
-This package lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build your dream projects with very few and reliable lines of code.
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
 
-It supports three types of classes - *Guest*, *Host*, *Stream*.
+It supports three two of classes - *Guest* & *Host*.
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Installation
-It's recommended to install this package using [Python's PIP](https://pypi.org/project/pip/), as the GitHub versions may be unstable and may require testing before being used in production.
-
-To install this library, run this command in a terminal window:
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
 ```shell
 pip install ensta
 ```
 
-To upgrade the installed version of this library, run:
+To upgrade to the latest version, run:
 ```shell
 pip install ensta --upgrade
 ```
 
-## Guest Mode
+## 🧔🏻‍♂️ Guest Mode
 This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available
-- Fetch someone's profile information
+- Check if username is available for registration
+- Fetch someone's profile data
 - Convert username to userid
 - Convert userid to username
 
-Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
 profile = guest.profile("cristiano")
 
@@ -56,26 +40,25 @@
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
 ```
 
-## Host Mode
-This mode requires the user to login through their [SessionID](https://github.com/diezo/ensta#session-id). SessionID shall be passed as an argument while initializing this class. It can be used to fetch data that's available only when the user is logged in. Additionally, the user can perform several actions on their profile.
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
 
-Methods supported till now are listed below:
+These are the methods supported till now:
 - Check authentication status of the user
-- Follow someone's account
-- Unfollow someone's account
-- Get someone's follower list of specified size
-- Get someone's following list of specified size
-- Toggle account privacy - 'Private' or 'Public'
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
 
-Here's an example where an instance of *Host* is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile:
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
 
 ```python
 from ensta import Host
 
 sessionid = "123456:abcdefg"  # Place your SessionId here
 
 host = Host(sessionid)
@@ -87,51 +70,28 @@
     if status.following:
         print("Following!")
     
     elif status.follow_requested:
         print("Requested to follow!")
 ```
 
-## Stream Mode
-This mode pulls data at realtime, so the program can process it simultaneously. It requires login through [SessionID](https://github.com/diezo/ensta#session-id).
-
-In a situation where you might need to fetch someone's entire follower list, this mode comes handy.
-
-These are the methods supported till now:
-- Fetch someone's follower list
-- Fetch someone's following list
-
-Here's an example where an instance of *Stream* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) first 100 followers:
-
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
 ```python
-from ensta import Stream
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-stream = Stream(sessionid)
-followers = stream.followers("cristiano")
+from ensta import Guest
 
-for user in followers:
-    if user is None:
-        print("Something went wrong.")
-        break
+guest = Guest()
+available = guest.username_availability("cristiano")
 
-    print(user.username)
-    print(user.full_name)
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
 ```
 
-## Considerations
-Here are some key points to consider when using this library in production:
-- You can use *Guest*, *Host* & *Stream* classes simultaneously, and create multiple instances of the same class when required.
-- Functions should return *None* on failure. So, add clauses for the same.
-
-- Some functions take Identifier as an argument while others take Username. These are the key differences between the two:
-  - The argument **Identifier** means you can pass either Username or UserID.
-  - The argument **Username** means you must pass the Username only, and not the UserID.
-
 ## Session ID
 When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
 
 In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
 - Visit [Instagram.com](https://instagram.com) and log into your account.
 - Once you're logged in, open DevTools (Ctrl + Shift + I).
 - Switch to **Application** tab.
@@ -143,8 +103,8 @@
 
 ## Donate ❤️
 If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
 
 [!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
 
 ## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
```

### Comparing `ensta-2.0/setup.py` & `ensta-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="2.0",
+    version="2.1",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

