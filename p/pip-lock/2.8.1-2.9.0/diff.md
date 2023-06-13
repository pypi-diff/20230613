# Comparing `tmp/pip-lock-2.8.1.tar.gz` & `tmp/pip-lock-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-lock-2.8.1.tar", last modified: Mon Feb 14 12:06:58 2022, max compression
+gzip compressed data, was "pip-lock-2.9.0.tar", last modified: Wed May 11 12:28:21 2022, max compression
```

## Comparing `pip-lock-2.8.1.tar` & `pip-lock-2.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-14 12:06:58.832414 pip-lock-2.8.1/
--rw-r--r--   0 chainz     (501) staff       (20)     3484 2022-02-14 12:06:48.000000 pip-lock-2.8.1/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1076 2022-02-08 12:17:32.000000 pip-lock-2.8.1/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      245 2022-02-08 12:17:32.000000 pip-lock-2.8.1/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     5609 2022-02-14 12:06:58.832533 pip-lock-2.8.1/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     4493 2022-02-08 12:17:32.000000 pip-lock-2.8.1/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-02-08 12:17:32.000000 pip-lock-2.8.1/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1299 2022-02-14 12:06:58.833044 pip-lock-2.8.1/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-02-08 12:17:32.000000 pip-lock-2.8.1/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-14 12:06:58.828734 pip-lock-2.8.1/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-14 12:06:58.830725 pip-lock-2.8.1/src/pip_lock/
--rw-r--r--   0 chainz     (501) staff       (20)     3863 2022-02-14 12:06:39.000000 pip-lock-2.8.1/src/pip_lock/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-09-19 14:42:11.000000 pip-lock-2.8.1/src/pip_lock/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-02-14 12:06:58.832175 pip-lock-2.8.1/src/pip_lock.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     5609 2022-02-14 12:06:58.000000 pip-lock-2.8.1/src/pip_lock.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      337 2022-02-14 12:06:58.000000 pip-lock-2.8.1/src/pip_lock.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-02-14 12:06:58.000000 pip-lock-2.8.1/src/pip_lock.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-02-14 12:06:57.000000 pip-lock-2.8.1/src/pip_lock.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       46 2022-02-14 12:06:58.000000 pip-lock-2.8.1/src/pip_lock.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)        9 2022-02-14 12:06:58.000000 pip-lock-2.8.1/src/pip_lock.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 12:28:21.222163 pip-lock-2.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     3547 2022-05-11 12:28:12.000000 pip-lock-2.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1076 2022-02-08 12:17:32.000000 pip-lock-2.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      101 2022-04-27 09:19:14.000000 pip-lock-2.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     5640 2022-05-11 12:28:21.222314 pip-lock-2.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     4493 2022-05-11 12:26:09.000000 pip-lock-2.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      635 2022-02-08 12:17:32.000000 pip-lock-2.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1316 2022-05-11 12:28:21.222943 pip-lock-2.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       74 2022-02-08 12:17:32.000000 pip-lock-2.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 12:28:21.216387 pip-lock-2.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 12:28:21.219720 pip-lock-2.9.0/src/pip_lock/
+-rw-r--r--   0 chainz     (501) staff       (20)     3863 2022-02-14 12:06:39.000000 pip-lock-2.9.0/src/pip_lock/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-09-19 14:42:11.000000 pip-lock-2.9.0/src/pip_lock/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-05-11 12:28:21.221432 pip-lock-2.9.0/src/pip_lock.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     5640 2022-05-11 12:28:20.000000 pip-lock-2.9.0/src/pip_lock.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      337 2022-05-11 12:28:21.000000 pip-lock-2.9.0/src/pip_lock.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 12:28:20.000000 pip-lock-2.9.0/src/pip_lock.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-05-11 12:28:19.000000 pip-lock-2.9.0/src/pip_lock.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       46 2022-05-11 12:28:21.000000 pip-lock-2.9.0/src/pip_lock.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        9 2022-05-11 12:28:21.000000 pip-lock-2.9.0/src/pip_lock.egg-info/top_level.txt
```

### Comparing `pip-lock-2.8.1/HISTORY.rst` & `pip-lock-2.9.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.9.0 (2022-05-11)
+------------------
+
+* Support Python 3.11.
+
 2.8.1 (2022-02-14)
 ------------------
 
 * Ignore all ``<name> @ <url>`` lines, rather than just for VCS URL’s.
 
 2.8.0 (2022-02-08)
 ------------------
```

### Comparing `pip-lock-2.8.1/LICENSE` & `pip-lock-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-lock-2.8.1/PKG-INFO` & `pip-lock-2.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pip-lock
-Version: 2.8.1
+Version: 2.9.0
 Summary: Check for differences between requirements.txt files and your environment.
 Home-page: https://github.com/adamchainz/pip-lock
 Author: Aaron Kirkbride, Adam Johnson, et al.
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pip-lock/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pip,requirements
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
@@ -46,15 +46,15 @@
 Check for differences between requirements.txt files and the current environment.
 
 Installation
 ============
 
 Install with ``python -m pip install pip-lock``.
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
@@ -151,9 +151,7 @@
 
 Example:
 
 .. code-block:: pycon
 
     >>> get_mismatches("requirements.txt")
     {'django': ('1.10.2', '1.9.0'), 'requests': ('2.11.1', '2.9.2'), 'request-oauthlib': ('0.7.0', None)}
-
-
```

### Comparing `pip-lock-2.8.1/README.rst` & `pip-lock-2.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Check for differences between requirements.txt files and the current environment.
 
 Installation
 ============
 
 Install with ``python -m pip install pip-lock``.
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
```

### Comparing `pip-lock-2.8.1/pyproject.toml` & `pip-lock-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip-lock-2.8.1/setup.cfg` & `pip-lock-2.9.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pip-lock
-version = 2.8.1
+version = 2.9.0
 description = Check for differences between requirements.txt files and your environment.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Aaron Kirkbride, Adam Johnson, et al.
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/pip-lock
 project_urls = 
@@ -19,17 +19,17 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python
 	Topic :: Utilities
-license_file = LICENSE
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires =
```

### Comparing `pip-lock-2.8.1/src/pip_lock/__init__.py` & `pip-lock-2.9.0/src/pip_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `pip-lock-2.8.1/src/pip_lock.egg-info/PKG-INFO` & `pip-lock-2.9.0/src/pip_lock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pip-lock
-Version: 2.8.1
+Version: 2.9.0
 Summary: Check for differences between requirements.txt files and your environment.
 Home-page: https://github.com/adamchainz/pip-lock
 Author: Aaron Kirkbride, Adam Johnson, et al.
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pip-lock/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: pip,requirements
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
@@ -46,15 +46,15 @@
 Check for differences between requirements.txt files and the current environment.
 
 Installation
 ============
 
 Install with ``python -m pip install pip-lock``.
 
-Python 3.7 to 3.10 supported.
+Python 3.7 to 3.11 supported.
 
 ----
 
 **Working on a Django project?**
 Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
@@ -151,9 +151,7 @@
 
 Example:
 
 .. code-block:: pycon
 
     >>> get_mismatches("requirements.txt")
     {'django': ('1.10.2', '1.9.0'), 'requests': ('2.11.1', '2.9.2'), 'request-oauthlib': ('0.7.0', None)}
-
-
```

