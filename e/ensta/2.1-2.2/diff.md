# Comparing `tmp/ensta-2.1.tar.gz` & `tmp/ensta-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-2.1.tar", last modified: Tue Jun 13 17:45:25 2023, max compression
+gzip compressed data, was "ensta-2.2.tar", last modified: Tue Jun 13 18:06:46 2023, max compression
```

## Comparing `ensta-2.1.tar` & `ensta-2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.192557 ensta-2.1/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5889 2023-06-13 17:45:25.192557 ensta-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5124 2023-06-13 17:23:39.000000 ensta-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.116706 ensta-2.1/ensta/
--rw-rw-rw-   0        0        0    11194 2023-06-13 14:18:20.000000 ensta-2.1/ensta/Guest.py
--rw-rw-rw-   0        0        0    22543 2023-06-13 16:38:17.000000 ensta-2.1/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-13 16:38:34.000000 ensta-2.1/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.176938 ensta-2.1/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-2.1/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-2.1/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-2.1/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-2.1/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-2.1/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.192557 ensta-2.1/ensta/lib/
--rw-rw-rw-   0        0        0     2483 2023-06-13 14:40:57.000000 ensta-2.1/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-2.1/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-2.1/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:45:25.145657 ensta-2.1/ensta.egg-info/
--rw-rw-rw-   0        0        0     5889 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 17:45:24.000000 ensta-2.1/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 17:45:25.192557 ensta-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-13 17:45:04.000000 ensta-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-13 18:06:24.000000 ensta-2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-13 18:06:46.049261 ensta-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-13 18:06:24.000000 ensta-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-13 18:06:24.000000 ensta-2.2/ensta/Guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22026 2023-06-13 18:06:24.000000 ensta-2.2/ensta/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 18:06:24.000000 ensta-2.2/ensta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/FollowPerson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/FollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/UnfollowedStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 18:06:24.000000 ensta-2.2/ensta/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/Commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 18:06:24.000000 ensta-2.2/ensta/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:06:46.049261 ensta-2.2/ensta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 18:06:46.000000 ensta-2.2/ensta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 18:06:46.053261 ensta-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-13 18:06:24.000000 ensta-2.2/setup.py
```

### Comparing `ensta-2.1/LICENSE.txt` & `ensta-2.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ensta
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Ensta
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ensta-2.1/PKG-INFO` & `ensta-2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.1
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
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
-
-It supports three two of classes - *Guest* & *Host*.
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
-```shell
-pip install ensta
-```
-
-To upgrade to the latest version, run:
-```shell
-pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
-- Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
-
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # Operation failed
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+Metadata-Version: 2.1
+Name: ensta
+Version: 2.2
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.2.tar.gz
+Author: Deepak Soni
+Author-email: lonelycube@proton.me
+License: MIT
+Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+
+It supports three two of classes - *Guest* & *Host*.
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Installation
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+```shell
+pip install ensta
+```
+
+To upgrade to the latest version, run:
+```shell
+pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
+
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host
+
+sessionid = "123456:abcdefg"  # Place your SessionId here
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## Session ID
+When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
+
+In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
+- Visit [Instagram.com](https://instagram.com) and log into your account.
+- Once you're logged in, open DevTools (Ctrl + Shift + I).
+- Switch to **Application** tab.
+- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
+- Once done, you will see the list of all cookies.
+- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
+
+An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
+
+## Donate ❤️
+If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Disclaimer
+This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
```

### Comparing `ensta-2.1/README.md` & `ensta-2.2/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
-
-It supports three two of classes - *Guest* & *Host*.
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
-```shell
-pip install ensta
-```
-
-To upgrade to the latest version, run:
-```shell
-pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
-- Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
-
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # Operation failed
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Disclaimer
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+
+It supports three two of classes - *Guest* & *Host*.
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Installation
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+```shell
+pip install ensta
+```
+
+To upgrade to the latest version, run:
+```shell
+pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
+
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host
+
+sessionid = "123456:abcdefg"  # Place your SessionId here
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## Session ID
+When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
+
+In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
+- Visit [Instagram.com](https://instagram.com) and log into your account.
+- Once you're logged in, open DevTools (Ctrl + Shift + I).
+- Switch to **Application** tab.
+- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
+- Once done, you will see the list of all cookies.
+- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
+
+An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
+
+## Donate ❤️
+If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Disclaimer
 This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
```

### Comparing `ensta-2.1/ensta/Guest.py` & `ensta-2.2/ensta/Guest.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-from json import JSONDecodeError
-import random
-import requests
-from .lib.Commons import (
-    update_session,
-    update_homepage_source,
-    update_app_id,
-    refresh_csrf_token,
-    format_username,
-    format_uid
-)
-from .containers.Profile import Profile
-
-
-class Guest:
-    request_session: requests.Session = None
-    homepage_source: str = None
-    insta_app_id: str = None
-    csrf_token: str = None
-
-    def __init__(self, homepage_source: str = None, app_id: str | int = None) -> None:
-        update_session(self)
-
-        if homepage_source is not None:
-            self.homepage_source = homepage_source
-        else:
-            update_homepage_source(self)
-
-        if app_id is not None:
-            self.insta_app_id = str(app_id)
-        else:
-            update_app_id(self)
-
-    def username_availability(self, username: str) -> bool | None:
-        username = format_username(username)
-        refresh_csrf_token(self)
-        body_json = {
-            "email": f"{username}@{self.csrf_token}.com",
-            "username": username,
-            "first_name": username.capitalize(),
-            "opt_into_one_tap": False
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": "0",
-            "x-instagram-ajax": "1007614758",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/emailsignup/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "errors" in response_json:
-                return "username" not in response_json["errors"]
-        except JSONDecodeError:
-            return None
-
-    def profile(self, username: str, __session__: requests.Session = None) -> Profile | None:
-        username = format_username(username)
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": "0",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{username}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            session = __session__
-            if __session__ is None: session = self.request_session
-
-            http_response = session.get(
-                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
-                headers=request_headers
-            )
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "data" in response_json:
-                    if "user" in response_json["data"]:
-
-                        profile_object_biography = None
-                        profile_object_country_block = None
-                        profile_object_full_name = None
-                        profile_object_following_count = None
-                        profile_object_follower_count = None
-                        profile_object_user_id = None
-                        profile_object_is_business_account = None
-                        profile_object_is_professional_account = None
-                        profile_object_is_supervision_enabled = None
-                        profile_object_is_joined_recently = None
-                        profile_object_is_private = None
-                        profile_object_is_verified = None
-                        profile_object_profile_picture_url = None
-                        profile_object_profile_picture_url_hd = None
-                        profile_object_pronouns = None
-
-                        if "biography" in response_json["data"]["user"]:
-                            profile_object_biography = response_json["data"]["user"]["biography"]
-
-                        if "country_block" in response_json["data"]["user"]:
-                            profile_object_country_block = response_json["data"]["user"]["country_block"]
-
-                        if "full_name" in response_json["data"]["user"]:
-                            profile_object_full_name = response_json["data"]["user"]["full_name"]
-
-                        if "edge_follow" in response_json["data"]["user"]:
-                            if "count" in response_json["data"]["user"]["edge_follow"]:
-                                profile_object_following_count = response_json["data"]["user"]["edge_follow"]["count"]
-
-                        if "edge_followed_by" in response_json["data"]["user"]:
-                            if "count" in response_json["data"]["user"]["edge_followed_by"]:
-                                profile_object_follower_count = response_json["data"]["user"]["edge_followed_by"]["count"]
-
-                        if "id" in response_json["data"]["user"]:
-                            profile_object_user_id = response_json["data"]["user"]["id"]
-
-                        if "is_business_account" in response_json["data"]["user"]:
-                            profile_object_is_business_account = response_json["data"]["user"]["is_business_account"]
-
-                        if "is_professional_account" in response_json["data"]["user"]:
-                            profile_object_is_professional_account = response_json["data"]["user"]["is_professional_account"]
-
-                        if "is_supervision_enabled" in response_json["data"]["user"]:
-                            profile_object_is_supervision_enabled = response_json["data"]["user"][
-                                "is_supervision_enabled"]
-
-                        if "is_joined_recently" in response_json["data"]["user"]:
-                            profile_object_is_joined_recently = response_json["data"]["user"]["is_joined_recently"]
-
-                        if "is_private" in response_json["data"]["user"]:
-                            profile_object_is_private = response_json["data"]["user"]["is_private"]
-
-                        if "is_verified" in response_json["data"]["user"]:
-                            profile_object_is_verified = response_json["data"]["user"]["is_verified"]
-
-                        if "profile_pic_url" in response_json["data"]["user"]:
-                            profile_object_profile_picture_url = response_json["data"]["user"]["profile_pic_url"]
-
-                        if "profile_pic_url_hd" in response_json["data"]["user"]:
-                            profile_object_profile_picture_url_hd = response_json["data"]["user"]["profile_pic_url_hd"]
-
-                        if "pronouns" in response_json["data"]["user"]:
-                            user_pronouns = []
-                            for pronoun in response_json["data"]["user"]["pronouns"]:
-                                user_pronouns.append(pronoun)
-                            profile_object_pronouns = user_pronouns
-
-                        return Profile(
-                            biography=profile_object_biography,
-                            country_block=profile_object_country_block,
-                            full_name=profile_object_full_name,
-                            follower_count=profile_object_follower_count,
-                            following_count=profile_object_following_count,
-                            user_id=profile_object_user_id,
-                            is_business_account=profile_object_is_business_account,
-                            is_professional_account=profile_object_is_professional_account,
-                            is_supervision_enabled=profile_object_is_supervision_enabled,
-                            is_joined_recently=profile_object_is_joined_recently,
-                            is_private=profile_object_is_private,
-                            is_verified=profile_object_is_verified,
-                            profile_picture_url=profile_object_profile_picture_url,
-                            profile_picture_url_hd=profile_object_profile_picture_url_hd,
-                            pronouns=profile_object_pronouns
-                        )
-        except JSONDecodeError:
-            return None
-
-    def get_uid(self, username: str) -> str | None:
-        username = username.strip().lower().replace(" ", "")
-        response = self.profile(username)
-
-        if response.user_id is not None:
-            return format_uid(response.user_id)
-
-    def get_username(self, uid: str | int) -> str | None:
-        uid = format_uid(uid)
-        refresh_csrf_token(self)
-        request_headers = {
-            "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
-        }
-
-        try:
-            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
-            response_json = http_response.json()
-
-            if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
-                return format_username(response_json["user"]["username"])
-
-        except JSONDecodeError:
-            return None
+from json import JSONDecodeError
+import random
+import requests
+from .lib.Commons import (
+    update_session,
+    update_homepage_source,
+    update_app_id,
+    refresh_csrf_token,
+    format_username,
+    format_uid
+)
+from .containers.Profile import Profile
+
+
+class Guest:
+    request_session: requests.Session = None
+    homepage_source: str = None
+    insta_app_id: str = None
+    csrf_token: str = None
+
+    def __init__(self, homepage_source: str = None, app_id: str | int = None) -> None:
+        update_session(self)
+
+        if homepage_source is not None:
+            self.homepage_source = homepage_source
+        else:
+            update_homepage_source(self)
+
+        if app_id is not None:
+            self.insta_app_id = str(app_id)
+        else:
+            update_app_id(self)
+
+    def username_availability(self, username: str) -> bool | None:
+        username = format_username(username)
+        refresh_csrf_token(self)
+        body_json = {
+            "email": f"{username}@{self.csrf_token}.com",
+            "username": username,
+            "first_name": username.capitalize(),
+            "opt_into_one_tap": False
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
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
+            "x-ig-www-claim": "0",
+            "x-instagram-ajax": "1007614758",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": "https://www.instagram.com/accounts/emailsignup/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/web_create_ajax/attempt/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "errors" in response_json:
+                return "username" not in response_json["errors"]
+        except JSONDecodeError:
+            return None
+
+    def profile(self, username: str, __session__: requests.Session = None) -> Profile | None:
+        username = format_username(username)
+        refresh_csrf_token(self)
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
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
+            "x-ig-www-claim": "0",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{username}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            session = __session__
+            if __session__ is None: session = self.request_session
+
+            http_response = session.get(
+                f"https://www.instagram.com/api/v1/users/web_profile_info/?username={username}",
+                headers=request_headers
+            )
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "data" in response_json:
+                    if "user" in response_json["data"]:
+
+                        profile_object_biography = None
+                        profile_object_country_block = None
+                        profile_object_full_name = None
+                        profile_object_following_count = None
+                        profile_object_follower_count = None
+                        profile_object_user_id = None
+                        profile_object_is_business_account = None
+                        profile_object_is_professional_account = None
+                        profile_object_is_supervision_enabled = None
+                        profile_object_is_joined_recently = None
+                        profile_object_is_private = None
+                        profile_object_is_verified = None
+                        profile_object_profile_picture_url = None
+                        profile_object_profile_picture_url_hd = None
+                        profile_object_pronouns = None
+
+                        if "biography" in response_json["data"]["user"]:
+                            profile_object_biography = response_json["data"]["user"]["biography"]
+
+                        if "country_block" in response_json["data"]["user"]:
+                            profile_object_country_block = response_json["data"]["user"]["country_block"]
+
+                        if "full_name" in response_json["data"]["user"]:
+                            profile_object_full_name = response_json["data"]["user"]["full_name"]
+
+                        if "edge_follow" in response_json["data"]["user"]:
+                            if "count" in response_json["data"]["user"]["edge_follow"]:
+                                profile_object_following_count = response_json["data"]["user"]["edge_follow"]["count"]
+
+                        if "edge_followed_by" in response_json["data"]["user"]:
+                            if "count" in response_json["data"]["user"]["edge_followed_by"]:
+                                profile_object_follower_count = response_json["data"]["user"]["edge_followed_by"]["count"]
+
+                        if "id" in response_json["data"]["user"]:
+                            profile_object_user_id = response_json["data"]["user"]["id"]
+
+                        if "is_business_account" in response_json["data"]["user"]:
+                            profile_object_is_business_account = response_json["data"]["user"]["is_business_account"]
+
+                        if "is_professional_account" in response_json["data"]["user"]:
+                            profile_object_is_professional_account = response_json["data"]["user"]["is_professional_account"]
+
+                        if "is_supervision_enabled" in response_json["data"]["user"]:
+                            profile_object_is_supervision_enabled = response_json["data"]["user"][
+                                "is_supervision_enabled"]
+
+                        if "is_joined_recently" in response_json["data"]["user"]:
+                            profile_object_is_joined_recently = response_json["data"]["user"]["is_joined_recently"]
+
+                        if "is_private" in response_json["data"]["user"]:
+                            profile_object_is_private = response_json["data"]["user"]["is_private"]
+
+                        if "is_verified" in response_json["data"]["user"]:
+                            profile_object_is_verified = response_json["data"]["user"]["is_verified"]
+
+                        if "profile_pic_url" in response_json["data"]["user"]:
+                            profile_object_profile_picture_url = response_json["data"]["user"]["profile_pic_url"]
+
+                        if "profile_pic_url_hd" in response_json["data"]["user"]:
+                            profile_object_profile_picture_url_hd = response_json["data"]["user"]["profile_pic_url_hd"]
+
+                        if "pronouns" in response_json["data"]["user"]:
+                            user_pronouns = []
+                            for pronoun in response_json["data"]["user"]["pronouns"]:
+                                user_pronouns.append(pronoun)
+                            profile_object_pronouns = user_pronouns
+
+                        return Profile(
+                            biography=profile_object_biography,
+                            country_block=profile_object_country_block,
+                            full_name=profile_object_full_name,
+                            follower_count=profile_object_follower_count,
+                            following_count=profile_object_following_count,
+                            user_id=profile_object_user_id,
+                            is_business_account=profile_object_is_business_account,
+                            is_professional_account=profile_object_is_professional_account,
+                            is_supervision_enabled=profile_object_is_supervision_enabled,
+                            is_joined_recently=profile_object_is_joined_recently,
+                            is_private=profile_object_is_private,
+                            is_verified=profile_object_is_verified,
+                            profile_picture_url=profile_object_profile_picture_url,
+                            profile_picture_url_hd=profile_object_profile_picture_url_hd,
+                            pronouns=profile_object_pronouns
+                        )
+        except JSONDecodeError:
+            return None
+
+    def get_uid(self, username: str) -> str | None:
+        username = username.strip().lower().replace(" ", "")
+        response = self.profile(username)
+
+        if response.user_id is not None:
+            return format_uid(response.user_id)
+
+    def get_username(self, uid: str | int) -> str | None:
+        uid = format_uid(uid)
+        refresh_csrf_token(self)
+        request_headers = {
+            "User-Agent": "Instagram 76.0.0.15.395 Android (24/7.0; 640dpi; 1440x2560; samsung; SM-G930F; herolte; samsungexynos8890; en_US; 138226743)"
+        }
+
+        try:
+            http_response = self.request_session.get(f"https://i.instagram.com/api/v1/users/{uid}/info/", headers=request_headers)
+            response_json = http_response.json()
+
+            if "status" in response_json and response_json["status"] == "ok" and "user" in response_json and "username" in response_json["user"]:
+                return format_username(response_json["user"]["username"])
+
+        except JSONDecodeError:
+            return None
```

### Comparing `ensta-2.1/ensta/Host.py` & `ensta-2.2/ensta/Host.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,517 +1,517 @@
-import requests
-from json import JSONDecodeError
-import random
-import string
-from collections.abc import Generator
-from .Guest import Guest
-from .lib.Commons import (
-    refresh_csrf_token,
-    update_app_id,
-    update_homepage_source,
-    update_session,
-    format_identifier
-)
-from .lib import (
-    AuthenticationError,
-    NetworkError,
-    IdentifierError,
-    CodeError
-)
-from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
-from .containers.Profile import Profile
-
-USERNAME = 0
-UID = 1
-
-
-class Host:
-    request_session: requests.Session = None
-    homepage_source: str = None
-    insta_app_id: str = None
-    preferred_color_scheme: str = "dark"
-    x_ig_www_claim: str = None
-    csrf_token: str = None
-    guest: Guest = None
-
-    def __init__(self, session_id: str) -> None:
-        self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
-        update_session(self)
-        update_homepage_source(self)
-        update_app_id(self)
-
-        self.guest = Guest(
-            homepage_source=self.homepage_source,
-            app_id=self.insta_app_id
-        )
-
-        self.request_session.cookies.set("sessionid", session_id)
-
-        if not self.authenticated():
-            raise AuthenticationError("Either User ID or Session ID is not valid.")
-
-    def update_homepage_source(self) -> None:
-        temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
-
-        if temp_homepage_source == "":
-            raise NetworkError("Couldn't load instagram homepage.")
-
-        self.homepage_source = temp_homepage_source
-
-    def authenticated(self) -> bool:
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/edit/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-        http_response = self.request_session.get("https://www.instagram.com/api/v1/accounts/edit/web_form_data/", headers=request_headers)
-
-        try:
-            http_response.json()
-            return True
-        except JSONDecodeError:
-            return False
-
-    def follow(self, identifier: str | int) -> FollowedStatus | None:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"] \
-                            and "previous_following" in response_json:
-                        return FollowedStatus(
-                            following=response_json["friendship_status"]["following"],
-                            follow_requested=response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"],
-                            previous_following=response_json["previous_following"]
-                        )
-        except JSONDecodeError:
-            return None
-
-    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success: return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        body_json = {
-            "container_module": "profile",
-            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
-            "user_id": identifier
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" in response_json:
-                if response_json["status"] == "ok" and "friendship_status" in response_json:
-                    if "following" in response_json["friendship_status"] \
-                            and "outgoing_request" in response_json["friendship_status"] \
-                            and "followed_by" in response_json["friendship_status"]:
-                        return UnfollowedStatus(
-                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
-                            is_my_follower=response_json["friendship_status"]["followed_by"]
-                        )
-        except JSONDecodeError:
-            return None
-
-    def followers(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success:
-            yield None
-            return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/followers/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        current_max_id = ""
-        generated_count = 0
-
-        while True:
-            current_max_id_text = ""
-
-            if current_max_id != "":
-                current_max_id_text = f"&max_id={current_max_id}"
-
-            try:
-                count_text = 35
-
-                if count < 35:
-                    count_text = count
-
-                http_response = self.request_session.get(f"https://www.instagram.com/api/v1/friendships/{identifier}/followers/?count={str(count_text)}{current_max_id_text}&search_surface=follow_list_page", headers=request_headers)
-                response_json = http_response.json()
-
-                if "status" not in response_json or "users" not in response_json:
-                    yield None
-                    return None
-
-                if response_json["status"] != "ok":
-                    yield None
-                    return None
-
-                for each_item in response_json["users"]:
-                    if generated_count < count or count == 0:
-
-                        prop_has_anonymous_profile_picture = None
-                        prop_user_id = None
-                        prop_username = None
-                        prop_full_name = None
-                        prop_is_private = None
-                        prop_is_verified = None
-                        prop_profile_picture_url = None
-                        prop_is_possible_scammer = None
-
-                        if "has_anonymous_profile_picture" in each_item:
-                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
-
-                        if "pk" in each_item:
-                            prop_user_id = each_item["pk"]
-
-                        if "username" in each_item:
-                            prop_username = each_item["username"]
-
-                        if "full_name" in each_item:
-                            prop_full_name = each_item["full_name"]
-
-                        if "is_private" in each_item:
-                            prop_is_private = each_item["is_private"]
-
-                        if "is_verified" in each_item:
-                            prop_is_verified = each_item["is_verified"]
-
-                        if "profile_pic_url" in each_item:
-                            prop_profile_picture_url = each_item["profile_pic_url"]
-
-                        if "is_possible_scammer" in each_item:
-                            prop_is_possible_scammer = each_item["is_possible_scammer"]
-
-                        yield FollowPerson(
-                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
-                            user_id=prop_user_id,
-                            username=prop_username,
-                            full_name=prop_full_name,
-                            is_private=prop_is_private,
-                            is_verified=prop_is_verified,
-                            profile_picture_url=prop_profile_picture_url,
-                            is_possible_scammer=prop_is_possible_scammer
-                        )
-
-                        generated_count += 1
-
-                if (generated_count < count or count == 0) and "next_max_id" in response_json:
-                    current_max_id = response_json["next_max_id"]
-                else:
-                    return None
-            except JSONDecodeError:
-                yield None
-                return None
-
-    def followings(self, identifier: str | int, count: int = 0) -> Generator[FollowPerson, None, None]:
-        conversion_success, identifier = self._identifier(identifier, UID)
-        if not conversion_success:
-            yield None
-            return None
-
-        # Actual Request
-        refresh_csrf_token(self)
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/following/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        current_max_id = ""
-        generated_count = 0
-
-        while True:
-            current_max_id_text = ""
-
-            if current_max_id != "":
-                current_max_id_text = f"&max_id={current_max_id}"
-
-            try:
-                count_text = 35
-
-                if count < 35:
-                    count_text = count
-
-                http_response = self.request_session.get(
-                    f"https://www.instagram.com/api/v1/friendships/{identifier}/following/?count={str(count_text)}{current_max_id_text}",
-                    headers=request_headers)
-                response_json = http_response.json()
-
-                if "status" not in response_json or "users" not in response_json:
-                    yield None
-                    return None
-
-                if response_json["status"] != "ok":
-                    yield None
-                    return None
-
-                for each_item in response_json["users"]:
-                    if generated_count < count or count == 0:
-
-                        prop_has_anonymous_profile_picture = None
-                        prop_user_id = None
-                        prop_username = None
-                        prop_full_name = None
-                        prop_is_private = None
-                        prop_is_verified = None
-                        prop_profile_picture_url = None
-                        prop_is_possible_scammer = None
-
-                        if "has_anonymous_profile_picture" in each_item:
-                            prop_has_anonymous_profile_picture = each_item["has_anonymous_profile_picture"]
-
-                        if "pk" in each_item:
-                            prop_user_id = each_item["pk"]
-
-                        if "username" in each_item:
-                            prop_username = each_item["username"]
-
-                        if "full_name" in each_item:
-                            prop_full_name = each_item["full_name"]
-
-                        if "is_private" in each_item:
-                            prop_is_private = each_item["is_private"]
-
-                        if "is_verified" in each_item:
-                            prop_is_verified = each_item["is_verified"]
-
-                        if "profile_pic_url" in each_item:
-                            prop_profile_picture_url = each_item["profile_pic_url"]
-
-                        if "is_possible_scammer" in each_item:
-                            prop_is_possible_scammer = each_item["is_possible_scammer"]
-
-                        yield FollowPerson(
-                            has_anonymous_profile_picture=prop_has_anonymous_profile_picture,
-                            user_id=prop_user_id,
-                            username=prop_username,
-                            full_name=prop_full_name,
-                            is_private=prop_is_private,
-                            is_verified=prop_is_verified,
-                            profile_picture_url=prop_profile_picture_url,
-                            is_possible_scammer=prop_is_possible_scammer
-                        )
-
-                        generated_count += 1
-
-                if (generated_count < count or count == 0) and "next_max_id" in response_json:
-                    current_max_id = response_json["next_max_id"]
-                else:
-                    return None
-            except JSONDecodeError:
-                yield None
-                return None
-
-    def _identifier(self, identifier: str | int, required: str | int):
-        identifier = format_identifier(identifier)
-
-        if len(identifier) <= 0:
-            raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
-
-        # Identifier: Username or UID?
-        is_username = False
-        for letter in identifier:
-            if letter not in string.digits:
-                is_username = True
-                break
-
-        if is_username and required == USERNAME:
-            return True, identifier
-
-        elif is_username and required == UID:
-            user_id = self.guest.get_uid(identifier)
-
-            if user_id is not None and user_id != "":
-                return True, user_id
-            else:
-                return False, None
-
-        elif not is_username and required == USERNAME:
-            username = self.guest.get_username(identifier)
-
-            if username is not None and username != "":
-                return True, username
-            else:
-                return False, None
-
-        elif not is_username and required == UID:
-            return True, identifier
-
-        else:
-            raise CodeError("Identifier Conversion (Else Block)")
-
-    def _set_account_privacy(self, privacy: str) -> bool:
-        is_private = (privacy == "private")
-
-        if privacy != "private" and privacy != "public":
-            raise CodeError("_set_account_privacy")
-
-        refresh_csrf_token(self)
-        body_json = {
-            "is_private": is_private
-        }
-        request_headers = {
-            "accept": "*/*",
-            "accept-language": "en-US,en;q=0.9",
-            "content-type": "application/x-www-form-urlencoded",
-            "sec-ch-prefers-color-scheme": self.preferred_color_scheme,
-            "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-            "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.91\", \"Google Chrome\";v=\"114.0.5735.91\"",
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"Windows\"",
-            "sec-ch-ua-platform-version": "\"15.0.0\"",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "viewport-width": "1475",
-            "x-asbd-id": "198387",
-            "x-csrftoken": self.csrf_token,
-            "x-ig-app-id": self.insta_app_id,
-            "x-ig-www-claim": self.x_ig_www_claim,
-            "x-instagram-ajax": "1007616494",
-            "x-requested-with": "XMLHttpRequest",
-            "Referer": "https://www.instagram.com/accounts/who_can_see_your_content/",
-            "Referrer-Policy": "strict-origin-when-cross-origin"
-        }
-
-        try:
-            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/set_private/", headers=request_headers, data=body_json)
-            response_json = http_response.json()
-
-            if "status" not in response_json:
-                return False
-
-            if response_json["status"] != "ok":
-                return False
-
-            return True
-        except JSONDecodeError:
-            return False
-
-    def switch_to_private_account(self) -> bool:
-        return self._set_account_privacy("private")
-
-    def switch_to_public_account(self) -> bool:
-        return self._set_account_privacy("public")
-
-    def profile(self, username: str) -> Profile | None:
-        return self.guest.profile(username, self.request_session)
+import requests
+from json import JSONDecodeError
+import random
+import string
+from collections.abc import Generator
+from .Guest import Guest
+from .lib.Commons import (
+    refresh_csrf_token,
+    update_app_id,
+    update_homepage_source,
+    update_session,
+    format_identifier
+)
+from .lib import (
+    AuthenticationError,
+    NetworkError,
+    IdentifierError,
+    CodeError
+)
+from .containers import (FollowedStatus, UnfollowedStatus, FollowPerson)
+from .containers.Profile import Profile
+
+USERNAME = 0
+UID = 1
+
+
+class Host:
+    request_session: requests.Session = None
+    homepage_source: str = None
+    insta_app_id: str = None
+    preferred_color_scheme: str = "dark"
+    x_ig_www_claim: str = None
+    csrf_token: str = None
+    guest: Guest = None
+
+    def __init__(self, session_id: str) -> None:
+        self.x_ig_www_claim = "hmac." + "".join(random.choices(string.ascii_letters + string.digits + "_-", k=48))
+        update_session(self)
+        update_homepage_source(self)
+        update_app_id(self)
+
+        self.guest = Guest(
+            homepage_source=self.homepage_source,
+            app_id=self.insta_app_id
+        )
+
+        self.request_session.cookies.set("sessionid", session_id)
+
+        if not self.authenticated():
+            raise AuthenticationError("Either User ID or Session ID is not valid.")
+
+    def update_homepage_source(self) -> None:
+        temp_homepage_source = requests.get("https://www.instagram.com/").text.strip()
+
+        if temp_homepage_source == "":
+            raise NetworkError("Couldn't load instagram homepage.")
+
+        self.homepage_source = temp_homepage_source
+
+    def authenticated(self) -> bool:
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
+            "Referer": "https://www.instagram.com/accounts/edit/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+        http_response = self.request_session.get("https://www.instagram.com/api/v1/accounts/edit/web_form_data/", headers=request_headers)
+
+        try:
+            http_response.json()
+            return True
+        except JSONDecodeError:
+            return False
+
+    def follow(self, identifier: str | int) -> FollowedStatus | None:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success: return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        body_json = {
+            "container_module": "profile",
+            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
+            "user_id": identifier
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
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
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=5))}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/create/{identifier}/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "friendship_status" in response_json:
+                    if "following" in response_json["friendship_status"] \
+                            and "outgoing_request" in response_json["friendship_status"] \
+                            and "followed_by" in response_json["friendship_status"] \
+                            and "previous_following" in response_json:
+                        return FollowedStatus(
+                            following=response_json["friendship_status"]["following"],
+                            follow_requested=response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"],
+                            previous_following=response_json["previous_following"]
+                        )
+        except JSONDecodeError:
+            return None
+
+    def unfollow(self, identifier: str | int) -> UnfollowedStatus | None:
+        conversion_success, identifier = self._identifier(identifier, UID)
+        if not conversion_success: return None
+
+        # Actual Request
+        refresh_csrf_token(self)
+        body_json = {
+            "container_module": "profile",
+            "nav_chain": f"PolarisProfileRoot:profilePage:1:via_cold_start",
+            "user_id": identifier
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
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
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": f"https://www.instagram.com/{''.join(random.choices(string.ascii_lowercase, k=6))}/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post(f"https://www.instagram.com/api/v1/friendships/destroy/{identifier}/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" in response_json:
+                if response_json["status"] == "ok" and "friendship_status" in response_json:
+                    if "following" in response_json["friendship_status"] \
+                            and "outgoing_request" in response_json["friendship_status"] \
+                            and "followed_by" in response_json["friendship_status"]:
+                        return UnfollowedStatus(
+                            unfollowed=not response_json["friendship_status"]["following"] and not response_json["friendship_status"]["outgoing_request"],
+                            is_my_follower=response_json["friendship_status"]["followed_by"]
+                        )
+        except JSONDecodeError:
+            return None
+
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
+    def _identifier(self, identifier: str | int, required: str | int):
+        identifier = format_identifier(identifier)
+
+        if len(identifier) <= 0:
+            raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
+
+        # Identifier: Username or UID?
+        is_username = False
+        for letter in identifier:
+            if letter not in string.digits:
+                is_username = True
+                break
+
+        if is_username and required == USERNAME:
+            return True, identifier
+
+        elif is_username and required == UID:
+            user_id = self.guest.get_uid(identifier)
+
+            if user_id is not None and user_id != "":
+                return True, user_id
+            else:
+                return False, None
+
+        elif not is_username and required == USERNAME:
+            username = self.guest.get_username(identifier)
+
+            if username is not None and username != "":
+                return True, username
+            else:
+                return False, None
+
+        elif not is_username and required == UID:
+            return True, identifier
+
+        else:
+            raise CodeError("Identifier Conversion (Else Block)")
+
+    def _set_account_privacy(self, privacy: str) -> bool:
+        is_private = (privacy == "private")
+
+        if privacy != "private" and privacy != "public":
+            raise CodeError("_set_account_privacy")
+
+        refresh_csrf_token(self)
+        body_json = {
+            "is_private": is_private
+        }
+        request_headers = {
+            "accept": "*/*",
+            "accept-language": "en-US,en;q=0.9",
+            "content-type": "application/x-www-form-urlencoded",
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
+            "x-instagram-ajax": "1007616494",
+            "x-requested-with": "XMLHttpRequest",
+            "Referer": "https://www.instagram.com/accounts/who_can_see_your_content/",
+            "Referrer-Policy": "strict-origin-when-cross-origin"
+        }
+
+        try:
+            http_response = self.request_session.post("https://www.instagram.com/api/v1/web/accounts/set_private/", headers=request_headers, data=body_json)
+            response_json = http_response.json()
+
+            if "status" not in response_json:
+                return False
+
+            if response_json["status"] != "ok":
+                return False
+
+            return True
+        except JSONDecodeError:
+            return False
+
+    def switch_to_private_account(self) -> bool:
+        return self._set_account_privacy("private")
+
+    def switch_to_public_account(self) -> bool:
+        return self._set_account_privacy("public")
+
+    def profile(self, username: str) -> Profile | None:
+        return self.guest.profile(username, self.request_session)
```

### Comparing `ensta-2.1/ensta/lib/Commons.py` & `ensta-2.2/ensta/lib/Commons.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import string
-import requests
-import requests.cookies
-import random
-from .Exceptions import NetworkError
-
-
-def update_app_id(self) -> None:
-    app_id_occurrence_string = "\"APP_ID\":\""
-    app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
-    app_id_raw_text = self.homepage_source[
-                      app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
-    self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
-
-
-def refresh_csrf_token(self) -> None:
-    self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
-    cookie_object = requests.cookies.create_cookie(domain="instagram.com", name="csrftoken", value=self.csrf_token)
-    self.request_session.cookies.set_cookie(cookie_object)
-
-
-def update_session(self) -> None:
-    self.request_session = requests.Session()
-
-
-def update_homepage_source(self) -> None:
-    request_headers = {
-        "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-        "accept-language": "en-US,en;q=0.9",
-        "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
-        "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
-        "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
-        "sec-ch-ua-mobile": "?0",
-        "sec-ch-ua-platform": "\"Windows\"",
-        "sec-ch-ua-platform-version": "\"15.0.0\"",
-        "sec-fetch-dest": "document",
-        "sec-fetch-mode": "navigate",
-        "sec-fetch-site": "none",
-        "sec-fetch-user": "?1",
-        "upgrade-insecure-requests": "1",
-        "viewport-width": "1475",
-        "Referrer-Policy": "strict-origin-when-cross-origin"
-    }
-    temp_homepage_source = requests.get("https://www.instagram.com/", headers=request_headers).text.strip()
-
-    if temp_homepage_source != "":
-        self.homepage_source = temp_homepage_source
-    else:
-        raise NetworkError("Couldn't load instagram homepage.")
-
-
-def format_username(username: str) -> str:
-    return username.replace(" ", "").lower()
-
-
-def format_uid(uid: str) -> str:
-    return uid.replace(" ", "")
-
-
-def format_identifier(identifier: str | int) -> str:
-    return str(identifier).lower().replace(" ", "")
+import string
+import requests
+import requests.cookies
+import random
+from .Exceptions import NetworkError
+
+
+def update_app_id(self) -> None:
+    app_id_occurrence_string = "\"APP_ID\":\""
+    app_id_first_occurrence = self.homepage_source.index(app_id_occurrence_string)
+    app_id_raw_text = self.homepage_source[
+                      app_id_first_occurrence + len(app_id_occurrence_string): app_id_first_occurrence + 30]
+    self.insta_app_id = app_id_raw_text[: app_id_raw_text.index("\"")]
+
+
+def refresh_csrf_token(self) -> None:
+    self.csrf_token = "".join(random.choices(string.ascii_letters + string.digits, k=32))
+    cookie_object = requests.cookies.create_cookie(domain="instagram.com", name="csrftoken", value=self.csrf_token)
+    self.request_session.cookies.set_cookie(cookie_object)
+
+
+def update_session(self) -> None:
+    self.request_session = requests.Session()
+
+
+def update_homepage_source(self) -> None:
+    request_headers = {
+        "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        "accept-language": "en-US,en;q=0.9",
+        "sec-ch-prefers-color-scheme": random.choice(["light", "dark"]),
+        "sec-ch-ua": "\"Not.A/Brand\";v=\"8\", \"Chromium\";v=\"114\", \"Google Chrome\";v=\"114\"",
+        "sec-ch-ua-full-version-list": "\"Not.A/Brand\";v=\"8.0.0.0\", \"Chromium\";v=\"114.0.5735.110\", \"Google Chrome\";v=\"114.0.5735.110\"",
+        "sec-ch-ua-mobile": "?0",
+        "sec-ch-ua-platform": "\"Windows\"",
+        "sec-ch-ua-platform-version": "\"15.0.0\"",
+        "sec-fetch-dest": "document",
+        "sec-fetch-mode": "navigate",
+        "sec-fetch-site": "none",
+        "sec-fetch-user": "?1",
+        "upgrade-insecure-requests": "1",
+        "viewport-width": "1475",
+        "Referrer-Policy": "strict-origin-when-cross-origin"
+    }
+    temp_homepage_source = requests.get("https://www.instagram.com/", headers=request_headers).text.strip()
+
+    if temp_homepage_source != "":
+        self.homepage_source = temp_homepage_source
+    else:
+        raise NetworkError("Couldn't load instagram homepage.")
+
+
+def format_username(username: str) -> str:
+    return username.replace(" ", "").lower()
+
+
+def format_uid(uid: str) -> str:
+    return uid.replace(" ", "")
+
+
+def format_identifier(identifier: str | int) -> str:
+    return str(identifier).lower().replace(" ", "")
```

### Comparing `ensta-2.1/ensta/lib/Exceptions.py` & `ensta-2.2/ensta/lib/Exceptions.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-class AuthenticationError(Exception):
-
-    def __init__(self, message):
-        super().__init__(message)
-
-
-class NetworkError(Exception):
-
-    def __init__(self, message):
-        super().__init__(message)
-
-
-class IdentifierError(Exception):
-
-    def __init__(self, message):
-        super().__init__(message)
-
-
-class CodeError(Exception):
-
-    def __init__(self, location: str = "Unknown"):
-        super().__init__(f"There was an error while executing this function, maybe caused due to a bug in the code. Please submit this as an issue on GitHub.\nFound in: {location}")
+class AuthenticationError(Exception):
+
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class NetworkError(Exception):
+
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class IdentifierError(Exception):
+
+    def __init__(self, message):
+        super().__init__(message)
+
+
+class CodeError(Exception):
+
+    def __init__(self, location: str = "Unknown"):
+        super().__init__(f"There was an error while executing this function, maybe caused due to a bug in the code. Please submit this as an issue on GitHub.\nFound in: {location}")
```

### Comparing `ensta-2.1/ensta.egg-info/PKG-INFO` & `ensta-2.2/ensta.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1
-Name: ensta
-Version: 2.1
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
-# 🤖 Ensta - Simple Instagram API
-[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
-[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
-
-This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
-
-It supports three two of classes - *Guest* & *Host*.
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Installation
-To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
-```shell
-pip install ensta
-```
-
-To upgrade to the latest version, run:
-```shell
-pip install ensta --upgrade
-```
-
-## 🧔🏻‍♂️ Guest Mode
-This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
-- Check if username is available for registration
-- Fetch someone's profile data
-- Convert username to userid
-- Convert userid to username
-
-Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
-
-```python
-from ensta import Guest
-
-guest = Guest()
-profile = guest.profile("cristiano")
-
-if profile is None:
-    print("Something went wrong.")
-else:
-    print(profile.biography)
-    print(profile.follower_count)
-    print(profile.following_count)
-```
-
-## 🧔🏻‍♂️ Host Mode
-This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
-
-These are the methods supported till now:
-- Check authentication status of the user
-- Send follow request to an account
-- Follow/unfollow accounts
-- Fetch someone's follower/following list
-- Toggle account privacy - 'Public' or 'Private'
-
-Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
-
-```python
-from ensta import Host
-
-sessionid = "123456:abcdefg"  # Place your SessionId here
-
-host = Host(sessionid)
-status = host.follow("cristiano")
-
-if status is None:
-    print("Something went wrong.")
-else:
-    if status.following:
-        print("Following!")
-    
-    elif status.follow_requested:
-        print("Requested to follow!")
-```
-
-## Important
-Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
-```python
-from ensta import Guest
-
-guest = Guest()
-available = guest.username_availability("cristiano")
-
-if available is None:  # Operation failed
-    print("Something went wrong.")
-else:
-    print(available)
-```
-
-## Session ID
-When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
-
-In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
-- Visit [Instagram.com](https://instagram.com) and log into your account.
-- Once you're logged in, open DevTools (Ctrl + Shift + I).
-- Switch to **Application** tab.
-- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
-- Once done, you will see the list of all cookies.
-- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
-
-An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
-
-## Donate ❤️
-If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
-
-[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
-
-## Disclaimer
-This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
+Metadata-Version: 2.1
+Name: ensta
+Version: 2.2
+Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
+Home-page: https://github.com/diezo/ensta
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v2.2.tar.gz
+Author: Deepak Soni
+Author-email: lonelycube@proton.me
+License: MIT
+Keywords: instagram-client,instagram,api-wrapper,instagram-scraper,instagram-api,instagram-sdk,instagram-photos,instagram-api-python,instabot,instagram-stories,instagram-bot,instapy,instagram-downloader,instagram-account,instagram-crawler,instagram-private-api,igtv,instagram-automation,reels,instagram-feed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# 🤖 Ensta - Simple Instagram API
+[![PyPI](https://img.shields.io/pypi/v/ensta)](https://pypi.org/project/ensta)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ensta)]()
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/ensta)](https://pypi.org/project/ensta)
+[![Twitter URL](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fdiezo%2Fensta)
+
+This library lets you use Instagram's Internal Web API through simple functions and classes, that can help developers like you build projects with a few and reliable lines of code.
+
+It supports three two of classes - *Guest* & *Host*.
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Installation
+To install this library using [Python's PIP](https://pypi.org/project/pip/), run this command in a command-line interface:
+```shell
+pip install ensta
+```
+
+To upgrade to the latest version, run:
+```shell
+pip install ensta --upgrade
+```
+
+## 🧔🏻‍♂️ Guest Mode
+This mode doesn't require login and can be used to fetch publicly available data from Instagram's Servers. Following methods are supported till now:
+- Check if username is available for registration
+- Fetch someone's profile data
+- Convert username to userid
+- Convert userid to username
+
+Here's an example where an instance of *Guest* Class is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
+
+```python
+from ensta import Guest
+
+guest = Guest()
+profile = guest.profile("cristiano")
+
+if profile is None:
+    print("Something went wrong.")
+else:
+    print(profile.biography)
+    print(profile.follower_count)
+    print(profile.following_count)
+```
+
+## 🧔🏻‍♂️ Host Mode
+This mode requires login through [SessionID](https://github.com/diezo/ensta#session-id). The SessionID should be passed as an argument while initializing this class. It can be used to fetch data that requires login. Additionally, users can perform several actions on their profile.
+
+These are the methods supported till now:
+- Check authentication status of the user
+- Send follow request to an account
+- Follow/unfollow accounts
+- Fetch someone's follower/following list
+- Toggle account privacy - 'Public' or 'Private'
+
+Here's an example where an instance of *Host* Class is created to follow [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) account:
+
+```python
+from ensta import Host
+
+sessionid = "123456:abcdefg"  # Place your SessionId here
+
+host = Host(sessionid)
+status = host.follow("cristiano")
+
+if status is None:
+    print("Something went wrong.")
+else:
+    if status.following:
+        print("Following!")
+    
+    elif status.follow_requested:
+        print("Requested to follow!")
+```
+
+## Important
+Every function should return **None** on failure. So, it's recommended to an add if statement before using the actual data to avoid TypeError. Here's an example:
+```python
+from ensta import Guest
+
+guest = Guest()
+available = guest.username_availability("cristiano")
+
+if available is None:  # Operation failed
+    print("Something went wrong.")
+else:
+    print(available)
+```
+
+## Session ID
+When you log in to *instagram.com* in your browser, your browser store your credentials in the form of [Cookies](https://en.wikipedia.org/wiki/HTTP_cookie). The type of cookie that instagram uses to remember your session is 'SessionID'.
+
+In order to use the [Host Class](https://github.com/diezo/ensta#host-mode), you need to pass this cookie as an argument so that Ensta can use it to log into your account. Follow these steps to get your SessionID:
+- Visit [Instagram.com](https://instagram.com) and log into your account.
+- Once you're logged in, open DevTools (Ctrl + Shift + I).
+- Switch to **Application** tab.
+- Under *Storage* options, expand the **Cookies** tab, and tap the first item.
+- Once done, you will see the list of all cookies.
+- Copy value of cookie named 'sessionid' and pass it as an argument whenever you use the **Host Class**.
+
+An alternative way to automatically fetch SessionID is to run the [fetch-sessionid.py](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script. Currently, this script can only fetch cookies from Google Chrome, and not any other browser.
+
+## Donate ❤️
+If this library has added value to your projects, you may consider supporting me in the development of this library by donating here:
+
+[!["Buy me a coffee"](https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png)](https://buymeacoffee.com/diezo)
+
+## Disclaimer
+This is a third-party library, not an official library from Instagram. The use of the library does not promote creation of bot accounts or spamming Instagram Users. You are liable for all the actions you take through this library. Use of such libraries maybe against [Instagram's Community Guidelines](https://help.instagram.com/477434105621119/).
```

