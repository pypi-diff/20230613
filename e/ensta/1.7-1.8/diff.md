# Comparing `tmp/ensta-1.7.tar.gz` & `tmp/ensta-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.7.tar", last modified: Tue Jun 13 09:08:30 2023, max compression
+gzip compressed data, was "ensta-1.8.tar", last modified: Tue Jun 13 14:12:31 2023, max compression
```

## Comparing `ensta-1.7.tar` & `ensta-1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     6728 2023-06-13 09:08:30.309595 ensta-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5963 2023-06-13 08:34:59.000000 ensta-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.274587 ensta-1.7/ensta/
--rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.7/ensta/Guest.py
--rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.7/ensta/Host.py
--rw-rw-rw-   0        0        0    14411 2023-06-13 08:32:24.000000 ensta-1.7/ensta/Stream.py
--rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.7/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.7/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.7/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.7/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.7/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.7/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/ensta/lib/
--rw-rw-rw-   0        0        0     1477 2023-06-13 08:32:05.000000 ensta-1.7/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.7/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.7/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.296637 ensta-1.7/ensta.egg-info/
--rw-rw-rw-   0        0        0     6728 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 09:08:30.309595 ensta-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-13 09:08:09.000000 ensta-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     6730 2023-06-13 14:12:31.667818 ensta-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5965 2023-06-13 10:14:35.000000 ensta-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.636442 ensta-1.8/ensta/
+-rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.8/ensta/Guest.py
+-rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.8/ensta/Host.py
+-rw-rw-rw-   0        0        0    14438 2023-06-13 09:23:10.000000 ensta-1.8/ensta/Stream.py
+-rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.8/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.8/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.8/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.8/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.8/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.8/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.667818 ensta-1.8/ensta/lib/
+-rw-rw-rw-   0        0        0     2457 2023-06-13 14:11:09.000000 ensta-1.8/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.8/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.8/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:12:31.652065 ensta-1.8/ensta.egg-info/
+-rw-rw-rw-   0        0        0     6730 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 14:12:31.000000 ensta-1.8/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 14:12:31.683318 ensta-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-13 14:12:13.000000 ensta-1.8/setup.py
```

### Comparing `ensta-1.7/LICENSE.txt` & `ensta-1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.7/PKG-INFO` & `ensta-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.7
+Version: 1.8
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
@@ -46,15 +46,15 @@
 
 Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
-profile = guest.profile("ronaldo")
+profile = guest.profile("cristiano")
 
 if profile is None:
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
```

### Comparing `ensta-1.7/README.md` & `ensta-1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
-profile = guest.profile("ronaldo")
+profile = guest.profile("cristiano")
 
 if profile is None:
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
```

### Comparing `ensta-1.7/ensta/Guest.py` & `ensta-1.8/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-1.7/ensta/Host.py` & `ensta-1.8/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-1.7/ensta/Stream.py` & `ensta-1.8/ensta/Stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
                     current_max_id = response_json["next_max_id"]
                 else:
                     return None
             except JSONDecodeError:
                 yield None
                 return None
 
-    def _identifier(self, identifier: str | int, required: str | int):
+    def _identifier(self, identifier: str | int, required: str | int) -> tuple[bool, str | None]:
         identifier = format_identifier(identifier)
 
         if len(identifier) <= 0:
             raise IdentifierError("No identifier was given. Please pass either UserId or Username as an argument.")
 
         # Identifier: Username or UID?
         is_username = False
```

### Comparing `ensta-1.7/ensta/containers/Profile.py` & `ensta-1.8/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-1.7/ensta/lib/Exceptions.py` & `ensta-1.8/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-1.7/ensta.egg-info/PKG-INFO` & `ensta-1.8/ensta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.7
+Version: 1.8
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
 Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
@@ -46,15 +46,15 @@
 
 Here's an example where an instance of *Guest* is created to fetch [Cristiano Ronaldo's](https://www.instagram.com/cristiano/) profile information:
 
 ```python
 from ensta import Guest
 
 guest = Guest()
-profile = guest.profile("ronaldo")
+profile = guest.profile("cristiano")
 
 if profile is None:
     print("Something went wrong.")
 else:
     print(profile.biography)
     print(profile.follower_count)
     print(profile.following_count)
```

### Comparing `ensta-1.7/setup.py` & `ensta-1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="1.7",
+    version="1.8",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
```

