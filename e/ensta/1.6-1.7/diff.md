# Comparing `tmp/ensta-1.6.tar.gz` & `tmp/ensta-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.6.tar", last modified: Tue Jun 13 08:46:10 2023, max compression
+gzip compressed data, was "ensta-1.7.tar", last modified: Tue Jun 13 09:08:30 2023, max compression
```

## Comparing `ensta-1.6.tar` & `ensta-1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.821377 ensta-1.6/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     6728 2023-06-13 08:46:10.821377 ensta-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5963 2023-06-13 08:34:59.000000 ensta-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.732075 ensta-1.6/ensta/
--rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.6/ensta/Guest.py
--rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.6/ensta/Host.py
--rw-rw-rw-   0        0        0    14411 2023-06-13 08:32:24.000000 ensta-1.6/ensta/Stream.py
--rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.6/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.798033 ensta-1.6/ensta/containers/
--rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.6/ensta/containers/FollowPerson.py
--rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.6/ensta/containers/FollowedStatus.py
--rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.6/ensta/containers/Profile.py
--rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.6/ensta/containers/UnfollowedStatus.py
--rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.6/ensta/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.818002 ensta-1.6/ensta/lib/
--rw-rw-rw-   0        0        0     1477 2023-06-13 08:32:05.000000 ensta-1.6/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.6/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.6/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:46:10.764659 ensta-1.6/ensta.egg-info/
--rw-rw-rw-   0        0        0     6728 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 08:46:10.000000 ensta-1.6/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 08:46:10.826738 ensta-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-13 08:45:55.000000 ensta-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     6728 2023-06-13 09:08:30.309595 ensta-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5963 2023-06-13 08:34:59.000000 ensta-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.274587 ensta-1.7/ensta/
+-rw-rw-rw-   0        0        0    11201 2023-06-12 15:22:13.000000 ensta-1.7/ensta/Guest.py
+-rw-rw-rw-   0        0        0    12446 2023-06-13 08:32:16.000000 ensta-1.7/ensta/Host.py
+-rw-rw-rw-   0        0        0    14411 2023-06-13 08:32:24.000000 ensta-1.7/ensta/Stream.py
+-rw-rw-rw-   0        0        0       93 2023-06-12 14:44:37.000000 ensta-1.7/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/ensta/containers/
+-rw-rw-rw-   0        0        0      347 2023-06-09 08:53:51.000000 ensta-1.7/ensta/containers/FollowPerson.py
+-rw-rw-rw-   0        0        0      222 2023-06-09 08:46:48.000000 ensta-1.7/ensta/containers/FollowedStatus.py
+-rw-rw-rw-   0        0        0      584 2023-06-09 07:33:57.000000 ensta-1.7/ensta/containers/Profile.py
+-rw-rw-rw-   0        0        0      153 2023-06-09 08:28:13.000000 ensta-1.7/ensta/containers/UnfollowedStatus.py
+-rw-rw-rw-   0        0        0      162 2023-06-09 08:48:05.000000 ensta-1.7/ensta/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.309595 ensta-1.7/ensta/lib/
+-rw-rw-rw-   0        0        0     1477 2023-06-13 08:32:05.000000 ensta-1.7/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      597 2023-06-09 15:54:08.000000 ensta-1.7/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      298 2023-06-09 09:10:42.000000 ensta-1.7/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:08:30.296637 ensta-1.7/ensta.egg-info/
+-rw-rw-rw-   0        0        0     6728 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 09:08:30.000000 ensta-1.7/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 09:08:30.309595 ensta-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-06-13 09:08:09.000000 ensta-1.7/setup.py
```

### Comparing `ensta-1.6/LICENSE.txt` & `ensta-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.6/PKG-INFO` & `ensta-1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.6
+Version: 1.7
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.6/README.md` & `ensta-1.7/README.md`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/Guest.py` & `ensta-1.7/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/Host.py` & `ensta-1.7/ensta/Host.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/Stream.py` & `ensta-1.7/ensta/Stream.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/containers/Profile.py` & `ensta-1.7/ensta/containers/Profile.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/lib/Commons.py` & `ensta-1.7/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta/lib/Exceptions.py` & `ensta-1.7/ensta/lib/Exceptions.py`

 * *Files identical despite different names*

### Comparing `ensta-1.6/ensta.egg-info/PKG-INFO` & `ensta-1.7/ensta.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.6
+Version: 1.7
 Summary: 🔥 Fastest & Simplest Python Package For Instagram Automation
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ensta-1.6/setup.py` & `ensta-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ensta",
     packages=["ensta", "ensta.lib", "ensta.containers"],
-    version="1.6",
+    version="1.7",
     license="MIT",
     description="🔥 Fastest & Simplest Python Package For Instagram Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.5.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.7.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

