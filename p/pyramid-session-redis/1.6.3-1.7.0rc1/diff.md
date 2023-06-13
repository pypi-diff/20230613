# Comparing `tmp/pyramid_session_redis-1.6.3.tar.gz` & `tmp/pyramid_session_redis-1.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_session_redis-1.6.3.tar", last modified: Tue Nov 16 23:03:06 2021, max compression
+gzip compressed data, was "pyramid_session_redis-1.7.0rc1.tar", last modified: Tue Jun 13 17:00:42 2023, max compression
```

## Comparing `pyramid_session_redis-1.6.3.tar` & `pyramid_session_redis-1.7.0rc1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)     9285 2021-11-16 23:01:45.000000 pyramid_session_redis-1.6.3/CHANGES.md
--rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2021-03-11 15:17:14.000000 pyramid_session_redis-1.6.3/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      198 2021-03-30 19:58:50.000000 pyramid_session_redis-1.6.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)    33371 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2021-03-11 15:18:11.000000 pyramid_session_redis-1.6.3/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)    26741 2021-11-16 22:58:54.000000 pyramid_session_redis-1.6.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      327 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2193 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/
--rw-r--r--   0 jvanasco   (501) admin       (80)    27889 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1628 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/compat.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3347 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/connection.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/
--rw-r--r--   0 jvanasco   (501) admin       (80)       25 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/.gitignore
--rw-r--r--   0 jvanasco   (501) admin       (80)       43 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/advanced.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)       21 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/api.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)     8331 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/conf.py
--rw-r--r--   0 jvanasco   (501) admin       (80)       39 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/contributing.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)       47 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/gettingstarted.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)     1682 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/index.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)     5128 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/make.bat
--rw-r--r--   0 jvanasco   (501) admin       (80)     5628 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/Makefile
--rw-r--r--   0 jvanasco   (501) admin       (80)      156 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/redis.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)     1765 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/exceptions.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     6617 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/legacy.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    24278 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/session.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    12430 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis/util.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-11-16 23:03:02.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-30 00:08:31.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)    33371 2021-11-16 23:03:02.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      177 2021-11-16 23:03:02.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1224 2021-11-16 23:03:02.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       22 2021-11-16 23:03:02.000000 pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-11-16 23:03:06.000000 pyramid_session_redis-1.6.3/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3678 2021-03-30 20:02:26.000000 pyramid_session_redis-1.6.3/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     5625 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/tests/test_config.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1537 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/tests/test_connection.py
--rw-r--r--   0 jvanasco   (501) admin       (80)   106350 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/tests/test_factory.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     5418 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/tests/test_serializers.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    49313 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/tests/test_session.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     6608 2021-03-30 20:01:37.000000 pyramid_session_redis-1.6.3/tests/test_util.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      441 2021-11-16 22:58:54.000000 pyramid_session_redis-1.6.3/TODO.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2021-11-16 23:01:22.000000 pyramid_session_redis-1.6.3/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.687448 pyramid_session_redis-1.7.0rc1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     9639 2023-06-13 17:00:22.000000 pyramid_session_redis-1.7.0rc1/CHANGES.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4951 2021-03-11 15:17:14.000000 pyramid_session_redis-1.7.0rc1/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      198 2021-03-30 19:58:50.000000 pyramid_session_redis-1.7.0rc1/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)    27831 2023-06-13 17:00:42.687861 pyramid_session_redis-1.7.0rc1/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)    26903 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)      441 2021-11-16 22:58:54.000000 pyramid_session_redis-1.7.0rc1/TODO.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-09 21:46:23.000000 pyramid_session_redis-1.7.0rc1/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      828 2023-06-13 17:00:42.690911 pyramid_session_redis-1.7.0rc1/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2402 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.602769 pyramid_session_redis-1.7.0rc1/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.627039 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    30089 2023-06-13 17:00:22.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      402 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/compat.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3596 2023-06-09 21:46:23.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/connection.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.651106 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/
+-rw-r--r--   0 jvanasco   (501) admin       (80)       25 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/.gitignore
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5628 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/Makefile
+-rw-r--r--   0 jvanasco   (501) admin       (80)       43 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/advanced.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)       21 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/api.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)     8327 2023-06-09 21:46:23.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/conf.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/contributing.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)       47 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/gettingstarted.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1682 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/index.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5128 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/make.bat
+-rw-r--r--   0 jvanasco   (501) admin       (80)      156 2021-03-30 20:01:37.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/redis.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1989 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/exceptions.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7839 2023-06-09 21:46:23.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/legacy.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-05-03 18:32:12.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)    27067 2023-05-03 18:32:12.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/session.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    14635 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/util.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.636908 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    27831 2023-06-13 17:00:42.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1281 2023-06-13 17:00:42.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-13 17:00:42.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-30 00:08:31.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      172 2023-06-13 17:00:42.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       22 2023-06-13 17:00:42.000000 pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 17:00:42.685687 pyramid_session_redis-1.7.0rc1/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3763 2023-05-03 18:32:12.000000 pyramid_session_redis-1.7.0rc1/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5720 2021-12-02 19:36:31.000000 pyramid_session_redis-1.7.0rc1/tests/test_config.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1589 2023-05-03 18:32:12.000000 pyramid_session_redis-1.7.0rc1/tests/test_connection.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)   106490 2023-06-10 19:25:49.000000 pyramid_session_redis-1.7.0rc1/tests/test_factory.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6130 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/tests/test_serializers.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    49363 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/tests/test_session.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    11517 2023-06-12 22:56:02.000000 pyramid_session_redis-1.7.0rc1/tests/test_support.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6600 2021-12-02 19:36:31.000000 pyramid_session_redis-1.7.0rc1/tests/test_util.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-05-03 21:41:03.000000 pyramid_session_redis-1.7.0rc1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_session_redis-1.6.3/CHANGES.md` & `pyramid_session_redis-1.7.0rc1/CHANGES.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Changelog
 =========
 
-* unreleased
-	* None
+* 2023.06.13
+    * version 1.7.0rc1
+    * Breaking Changes:
+      * The `session_id` will now always be serialized into a string.
+        * If a custom `id_generator` is used, it MUST return a string.
+        * Default usage of this package should not be affected at all.      
+	* code style changes
+	* dropping PY2
+	* initial typing support
+	* remove some webob dependencies
 
 * 2021.11.16
 	* version 1.6.3
 	* detect Redis version to better handle deprecated kwargs
 	* drop testing/support for python3.5
 	* minimum six requirement. thank you, @Wim-De-Clercq 
 	* cleanup changelog
@@ -21,15 +29,14 @@
 		* add redis_ prefix for redis passthrough kwargs
 			Add redis_ prefix for redis passthrough kwargs to
 			RedisSessionFactory().
 		* add tests for old and new encoding kwargs
 			Add tests for old and new encoding args for RedisSessionFactory()
 	* add tests for incompatible kwargs (test_session_factory_incompatible_kwargs)
 
-
 * 2021.04.01
 	* version 1.6.1
 	* fix invalid `expires` default. thank you, @olemoign
 	* doc fixes
 
 * 2021.03.30
     * version 1.6.0
```

### Comparing `pyramid_session_redis-1.6.3/LICENSE.txt` & `pyramid_session_redis-1.7.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyramid_session_redis-1.6.3/PKG-INFO` & `pyramid_session_redis-1.7.0rc1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,737 +1,727 @@
-Metadata-Version: 2.1
-Name: pyramid_session_redis
-Version: 1.6.3
-Summary: High performance and actively maintained server-side session framework for Pyramid and Redis.
-Home-page: https://github.com/jvanasco/pyramid_session_redis
-Author: Jonathan Vanasco
-Author-email: jonathan@findmeon.com
-License: BSD
-Description: [![Build Status](https://travis-ci.org/jvanasco/pyramid_session_redis.png)](https://travis-ci.org/jvanasco/pyramid_session_redis)
-        
-        
-        Overview
-        ========
-        
-        `pyramid_session_redis` is a mature, stable and actively maintained Server-Side
-        Sessions plugin for the Pyramid web framework.
-        
-        Originally, this library was a fork of
-        [`pyramid_redis_sessions`](`/ericrasmussen/pyramid_redis_sessions`), focused on
-        improvements and API changes designed for high performance (particularly with
-        servers under load), and a slightly different API designed for developer
-        convenience.
-        
-        This package was planning to follow a multi-version release process, however
-        that plan was abandoned in favor of ensuring backards compatibility.
-        
-        The `main` and `1.6` branches are designed to support both:
-        
-        * Python 2
-        * Python 3
-        
-        and
-        
-        * Pyramid 1.x
-        * Pyramid 2.0
-        
-        
-        Prior Branches
-        --------------
-        
-        The 1.5.x branch is in maintenance mode. No updates are expected, as 1.6 is
-        backwards compatible.
-        
-        The 1.4.x branch is EOL. It led to the stable 1.5.0 API release.
-        
-        The 1.2.x branch is EOL as of 1.2.2. Previous plans were to support a final
-        1.3.0 release.
-        
-        Prior Branch Details
-        ____________________
-        
-        The 1.2.x branch and earlier are largely a "drop-in-replacement" compatible with
-        Eric Rasmussen's `pyramid_redis_sessions` as-is.  If you are migrating from that
-        project and do not want to upgrade code, you should pin your install of this
-        library to `pyramid_session_redis<=1.3.0` or `pyramid_session_redis<1.3`
-        
-        **Please be aware that you will be limited to using outdated versions of Pyramid 
-        1.x if using the 1.2.x branch.**
-        
-        Starting with the 1.4.x branch, several design changes were made and this library
-        is not a drop-in replacement, **HOWEVER** upgrading will only require minimal
-        editing of your code: some editing for migration; some kwargs have changed;
-        the structure of the package changed (imports); and advanced users who leverage
-        the internal systems may need to upgrade. It should not take more than 5 minutes
-        to convert.  The package is still a plug-and-play Pyramid ISessions interface, so
-        there are very small changes.
-        
-        Prior Branch Incompatibilities
-        ______________________________
-        
-        IMPORTANT: The internal payload structure changed in the 1.4 branch, and is no
-        longer compatible with sessions created under 1.2 - they will be invalid.
-        
-        PRs that can handle a graceful fallback are welcome.
-        
-        The 1.2 format guaranteed internal sessions to be in this format:
-        
-            {'managed_dict': {},
-             'created': INT,
-             'timeout': INT,
-             }
-        
-        The 1.4 version streamlines the keys for a lighter footprint and generally
-        looks like this:
-        
-            {'m': {},  # managed_dict
-             'c': INT,  # created
-             'v': SESSION_API_VERSION,  # api version INT
-             # the following are optional and not guaranteed to be in a session
-             't': INT,  # timeout
-             'x': INT,  # expiry
-             }
-        
-        Key Takeaways:
-        
-        * Keys were shortened to 1 letter
-        * An API Version is now used, to handle graceful changes in the future
-        * The Timeout is no longer guaranteed to be present.
-          The library now supports the entire Timeout to be handled in Redis
-        * An "Expiry Timeout" may also exist
-        
-        Key Concepts
-        ============================================
-        
-        
-        Timeout vs Expires/MaxAge
-        -------------------------
-        
-        This package allows you to set both *Timeout* and *Expiry* values.  The two
-        concepts are closely related, but very different.
-        
-        A *Timeout* is an internal value and a moving target. It specifies how long a
-        Session should last before it times out due to inactivity. The timeout is
-        constantly refreshed when the session is accessed.
-        
-        For example, consider these settings:
-        
-            timeout = 1800
-            timeout_trigger = 900
-        
-        The `timeout` setting is specifying the Session should remain active for 1800
-        seconds since it's last activity.  The `timeout_trigger` setting is an
-        optimization that defers modifying the Session's timeout on READ operations until
-        at least 900 seconds have passed since the last modification. Modifications will
-        always occur on WRITE operations.  Depending on your configuration, the timeout
-        may be stored in Redis, as part of the Python Payload, or both.
-        
-        To illustrate how the above settings work, consider a timeline in which a User
-        visits a website and then visits it again 2000 seconds later:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit N | 2000s | Session B (new)
-        
-        When the User makes the last visit, the Session would have timed out, because it
-        exceeded the 1800 second mark in the timeout.
-        
-        Now assume the User makes 3 visits in this timeline, and a second visit happens
-        at the 899 mark:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit 2 | 899s  | Session A
-        > Visit N | 2000s | Session B (new)
-        
-        When the User makes the last visit, the Session would still
-        have timed out, because the second visit did not meet the timeout_trigger
-        threshold.
-        
-        But, if the second visit happens just 2 seconds later, at the 901 mark, the
-        timeout_trigger is reached and the session's timeout will be extended:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit 2 | 901s  | Session A (update timeout trigger)
-        > Visit N | 2000s | Session A (update timeout trigger)
-        
-        When the User makes the last visit, it would still happen within the context of
-        the original Session and the timeout will be extended even further.
-        
-        *Expires* and *Max-Age* are generally values that related to Cookie settings.
-        
-        *Expires* is created on a Cookie as either a specified Date, or a null value; if
-        the value is null (explicit or unspecified), the Cookie will be set as a
-        "Session" cookie and only last for the duration of the web browser application
-        being open.
-        
-        *Max-Age* is created on a Cookie as the number of seconds until the Cookie
-        expires.  A zero or negative value will expire (delete) the cookie immediately.
-        If both Expires and Max-Age are set, Max-Age has precedence.
-        
-        
-        The Confusion?
-        --------------
-        
-        If Redis stores our Timeout info, it stores it in an "expiry" value via `SETEX`
-        or similar calls.  
-        
-        
-        Key Differences From pyramid_redis_sessions
-        ============================================
-        
-        Depending on your needs, this package is probably more desirable than the
-        original project. This package was designed to significantly cut down on the
-        communication between Redis and Pyramid. Some options are offered to minimize
-        the size of Redis payloads as well.
-        
-        This package contains additional hooks and features to aid developers who are
-        using Redis-based sessions in high-traffic situations.
-        
-        This package does not recommend any "best deployment" strategies, but supports a
-        wide range of strategies to implement the "best deployment" under any given
-        circumstance.
-        
-        Through 1.2.x
-        -------------
-        
-        * The original package communicates with Redis on most attribute accesses and
-          writes within a given request. The traffic can be burdensome in some
-          implementations. `pyramid_session_redis` will queue a single `persist` or
-          `refresh` task per-request using Pyramid's `add_finished_callback` hook.
-        * The original version used `EXISTS` to check if a Session existed or not, then
-          proceeded to `GET` or `SET` a new Session.  `pyramid_session_redis` will
-          immediately attempt a `GET`, and will `SET` a new Session on failure.
-          This approach eliminates a call.
-        * Separate calls to `SET` and `EXPIRE` were replaced with a single `SETEX`.
-        * A flag can be set to enable a LRU Cache (least recently used) mode. No expiry
-          data will be sent to Redis, allowing the Redis server to handle the LRU logic
-          itself.
-        * The active Session is decoupled from the `request.session` attributs; this
-          allows for the Session to be set up on alternate attributes and supports
-          integration with
-          [pyramid_session_multi](https://github.com/jvanasco/pyramid_session_multi).
-        * The original library does not detect changes in nested dictionaries. This
-          package uses `hashlib.md5` to fingerprint the serialized value on READ; if no
-          changes were detected, a failsafe will `Serialize+md5` the data to decide if a
-          WRITE should occur. This behavior can be disabled by setting `detect_changes`
-          to `False`.
-        * The original library raises a fatal error if a Session can not be
-          deserialized. By passing in `deserialized_fails_new` to the constructor,
-          you can create a new Session on deserialization errors.
-        * Support for disabling Sessions on CDN generated content via
-          `func_check_response_allow_cookies`
-        * Thanks to @ github/hongyuan1306, Token Generation has been consolidated to use
-          Python3's stdlib (or reimplemented if not available). Tokens are also 32,
-          not 20, characters.
-        * Redis is supported in a LRU mode (see http://redis.io/topics/lru-cache) by
-          setting the option `set_redis_ttl` to `False` (by default, it is `True`).
-          This will eliminate calls to `EXPIRE` and will use `SET` instead of `SETEX`.
-        * In the 1.2.x branch, the created time can be set to an integer via
-          `use_int_time=True`. This will cast the `created` time via
-          `int(math.ceil(time.time()))`. This reduces a payload by several bits.
-        
-        Other Updates 1.4.x+
-        --------------------
-        
-        * Only `int()` time is supported; Fractional time wastes bytes.
-        * Sessions now have version control to support future upgrades via a "version"
-          `v` key.
-        * The format of the internal payload was rewritten, the encoded payload now
-          uses 1-letter keys instead of words. This should offset the addition of an
-          expires timestamp and version id.
-        * There was no logic for Python timeout control (whoops!) this has been fixed.
-          An "expires" `x` key now tracks the expiration.
-        * Added a `timeout_trigger` option.  This will defer expiry data updates to
-          lower usage on Redis.  This is explained below in more detail.
-        * In high load situations, Redis can have performance and storage issues because
-          in the original package Session IDs are created on every request (such as a
-          getting spidered by a botnet that does not respect Sessions). In this package,
-          a 'lazycreate' method is used: a session_id/cookie will not be generated
-          unless a session is needed in the callback routine. In order to generate
-          session_id/cookie beforehand, one can use the `RedisSession.ensure_id`
-          function.  To safely check if a session id exists, one can use the
-          `RedisSession.session_id_safecheck` method as well.
-        * Added `func_invalid_logger` to the constructor. This can be used to log
-          invalid Sessions. It is incredibly useful when integrated with a statsd
-          system. (see below)
-        * Added `set_redis_ttl_readheavy` to the factory and session constructors.
-          This option will optimize Sessions which have Redis-maintained TTLs by
-          executing a GET+EXPIRE together within a pipeline.
-        
-        
-        
-        Installation
-        ============
-        
-        Install via pypi:
-        
-            pip install pyramid_session_redis
-        
-        
-        Configuration
-        =============
-        
-        Configure `pyramid_session_redis` via your Paste config file or however you
-        prefer to configure Pyramid. Only `redis.sessions.secret` is required.
-        All other settings are optional.
-        
-        For complete documentation on the `RedisSessionFactory` that uses these
-        settings, see :doc:`api`. Otherwise, keep reading for the quick list:
-        
-        
-            # session settings
-            redis.sessions.secret = your_cookie_signing_secret
-            redis.sessions.timeout = 1200
-        
-            # session cookie settings
-            redis.sessions.cookie_name = session
-            redis.sessions.cookie_max_age = max_age_in_seconds
-            redis.sessions.cookie_path = /
-            redis.sessions.cookie_domain =
-            redis.sessions.cookie_secure = False
-            redis.sessions.cookie_httponly = False
-            redis.sessions.cookie_on_exception = True
-        
-            # you can supply a redis connection string as a URL
-            redis.sessions.url = redis://username:password@localhost:6379/0
-        
-            # or as individual settings (note: the URL gets preference if you do both)
-            redis.sessions.host = localhost
-            redis.sessions.port = 6379
-            redis.sessions.db = 0
-            redis.sessions.password = None
-        
-            # additional options can be supplied to redis-py's StrictRedis
-            redis.sessions.socket_timeout =
-            redis.sessions.connection_pool =
-            redis.sessions.charset = utf-8
-            redis.sessions.errors = strict
-            redis.sessions.unix_socket_path =
-        
-            # in the advanced section we'll cover how to instantiate your own client
-            redis.sessions.client_callable = my.dotted.python.callable
-        
-            # along with defining your own serialize and deserialize methods
-            redis.sessions.serialize = cPickle.dumps
-            redis.sessions.deserialize = cPickle.loads
-        
-            # you can specify a prefix to be used with session keys in redis
-            redis.sessions.prefix = mycoolprefix
-        
-            # or you can supply your own UID generator callable for session keys
-            redis.sessions.id_generator = niftyuid
-        
-        
-        Initialization
-        ==============
-        
-        Lastly, you need to tell Pyramid to use `pyramid_session_redis` as your
-        Session factory. The preferred way is adding it with `config.include`,
-        like this:
-        
-            def main(global_config, **settings):
-                config = Configurator(settings=settings)
-                config.include('pyramid_session_redis')
-        
-        Alternately, instead of using the Configurator's include method, you can
-        activate Pyramid by changing your application's ".ini" file, use the following
-        line:
-        
-            pyramid.includes = pyramid_session_redis
-        
-        The above method is recommended because it's simpler, idiomatic, and still fully
-        configurable. It even has the added benefit of automatically resolving dotted
-        python paths used in the advanced options.
-        
-        However, you can also explicitly pass a settings dict to the
-        `session_factory_from_settings` function. This can be helpful if you configure
-        or modify your settings in code:
-        
-            from pyramid_session_redis import session_factory_from_settings
-        
-            def main(global_config, **settings):
-                config = Configurator(settings=settings)
-                session_factory = pyramid_session_redis(settings)
-                config.set_session_factory(session_factory)
-        
-        
-        Timeout Notes
-        =============
-        
-        If ``set_redis_ttl`` is False, it does not imply there is no timeout at all --
-        only that Redis will not be sent timeout data via `SETEX` or `EXPIRE`.
-        Timeout data will still be stored in Python.
-        
-        If Redis is functioning as an LRU Cache, abandoned sessions will never be seen
-        by Python, but will eventually be cleared out to make room for new sessions by
-        the inherent Redis LRU logic.
-        
-        Timeout data stored in Python is relatively small when compared to the timeout
-        data stored in Redis.
-        
-        If you want to NEVER have sessions timeout, set the initial `timeout`
-        to "0" or "None".
-        
-        Setting a `timeout_trigger` will require Python to track the expiry.
-        
-        Enabling `set_redis_ttl_readheavy` requires a `timeout` and `set_redis_ttl`;
-        it also requires not enabling `timeout_trigger` or `python_expires`.
-        
-        
-        Timeout Examples
-        ----------------
-        
-        Timeout in Python, with Redis TTL via `SETEX`/`EXPIRE`:
-        
-            timeout = 60
-        
-        Timeout in Python, no Redis TTL (only `SET` used)
-        
-            timeout = 60
-            assume_redis_ttl = True
-        
-        No Timeout in Python, no Redis TTL (only `SET` used)
-        
-            timeout = 0  # or None
-            assume_redis_ttl = True
-        
-        
-        Warning: Session Locking and Race Conditions
-        ============================================
-        
-        This package does not incorporate any sort of locking for session updating or
-        handling of race conditions.
-        
-        This should not be a problem for the vast majority of users, and is a feature
-        not present on any known Pyramid Session providers.
-        
-        For more information, please see:
-        
-        * https://github.com/jvanasco/pyramid_session_redis/issues/9
-        * https://github.com/Pylons/pyramid/issues/3041
-        
-        
-        Feature - Timeout Triggers
-        ==========================
-        
-        A timeout trigger can be used to limit the amount of updates/writes.
-        It may be more beneficial to your usage pattern.
-        
-        For the sake of clarity, I'll use an oversimplification that Redis essentially
-        has two different internal data stores that are used independently: one for a
-        Key's payload and another for the Key's expiry.
-        
-        In the 'classic' behavior (project this was forked from): every time you access
-        an existing session, the GET is followed by sending Redis a new EXPIRE time;
-        essentially every "read" has a corresponding "write" for the Redis-tracked
-        expiry record.
-        
-        In order to minimize the writes via SETEX, I introduced the timeout trigger.
-        The trigger works by storing some timeout information in the Redis data payload,
-        and using that information to determine when to send a write. Instead of having
-        a GET+EXPIRE for every read, we only have a single GET and eliminate the write
-        caused by the EXPIRE. This has a maintenance cost though - once we hit the
-        timeout trigger, instead of just the GET we need to update the internal timeout
-        payload and issue a SET.
-        
-        Going back to your situation: when the user stops activity at 40 minutes in, if
-        the timeout trigger is enabled then there has never been an update to the
-        internal payload or Redis about the user activity since the session was first
-        created. The purpose of the trigger is to defer that "write" operation.
-        
-        In order to make a session valid for "reading" for around an hour, you should
-        do something like:
-        
-        * a two-hour session with a 10 minute trigger, or
-        * a one-hour session with a 50 minute trigger
-        
-        You can also disable the functionality by setting the trigger to 0. Up to a few
-        thousand daily users, you shouldn't have any issues with the overhead of the
-        "classic" mode. When you hit 10k users and/or start to have clustered web
-        servers communicating with dedicated Redis instances, setting a new EXPIRE after
-        every read operation becomes something you want to avoid.
-        
-        
-        Scenario 1 - Classic Redis
-        --------------------------
-        
-        In the typical "classic" Redis usage pattern, the session usage is refreshed via
-        an `EXPIRE` call on every session view.
-        
-        This is useful, but means many session operations will trigger two Redis calls
-        (`GET` + `EXPIRE`).  On a high performance system, this can be a lot.
-        
-        This is a typical scenario with refreshing:
-        
-            timeout = 200
-        
-        The following timeline would occur:
-        
-        | time | Redis calls    | timeout |
-        | ---- | -------------- | ------- |
-        | 0    | `GET`+`SETEX`  | 200     |
-        | 100  | `GET`+`EXPIRE` | 300     |
-        | 200  | `GET`+`EXPIRE` | 400     |
-        | 300  | `GET`+`EXPIRE` | 500     |
-        | 400  | `GET`+`EXPIRE` | 600     |
-        | 500  | `GET`+`EXPIRE` | 700     |
-        
-        
-        Scenario 2 - Timeout Trigger
-        --------------------------
-        
-        The 1.4.x branch introduces a `timeout_trigger` to augment the Session's
-        `timeout`.
-        
-        Whereas a `timeout` states how long a session is good for, a `timeout_trigger`
-        defers how long a Session's refresh should be deferred for:
-        
-        Given the following example, the package will use a 1200s timeout for requests,
-        but only trigger an update of the expiry time when the current time is within
-        600s of the expiry:
-        
-            timeout = 1200
-            timeout_trigger = 600
-        
-        The following timeline would occur:
-        
-        | time | Redis calls  | timeout | next threshold |
-        | ---- | ------------ | ------- | -------------- |
-        | 0    | `GET`+`SET`* | 1200    | 600            |
-        | 1    | `GET`        | 1200    | 600            |
-        | ...  |              |         |                |
-        | 599  | `GET`        | 1200    | 600            |
-        | 600  | `GET`+`SET`* | 1800    | 1200           |
-        | 601  | `GET`        | 1800    | 1200           |
-        | ...  |              |         |                |
-        | 1199 | `GET`        | 1800    | 1200           |
-        | 1200 | `GET`+`SET`* | 2400    | 1800           |
-        
-        * This method is compatible with setting a TTL in redis via `SETEX` or doing
-        everything within Python if Redis is in a LRU mode
-        
-        The removes all calls to `EXPIRE` before the threshold is reached, which can be
-         a considerable savings in read-heavy situations.
-        
-        The caveat to this method: an expiry timestamp must be stored within the payload
-        AND updating the timeout requires a `SET` operation.
-        
-        
-        Feature - set_redis_ttl_readheavy
-        =================================
-        
-        This is a new option in `1.4.2` which should improve performance on readheavy
-        installations BUT may degrade performance on writeheavy installations.  This
-        option will aggregate a GET+EXPIRE on every read.
-        
-        `set_redis_ttl_readheavy` requires the following:
-        
-        * a `timeout` value is set
-        * `set_redis_ttl` is `True`
-        * `timeout_trigger` is NOT set
-        * `python_expires` is NOT True
-        
-        The default behavior of this library during a read-only request is this:
-        
-        * On session access, query Redis via `redis.GET {session_id}`
-        * In a Pyramid callback, update Redis via `redis.EXPIRE {session_id} {expiry}`
-        
-        During a read-write:
-        
-        * On session access, query Redis via `redis.GET {session_id}`
-        * In a Pyramid callback, update Redis via
-          `redis.SETEX {session_id} {payload} {expiry}`
-        
-        The new `set_redis_ttl_readheavy` changes this. If enabled during a read-only
-        request, the behavior will be lighter on the Redis instance:
-        
-        * On session access, open a pipeline with two Redis commands:
-          `pipeline.GET {session_id}`,
-          `pipeline.EXPIRE {session_id} {expiry}`.
-        * In a Pyramid callback, the duplicate expire is suppressed.
-        
-        However during a read-write, the activity will be:
-        
-        * On session access, open a pipeline with two Redis commands:
-          `pipeline.GET {session_id}`,
-          `pipeline.EXPIRE {session_id} {expiry}`.
-        * In a Pyramid callback, update Redis via
-          `redis.SETEX {session_id} {payload} {expiry}`
-        
-        Read-heavy applications should see a slight performance bump via the pipeined
-        GET+EXPIRE, however write-heavy applications are likely to see a performance
-        degradation as it adds an extra EXPIRE to every request.
-        
-        
-        Invalid Logging
-        ================
-        
-        The default behavior of this library is to silently create new session when bad
-        session data is encountered, such as a cookie with an invalid id or corrupted
-        datastore.  A graceful "new session" is the ideal situation for end-users.
-        
-        The problem with that strategy is that problems in code or your application
-        stack can be hidden, and you might not know about a bad datastore.
-        
-        The 1.4 release introduces `func_invalid_logger` to the factory constructor.
-        This can be used to track the invalid sessions that are safely caught and
-        silently upgraded.
-        
-        How?  The package tracks why a session is invalid with variant classes of
-        `pyramid_session_redis.exceptions.InvalidSession`.
-        
-        Specifically there are the following classes:
-        
-        * ``InvalidSession(Exception)``
-          Catchall base class
-        * ``InvalidSession_NoSessionCookie(InvalidSession)``
-          The Session is invalid because there is no cookie.
-          This is the same as "new session".
-        * ``InvalidSession_NotInBackend(InvalidSession)``
-          The Session id was not in the backend.
-        * ``InvalidSession_DeserializationError(InvalidSession)``
-            Error deserializing.
-            This is raised if ``deserialized_fails_new`` is True. Otherwise the
-            exception is wrapped in a ``RawDeserializationError`` and raised without
-            being caught.
-        * ``InvalidSession_PayloadTimeout(InvalidSession)``
-            The inner Python payload timed out.
-        * ``InvalidSession_PayloadLegacy(InvalidSession)``
-            The Session is running on an earlier version.
-        
-        The factory accepts a `func_invalid_logger` callable argument. The input is the
-        raised exception BEFORE a new cookie is generated, and will be the request and
-        an instance of `InvalidSession`.
-        
-            from pyramid_session_redis.exceptions import *
-            from my_statsd import new_statsd_client()
-        
-            statsd_client = new_statsd_client()
-        
-            def my_logger(request, raised_exception):
-                """
-                raised_exception will be an instance of InvalidSession
-                log the exception to statsd for metrics
-                """
-                if isinstance(raised_exception, InvalidSession_NoSessionCookie):
-                    statsd_client.incr('invalid_session.NoSessionCookie')
-                elif isinstance(raised_exception, InvalidSession_NotInBackend):
-                    statsd_client.incr('invalid_session.NotInBackend')
-                elif isinstance(raised_exception, InvalidSession_DeserializationError):
-                    statsd_client.incr('invalid_session.DeserializationError')
-        
-            factory = RedisSessionFactory(...
-                                          func_invalid_logger=my_logger,
-                                          ...
-                                          )
-        
-        The `func_invalid_logger` argument may be provided as a dotted-notation string
-        in a configuration file.
-        
-        
-        Uncaught Errors
-        ================
-        
-        The exception `pyramid_session_redis.exceptions.RawDeserializationError` will be
-        raised if deserialization of a payload fails and `deserialized_fails_new` is not
-        `True`. The first arg will be the caught exception. This allows for a standard
-        error across multiple deserialization options.
-        
-        
-        FAQ:
-        =====
-        
-        Q. What serialization is used?
-        ------------------------------
-        
-        A. Serialization is used at two points
-        
-        * Serializing the Session data.
-          The server-side data serialization is handled by `pickle`. This Session data is
-          created on the server by your application and remains on the server. `pickle`
-          is safe to use in this context, as user-generated payloads can not be introduced
-          to these (de)serialization routines. If you wish to avoid `pickle`, or your
-          prefer to use another encoder, you can easily specify a different (de)serialization
-          routine such as a custom JSON, msgpack or pretty much anything else.
-        
-        * Serializing the `session_id` to encode into a signed cookie.
-          This library uses `WebOb.cookies.SignedSerializer` to securely manage a HMAC
-          signature of the `session_id` combined with a site-secret. The library allows
-          for a custom replacement to be provided as well.
-          
-          In the original library, the session id and signature were turned into a
-          cookie-safe value via `pickle` (de)serialization - a detail that remained in
-          this library through `<=v1.5.0`. This approach was identified as a security
-          risk, and was removed from this library starting in `v1.5.1`.  
-        
-        
-        Examples
-        ========
-        
-        There is an example of using this package in `pyramid_session_multi`
-        [examples/single_file_app.py](https://github.com/jvanasco/pyramid_session_multi/blob/main/examples/single_file_app.py).
-        
-        
-        Further Reading:
-        ================
-        
-        For more information about Redis performance under Python please see an
-        associated project:
-        
-        * https://github.com/jvanasco/dogpile_backend_redis_advanced
-        
-        To suport multiple Sessions under Pyramid
-        
-        * https://github.com/jvanasco/pyramid_session_multi
-        
-        Until Nov 2016 this was maintained as `jvanasco/pyramid_redis_sessions`
-        
-        * The main branch for `jvanasco/pyramid_redis_sessions` was "custom_deployment"
-        * The branched named "main" is the upstream source from ericrasmussen
-        
-        As of Nov 2016, this was forked into it's own project to allow for distribution
-        under PyPi.
-        
-        All support is handled via GitHub : https://github.com/jvanasco/pyramid_session_redis
-        
-        
-        ToDo
-        =====
-        
-        see `TODO.md`
-        
-        
-        Changelog
-        ==========
-        
-        see `CHANGES.md`
-        
-        
-        Support
-        =======
-        
-        You can report bugs or open feature/support requests via GitHub
-        
-        * https://github.com/jvanasco/pyramid_session_redis
-        
-        
-        License
-        =======
-        
-        `pyramid_session_redis` is available under a FreeBSD-derived license. See
-        `LICENSE.txt <https://github.com/jvanasco/pyramid_session_redis/blob/main/LICENSE.txt>`_
-        for details.
-        
-Keywords: pyramid session redis
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Framework :: Pyramid
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: testing
+[![Build Status](https://travis-ci.org/jvanasco/pyramid_session_redis.png)](https://travis-ci.org/jvanasco/pyramid_session_redis)
+
+
+Overview
+========
+
+`pyramid_session_redis` is a mature, stable and actively maintained Server-Side
+Sessions plugin for the Pyramid web framework.
+
+Originally, this library was a fork of
+[`pyramid_redis_sessions`](https://github.com/ericrasmussen/pyramid_redis_sessions), focused on
+improvements and API changes designed for high performance (particularly with
+servers under load), and a slightly different API designed for developer
+convenience.
+
+Compatibility
+-------------
+
+`main` and `1.7` branches require:
+
+* Python 3.6+
+* Pyramid 2.0
+
+
+The `1.6` branch is designed to support both:
+
+* Python 2
+* Python 3
+
+and
+
+* Pyramid 1.x
+* Pyramid 2.0
+
+
+Breaking Changes
+----------------
+
+Starting in `1.7`, the NullSerializer will ensure data is serialized into a string.
+
+
+Prior Branches
+--------------
+
+The 1.6.x branch is in maintenance mode. This is the last branch to support
+Python2 and Pyramid1.
+
+The 1.5.x branch is EOL. No updates are expected, as 1.6 is backwards compatible.
+
+The 1.4.x branch is EOL. It led to the stable 1.5.0 API release.
+
+The 1.2.x branch is EOL as of 1.2.2. Previous plans were to support a final
+1.3.0 release.
+
+Prior Branch Details
+____________________
+
+The 1.2.x branch and earlier are largely a "drop-in-replacement" compatible with
+Eric Rasmussen's `pyramid_redis_sessions` as-is.  If you are migrating from that
+project and do not want to upgrade code, you should pin your install of this
+library to `pyramid_session_redis<=1.3.0` or `pyramid_session_redis<1.3`
+
+**Please be aware that you will be limited to using outdated versions of Pyramid 
+1.x if using the 1.2.x branch.**
+
+Starting with the 1.4.x branch, several design changes were made and this library
+is not a drop-in replacement, **HOWEVER** upgrading will only require minimal
+editing of your code: some editing for migration; some kwargs have changed;
+the structure of the package changed (imports); and advanced users who leverage
+the internal systems may need to upgrade. It should not take more than 5 minutes
+to convert.  The package is still a plug-and-play Pyramid ISessions interface, so
+there are very small changes.
+
+Prior Branch Incompatibilities
+______________________________
+
+IMPORTANT: The internal payload structure changed in the 1.4 branch, and is no
+longer compatible with sessions created under 1.2 - they will be invalid.
+
+PRs that can handle a graceful fallback are welcome.
+
+The 1.2 format guaranteed internal sessions to be in this format:
+
+    {'managed_dict': {},
+     'created': INT,
+     'timeout': INT,
+     }
+
+The 1.4 version streamlines the keys for a lighter footprint and generally
+looks like this:
+
+    {'m': {},  # managed_dict
+     'c': INT,  # created
+     'v': SESSION_API_VERSION,  # api version INT
+     # the following are optional and not guaranteed to be in a session
+     't': INT,  # timeout
+     'x': INT,  # expiry
+     }
+
+Key Takeaways:
+
+* Keys were shortened to 1 letter
+* An API Version is now used, to handle graceful changes in the future
+* The Timeout is no longer guaranteed to be present.
+  The library now supports the entire Timeout to be handled in Redis
+* An "Expiry Timeout" may also exist
+
+Key Concepts
+============================================
+
+
+Timeout vs Expires/MaxAge
+-------------------------
+
+This package allows you to set both *Timeout* and *Expiry* values.  The two
+concepts are closely related, but very different.
+
+A *Timeout* is an internal value and a moving target. It specifies how long a
+Session should last before it times out due to inactivity. The timeout is
+constantly refreshed when the session is accessed.
+
+For example, consider these settings:
+
+    timeout = 1800
+    timeout_trigger = 900
+
+The `timeout` setting is specifying the Session should remain active for 1800
+seconds since it's last activity.  The `timeout_trigger` setting is an
+optimization that defers modifying the Session's timeout on READ operations until
+at least 900 seconds have passed since the last modification. Modifications will
+always occur on WRITE operations.  Depending on your configuration, the timeout
+may be stored in Redis, as part of the Python Payload, or both.
+
+To illustrate how the above settings work, consider a timeline in which a User
+visits a website and then visits it again 2000 seconds later:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit N | 2000s | Session B (new)
+
+When the User makes the last visit, the Session would have timed out, because it
+exceeded the 1800 second mark in the timeout.
+
+Now assume the User makes 3 visits in this timeline, and a second visit happens
+at the 899 mark:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit 2 | 899s  | Session A
+> Visit N | 2000s | Session B (new)
+
+When the User makes the last visit, the Session would still
+have timed out, because the second visit did not meet the timeout_trigger
+threshold.
+
+But, if the second visit happens just 2 seconds later, at the 901 mark, the
+timeout_trigger is reached and the session's timeout will be extended:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit 2 | 901s  | Session A (update timeout trigger)
+> Visit N | 2000s | Session A (update timeout trigger)
+
+When the User makes the last visit, it would still happen within the context of
+the original Session and the timeout will be extended even further.
+
+*Expires* and *Max-Age* are generally values that related to Cookie settings.
+
+*Expires* is created on a Cookie as either a specified Date, or a null value; if
+the value is null (explicit or unspecified), the Cookie will be set as a
+"Session" cookie and only last for the duration of the web browser application
+being open.
+
+*Max-Age* is created on a Cookie as the number of seconds until the Cookie
+expires.  A zero or negative value will expire (delete) the cookie immediately.
+If both Expires and Max-Age are set, Max-Age has precedence.
+
+
+The Confusion?
+--------------
+
+If Redis stores our Timeout info, it stores it in an "expiry" value via `SETEX`
+or similar calls.  
+
+
+Key Differences From pyramid_redis_sessions
+============================================
+
+Depending on your needs, this package is probably more desirable than the
+original project. This package was designed to significantly cut down on the
+communication between Redis and Pyramid. Some options are offered to minimize
+the size of Redis payloads as well.
+
+This package contains additional hooks and features to aid developers who are
+using Redis-based sessions in high-traffic situations.
+
+This package does not recommend any "best deployment" strategies, but supports a
+wide range of strategies to implement the "best deployment" under any given
+circumstance.
+
+Through 1.2.x
+-------------
+
+* The original package communicates with Redis on most attribute accesses and
+  writes within a given request. The traffic can be burdensome in some
+  implementations. `pyramid_session_redis` will queue a single `persist` or
+  `refresh` task per-request using Pyramid's `add_finished_callback` hook.
+* The original version used `EXISTS` to check if a Session existed or not, then
+  proceeded to `GET` or `SET` a new Session.  `pyramid_session_redis` will
+  immediately attempt a `GET`, and will `SET` a new Session on failure.
+  This approach eliminates a call.
+* Separate calls to `SET` and `EXPIRE` were replaced with a single `SETEX`.
+* A flag can be set to enable a LRU Cache (least recently used) mode. No expiry
+  data will be sent to Redis, allowing the Redis server to handle the LRU logic
+  itself.
+* The active Session is decoupled from the `request.session` attributs; this
+  allows for the Session to be set up on alternate attributes and supports
+  integration with
+  [pyramid_session_multi](https://github.com/jvanasco/pyramid_session_multi).
+* The original library does not detect changes in nested dictionaries. This
+  package uses `hashlib.md5` to fingerprint the serialized value on READ; if no
+  changes were detected, a failsafe will `Serialize+md5` the data to decide if a
+  WRITE should occur. This behavior can be disabled by setting `detect_changes`
+  to `False`.
+* The original library raises a fatal error if a Session can not be
+  deserialized. By passing in `deserialized_fails_new` to the constructor,
+  you can create a new Session on deserialization errors.
+* Support for disabling Sessions on CDN generated content via
+  `func_check_response_allow_cookies`
+* Thanks to @ github/hongyuan1306, Token Generation has been consolidated to use
+  Python3's stdlib (or reimplemented if not available). Tokens are also 32,
+  not 20, characters.
+* Redis is supported in a LRU mode (see http://redis.io/topics/lru-cache) by
+  setting the option `set_redis_ttl` to `False` (by default, it is `True`).
+  This will eliminate calls to `EXPIRE` and will use `SET` instead of `SETEX`.
+* In the 1.2.x branch, the created time can be set to an integer via
+  `use_int_time=True`. This will cast the `created` time via
+  `int(math.ceil(time.time()))`. This reduces a payload by several bits.
+
+Other Updates 1.4.x+
+--------------------
+
+* Only `int()` time is supported; Fractional time wastes bytes.
+* Sessions now have version control to support future upgrades via a "version"
+  `v` key.
+* The format of the internal payload was rewritten, the encoded payload now
+  uses 1-letter keys instead of words. This should offset the addition of an
+  expires timestamp and version id.
+* There was no logic for Python timeout control (whoops!) this has been fixed.
+  An "expires" `x` key now tracks the expiration.
+* Added a `timeout_trigger` option.  This will defer expiry data updates to
+  lower usage on Redis.  This is explained below in more detail.
+* In high load situations, Redis can have performance and storage issues because
+  in the original package Session IDs are created on every request (such as a
+  getting spidered by a botnet that does not respect Sessions). In this package,
+  a 'lazycreate' method is used: a session_id/cookie will not be generated
+  unless a session is needed in the callback routine. In order to generate
+  session_id/cookie beforehand, one can use the `RedisSession.ensure_id`
+  function.  To safely check if a session id exists, one can use the
+  `RedisSession.session_id_safecheck` method as well.
+* Added `func_invalid_logger` to the constructor. This can be used to log
+  invalid Sessions. It is incredibly useful when integrated with a statsd
+  system. (see below)
+* Added `set_redis_ttl_readheavy` to the factory and session constructors.
+  This option will optimize Sessions which have Redis-maintained TTLs by
+  executing a GET+EXPIRE together within a pipeline.
+
+
+
+Installation
+============
+
+Install via pypi:
+
+    pip install pyramid_session_redis
+
+
+Configuration
+=============
+
+Configure `pyramid_session_redis` via your Paste config file or however you
+prefer to configure Pyramid. Only `redis.sessions.secret` is required.
+All other settings are optional.
+
+For complete documentation on the `RedisSessionFactory` that uses these
+settings, see :doc:`api`. Otherwise, keep reading for the quick list:
+
+
+    # session settings
+    redis.sessions.secret = your_cookie_signing_secret
+    redis.sessions.timeout = 1200
+
+    # session cookie settings
+    redis.sessions.cookie_name = session
+    redis.sessions.cookie_max_age = max_age_in_seconds
+    redis.sessions.cookie_path = /
+    redis.sessions.cookie_domain =
+    redis.sessions.cookie_secure = False
+    redis.sessions.cookie_httponly = False
+    redis.sessions.cookie_on_exception = True
+
+    # you can supply a redis connection string as a URL
+    redis.sessions.url = redis://username:password@localhost:6379/0
+
+    # or as individual settings (note: the URL gets preference if you do both)
+    redis.sessions.host = localhost
+    redis.sessions.port = 6379
+    redis.sessions.db = 0
+    redis.sessions.password = None
+
+    # additional options can be supplied to redis-py's StrictRedis
+    redis.sessions.socket_timeout =
+    redis.sessions.connection_pool =
+    redis.sessions.charset = utf-8
+    redis.sessions.errors = strict
+    redis.sessions.unix_socket_path =
+
+    # in the advanced section we'll cover how to instantiate your own client
+    redis.sessions.client_callable = my.dotted.python.callable
+
+    # along with defining your own serialize and deserialize methods
+    redis.sessions.serialize = cPickle.dumps
+    redis.sessions.deserialize = cPickle.loads
+
+    # you can specify a prefix to be used with session keys in redis
+    redis.sessions.prefix = mycoolprefix
+
+    # or you can supply your own UID generator callable for session keys
+    redis.sessions.id_generator = niftyuid
+
+
+Initialization
+==============
+
+Lastly, you need to tell Pyramid to use `pyramid_session_redis` as your
+Session factory. The preferred way is adding it with `config.include`,
+like this:
+
+    def main(global_config, **settings):
+        config = Configurator(settings=settings)
+        config.include('pyramid_session_redis')
+
+Alternately, instead of using the Configurator's include method, you can
+activate Pyramid by changing your application's ".ini" file, use the following
+line:
+
+    pyramid.includes = pyramid_session_redis
+
+The above method is recommended because it's simpler, idiomatic, and still fully
+configurable. It even has the added benefit of automatically resolving dotted
+python paths used in the advanced options.
+
+However, you can also explicitly pass a settings dict to the
+`session_factory_from_settings` function. This can be helpful if you configure
+or modify your settings in code:
+
+    from pyramid_session_redis import session_factory_from_settings
+
+    def main(global_config, **settings):
+        config = Configurator(settings=settings)
+        session_factory = session_factory_from_settings(settings)
+        config.set_session_factory(session_factory)
+
+
+Timeout Notes
+=============
+
+If ``set_redis_ttl`` is False, it does not imply there is no timeout at all --
+only that Redis will not be sent timeout data via `SETEX` or `EXPIRE`.
+Timeout data will still be stored in Python.
+
+If Redis is functioning as an LRU Cache, abandoned sessions will never be seen
+by Python, but will eventually be cleared out to make room for new sessions by
+the inherent Redis LRU logic.
+
+Timeout data stored in Python is relatively small when compared to the timeout
+data stored in Redis.
+
+If you want to NEVER have sessions timeout, set the initial `timeout`
+to "0" or "None".
+
+Setting a `timeout_trigger` will require Python to track the expiry.
+
+Enabling `set_redis_ttl_readheavy` requires a `timeout` and `set_redis_ttl`;
+it also requires not enabling `timeout_trigger` or `python_expires`.
+
+
+Timeout Examples
+----------------
+
+Timeout in Python, with Redis TTL via `SETEX`/`EXPIRE`:
+
+    timeout = 60
+
+Timeout in Python, no Redis TTL (only `SET` used)
+
+    timeout = 60
+    assume_redis_ttl = True
+
+No Timeout in Python, no Redis TTL (only `SET` used)
+
+    timeout = 0  # or None
+    assume_redis_ttl = True
+
+
+Warning: Session Locking and Race Conditions
+============================================
+
+This package does not incorporate any sort of locking for session updating or
+handling of race conditions.
+
+This should not be a problem for the vast majority of users, and is a feature
+not present on any known Pyramid Session providers.
+
+For more information, please see:
+
+* https://github.com/jvanasco/pyramid_session_redis/issues/9
+* https://github.com/Pylons/pyramid/issues/3041
+
+
+Feature - Timeout Triggers
+==========================
+
+A timeout trigger can be used to limit the amount of updates/writes.
+It may be more beneficial to your usage pattern.
+
+For the sake of clarity, I'll use an oversimplification that Redis essentially
+has two different internal data stores that are used independently: one for a
+Key's payload and another for the Key's expiry.
+
+In the 'classic' behavior (project this was forked from): every time you access
+an existing session, the GET is followed by sending Redis a new EXPIRE time;
+essentially every "read" has a corresponding "write" for the Redis-tracked
+expiry record.
+
+In order to minimize the writes via SETEX, I introduced the timeout trigger.
+The trigger works by storing some timeout information in the Redis data payload,
+and using that information to determine when to send a write. Instead of having
+a GET+EXPIRE for every read, we only have a single GET and eliminate the write
+caused by the EXPIRE. This has a maintenance cost though - once we hit the
+timeout trigger, instead of just the GET we need to update the internal timeout
+payload and issue a SET.
+
+Going back to your situation: when the user stops activity at 40 minutes in, if
+the timeout trigger is enabled then there has never been an update to the
+internal payload or Redis about the user activity since the session was first
+created. The purpose of the trigger is to defer that "write" operation.
+
+In order to make a session valid for "reading" for around an hour, you should
+do something like:
+
+* a two-hour session with a 10 minute trigger, or
+* a one-hour session with a 50 minute trigger
+
+You can also disable the functionality by setting the trigger to 0. Up to a few
+thousand daily users, you shouldn't have any issues with the overhead of the
+"classic" mode. When you hit 10k users and/or start to have clustered web
+servers communicating with dedicated Redis instances, setting a new EXPIRE after
+every read operation becomes something you want to avoid.
+
+
+Scenario 1 - Classic Redis
+--------------------------
+
+In the typical "classic" Redis usage pattern, the session usage is refreshed via
+an `EXPIRE` call on every session view.
+
+This is useful, but means many session operations will trigger two Redis calls
+(`GET` + `EXPIRE`).  On a high performance system, this can be a lot.
+
+This is a typical scenario with refreshing:
+
+    timeout = 200
+
+The following timeline would occur:
+
+| time | Redis calls    | timeout |
+| ---- | -------------- | ------- |
+| 0    | `GET`+`SETEX`  | 200     |
+| 100  | `GET`+`EXPIRE` | 300     |
+| 200  | `GET`+`EXPIRE` | 400     |
+| 300  | `GET`+`EXPIRE` | 500     |
+| 400  | `GET`+`EXPIRE` | 600     |
+| 500  | `GET`+`EXPIRE` | 700     |
+
+
+Scenario 2 - Timeout Trigger
+--------------------------
+
+The 1.4.x branch introduces a `timeout_trigger` to augment the Session's
+`timeout`.
+
+Whereas a `timeout` states how long a session is good for, a `timeout_trigger`
+defers how long a Session's refresh should be deferred for:
+
+Given the following example, the package will use a 1200s timeout for requests,
+but only trigger an update of the expiry time when the current time is within
+600s of the expiry:
+
+    timeout = 1200
+    timeout_trigger = 600
+
+The following timeline would occur:
+
+| time | Redis calls  | timeout | next threshold |
+| ---- | ------------ | ------- | -------------- |
+| 0    | `GET`+`SET`* | 1200    | 600            |
+| 1    | `GET`        | 1200    | 600            |
+| ...  |              |         |                |
+| 599  | `GET`        | 1200    | 600            |
+| 600  | `GET`+`SET`* | 1800    | 1200           |
+| 601  | `GET`        | 1800    | 1200           |
+| ...  |              |         |                |
+| 1199 | `GET`        | 1800    | 1200           |
+| 1200 | `GET`+`SET`* | 2400    | 1800           |
+
+* This method is compatible with setting a TTL in redis via `SETEX` or doing
+everything within Python if Redis is in a LRU mode
+
+The removes all calls to `EXPIRE` before the threshold is reached, which can be
+ a considerable savings in read-heavy situations.
+
+The caveat to this method: an expiry timestamp must be stored within the payload
+AND updating the timeout requires a `SET` operation.
+
+
+Feature - set_redis_ttl_readheavy
+=================================
+
+This is a new option in `1.4.2` which should improve performance on readheavy
+installations BUT may degrade performance on writeheavy installations.  This
+option will aggregate a GET+EXPIRE on every read.
+
+`set_redis_ttl_readheavy` requires the following:
+
+* a `timeout` value is set
+* `set_redis_ttl` is `True`
+* `timeout_trigger` is NOT set
+* `python_expires` is NOT True
+
+The default behavior of this library during a read-only request is this:
+
+* On session access, query Redis via `redis.GET {session_id}`
+* In a Pyramid callback, update Redis via `redis.EXPIRE {session_id} {expiry}`
+
+During a read-write:
+
+* On session access, query Redis via `redis.GET {session_id}`
+* In a Pyramid callback, update Redis via
+  `redis.SETEX {session_id} {payload} {expiry}`
+
+The new `set_redis_ttl_readheavy` changes this. If enabled during a read-only
+request, the behavior will be lighter on the Redis instance:
+
+* On session access, open a pipeline with two Redis commands:
+  `pipeline.GET {session_id}`,
+  `pipeline.EXPIRE {session_id} {expiry}`.
+* In a Pyramid callback, the duplicate expire is suppressed.
+
+However during a read-write, the activity will be:
+
+* On session access, open a pipeline with two Redis commands:
+  `pipeline.GET {session_id}`,
+  `pipeline.EXPIRE {session_id} {expiry}`.
+* In a Pyramid callback, update Redis via
+  `redis.SETEX {session_id} {payload} {expiry}`
+
+Read-heavy applications should see a slight performance bump via the pipeined
+GET+EXPIRE, however write-heavy applications are likely to see a performance
+degradation as it adds an extra EXPIRE to every request.
+
+
+Invalid Logging
+================
+
+The default behavior of this library is to silently create new session when bad
+session data is encountered, such as a cookie with an invalid id or corrupted
+datastore.  A graceful "new session" is the ideal situation for end-users.
+
+The problem with that strategy is that problems in code or your application
+stack can be hidden, and you might not know about a bad datastore.
+
+The 1.4 release introduces `func_invalid_logger` to the factory constructor.
+This can be used to track the invalid sessions that are safely caught and
+silently upgraded.
+
+How?  The package tracks why a session is invalid with variant classes of
+`pyramid_session_redis.exceptions.InvalidSession`.
+
+Specifically there are the following classes:
+
+* ``InvalidSession(Exception)``
+  Catchall base class
+* ``InvalidSession_NoSessionCookie(InvalidSession)``
+  The Session is invalid because there is no cookie.
+  This is the same as "new session".
+* ``InvalidSession_NotInBackend(InvalidSession)``
+  The Session id was not in the backend.
+* ``InvalidSession_DeserializationError(InvalidSession)``
+    Error deserializing.
+    This is raised if ``deserialized_fails_new`` is True. Otherwise the
+    exception is wrapped in a ``RawDeserializationError`` and raised without
+    being caught.
+* ``InvalidSession_PayloadTimeout(InvalidSession)``
+    The inner Python payload timed out.
+* ``InvalidSession_PayloadLegacy(InvalidSession)``
+    The Session is running on an earlier version.
+
+The factory accepts a `func_invalid_logger` callable argument. The input is the
+raised exception BEFORE a new cookie is generated, and will be the request and
+an instance of `InvalidSession`.
+
+    from pyramid_session_redis.exceptions import *
+    from my_statsd import new_statsd_client()
+
+    statsd_client = new_statsd_client()
+
+    def my_logger(request, raised_exception):
+        """
+        raised_exception will be an instance of InvalidSession
+        log the exception to statsd for metrics
+        """
+        if isinstance(raised_exception, InvalidSession_NoSessionCookie):
+            statsd_client.incr('invalid_session.NoSessionCookie')
+        elif isinstance(raised_exception, InvalidSession_NotInBackend):
+            statsd_client.incr('invalid_session.NotInBackend')
+        elif isinstance(raised_exception, InvalidSession_DeserializationError):
+            statsd_client.incr('invalid_session.DeserializationError')
+
+    factory = RedisSessionFactory(...
+                                  func_invalid_logger=my_logger,
+                                  ...
+                                  )
+
+The `func_invalid_logger` argument may be provided as a dotted-notation string
+in a configuration file.
+
+
+Uncaught Errors
+================
+
+The exception `pyramid_session_redis.exceptions.RawDeserializationError` will be
+raised if deserialization of a payload fails and `deserialized_fails_new` is not
+`True`. The first arg will be the caught exception. This allows for a standard
+error across multiple deserialization options.
+
+
+FAQ:
+=====
+
+Q. What serialization is used?
+------------------------------
+
+A. Serialization is used at two points
+
+* Serializing the Session data.
+  The server-side data serialization is handled by `pickle`. This Session data is
+  created on the server by your application and remains on the server. `pickle`
+  is safe to use in this context, as user-generated payloads can not be introduced
+  to these (de)serialization routines. If you wish to avoid `pickle`, or your
+  prefer to use another encoder, you can easily specify a different (de)serialization
+  routine such as a custom JSON, msgpack or pretty much anything else.
+
+* Serializing the `session_id` to encode into a signed cookie.
+  This library uses `WebOb.cookies.SignedSerializer` to securely manage a HMAC
+  signature of the `session_id` combined with a site-secret. The library allows
+  for a custom replacement to be provided as well.
+  
+  In the original library, the session id and signature were turned into a
+  cookie-safe value via `pickle` (de)serialization - a detail that remained in
+  this library through `<=v1.5.0`. This approach was identified as a security
+  risk, and was removed from this library starting in `v1.5.1`.  
+
+
+Examples
+========
+
+There is an example of using this package in `pyramid_session_multi`
+[examples/single_file_app.py](https://github.com/jvanasco/pyramid_session_multi/blob/main/examples/single_file_app.py).
+
+
+Further Reading:
+================
+
+For more information about Redis performance under Python please see an
+associated project:
+
+* https://github.com/jvanasco/dogpile_backend_redis_advanced
+
+To suport multiple Sessions under Pyramid
+
+* https://github.com/jvanasco/pyramid_session_multi
+
+Until Nov 2016 this was maintained as `jvanasco/pyramid_redis_sessions`
+
+* The main branch for `jvanasco/pyramid_redis_sessions` was "custom_deployment"
+* The branched named "main" is the upstream source from ericrasmussen
+
+As of Nov 2016, this was forked into it's own project to allow for distribution
+under PyPi.
+
+All support is handled via GitHub : https://github.com/jvanasco/pyramid_session_redis
+
+
+ToDo
+=====
+
+see `TODO.md`
+
+
+Changelog
+==========
+
+see `CHANGES.md`
+
+
+Support
+=======
+
+You can report bugs or open feature/support requests via GitHub
+
+* https://github.com/jvanasco/pyramid_session_redis
+
+
+License
+=======
+
+`pyramid_session_redis` is available under a FreeBSD-derived license. See
+`LICENSE.txt <https://github.com/jvanasco/pyramid_session_redis/blob/main/LICENSE.txt>`_
+for details.
```

### Comparing `pyramid_session_redis-1.6.3/README.md` & `pyramid_session_redis-1.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,79 @@
+Metadata-Version: 2.1
+Name: pyramid_session_redis
+Version: 1.7.0rc1
+Summary: High performance and actively maintained server-side session framework for Pyramid and Redis.
+Home-page: https://github.com/jvanasco/pyramid_session_redis
+Author: Jonathan Vanasco
+Author-email: jonathan@findmeon.com
+License: BSD
+Keywords: pyramid session redis
+Classifier: Intended Audience :: Developers
+Classifier: Framework :: Pyramid
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE.txt
+
 [![Build Status](https://travis-ci.org/jvanasco/pyramid_session_redis.png)](https://travis-ci.org/jvanasco/pyramid_session_redis)
 
 
 Overview
 ========
 
 `pyramid_session_redis` is a mature, stable and actively maintained Server-Side
 Sessions plugin for the Pyramid web framework.
 
 Originally, this library was a fork of
-[`pyramid_redis_sessions`](`/ericrasmussen/pyramid_redis_sessions`), focused on
+[`pyramid_redis_sessions`](https://github.com/ericrasmussen/pyramid_redis_sessions), focused on
 improvements and API changes designed for high performance (particularly with
 servers under load), and a slightly different API designed for developer
 convenience.
 
-This package was planning to follow a multi-version release process, however
-that plan was abandoned in favor of ensuring backards compatibility.
+Compatibility
+-------------
+
+`main` and `1.7` branches require:
+
+* Python 3.6+
+* Pyramid 2.0
+
 
-The `main` and `1.6` branches are designed to support both:
+The `1.6` branch is designed to support both:
 
 * Python 2
 * Python 3
 
 and
 
 * Pyramid 1.x
 * Pyramid 2.0
 
 
+Breaking Changes
+----------------
+
+Starting in `1.7`, the NullSerializer will ensure data is serialized into a string.
+
+
 Prior Branches
 --------------
 
-The 1.5.x branch is in maintenance mode. No updates are expected, as 1.6 is
-backwards compatible.
+The 1.6.x branch is in maintenance mode. This is the last branch to support
+Python2 and Pyramid1.
+
+The 1.5.x branch is EOL. No updates are expected, as 1.6 is backwards compatible.
 
 The 1.4.x branch is EOL. It led to the stable 1.5.0 API release.
 
 The 1.2.x branch is EOL as of 1.2.2. Previous plans were to support a final
 1.3.0 release.
 
 Prior Branch Details
@@ -337,15 +375,15 @@
 `session_factory_from_settings` function. This can be helpful if you configure
 or modify your settings in code:
 
     from pyramid_session_redis import session_factory_from_settings
 
     def main(global_config, **settings):
         config = Configurator(settings=settings)
-        session_factory = pyramid_session_redis(settings)
+        session_factory = session_factory_from_settings(settings)
         config.set_session_factory(session_factory)
 
 
 Timeout Notes
 =============
 
 If ``set_redis_ttl`` is False, it does not imply there is no timeout at all --
```

### Comparing `pyramid_session_redis-1.6.3/setup.py` & `pyramid_session_redis-1.7.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
+# ==============================================================================
+
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # manage package version
 # store version in the init.py
 with open(os.path.join(HERE, "src", "pyramid_session_redis", "__init__.py")) as v_file:
     package_version = (
-        re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
+        re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)  # type: ignore[union-attr]
     )
 
 long_description = (
     description
 ) = "High performance and actively maintained server-side session framework for Pyramid and Redis."
 with open(os.path.join(HERE, "README.md")) as f:
     long_description = f.read()
 
 
 # set up requires
 install_requires = [
     "redis>=2.4.11, != 2.9.1",
-    "pyramid>=1.3",
-    "six>=1.12.0",
+    "pyramid>=2",
     "zope.interface",  # in Pyramid
 ]
 testing_requires = [
+    "mypy",
     "nose",
     "pytest",
+    "typing_extensions",  # for 3.8 `Literal`
     "webob",  # in Pyramid
 ]
 testing_extras = install_requires + testing_requires + ["coverage"]
 docs_extras = [
     "sphinx",
 ]
 
@@ -44,32 +47,33 @@
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="pyramid session redis",
     author="Jonathan Vanasco",
     author_email="jonathan@findmeon.com",
     url="https://github.com/jvanasco/pyramid_session_redis",
     license="BSD",
     test_suite="nose.collector",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"pyramid_session_redis": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     entry_points="",
     install_requires=install_requires,
     tests_require=testing_requires,
     extras_require={
         "testing": testing_extras,
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/__init__.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,65 @@
 # -*- coding: utf-8 -*-
 # stdlib
 import functools
-import time
+import pickle
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import Optional
+from typing import Type
+from typing import TYPE_CHECKING
 
 # pypi
-from pyramid.exceptions import ConfigurationError
-
-from redis import VERSION as redis_version  # since at least the 2.x branch
-
-from webob.cookies import SignedSerializer
+from redis import VERSION as _redis_version  # since at least the 2.x branch
+from webob.cookies import SignedSerializer  # type: ignore[import]
 
 # local
-from .compat import pickle
+from . import compat  # noqa: F401 ; trigger compat routines
 from .connection import get_default_connection
-from .exceptions import InvalidSession, InvalidSession_NoSessionCookie
+from .exceptions import InvalidSession
+from .exceptions import InvalidSession_NoSessionCookie
 from .session import RedisSession
-from .util import LAZYCREATE_SESSION
-from .util import NotSpecified
-from .util import _NullSerializer
 from .util import _generate_session_id
+from .util import _NullSerializer
 from .util import _parse_settings
-from .util import configs_bool  # not used here, but included for legacy
+from .util import configs_bool  # noqa: F401 ; included for legacy
 from .util import configs_dotable
 from .util import create_unique_session_id
 from .util import empty_session_payload
+from .util import LazyCreateSession
+from .util import NotSpecified
+from .util import TYPING_COOKIE_EXPIRES
+from .util import TYPING_SESSION_ID
 from .util import warn_future
 
 
-__VERSION__ = "1.6.3"
+__VERSION__ = "1.7.0rc1"
 
 
+# typing
+if TYPE_CHECKING:
+    from pyramid.config import Configurator
+    from pyramid.request import Request
+    from pyramid.response import Response
+    from redis.connection import ConnectionPool
+
+# try to pull out the redis version
+# the official type can have a str, so we need to cast
+# we only ever use the major
+REDIS_VERSION_MAIN: int = 0
+try:
+    REDIS_VERSION_MAIN = int(_redis_version[0])
+except Exception:
+    pass
+
 # ==============================================================================
 
 
-def check_response_allow_cookies(response):
+def check_response_allow_cookies(response: "Response") -> bool:
     """
     reference implementation for ``func_check_response_allow_cookies``
     If view has set any of these response headers, do not add a session
     cookie on this response. This way views generating cacheable content,
     like images, can signal the downstream web server that this content
     is safe. Otherwise if we set a cookie on these responses it could
     result to user session leakage.
@@ -47,15 +69,15 @@
     cookieless_headers = ["expires", "cache-control"]
     for header in cookieless_headers:
         if header in response.headers:
             return False
     return True
 
 
-def includeme(config):
+def includeme(config: "Configurator") -> None:
     """
     This function is detected by Pyramid so that you can easily include
     `pyramid_session_redis` in your `main` method like so::
 
         config.include('pyramid_session_redis')
 
     Parameters:
@@ -70,15 +92,15 @@
         key = "redis.sessions.%s" % option
         if key in settings:
             settings[key] = config.maybe_dotted(settings[key])
     session_factory = session_factory_from_settings(settings)
     config.set_session_factory(session_factory)
 
 
-def session_factory_from_settings(settings):
+def session_factory_from_settings(settings: dict) -> Callable:
     """
     Convenience method to construct a ``RedisSessionFactory`` from Paste config
     settings. Only settings prefixed with "redis.sessions" will be inspected
     and, if needed, coerced to their appropriate types (for example, casting
     the ``timeout`` value as an `int`).
 
     Parameters:
@@ -87,67 +109,67 @@
     A dict of Pyramid application settings
     """
     options = _parse_settings(settings)
     return RedisSessionFactory(**options)
 
 
 def RedisSessionFactory(
-    secret,
-    timeout=1200,
-    cookie_name="session",
-    cookie_max_age=None,
-    cookie_path="/",
-    cookie_domain=None,
-    cookie_secure=False,
-    cookie_httponly=True,
-    cookie_expires=None,
-    cookie_comment=None,
-    cookie_samesite=None,
-    cookie_on_exception=True,
-    url=None,
-    host="localhost",
-    port=6379,
-    db=0,
-    password=None,
-    client_callable=None,
-    serialize=pickle.dumps,
-    deserialize=pickle.loads,
-    id_generator=_generate_session_id,
-    set_redis_ttl=True,
-    set_redis_ttl_readheavy=None,
-    detect_changes=True,
-    deserialized_fails_new=None,
-    func_check_response_allow_cookies=None,
-    func_invalid_logger=None,
-    timeout_trigger=None,
-    python_expires=True,
-    cookie_signer=None,
-    socket_timeout=None,  # redis, deprecated
-    connection_pool=None,  # redis, deprecated
-    charset=None,  # redis, deprecated
-    errors=None,  # redis, deprecated
-    unix_socket_path=None,  # redis, deprecated
-    redis_socket_timeout=None,
-    redis_connection_pool=None,
-    redis_encoding=None,
-    redis_encoding_errors=None,
-    redis_unix_socket_path=None,
-):
+    secret: str,
+    timeout: Optional[int] = 1200,
+    cookie_name: str = "session",
+    cookie_max_age: Optional[int] = None,
+    cookie_path: str = "/",
+    cookie_domain: Optional[str] = None,
+    cookie_secure: bool = False,
+    cookie_httponly: bool = True,
+    cookie_expires: TYPING_COOKIE_EXPIRES = None,  # TYPING_COOKIE_EXPIRES includes None
+    cookie_comment: Optional[str] = None,
+    cookie_samesite: Optional[str] = None,
+    cookie_on_exception: bool = True,
+    url: Optional[str] = None,
+    host: str = "localhost",
+    port: int = 6379,
+    db: int = 0,
+    password: Optional[str] = None,
+    client_callable: Optional[Callable] = None,
+    serialize: Callable = pickle.dumps,
+    deserialize: Callable = pickle.loads,
+    id_generator: Callable = _generate_session_id,
+    set_redis_ttl: bool = True,
+    set_redis_ttl_readheavy: Optional[bool] = None,
+    detect_changes: bool = True,
+    deserialized_fails_new: Optional[bool] = None,
+    func_check_response_allow_cookies: Optional[Callable] = None,
+    func_invalid_logger: Optional[Callable] = None,
+    timeout_trigger: Optional[int] = None,
+    python_expires: bool = True,
+    cookie_signer: Optional[Type] = None,
+    socket_timeout: Optional[int] = None,  # redis, deprecated
+    connection_pool: Optional["ConnectionPool"] = None,  # redis, deprecated
+    charset: Optional[str] = None,  # redis, deprecated
+    errors: Optional[str] = None,  # redis, deprecated
+    unix_socket_path: Optional[str] = None,  # redis, deprecated
+    redis_socket_timeout: Optional[int] = None,
+    redis_connection_pool: Optional["ConnectionPool"] = None,
+    redis_encoding: Optional[str] = None,
+    redis_encoding_errors: Optional[str] = None,
+    redis_unix_socket_path: Optional[str] = None,
+) -> Callable:
     """
     Constructs and returns a session factory that will provide session data
     from a Redis server. The returned factory can be supplied as the
     ``session_factory`` argument of a :class:`pyramid.config.Configurator`
     constructor, or used as the ``session_factory`` argument of the
     :meth:`pyramid.config.Configurator.set_session_factory` method.
 
     Parameters:
 
     ``secret``
-    A string which is used to sign the cookie.  As an alternate, you can set this
-    to ``None`` and provide a ``cookie_signer`` argument.
+    A string which is used to sign the cookie.  As an alternate, you can set
+    this to ``None`` and provide a ``cookie_signer`` argument.
 
     ``timeout``
     A number of seconds of inactivity before a session times out.
     If set to 0 or None, no timeout will occur or be managed in Redis or Python.
 
     ``cookie_name``
     The name of the cookie used for sessioning. Default: ``session``.
@@ -181,14 +203,15 @@
     The 'httpOnly' flag of the session cookie.
     This is passed on to the underlying ``WebOb.response.Response.set_cookie``
     framework as ``httponly``.
 
     ``cookie_expires``
     Default: ``None``.
     Passed to `WebOb.response.Response.set_cookie` as ``expires``.
+    This is a ``datetime.datetime``, ``datetime.timedelta``, or ``None``.
     BEWARE: WebOb may be removing this in 1.9.
 
     ``cookie_comment``
     Default: ``None``.
     The 'comment' attribute of the session cookie.
     This is paseed on to the underlying ``WebOb.response.Response.set_cookie``
     framework as ``comment``.
@@ -196,15 +219,15 @@
 
     ``cookie_samesite``
     Default: ``None``.
     The 'SameSite' attribute of the session cookie.
     This is paseed on to the underlying ``WebOb.response.Response.set_cookie``
     framework as ``samesite`` and **requires WebOb 1.8.0 or higher**.
     If set to ``None`` or not specified, it will not be passed on.
-    Should only be ``"Strict"`` or ``"Lax"``.
+    Should only be ``"strict"``, ``"lax"`` or ``"none"``.
 
     ``cookie_on_exception``
     Boolean value; Default: ``True``.
     If ``True``, set a session cookie even if an exception occurs
     while rendering a view.
 
     ``url``
@@ -231,44 +254,46 @@
 
     ``client_callable``
     Default: ``None``.
     A python callable that accepts a Pyramid `request` and Redis config options
     and returns a Redis client such as redis-py's `StrictRedis`.
 
     ``serialize``
-    Default: ``pickle.dumps``. PY2=cPickle
+    Default: ``pickle.dumps``
     A function to serialize the session dict for storage in Redis.
 
     ``deserialize``
-    Default: ``pickle.loads``. PY2=cPickle
+    Default: ``pickle.loads``.
     A function to deserialize the stored session data in Redis.
 
     ``id_generator``
     Default: private function that uses sha1 with the time and random elements
     to create a 40 character unique ID.
     A function to create a unique ID to be used as the session key when a
     session is first created.
+    As of `v1.7`, ``id_generator`` MUST return a str.
 
     ``set_redis_ttl``
     Boolean value;  Default `True`.
     If set to ``True``, will set a TTL. If
     ``False`` will not set a TTL and assumes that Redis is configured as a
     least-recently-used cache [http://redis.io/topics/lru-cache] and will NOT
     send EXPIRY data of sessions to Redis (the value of `timeout` will be
     ignored if set). This does not require or imply that no ``timeout`` data is
     handled within the Python payload, it just determines if Redis will be
     involved with timeout logic.
 
     ``set_redis_ttl_readheavy``
      Boolean value; Default: ``None``.
      If ``True``, sets TTL data in Redis within
-     a PIPELINE via GET+EXPIRE and supresses automatic TTL refresh during the deferred
-     cleanup phase. If not ``True``, an EXPIRE is sent as a separate action during
-     the deferred cleanup phase.  The optimized behavior improves performance on
-     read-heavy operations, but may degrade performance on write-heavy operations.
+     a PIPELINE via GET+EXPIRE and supresses automatic TTL refresh during the
+     deferred cleanup phase. If not ``True``, an EXPIRE is sent as a separate
+     action during the deferred cleanup phase.  The optimized behavior improves
+     performance on read-heavy operations, but may degrade performance on
+     write-heavy operations.
      This requires a ``timeout`` and ``set_redis_ttl`` to be True; it is not
      compatible with ``timeout_trigger`` or ``python_expires``.
 
     ``detect_changes``
     Boolean value; Default: ``True``.
     If set to ``True``, will calculate nested changes after
     serialization to ensure persistence of nested data.
@@ -302,15 +327,15 @@
     ``python_expires``
     Boolean value; Default ``True``.
     If ``True``, allows for timeout logic to be
     tracked in Python.
 
     ``cookie_signer``
     Default: ``None``
-    If specified,  ``secret`` must be ``None``.
+    If specified,  ``secret`` MUST be ``None``.
     An object with two methods, ``loads`` and ``dumps``.
     The ``loads`` method should accept bytes and return a Python object.
     The ``dumps`` method should accept a Python object and return bytes.
     A ``ValueError`` should be raised for malformed inputs.
 
     ``redis_socket_timeout``
     Default: ``None``.
@@ -389,16 +414,16 @@
         redis_connection_pool  | connection_pool
         redis_encoding         | charset
         redis_encoding_errors  | errors
         redis_unix_socket_path | unix_socket_path
 
     Users are encouraged to use the modern `redis_` namespace and not the
     deprecated legacy kwargs. Warnings will be emitted when deprecated kwargs
-    are used. Submitting two equivalent kwargs will result in a ValueError being
-    raised.
+    are used. Submitting two equivalent kwargs will result in a ValueError
+    being raised.
     """
     if timeout == 0:
         timeout = None
 
     if timeout_trigger and not python_expires:  # fix this
         python_expires = True
 
@@ -406,26 +431,27 @@
     if set_redis_ttl_readheavy:
         if (not timeout) or (not set_redis_ttl):
             raise ValueError(
                 "`set_redis_ttl_readheavy` requires a `timeout` and `set_redis_ttl`"
             )
         if timeout_trigger or python_expires:
             raise ValueError(
-                "`set_redis_ttl_readheavy` is not compatible with `timeout_trigger` and `python_expires`"
+                "`set_redis_ttl_readheavy` is not compatible with"
+                "`timeout_trigger` and `python_expires`"
             )
-    optimize_redis_ttl = False
+    # optimize_redis_ttl = False
 
     _set_redis_ttl_onexit = False
     if (timeout and set_redis_ttl) and (
         not timeout_trigger and not python_expires and not set_redis_ttl_readheavy
     ):
         _set_redis_ttl_onexit = True
 
     # good for all factory() requests
-    set_cookie_kwargs = {
+    set_cookie_kwargs: Dict[str, Any] = {
         "max_age": cookie_max_age,
         "path": cookie_path,
         "domain": cookie_domain,
         "secure": cookie_secure,
         "httponly": cookie_httponly,
     }
     if cookie_comment is not None:
@@ -442,15 +468,16 @@
         )
         if redis_socket_timeout:
             raise ValueError(
                 "Submit only one of `redis_socket_timeout`, `socket_timeout`"
             )
     if connection_pool is not None:
         warn_future(
-            "`connection_pool` has been deprecated in favor of `redis_connection_pool`"
+            "`connection_pool` has been deprecated in favor of"
+            "`redis_connection_pool`"
         )
         if redis_connection_pool:
             raise ValueError(
                 "Submit only one of `redis_connection_pool`, `connection_pool`"
             )
     if charset is not None:
         warn_future("`charset` has been deprecated in favor of `redis_encoding`")
@@ -475,15 +502,16 @@
             "`redis_encoding_errors` instead of `errors`, which will passed to "
             "Redis as the `encoding_errors` kwarg."
         )
         if redis_encoding_errors:
             raise ValueError("Submit only one of `redis_encoding_errors`, `errors`")
     if unix_socket_path is not None:
         warn_future(
-            "`unix_socket_path` has been deprecated in favor of `redis_unix_socket_path`"
+            "`unix_socket_path` has been deprecated in favor of"
+            "`redis_unix_socket_path`"
         )
         if redis_unix_socket_path:
             raise ValueError(
                 "Submit only one of `redis_unix_socket_path`, `unix_socket_path`"
             )
 
     # favor the new terms to the old.
@@ -512,63 +540,74 @@
     )
 
     # accept newer encoding and encoding_errors args while
     # retaining backwards compatibility
     if redis_encoding is not None:
         redis_options["encoding"] = redis_encoding
     else:
-        if redis_version[0] < 4:
+        if REDIS_VERSION_MAIN < 4:
             # legacy kwarg still supported; will trigger Redis warnings/errors
             redis_options["charset"] = "utf-8" if charset is None else charset
         else:
             # modern deprecation
             if charset is not None:
                 redis_options["encoding"] = charset
     if redis_encoding_errors is not None:
         redis_options["encoding_errors"] = redis_encoding_errors
     else:
-        if redis_version[0] < 4:
+        if REDIS_VERSION_MAIN < 4:
             # legacy kwarg still supported; will trigger Redis warnings/errors
             redis_options["errors"] = "strict" if errors is None else errors
         else:
             # modern deprecation
             if errors is not None:
                 redis_options["encoding_errors"] = errors
 
     # good for all factory() requests
     new_payload_func = functools.partial(
-        empty_session_payload, timeout=timeout, python_expires=python_expires
+        empty_session_payload,
+        timeout=timeout,
+        python_expires=python_expires,
     )
 
     # good for all factory() requests
     delete_cookie_func = functools.partial(
         _delete_cookie,
         cookie_name=cookie_name,
         cookie_path=cookie_path,
         cookie_domain=cookie_domain,
     )
 
     _secret_cookiesigner = (secret, cookie_signer)
+    _cookie_signer: Type
     if all(_secret_cookiesigner) or not any(_secret_cookiesigner):
         raise ValueError(
             "One, and only one, of `secret` and `cookie_signer` must be provided."
         )
     if secret is not None:
-        # the second argument is the salt. customizing this would needlessly complicate integration
-        cookie_signer = SignedSerializer(
-            secret, "pyramid_session_redis.", "sha512", serializer=_NullSerializer()
+        # the second argument is the salt.
+        # customizing this would needlessly complicate integration
+        _cookie_signer = SignedSerializer(
+            secret,
+            "pyramid_session_redis.",
+            "sha512",
+            serializer=_NullSerializer(),  # convert to a string
         )
+    else:
+        _cookie_signer = cookie_signer
 
-    def factory(request, new_session_id_func=create_unique_session_id):
-
+    def factory(
+        request: "Request",
+        new_session_id_func: Callable = create_unique_session_id,
+    ):
         # an explicit client callable gets priority over the default
         redis_conn = (
             client_callable(request, **redis_options)
             if client_callable is not None
-            else get_default_connection(request, url=url, **redis_options)
+            else get_default_connection(request, url=url, **redis_options)  # type: ignore[arg-type]
         )
 
         new_session_func = functools.partial(
             new_session_id_func,
             redis=redis_conn,
             timeout=timeout,
             serialize=serialize,
@@ -576,18 +615,21 @@
             set_redis_ttl=set_redis_ttl,
             # set_redis_ttl_readheavy=set_redis_ttl_readheavy,  # not needed on NEW
             # _set_redis_ttl_onexit=_set_redis_ttl_onexit,  # not needed on NEW
             new_payload_func=new_payload_func,
             python_expires=python_expires,
         )
 
+        session_id: TYPING_SESSION_ID
         try:
             # attempt to retrieve a session_id from the cookie
             session_id = _get_session_id_from_cookie(
-                request=request, cookie_name=cookie_name, cookie_signer=cookie_signer
+                request=request,
+                cookie_name=cookie_name,
+                cookie_signer=_cookie_signer,
             )
             if not session_id:
                 raise InvalidSession_NoSessionCookie("No `session_id` in cookie.")
             session_cookie_was_valid = True
             session = RedisSession(
                 redis=redis_conn,
                 session_id=session_id,
@@ -605,15 +647,15 @@
                 timeout=timeout,
                 python_expires=python_expires,
             )
         except InvalidSession as e:
             if func_invalid_logger is not None:
                 # send the instance for logging
                 func_invalid_logger(request, e)
-            session_id = LAZYCREATE_SESSION
+            session_id = LazyCreateSession
             session_cookie_was_valid = False
             session = RedisSession(
                 redis=redis_conn,
                 session_id=session_id,
                 new=True,
                 new_session=new_session_func,
                 new_payload_func=new_payload_func,
@@ -627,17 +669,17 @@
                 timeout=timeout,
                 python_expires=python_expires,
             )
 
         set_cookie_func = functools.partial(
             _set_cookie,
             session,
-            cookie_signer=cookie_signer,
+            cookie_signer=_cookie_signer,
             cookie_name=cookie_name,
-            **set_cookie_kwargs
+            **set_cookie_kwargs,
         )
         cookie_callback = functools.partial(
             _cookie_callback,
             session,
             session_cookie_was_valid=session_cookie_was_valid,
             cookie_on_exception=cookie_on_exception,
             set_cookie_func=set_cookie_func,
@@ -647,15 +689,19 @@
         request.add_response_callback(cookie_callback)
         request.add_finished_callback(session._deferred_callback)
         return session
 
     return factory
 
 
-def _get_session_id_from_cookie(request, cookie_name, cookie_signer):
+def _get_session_id_from_cookie(
+    request: "Request",
+    cookie_name: str,
+    cookie_signer: Type,  # has `.loads`, `.dumps`; MUST return a str
+):
     """
     Attempts to retrieve and return a session ID from a session cookie in the
     current request. Returns None if the cookie isn't found or the value cannot
     be deserialized for any reason.
     """
     cookieval = request.cookies.get(cookie_name)
     if cookieval is not None:
@@ -664,36 +710,48 @@
             return session_id
         except ValueError:
             pass
 
     return None
 
 
-def _set_cookie(session, request, response, cookie_signer, cookie_name, **kwargs):
+def _set_cookie(
+    session,
+    request: "Request",
+    response: "Response",
+    cookie_signer: Type,  # has `.loads`, `.dumps`; MUST return a str
+    cookie_name: str,
+    **kwargs,
+):
     """
     `session` is via functools.partial
     `request` and `response` are appended by add_response_callback
     """
     cookieval = cookie_signer.dumps(session.session_id)
     response.set_cookie(cookie_name, cookieval, **kwargs)
 
 
-def _delete_cookie(response, cookie_name, cookie_path, cookie_domain):
+def _delete_cookie(
+    response: "Response",
+    cookie_name: str,
+    cookie_path: str,
+    cookie_domain: str,
+):
     response.delete_cookie(cookie_name, path=cookie_path, domain=cookie_domain)
 
 
 def _cookie_callback(
     session,
-    request,
-    response,
+    request: "Request",
+    response: "Response",
     session_cookie_was_valid,
     cookie_on_exception,
-    set_cookie_func,
-    delete_cookie_func,
-    func_check_response_allow_cookies,
+    set_cookie_func: Callable,
+    delete_cookie_func: Callable,
+    func_check_response_allow_cookies: Optional[Callable],
 ):
     """
     Response callback to set the appropriate Set-Cookie header.
     `session` is via functools.partial
     `request` and `response` are appended by add_response_callback
     """
     # `session._session_state` will not exist after `invalidate` and other methods
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/connection.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,42 +39,53 @@
     redis.sessions.client_callable = my_cool_app.my_redis_client_getter
 
 
 This option is available so that developers can define their own Redis
 instances as needed, but most users should not need to customize how they
 connect.
 """
+# stdlib
+from typing import Optional
+from typing import Type
+from typing import TYPE_CHECKING
 
+# pypi
 from redis import StrictRedis
 
+# typing
+if TYPE_CHECKING:
+    from pyrarmid.request import Request
 
 # ==============================================================================
 
 
 def get_default_connection(
-    request, url=None, redis_client=StrictRedis, **redis_options
-):
+    request: "Request",
+    url: Optional[str] = None,
+    client_class: Type[StrictRedis] = StrictRedis,
+    **redis_options,
+) -> StrictRedis:
     """
     Default Redis connection handler. Once a connection is established it is
     saved in `request.registry`.
 
     :param request: The current Pyramid ``Request`` object.
     :param url: string. An optional connection string that will be passed
         directly to `StrictRedis.from_url`. The connection string should be in
         the form `redis://username:password@localhost:6379/0`
     :param settings: dict. A dict of keyword args to be passed directly
         to `StrictRedis`.
     :returns: An instance of `StrictRedis`
     """
     # attempt to get an existing connection from the registry
-    redis = getattr(request.registry, "_redis_sessions", None)
+    client = getattr(request.registry, "_redis_sessions", None)
 
     # if we found an active connection, return it
-    if redis is not None:
-        return redis
+    if client is not None:
+        return client
 
     # otherwise create a new connection
     if url is not None:
         # remove defaults to avoid duplicating settings in the `url`
         redis_options.pop("password", None)
         redis_options.pop("host", None)
         redis_options.pop("port", None)
@@ -83,15 +94,15 @@
         # argument. instead, sockets should be encoded in the URL if
         # used. example:
         #     unix://[:password]@/path/to/socket.sock?db=0
         redis_options.pop("unix_socket_path", None)
         # connection pools are also no longer a valid option for
         # loading via URL
         redis_options.pop("connection_pool", None)
-        redis = redis_client.from_url(url, **redis_options)
+        redis = client_class.from_url(url, **redis_options)
     else:
-        redis = redis_client(**redis_options)
+        redis = client_class(**redis_options)
 
     # save the new connection in the registry
     setattr(request.registry, "_redis_sessions", redis)
 
     return redis
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/conf.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"pyramid_session_redis"
-copyright = u"2016-2019, Jonathan Vanasco"
+project = "pyramid_session_redis"
+copyright = "2016-2019, Jonathan Vanasco"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = package_version
@@ -172,31 +172,31 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "pyramid_session_redisdoc"
 
 
 # -- Options for LaTeX output -------------------------------------------------
 
-latex_elements = {
+latex_elements: dict = {
     # The paper size ('letterpaper' or 'a4paper').
     #'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     #'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
     #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual])
 latex_documents = [
     (
         "index",
         "pyramid_session_redis.tex",
-        u"pyramid\\_session\\_redis Documentation",
-        u"Jonathan Vanasco",
+        "pyramid\\_session\\_redis Documentation",
+        "Jonathan Vanasco",
         "manual",
     )
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
@@ -222,16 +222,16 @@
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         "index",
         "pyramid_session_redis",
-        u"pyramid_session_redis Documentation",
-        [u"Jonathan Vanasco"],
+        "pyramid_session_redis Documentation",
+        ["Jonathan Vanasco"],
         1,
     )
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
@@ -241,19 +241,19 @@
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         "index",
         "pyramid_session_redis",
-        u"pyramid_session_redis Documentation",
-        u"Jonathan Vanasco",
+        "pyramid_session_redis Documentation",
+        "Jonathan Vanasco",
         "pyramid_session_redis",
-        u"Fast pyramid sessions with redis.",
-        u"Miscellaneous",
+        "Fast pyramid sessions with redis.",
+        "Miscellaneous",
     )
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/index.rst` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/make.bat` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/docs/Makefile` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/exceptions.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     pass
 
 
 class InvalidSession_Lazycreate(InvalidSession):
     """
     The session is expected to lazycreate.
     This SHOULD NOT be accessed outside of the package.
-    If you encounter this, please file a bug report with details of the situation.
+    If you encounter this, please file a bug report with details of
+    the situation.
     """
 
     pass
 
 
 class InvalidSession_NotInBackend(InvalidSession):
     """
@@ -34,15 +35,16 @@
 
     pass
 
 
 class InvalidSession_DeserializationError(InvalidSession):
     """
     The session did not deserialize correctly.
-    This is only raised/caught/silently handled if `deserialized_fails_new` is True
+    This is only raised/caught/silently handled if `deserialized_fails_new`
+    is True
     This is supported by the func_invalid_logger factory callable
     """
 
     pass
 
 
 class InvalidSession_PayloadTimeout(InvalidSession):
@@ -68,7 +70,19 @@
     Core class for deserialization errors.
     The `message` is the caught exception.
     This allows deserializers to switch with keeping a consistent interface.
     This is only raised if `deserialized_fails_new` is not True
     """
 
     pass
+
+
+class InvalidSessionId_Deserialization(Exception):
+    """Base class for Serialization Issues"""
+
+    pass
+
+
+class InvalidSessionId_Serialization(Exception):
+    """Base class for Serialization Issues"""
+
+    pass
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/legacy.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/legacy.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,195 +9,251 @@
 PLEASE DO NOT USE ME.
 PLEASE DO NOT USE ME.
 
 The functions in this namespace are provided for migrating sessions only.
 
 The legacy system has security issues.
 
-The following functions are taken from Pyramid and appear under their licensing.
+The following functions are taken from Pyramid and appear
+under their licensing.
 
 * `pyramid.session.signed_serialize`
 * `pyramid.sessionsigned_deserialize`
 
 See LICENSE.TXT for more details
 """
 # stdlib
 import base64
 import binascii
 import hashlib
 import hmac
+import pickle
+from types import ModuleType
+from typing import Any
+from typing import AnyStr
+from typing import Optional
+from typing import Type
 
 # pypi
 from pyramid.util import strings_differ
 from webob.cookies import SignedSerializer
 
-
 # local
-from .compat import bytes_
-from .compat import native_
-from .compat import pickle
 from .util import _NullSerializer
 
-
 # ==============================================================================
 
 
-def signed_serialize(data, secret):
+# originally in _compat
+def bytes_(
+    s: str,
+    encoding: str = "latin-1",
+    errors: str = "strict",
+) -> bytes:
+    return _ensure_binary(s, encoding, errors)
+
+
+# lifted from six
+def _ensure_binary(
+    s: str,
+    encoding: str = "utf-8",
+    errors: str = "strict",
+) -> bytes:
+    """Coerce **s** to six.binary_type.
+
+    For Python 2:
+      - `unicode` -> encoded to `str`
+      - `str` -> `str`
+
+    For Python 3:
+      - `str` -> encoded to `bytes`
+      - `bytes` -> `bytes`
+    """
+    if isinstance(s, bytes):
+        return s
+    if isinstance(s, str):
+        return s.encode(encoding, errors)
+    raise TypeError("not expecting type '%s'" % type(s))
+
+
+# - - -
+
+
+def _fallback_conversion(
+    secret: AnyStr,
+) -> bytes:
+    _secret: bytes
+    if isinstance(secret, str):
+        _secret = bytes_(secret, "utf-8")
+    else:
+        _secret = secret
+    return _secret
+
+
+def signed_serialize(
+    data: Any,
+    secret: AnyStr,
+) -> str:
     """Serialize any pickleable structure (``data``) and sign it
     using the ``secret`` (must be a string).  Return the
     serialization, which includes the signature as its first 40 bytes.
     The ``signed_deserialize`` method will deserialize such a value.
     This function is useful for creating signed cookies.  For example:
     .. code-block:: python
        cookieval = signed_serialize({'a':1}, 'secret')
        response.set_cookie('signed_cookie', cookieval)
     :param data: data to serialize
     :param secret: secret for signing
     :returns signature: a signed string, compatible with `signed_deserialize`
     """
-    pickled = pickle.dumps(data, pickle.HIGHEST_PROTOCOL)
-    try:
-        # bw-compat with pyramid <= 1.5b1 where latin1 is the default
-        secret = bytes_(secret)
-    except UnicodeEncodeError:
-        secret = bytes_(secret, "utf-8")
-    sig = hmac.new(secret, pickled, hashlib.sha1).hexdigest()
-    return sig + native_(base64.b64encode(pickled))
+    _pickled: bytes = pickle.dumps(data, pickle.HIGHEST_PROTOCOL)
+    _secret: bytes = _fallback_conversion(secret)
+    sig: str = hmac.new(_secret, _pickled, hashlib.sha1).hexdigest()
+    return sig + base64.b64encode(_pickled).decode()
 
 
-def signed_deserialize(serialized, secret, hmac=hmac):
+def signed_deserialize(
+    serialized: str,
+    secret: AnyStr,
+    hmac: ModuleType = hmac,
+) -> Any:
     """Deserialize the value returned from ``signed_serialize``.  If
     the value cannot be deserialized for any reason, a
     :exc:`ValueError` exception will be raised.
     This function is useful for deserializing a signed cookie value
     created by ``signed_serialize``.  For example:
     .. code-block:: python
        cookieval = request.cookies['signed_cookie']
        data = signed_deserialize(cookieval, 'secret')
     :param serialized: a serialized string
     :param secret: secret for signing
     :returns data: the input which was serialized via `signed_serialize`
     """
     # hmac parameterized only for unit tests
     try:
-        input_sig, pickled = (
-            bytes_(serialized[:40]),
-            base64.b64decode(bytes_(serialized[40:])),
-        )
+        input_sig: bytes = bytes_(serialized[:40])
+        pickled: bytes = base64.b64decode(bytes_(serialized[40:]))
     except (binascii.Error, TypeError) as e:
         # Badly formed data can make base64 die
         raise ValueError("Badly formed base64 data: %s" % e)
-
-    try:
-        # bw-compat with pyramid <= 1.5b1 where latin1 is the default
-        secret = bytes_(secret)
-    except UnicodeEncodeError:
-        secret = bytes_(secret, "utf-8")
-    sig = bytes_(hmac.new(secret, pickled, hashlib.sha1).hexdigest())
+    _secret: bytes = _fallback_conversion(secret)
+    sig: bytes = bytes_(hmac.new(_secret, pickled, hashlib.sha1).hexdigest())
 
     # Avoid timing attacks (see
     # http://seb.dbzteam.org/crypto/python-oauth-timing-hmac.pdf)
     if strings_differ(sig, input_sig):
         raise ValueError("Invalid signature")
 
     return pickle.loads(pickled)
 
 
 # ==============================================================================
 
 
 class LegacyCookieSerializer(object):
-    secret = None
+    secret: bytes
 
-    def __init__(self, secret):
+    def __init__(self, secret: AnyStr):
         """
         :param secret: The secret for this serializer
         """
-        self.secret = secret
+        _secret: bytes = _fallback_conversion(secret)
+        self.secret = _secret
 
-    def loads(self, data):
+    def loads(self, data: str) -> Any:
         """
         :param data: data to be deserialized
         """
         return signed_deserialize(data, self.secret)
 
-    def dumps(self, data):
+    def dumps(self, data: Any) -> str:
         """
         :param data: data to be serialized
         """
         return signed_serialize(data, self.secret)
 
 
 class GracefulCookieSerializer(object):
     """
     `GracefulCookieSerializer` is designed to help developers migrate sessions
     across Pyramid/pyramid_session_redis versions by catching deserialization
     failures due to a change in how cookies are signed/checked.
 
     This class will:
-        * attempt to deserialize with new format, and fallback to the legacy if that fails
-        * serialize into the new format
-
-    By providing a `logging_hook` (see tests for example usage), a developer can profile
-    their app to understand how the migration of users is progressing.
+      * attempt to deserialize with new format, and fallback to the legacy
+        if that fails
+      * serialize into the new format
+
+    By providing a `logging_hook` (see tests for example usage), a developer
+    can profile their app to understand how the migration of users is
+    progressing.
 
     !!!!! IMPORTANT !!!!!
 
-    Using this or any pickle-based serializer is not recommended, as it can lead to
-    a code exploit during deserialization. This is only provided as a temporary migration tool.
+    Using this or any pickle-based serializer is not recommended, as it can
+    lead to a code exploit during deserialization. This is only provided as
+    a temporary migration tool.
     """
 
-    secret = None
-    serializer_current = None
-    serializer_legacy = None
-    logging_hook = None
-
-    def __init__(self, secret, logging_hook=None):
+    secret: bytes
+    serializer_current: SignedSerializer  # has .dumps/.loads
+    serializer_legacy: LegacyCookieSerializer  # has .dumps/.loads
+    logging_hook: Optional[Type]  # has .attempt, .success
+
+    def __init__(
+        self,
+        secret: AnyStr,
+        logging_hook: Optional[Type] = None,
+    ):
         """
         :param secret: string. the secret
         :param logging_hook: callable; default None.
 
         `logging_hook` is a callable that supports at least two methods
             * `LoggingHook.attempt("current")`
             * `LoggingHook.success("current")`
         Each method will be invoked with a string, which will have one of 3
         possible values:
             "global" (only attempt), a global attempt was made
             "current" - attempt/success for the current serializer
             "legacy" - attempt/success for the legacy serializer
         """
-        self.secret = secret
+        _secret: bytes = _fallback_conversion(secret)
+        self.secret = _secret
         self.serializer_current = SignedSerializer(
-            secret, "pyramid_session_redis.", "sha512", serializer=_NullSerializer()
+            secret,
+            "pyramid_session_redis.",
+            "sha512",
+            serializer=_NullSerializer(),
         )
-        self.serializer_legacy = LegacyCookieSerializer(secret)
+        self.serializer_legacy = LegacyCookieSerializer(_secret)
         self.logging_hook = logging_hook
 
-    def loads(self, data):
+    def loads(self, data: str) -> Any:
         """
         :param data: data to be deserialized
         """
-        if self.logging_hook:
+        if self.logging_hook is not None:
             _hook = self.logging_hook
             _hook.attempt("global")
             try:
                 _hook.attempt("current")
                 val = self.serializer_current.loads(data)
                 _hook.success("current")
                 return val
-            except:
+            except Exception as exc:  # noqa: F841
                 _hook.attempt("legacy")
                 val = self.serializer_legacy.loads(data)
                 _hook.success("legacy")
                 return val
 
         # no hooks configured
         try:
             return self.serializer_current.loads(data)
-        except:
+        except Exception as exc:  # noqa: F841
             return self.serializer_legacy.loads(data)
 
-    def dumps(self, data):
+    def dumps(self, data: Any) -> str:
         """
         :param data: data to be serialized
         """
         return self.serializer_current.dumps(data)
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/session.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,118 @@
 # -*- coding: utf-8 -*-
 
 # stdlib
 import hashlib
+import pickle
+from secrets import token_hex
+from typing import Any
+from typing import Callable
+from typing import Iterator
+from typing import Optional
+from typing import Tuple
+from typing import TYPE_CHECKING
+from typing import Union
 
 # pypi
 from pyramid.decorator import reify
-from pyramid.exceptions import ConfigurationError
 from pyramid.interfaces import ISession
 from zope.interface import implementer
 
 # local
-from .compat import pickle
-from .compat import to_unicode
-from .compat import token_hex
-from .exceptions import InvalidSession
 from .exceptions import InvalidSession_DeserializationError
 from .exceptions import InvalidSession_Lazycreate
 from .exceptions import InvalidSession_NotInBackend
 from .exceptions import InvalidSession_PayloadLegacy
 from .exceptions import InvalidSession_PayloadTimeout
 from .exceptions import RawDeserializationError
-from .util import LAZYCREATE_SESSION
-from .util import NotSpecified
-from .util import SESSION_API_VERSION
 from .util import decode_session_payload as decode_session_payload_func
 from .util import empty_session_payload
 from .util import encode_session_payload as encode_session_payload_func
 from .util import int_time
+from .util import LazyCreateSession
+from .util import NotSpecified
 from .util import persist
 from .util import recookie
 from .util import refresh
+from .util import SESSION_API_VERSION
+from .util import TYPING_COOKIE_EXPIRES
+from .util import TYPING_COOKIE_EXPIRES__A
+from .util import TYPING_COOKIE_MAX_AGE__A
+from .util import TYPING_KEY
+from .util import TYPING_SESSION_ID
+
 
+# typing
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal  # type: ignore[assignment]
+if TYPE_CHECKING:
+    from pyramid.request import Request
 
 # ==============================================================================
 
 
-def hashed_value(serialized):
+def hashed_value(serialized: bytes) -> str:
     """
     quick hash of serialized data
     only used for comparison
 
     :param serialized: string. serialized data to hash.
     :returns hash: string.
     """
     return hashlib.md5(serialized).hexdigest()
 
 
 class _SessionState(object):
     # markers for update
-    please_persist = None
-    please_recookie = None
-    please_refresh = None
+    please_persist: Optional[bool] = None
+    please_recookie: Optional[bool] = None
+    please_refresh: Optional[bool] = None
 
     # these markers are consulted in cleanup routines
-    dont_persist = None
-    dont_refresh = None
+    dont_persist: Optional[bool] = None
+    dont_refresh: Optional[bool] = None
 
     # optional attributes, not set by default
-    cookie_expires = NotSpecified
-    cookie_max_age = NotSpecified
+    cookie_expires: TYPING_COOKIE_EXPIRES__A = (
+        NotSpecified  # TYPING_COOKIE_EXPIRES__A includes None
+    )
+    cookie_max_age: TYPING_COOKIE_MAX_AGE__A = (
+        NotSpecified  # TYPING_COOKIE_MAX_AGE__A includes None
+    )
 
     def __init__(
         self,
-        session_id,
-        managed_dict,
-        created,
-        timeout,
-        expires,
-        version,
-        new,
-        persisted_hash,
+        session_id: TYPING_SESSION_ID,
+        managed_dict: dict,
+        created: int,
+        timeout: int,
+        expires: int,
+        version: int,
+        new: bool,
+        persisted_hash: Optional[str],
     ):
         """
         all these args are guaranteed to be submitted for the object;
         no need to create default object attributes
         """
         self.session_id = session_id
         self.managed_dict = managed_dict
         self.created = created
         self.timeout = timeout
         self.expires = expires
         self.version = version
         self.new = new
         self.persisted_hash = persisted_hash
 
-    def should_persist(self, session):
+    def should_persist(
+        self,
+        session: "RedisSession",
+    ) -> Union[Literal[False], bytes]:
         """
         this is a backup routine
         compares the persisted hash with a hash of the current value
         returns `False` or `serialized_session`
 
         :param session:
         :returns serialized_session:
@@ -143,16 +167,16 @@
 
     ``new_session``
     A function that takes no arguments. It should insert a new session into
     Redis under a new session_id, and return that session_id.
 
     ``new_session_payload``
     UNDER DEVELOPMENT
-    A function that takes no arguments.  It is used to to generate a new session
-    payload without creating the id (as new_session might)
+    A function that takes no arguments.  It is used to to generate a new
+    session payload without creating the id (as new_session might)
 
     ``serialize``
     A function to serialize pickleable Python objects. Default:
     ``cPickle.dumps``.
 
     ``deserialize``
     The dual of ``serialize``, to convert serialized strings back to Python
@@ -203,52 +227,55 @@
     ``timeout_trigger`` will enable this.
 
     """
 
     def __init__(
         self,
         redis,
-        session_id,  # could be ``LAZYCREATE_SESSION``
-        new,
-        new_session,
-        new_payload_func=None,
-        serialize=pickle.dumps,
-        deserialize=pickle.loads,
-        set_redis_ttl=True,
-        detect_changes=True,
-        deserialized_fails_new=None,
-        encode_session_payload_func=None,
-        decode_session_payload_func=None,
-        timeout=None,
-        timeout_trigger=None,
-        python_expires=None,
-        set_redis_ttl_readheavy=None,
-        _set_redis_ttl_onexit=None,
+        session_id: TYPING_SESSION_ID,
+        new: bool,
+        new_session: Callable,
+        new_payload_func: Optional[Callable] = None,
+        serialize: Callable = pickle.dumps,  # dict->bytes
+        deserialize: Callable = pickle.loads,  # bytes->dict
+        set_redis_ttl: bool = True,
+        detect_changes: bool = True,
+        deserialized_fails_new: Optional[bool] = None,
+        encode_session_payload_func: Optional[Callable] = None,
+        decode_session_payload_func: Optional[Callable] = None,
+        timeout: Optional[int] = None,
+        timeout_trigger: Optional[int] = None,
+        python_expires: Optional[bool] = None,
+        set_redis_ttl_readheavy: Optional[bool] = None,
+        _set_redis_ttl_onexit: Optional[bool] = None,
     ):
         if timeout_trigger and not python_expires:  # fix this
             python_expires = True
         self.redis = redis
-        self.serialize = serialize
-        self.deserialize = deserialize
-        self.new_session = new_session
+        self.serialize = serialize  # type: ignore[method-assign]
+        self.deserialize = deserialize  # type: ignore[method-assign]
+        self.new_session = new_session  # type: ignore[method-assign]
         if new_payload_func is not None:
-            self.new_payload = new_payload_func
+            self.new_payload = new_payload_func  # type: ignore[method-assign]
         if encode_session_payload_func is not None:
-            self.encode_session_payload = encode_session_payload_func
+            self.encode_session_payload = encode_session_payload_func  # type: ignore[method-assign]
         if decode_session_payload_func is not None:
-            self.decode_session_payload = decode_session_payload_func
+            self.decode_session_payload = decode_session_payload_func  # type: ignore[method-assign]
         self._set_redis_ttl = set_redis_ttl
         self._set_redis_ttl_readheavy = set_redis_ttl_readheavy
         self._detect_changes = detect_changes
         self._deserialized_fails_new = deserialized_fails_new
         self._timeout = timeout
         self._timeout_trigger = timeout_trigger
         self._python_expires = python_expires
         self._new = new
-        self._session_state = self._make_session_state(session_id=session_id, new=new)
+        self._session_state = self._make_session_state(
+            session_id=session_id,
+            new=new,
+        )
         if _set_redis_ttl_onexit:
             self._session_state.please_refresh = True
 
     def _resync(self):
         """resyncs the session. this is really only needed for testing."""
         self._session_state = self._make_session_state(
             session_id=self.session_id, new=self._new
@@ -265,63 +292,71 @@
     def encode_session_payload(self, *args, **kwargs):
         """
         used to recode for serialization
         this can be overridden via __init__
         """
         return encode_session_payload_func(*args, **kwargs)
 
-    def decode_session_payload(self, payload):
+    def decode_session_payload(self, payload: dict) -> dict:
         """
         used to recode for serialization
         this can be overridden via __init__
 
         :param payload:
+        :type payload: dict
         :returns decoded payload:
         """
         return decode_session_payload_func(payload)
 
-    def serialize(self):
+    def serialize(self, data: dict) -> bytes:
         # this should be set via __init__
         raise NotImplementedError()
 
-    def deserialize(self):
+    def deserialize(self, serialized: bytes) -> dict:
         # this should be set via __init__
         raise NotImplementedError()
 
     @reify
-    def _session_state(self):
+    def _session_state(self) -> _SessionState:
         """this should only be executed after an `invalidate()`
-        The `invalidate()` will "del self._session_state", which will remove the
-        '_session_state' entry from the object dict (as created by __init__ or by
-        this function which reify's the return value). Removing that function
-        allows this method to execute, and `reify` puts the new result in the
-        object's dict.
-        """
-        return self._make_session_state(session_id=LAZYCREATE_SESSION, new=True)
+        The `invalidate()` will "del self._session_state", which will remove
+        the '_session_state' entry from the object dict (as created by __init__
+        or by this function which reify's the return value). Removing that
+        function allows this method to execute, and `reify` puts the new result
+        in the object's dict.
+        """
+        return self._make_session_state(
+            session_id=LazyCreateSession,
+            new=True,
+        )
 
     @reify
-    def timestamp(self):
+    def timestamp(self) -> int:
         return int_time()
 
-    def _make_session_state(self, session_id, new):
+    def _make_session_state(
+        self,
+        session_id: TYPING_SESSION_ID,
+        new: bool,
+    ) -> _SessionState:
         """
         This will try to load the session_id in Redis via ``from_redis``.
         If this fails, it will raise ``InvalidSession`` variants
 
         :param session_id:
         :param new:
         :returns `_SessionState``:
         """
-        if session_id == LAZYCREATE_SESSION:
+        if session_id is LazyCreateSession:
             persisted_hash = None
             persisted = self.new_payload()
         else:
-            # self.from_redis needs to take a session_id here, because otherwise it
-            # would look up self.session_id, which is not ready yet as
-            # session_state has not been created yet.
+            # self.from_redis needs to take a session_id here, because
+            # otherwise it would look up self.session_id, which is not ready
+            # yet as session_state has not been created yet.
             (persisted, persisted_hash) = self.from_redis(
                 session_id=session_id,
                 persisted_hash=(True if self._detect_changes else False),
             )
             expires = persisted.get("x")
             if expires:
                 if self.timestamp > expires:
@@ -341,42 +376,42 @@
             expires=persisted.get("x"),  # expires
             version=persisted.get("v"),  # session api version
             new=new,
             persisted_hash=persisted_hash,
         )
 
     @property
-    def session_id(self):
+    def session_id(self) -> str:
         return self._session_state.session_id
 
     @property
-    def managed_dict(self):
+    def managed_dict(self) -> dict:
         return self._session_state.managed_dict
 
     @property
-    def created(self):
+    def created(self) -> int:
         return self._session_state.created
 
     @property
-    def timeout(self):
+    def timeout(self) -> int:
         return self._session_state.timeout
 
     @property
-    def expires(self):
+    def expires(self) -> int:
         return self._session_state.expires
 
     @property
-    def version(self):
+    def version(self) -> int:
         return self._session_state.version
 
     @property
-    def new(self):
+    def new(self) -> bool:
         return self._session_state.new
 
-    def to_redis(self):
+    def to_redis(self) -> bytes:
         """Serialize a dict of the data that needs to be persisted for this
         session, for storage in Redis.
 
         Primarily used by the ``@persist`` decorator to save the current
         session state to Redis.
         """
         data = self.encode_session_payload(
@@ -385,100 +420,117 @@
             self.timeout,
             self.expires,
             timeout_trigger=self._timeout_trigger,
             python_expires=self._python_expires,
         )
         return self.serialize(data)
 
-    def from_redis(self, session_id=None, persisted_hash=None):
+    def from_redis(
+        self,
+        session_id: Optional[TYPING_SESSION_ID] = None,
+        persisted_hash: Optional[bool] = None,
+    ) -> Union[dict, Tuple[dict, Union[str, None]]]:
         """
         Get and deserialize the persisted data for this session from Redis.
         If ``persisted_hash`` is ``None`` (default), returns a single
         variable `deserialized`.
         If set to ``True`` or ``False``, returns a tuple.
         """
         _session_id = session_id or self.session_id
-        if _session_id == LAZYCREATE_SESSION:
-            raise InvalidSession_Lazycreate("`session_id` is LAZYCREATE_SESSION")
+        if _session_id is LazyCreateSession:
+            raise InvalidSession_Lazycreate(  # noaq: E501
+                "`session_id` is LazyCreateSession"
+            )
 
         # optimize a `TTL refresh` under certain conditions
         persisted = None
         if self._set_redis_ttl_readheavy:
             with self.redis.pipeline() as pipe:
                 persisted = pipe.get(_session_id)
-                _updated = pipe.expire(_session_id, self._timeout)
+                _updated = pipe.expire(  # noqa: F841
+                    _session_id,
+                    self._timeout,
+                )
             # mark that we shouldn't refresh
             self._session_state.dont_refresh = True
         else:
             persisted = self.redis.get(_session_id)
 
         if persisted is None:
             raise InvalidSession_NotInBackend(
                 "`session_id` (%s) not in Redis" % _session_id
             )
         try:
             deserialized = self.deserialize(persisted)
         except Exception as e:
             if self._deserialized_fails_new:
                 raise InvalidSession_DeserializationError(
-                    "`session_id` (%s) did not deserialize correctly" % _session_id
+                    "`session_id` (%s) did not deserialize correctly"
+                    % _session_id  # noaq: E501
                 )
             raise RawDeserializationError(e)
+        # TODO: typing on return can be better?
         if persisted_hash is True:
+            # -> tuple[dict, str]
             return (deserialized, hashed_value(persisted))
         elif persisted_hash is False:
+            # -> tuple[dict, None]
             return (deserialized, None)
+        # -> dict
         return deserialized
 
-    def invalidate(self):
+    def invalidate(self) -> None:
         """Invalidate the session."""
-        if self.session_id != LAZYCREATE_SESSION:
+        if self.session_id != LazyCreateSession:
             self.redis.delete(self.session_id)
         # Delete the self._session_state attribute so that direct access to or
         # indirect access via other methods and properties to .session_id,
         # .managed_dict, .created, .timeout and .new (i.e. anything stored in
         # self._session_state) after this will trigger the creation of a new
         # session with a new session_id via the `_session_state()` reified
         # property.
         del self._session_state
 
-    def ensure_id(self):
+    def ensure_id(self) -> str:
         # this ensures we have a session_id
-        if self._session_state.session_id == LAZYCREATE_SESSION:
+        if self._session_state.session_id is LazyCreateSession:
             self._session_state.session_id = self.new_session()
         return self._session_state.session_id
 
     @property
-    def session_id_safecheck(self):
+    def session_id_safecheck(self) -> Optional[str]:
         """if we don't have a managed_dict, return None"""
         if not self.managed_dict:
             return None
         return self.ensure_id()
 
-    def do_persist(self, serialized_session=None):
+    def do_persist(self, serialized_session=None) -> None:
         """
         Actually and immediately persist to Redis backend
-        Only set a timeout in Redis timeout if we have timeouts AND are not in LRU mode
+        Only set a timeout in Redis timeout if we have timeouts AND are not
+        in LRU mode.
         Note: this package uses StrictRedis(`key, timeout, value`)
               not Redis(`key, value, timeout`)
         """
         self.ensure_id()
         if serialized_session is None:
             serialized_session = self.to_redis()
         serverside_timeout = (
-            True if ((self.timeout is not None) and (self._set_redis_ttl)) else False
+            True
+            if ((self.timeout is not None) and (self._set_redis_ttl))
+            else False  # noaq: E501
         )
         if serverside_timeout:
             self.redis.setex(self.session_id, self.timeout, serialized_session)
         else:
             self.redis.set(self.session_id, serialized_session)
         self._session_state.please_persist = False
         self._session_state.dont_refresh = True
 
-    def do_refresh(self, force_redis_ttl=None):
+    def do_refresh(self, force_redis_ttl=None) -> None:
         """
         Actually and immediately refresh the TTL to Redis backend.
         Does nothing if no timeout set (in LRU mode).
         Optional kwarg for developers ``force_redis_ttl`` (default None)
         can be provided to force a new Redis TTL.
         """
         if force_redis_ttl is not None:
@@ -488,180 +540,197 @@
                 if self._set_redis_ttl:
                     # set a TTL if unless we're in LRU mode
                     self.redis.expire(self.session_id, self.timeout)
         self._session_state.please_refresh = False
 
     # dict modifying methods decorated with @persist
     @persist
-    def __delitem__(self, key):
+    def __delitem__(self, key: TYPING_KEY) -> None:
         del self.managed_dict[key]
 
     @persist
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: TYPING_KEY, value: Any) -> None:
         self.managed_dict[key] = value
 
     @persist
-    def setdefault(self, key, default=None):
+    def setdefault(self, key: TYPING_KEY, default: Optional[Any] = None):
+        # TODO: typing
+        # this should always return `None`, but mypy doesn't like that
+        # unless this should somehow not return `None`
         return self.managed_dict.setdefault(key, default)
 
     @persist
-    def clear(self):
+    def clear(self) -> None:
         return self.managed_dict.clear()
 
     @persist
-    def pop(self, key, default=None):
+    def pop(self, key: TYPING_KEY, default: Optional[Any] = None) -> Any:
         return self.managed_dict.pop(key, default)
 
     @persist
-    def update(self, other):
+    def update(self, other) -> None:
+        # TODO: typing
         return self.managed_dict.update(other)
 
     @persist
-    def popitem(self):
+    def popitem(self) -> tuple:
+        # TODO: Deprecate? I can't imagine a usecase for this
         return self.managed_dict.popitem()
 
     # dict read-only methods decorated with @refresh
     @refresh
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return self.managed_dict[key]
 
     @refresh
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> bool:
         return key in self.managed_dict
 
     @refresh
     def keys(self):
+        # TODO: typing
         return self.managed_dict.keys()
 
     @refresh
     def items(self):
+        # TODO: typing
         return self.managed_dict.items()
 
     @refresh
-    def get(self, key, default=None):
+    def get(self, key: TYPING_KEY, default: Optional[Any] = None):
         return self.managed_dict.get(key, default)
 
     @refresh
-    def __iter__(self):
+    def __iter__(self) -> Iterator:
         return self.managed_dict.__iter__()
 
     @refresh
-    def has_key(self, key):
+    def has_key(self, key: TYPING_KEY) -> bool:
         return key in self.managed_dict
 
     @refresh
     def values(self):
+        # TODO: typing
         return self.managed_dict.values()
 
     @refresh
     def itervalues(self):
+        # TODO: typing
         try:
             values = self.managed_dict.itervalues()
-        except AttributeError:  # pragma: no cover
+        except AttributeError:
             values = self.managed_dict.values()
         return values
 
     @refresh
     def iteritems(self):
+        # TODO: typing
         try:
             items = self.managed_dict.iteritems()
-        except AttributeError:  # pragma: no cover
+        except AttributeError:
             items = self.managed_dict.items()
         return items
 
     @refresh
     def iterkeys(self):
+        # TODO: typing
         try:
             keys = self.managed_dict.iterkeys()
-        except AttributeError:  # pragma: no cover
+        except AttributeError:
             keys = self.managed_dict.keys()
         return keys
 
     @persist
-    def changed(self):
+    def changed(self) -> None:
         """Persist all the data that needs to be persisted for this session
         immediately with ``@persist``.
         """
         pass
 
     # session methods persist or refresh using above dict methods
-    def new_csrf_token(self):
+    def new_csrf_token(self) -> str:
         token = token_hex(32)
         self["_csrft_"] = token
         return token
 
-    def get_csrf_token(self):
+    def get_csrf_token(self) -> str:
         token = self.get("_csrft_", None)
         if token is None:
             token = self.new_csrf_token()
-        else:
-            token = to_unicode(token)
         return token
 
-    def flash(self, msg, queue="", allow_duplicate=True):
+    def flash(
+        self,
+        msg: str,
+        queue: str = "",
+        allow_duplicate: bool = True,
+    ) -> None:
         storage = self.setdefault("_f_" + queue, [])
         if allow_duplicate or (msg not in storage):
             storage.append(msg)
             self.changed()  # notify Redis of change to ``storage`` mutable
 
-    def peek_flash(self, queue=""):
+    def peek_flash(self, queue: str = ""):
         storage = self.get("_f_" + queue, [])
         return storage
 
-    def pop_flash(self, queue=""):
+    def pop_flash(self, queue: str = ""):
         storage = self.pop("_f_" + queue, [])
         return storage
 
     # RedisSession extra methods
 
     @recookie
-    def adjust_cookie_expires(self, expires):
+    def adjust_cookie_expires(self, expires: TYPING_COOKIE_EXPIRES) -> None:
         """
         Adjust the `expires` value on the cookie.
         The underlying functionality may be removed in WebOb 1.9.
 
         This method ONLY affects the SetCookie Headers.
         This method does not affect the session logic or any values.
 
-        A datetime.timedelta object representing an amount of time, datetime.datetime or None.
+        A datetime.timedelta object representing an amount of time,
+        datetime.datetime or None.
 
         Expires and Max-Age have a somewhat convoluted relationship;
         Max-Age always takes precedence. You should be using Max-Age instead
         """
         self._session_state.cookie_expires = expires
 
     @recookie
-    def adjust_cookie_max_age(self, max_age):
+    def adjust_cookie_max_age(self, max_age: int) -> None:
         """
         Permanently adjusts the max-age for this cookie to ``max_age``
         This value is used as the Max-Age of the generated cookie
 
         This method ONLY affects the SetCookie Headers.
         This method does not affect the session logic or any values.
 
-        An integer representing a number of seconds, datetime.timedelta, or None.
+        An integer representing a number of seconds, datetime.timedelta,
+        or None.
 
         Expires and Max-Age have a somewhat convoluted relationship;
         Max-Age always takes precedence. You should be using Max-Age.
         """
         self._session_state.cookie_max_age = max_age
 
     @persist
-    def adjust_session_expires(self, expires_epoch):
+    def adjust_session_expires(self, expires_epoch: int) -> None:
         """
         Updates the epoch used for Python timeout on expiry logic.
         """
         self._session_state.expires = expires_epoch
 
     @persist
-    def adjust_session_timeout(self, timeout_seconds):
+    def adjust_session_timeout(self, timeout_seconds: int) -> None:
         """
-        Permanently adjusts the `timeout` for this Session to ``timeout_seconds``
-        for as long as this Session is active. Useful in situations where you
-        want to change the expiry time for a Session dynamically.
+        Permanently adjusts the `timeout` for this Session to
+        ``timeout_seconds`` for as long as this Session is active.
+        Useful in situations where you want to change the expiry time for
+        a Session dynamically.
         """
         self._session_state.timeout = timeout_seconds
 
     # rename these
     adjust_expires_for_session = adjust_session_expires
     adjust_timeout_for_session = adjust_session_timeout
 
@@ -670,28 +739,29 @@
         """
         Boolean property indicating whether the session is in the state where
         it has been invalidated but a new session has not been created in its
         place.
         """
         return "_session_state" not in self.__dict__
 
-    def _deferred_callback(self, request):
+    def _deferred_callback(self, request: "Request"):
         """
         Finished callback to persist the data if needed.
         `request` is appended by pyramid's `add_finished_callback` which should
         invkoe this.
         """
         if "_session_state" not in self.__dict__:
-            # _session_state is a reified property, which is saved into the dict
-            # if we call `session.invalidate()` the session is immediately deleted
-            # however, accessing it here will trigger a new _session_state creation
-            # and insert a placeholder for the session_id into Redis.  this would be
-            # ok in certain situations, however since we don't access any actual
-            # data in the session, it won't have the cookie callback triggered --
-            # which means the cookie will never get sent to the user, and a phantom
+            # _session_state is a reified property, which is saved into the
+            # dict if we call `session.invalidate()` the session is immediately
+            # deleted however, accessing it here will trigger a new
+            # _session_state creation and insert a placeholder for the
+            # session_id into Redis.  this would be ok in certain situations,
+            # however since we don't access any actual data in the session,
+            # it won't have the cookie callback triggered -- which means the
+            # cookie will never get sent to the user, and a phantom
             # session_id+placeholder will be in Redis until it times out.
             return
         if not self._session_state.dont_persist:
             if self._session_state.please_persist:
                 self.do_persist()
                 self._session_state.please_refresh = False
             else:
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis/util.py` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 # -*- coding: utf-8 -*-
 
 # stdlib
-import warnings
+import datetime
+from enum import Enum
 from functools import partial
 from math import ceil
+from secrets import token_urlsafe
 from time import time as time_time
+import typing
+from typing import Callable
+from typing import Optional
+from typing import Type
+from typing import TYPE_CHECKING
+from typing import Union
+import warnings
 
 # pypi
 from pyramid.exceptions import ConfigurationError
 from pyramid.settings import asbool
 from redis.exceptions import WatchError
 
 # local
-from .compat import PY2
-from .compat import PY3
-from .compat import token_urlsafe
-from .compat import webob_bytes_
-from .compat import webob_text_
+from .exceptions import InvalidSessionId_Deserialization
+from .exceptions import InvalidSessionId_Serialization
 
+if TYPE_CHECKING:
+    from .session import RedisSession
 
 # ==============================================================================
 
 
+# we use an Enum for typing support
+
+
 # create a custom class+object instance for handling lazycreated ids
 # (this is what dogpile cache's NO_VALUE does)
-class LazyCreateSession(object):
+class LazyCreateSession(Enum):
     pass
 
 
-LAZYCREATE_SESSION = LazyCreateSession()
-
-
 # used to differentiate from `None`
-class NotSpecified(object):
+class NotSpecified(Enum):
     pass
 
 
 # this stored in the sessions. it is used to detect api version mismatches
-SESSION_API_VERSION = 1
+SESSION_API_VERSION: int = 1
+
+
+TYPING_COOKIE_EXPIRES = Union[datetime.timedelta, datetime.datetime, None, NotSpecified]
+TYPING_KEY = Union[str, int]
+TYPING_SESSION_ID = Union[str, Type[LazyCreateSession]]
+
+# for ASSIGNMENT we need a `Type[NotSpecified]`
+TYPING_COOKIE_EXPIRES__A = Union[
+    datetime.timedelta, datetime.datetime, None, Type[NotSpecified]
+]
+TYPING_COOKIE_MAX_AGE__A = Union[int, None, Type[NotSpecified]]
 
 
 # ------------------------------------------------------------------------------
 
 
-def warn_future(message):
+def warn_future(message: str) -> None:
     warnings.warn(message, FutureWarning, stacklevel=2)
 
 
-def to_binary(value, enc="UTF-8"):  # pragma: no cover
-    if PY3 and isinstance(value, str):
-        value = value.encode(enc)
-    return value
+def is_integer(n: typing.Any) -> bool:
+    try:
+        r = float(n)
+        return r.is_integer()
+    except ValueError:
+        return False
 
 
-def to_unicode(value):  # pragma: no cover
-    if PY2:
-        value = unicode(value)
+def to_binary(value: typing.AnyStr, enc: str = "UTF-8") -> bytes:
+    if isinstance(value, str):
+        return value.encode(enc)
     return value
 
 
-def _generate_session_id():
+def _generate_session_id() -> str:
     """
     Produces a base64 encoded, urlsafe random string with 48-byte
     cryptographically strong randomness as the session id. See
 
         http://security.stackexchange.com/questions/24850/
         choosing-a-session-id-algorithm-for-a-client-server-relationship
 
@@ -73,16 +94,16 @@
     supply your own function in your ini file with:
 
         redis.sessions.id_generator = my_random_id_generator
 
     This uses 48 bytes instead of 32 to maintain backwards
     compatibility to pyramid_redis_sessions.  The earlier packaged used
     a 64character digest; however 48bits using the new method will
-    encode to a 64 character url-safe string, while 32 bits will only be encoded
-    to a 40 character string.
+    encode to a 64 character url-safe string, while 32 bits will only be
+    encoded to a 40 character string.
     """
     return token_urlsafe(48)
 
 
 # ---------------------
 
 # `_parse_settings` and `includeme` may need to coerce strings into other types
@@ -114,30 +135,33 @@
 
 configs_int_none = ("timeout", "timeout_trigger")
 
 
 # ---------------------
 
 
-def prefixed_id(prefix="session:"):
+def prefixed_id(prefix: str = "session:") -> str:
     """
     :param prefix: string. the prefix
     Adds a prefix to the unique session id, for cases where you want to
     visually distinguish keys in redis.
     """
-    session_id = _generate_session_id()
-    prefixed_id = prefix + session_id
+    session_id: str = _generate_session_id()
+    prefixed_id: str = prefix + session_id
     return prefixed_id
 
 
-def int_time():
+def int_time() -> int:
     return int(ceil(time_time()))
 
 
-def empty_session_payload(timeout=0, python_expires=None):
+def empty_session_payload(
+    timeout: int = 0,
+    python_expires: Optional[bool] = None,
+) -> dict:
     """
     creates an empty session payload
 
     :param timeout: int. default 0.
     :param python_expires: bool. default None.
     """
     _created = int_time()
@@ -150,16 +174,21 @@
         data["t"] = timeout  # timeout
         if python_expires:
             data["x"] = _created + timeout
     return data
 
 
 def encode_session_payload(
-    managed_dict, created, timeout, expires, timeout_trigger=None, python_expires=None
-):
+    managed_dict: dict,
+    created: int,
+    timeout: int,
+    expires: int,
+    timeout_trigger: Optional[int] = None,
+    python_expires: Optional[bool] = None,
+) -> dict:
     """
     called by a session to recode for storage;
     inverse of ``decode_session_payload``
 
     :param managed_dict: internal dict for encoding.
     :param created: int. time created.
     :param timeout: int. seconds.
@@ -179,15 +208,15 @@
         if python_expires:
             time_now = int_time()
             if not timeout_trigger or (time_now >= (expires - timeout_trigger)):
                 data["x"] = time_now + timeout  # expires
     return data
 
 
-def decode_session_payload(payload):
+def decode_session_payload(payload: dict) -> dict:
     """
     decode a serialized session payload to kwargs
     inverse of ``encode_session_payload``
 
     :param payload: dict with encoding compatible with `encode_session_payload`
     :returns payload: dict with legacy/readble format.
     """
@@ -198,29 +227,32 @@
         "timeout": payload.get("t"),
         "expires": payload.get("x"),
     }
 
 
 def _insert_session_id_if_unique(
     redis,
-    timeout,
-    session_id,
-    serialize,
-    set_redis_ttl,
-    data_payload=None,
-    new_payload_func=None,
-    python_expires=None,
-):
+    timeout: int,
+    session_id: str,
+    serialize: Callable,
+    set_redis_ttl: bool,
+    data_payload: Optional[dict] = None,
+    new_payload_func: Optional[Callable] = None,
+    python_expires: Optional[bool] = None,
+) -> Optional[str]:
     """
     Attempt to insert a given ``session_id`` and return the successful id
     or ``None``.  ``timeout`` could be 0/None, in that case do-not track
     the timeout data
 
     This will create an empty/null session and redis entry for the id.
 
+    The return value will be the input `session_id` upon success, or `None` upon
+    a failure.
+
     ``data_payload`` = payload to use
     ``new_payload_func`` = specify a fallback function to generate a payload
     if both are ``None``, then `empty_session_payload`
 
     :param redis: redis connection
     :param timeout: int seconds. used to initialize empty session.
     :param session_id: string.
@@ -231,15 +263,18 @@
     :param python_expires: bool. default None.
     :returns session_id: string.
     """
     if data_payload is None:
         if new_payload_func is not None:
             data_payload = new_payload_func()
         else:
-            data_payload = empty_session_payload(timeout, python_expires=python_expires)
+            data_payload = empty_session_payload(
+                timeout,
+                python_expires=python_expires,
+            )
     _payload = serialize(data_payload)
     with redis.pipeline() as pipe:
         try:
             # start pipeline with a watch
             pipe.watch(session_id)
             # after `watch` the pipline is in immediate execution mode
             value = pipe.get(session_id)
@@ -257,52 +292,53 @@
             return session_id
         except WatchError:
             return None
 
 
 def create_unique_session_id(
     redis,
-    timeout,
-    serialize,
-    generator=_generate_session_id,
-    set_redis_ttl=True,
-    data_payload=None,
-    new_payload_func=None,
-    python_expires=None,
-):
+    timeout: int,
+    serialize: Callable,
+    generator: Callable = _generate_session_id,
+    set_redis_ttl: bool = True,
+    data_payload: Optional[dict] = None,
+    new_payload_func: Optional[Callable] = None,
+    python_expires: Optional[bool] = None,
+) -> str:
     """
     Returns a unique session id after inserting it successfully in Redis.
 
     :param redis: redis connection
     :param timeout: int seconds. used to initialize empty session.
     :param serialize: callable. used to serialize an empty session.
     :param generator: callable. used to generate an id.
     :param set_redis_ttl:  bool
     :param data_payload: dict. default None. initialize session with this payload.
     :param new_payload_func: callable. default None. create a new payload with this.
     :param python_expires: bool. default None.
     :returns:
     """
     while 1:
-        session_id = generator()
+        session_id: str = generator()
+        # attempt will be the session_id
         attempt = _insert_session_id_if_unique(
             redis,
             timeout,
             session_id,
             serialize,
             set_redis_ttl,
             data_payload=data_payload,
             new_payload_func=new_payload_func,
             python_expires=python_expires,
         )
         if attempt is not None:
             return attempt
 
 
-def _parse_settings(settings):
+def _parse_settings(settings: dict) -> dict:
     """
     Convenience function to collect settings prefixed by 'redis.sessions' and
     coerce settings to ``int``, ``float``, and ``bool`` as needed.
 
     :param settings: dict
     """
     keys = [s for s in settings if s.startswith("redis.sessions.")]
@@ -353,74 +389,93 @@
     if "prefix" in options:
         prefix = options.pop("prefix")
         options["id_generator"] = partial(prefixed_id, prefix=prefix)
 
     return options
 
 
-def persist(wrapped):
+def persist(wrapped: Callable) -> Callable:
     """
     Decorator to persist in Redis all the data that needs to be persisted for
     this session and reset the expire time.
     This will mark the `_session_state.please_persist` as True, to be
     handled in a callback.
     To immediately persist a session, call `session.do_persist`.
 
     :param wrapped: a function to wrap with this decorator.
     :returns wrapped_refresh: a wrapped function.
     """
 
-    def wrapped_persist(session, *arg, **kw):
+    def wrapped_persist(session: "RedisSession", *arg, **kw):
         result = wrapped(session, *arg, **kw)
         session._session_state.please_persist = True
         return result
 
     return wrapped_persist
 
 
-def recookie(wrapped):
+def recookie(wrapped: Callable) -> Callable:
     """
     Decorator to mark a session as needing to recookie.
     This is necessary when setting a new max-age/etc
 
     :param wrapped: a function to wrap with this decorator.
     :returns wrapped_recookie: a wrapped function.
     """
 
-    def wrapped_recookie(session, *arg, **kw):
+    def wrapped_recookie(session: "RedisSession", *arg, **kw):
         result = wrapped(session, *arg, **kw)
         session._session_state.please_recookie = True
         return result
 
     return wrapped_recookie
 
 
-def refresh(wrapped):
+def refresh(wrapped: Callable) -> Callable:
     """
     Decorator to reset the expire time for this session's key in Redis.
     This will mark the `_session_state.please_refresh` as True, to be
     handled in a callback.
     To immediately persist a session, call `session.do_refresh`.
 
     :param wrapped: a function to wrap with this decorator.
     :returns wrapped_refresh: a wrapped function.
     """
 
-    def wrapped_refresh(session, *arg, **kw):
+    def wrapped_refresh(session: "RedisSession", *arg, **kw):
         result = wrapped(session, *arg, **kw)
         session._session_state.please_refresh = True
         return result
 
     return wrapped_refresh
 
 
 class _NullSerializer(object):
     """
-    A fake serializer for compatibility with ``webob.cookies.SignedSerializer``.
-    Our usage is only signing the session_id, which is a string.
+    A cheap serializer for compatibility with ``webob.cookies.SignedSerializer``.
+    Our usage is only for encoding a signed session_id.
+
+    By default, webob uses json loads/dumps.  As this library only uses strings
+    for session, id, we can have a quick savings here.
+
+    The webob interface dictates:
+
+        https://github.com/Pylons/webob/blob/main/src/webob/cookies.py#L663
+
+        An object with two methods: `loads`` and ``dumps``.  The ``loads`` method
+        should accept bytes and return a Python object.  The ``dumps`` method
+        should accept a Python object and return bytes.  A ``ValueError`` should
+        be raised for malformed inputs.  Default: ``None`, which will use a
+        derivation of :func:`json.dumps` and ``json.loads``.
     """
 
-    def dumps(self, appstruct):
-        return webob_bytes_(appstruct, encoding="utf-8")
+    def dumps(self, s: str) -> bytes:
+        try:
+            return s.encode("utf-8", "strict")
+        except Exception as exc:
+            raise InvalidSessionId_Serialization(exc)
 
-    def loads(self, bstruct):
-        return webob_text_(bstruct, encoding="utf-8")
+    def loads(self, s: bytes) -> str:
+        try:
+            return str(s, "utf-8", "strict")
+        except Exception as exc:
+            raise InvalidSessionId_Deserialization(exc)
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/PKG-INFO` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,737 +1,751 @@
 Metadata-Version: 2.1
 Name: pyramid-session-redis
-Version: 1.6.3
+Version: 1.7.0rc1
 Summary: High performance and actively maintained server-side session framework for Pyramid and Redis.
 Home-page: https://github.com/jvanasco/pyramid_session_redis
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
-Description: [![Build Status](https://travis-ci.org/jvanasco/pyramid_session_redis.png)](https://travis-ci.org/jvanasco/pyramid_session_redis)
-        
-        
-        Overview
-        ========
-        
-        `pyramid_session_redis` is a mature, stable and actively maintained Server-Side
-        Sessions plugin for the Pyramid web framework.
-        
-        Originally, this library was a fork of
-        [`pyramid_redis_sessions`](`/ericrasmussen/pyramid_redis_sessions`), focused on
-        improvements and API changes designed for high performance (particularly with
-        servers under load), and a slightly different API designed for developer
-        convenience.
-        
-        This package was planning to follow a multi-version release process, however
-        that plan was abandoned in favor of ensuring backards compatibility.
-        
-        The `main` and `1.6` branches are designed to support both:
-        
-        * Python 2
-        * Python 3
-        
-        and
-        
-        * Pyramid 1.x
-        * Pyramid 2.0
-        
-        
-        Prior Branches
-        --------------
-        
-        The 1.5.x branch is in maintenance mode. No updates are expected, as 1.6 is
-        backwards compatible.
-        
-        The 1.4.x branch is EOL. It led to the stable 1.5.0 API release.
-        
-        The 1.2.x branch is EOL as of 1.2.2. Previous plans were to support a final
-        1.3.0 release.
-        
-        Prior Branch Details
-        ____________________
-        
-        The 1.2.x branch and earlier are largely a "drop-in-replacement" compatible with
-        Eric Rasmussen's `pyramid_redis_sessions` as-is.  If you are migrating from that
-        project and do not want to upgrade code, you should pin your install of this
-        library to `pyramid_session_redis<=1.3.0` or `pyramid_session_redis<1.3`
-        
-        **Please be aware that you will be limited to using outdated versions of Pyramid 
-        1.x if using the 1.2.x branch.**
-        
-        Starting with the 1.4.x branch, several design changes were made and this library
-        is not a drop-in replacement, **HOWEVER** upgrading will only require minimal
-        editing of your code: some editing for migration; some kwargs have changed;
-        the structure of the package changed (imports); and advanced users who leverage
-        the internal systems may need to upgrade. It should not take more than 5 minutes
-        to convert.  The package is still a plug-and-play Pyramid ISessions interface, so
-        there are very small changes.
-        
-        Prior Branch Incompatibilities
-        ______________________________
-        
-        IMPORTANT: The internal payload structure changed in the 1.4 branch, and is no
-        longer compatible with sessions created under 1.2 - they will be invalid.
-        
-        PRs that can handle a graceful fallback are welcome.
-        
-        The 1.2 format guaranteed internal sessions to be in this format:
-        
-            {'managed_dict': {},
-             'created': INT,
-             'timeout': INT,
-             }
-        
-        The 1.4 version streamlines the keys for a lighter footprint and generally
-        looks like this:
-        
-            {'m': {},  # managed_dict
-             'c': INT,  # created
-             'v': SESSION_API_VERSION,  # api version INT
-             # the following are optional and not guaranteed to be in a session
-             't': INT,  # timeout
-             'x': INT,  # expiry
-             }
-        
-        Key Takeaways:
-        
-        * Keys were shortened to 1 letter
-        * An API Version is now used, to handle graceful changes in the future
-        * The Timeout is no longer guaranteed to be present.
-          The library now supports the entire Timeout to be handled in Redis
-        * An "Expiry Timeout" may also exist
-        
-        Key Concepts
-        ============================================
-        
-        
-        Timeout vs Expires/MaxAge
-        -------------------------
-        
-        This package allows you to set both *Timeout* and *Expiry* values.  The two
-        concepts are closely related, but very different.
-        
-        A *Timeout* is an internal value and a moving target. It specifies how long a
-        Session should last before it times out due to inactivity. The timeout is
-        constantly refreshed when the session is accessed.
-        
-        For example, consider these settings:
-        
-            timeout = 1800
-            timeout_trigger = 900
-        
-        The `timeout` setting is specifying the Session should remain active for 1800
-        seconds since it's last activity.  The `timeout_trigger` setting is an
-        optimization that defers modifying the Session's timeout on READ operations until
-        at least 900 seconds have passed since the last modification. Modifications will
-        always occur on WRITE operations.  Depending on your configuration, the timeout
-        may be stored in Redis, as part of the Python Payload, or both.
-        
-        To illustrate how the above settings work, consider a timeline in which a User
-        visits a website and then visits it again 2000 seconds later:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit N | 2000s | Session B (new)
-        
-        When the User makes the last visit, the Session would have timed out, because it
-        exceeded the 1800 second mark in the timeout.
-        
-        Now assume the User makes 3 visits in this timeline, and a second visit happens
-        at the 899 mark:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit 2 | 899s  | Session A
-        > Visit N | 2000s | Session B (new)
-        
-        When the User makes the last visit, the Session would still
-        have timed out, because the second visit did not meet the timeout_trigger
-        threshold.
-        
-        But, if the second visit happens just 2 seconds later, at the 901 mark, the
-        timeout_trigger is reached and the session's timeout will be extended:
-        
-        > Visit 1 | 0s    | Session A (new)
-        > Visit 2 | 901s  | Session A (update timeout trigger)
-        > Visit N | 2000s | Session A (update timeout trigger)
-        
-        When the User makes the last visit, it would still happen within the context of
-        the original Session and the timeout will be extended even further.
-        
-        *Expires* and *Max-Age* are generally values that related to Cookie settings.
-        
-        *Expires* is created on a Cookie as either a specified Date, or a null value; if
-        the value is null (explicit or unspecified), the Cookie will be set as a
-        "Session" cookie and only last for the duration of the web browser application
-        being open.
-        
-        *Max-Age* is created on a Cookie as the number of seconds until the Cookie
-        expires.  A zero or negative value will expire (delete) the cookie immediately.
-        If both Expires and Max-Age are set, Max-Age has precedence.
-        
-        
-        The Confusion?
-        --------------
-        
-        If Redis stores our Timeout info, it stores it in an "expiry" value via `SETEX`
-        or similar calls.  
-        
-        
-        Key Differences From pyramid_redis_sessions
-        ============================================
-        
-        Depending on your needs, this package is probably more desirable than the
-        original project. This package was designed to significantly cut down on the
-        communication between Redis and Pyramid. Some options are offered to minimize
-        the size of Redis payloads as well.
-        
-        This package contains additional hooks and features to aid developers who are
-        using Redis-based sessions in high-traffic situations.
-        
-        This package does not recommend any "best deployment" strategies, but supports a
-        wide range of strategies to implement the "best deployment" under any given
-        circumstance.
-        
-        Through 1.2.x
-        -------------
-        
-        * The original package communicates with Redis on most attribute accesses and
-          writes within a given request. The traffic can be burdensome in some
-          implementations. `pyramid_session_redis` will queue a single `persist` or
-          `refresh` task per-request using Pyramid's `add_finished_callback` hook.
-        * The original version used `EXISTS` to check if a Session existed or not, then
-          proceeded to `GET` or `SET` a new Session.  `pyramid_session_redis` will
-          immediately attempt a `GET`, and will `SET` a new Session on failure.
-          This approach eliminates a call.
-        * Separate calls to `SET` and `EXPIRE` were replaced with a single `SETEX`.
-        * A flag can be set to enable a LRU Cache (least recently used) mode. No expiry
-          data will be sent to Redis, allowing the Redis server to handle the LRU logic
-          itself.
-        * The active Session is decoupled from the `request.session` attributs; this
-          allows for the Session to be set up on alternate attributes and supports
-          integration with
-          [pyramid_session_multi](https://github.com/jvanasco/pyramid_session_multi).
-        * The original library does not detect changes in nested dictionaries. This
-          package uses `hashlib.md5` to fingerprint the serialized value on READ; if no
-          changes were detected, a failsafe will `Serialize+md5` the data to decide if a
-          WRITE should occur. This behavior can be disabled by setting `detect_changes`
-          to `False`.
-        * The original library raises a fatal error if a Session can not be
-          deserialized. By passing in `deserialized_fails_new` to the constructor,
-          you can create a new Session on deserialization errors.
-        * Support for disabling Sessions on CDN generated content via
-          `func_check_response_allow_cookies`
-        * Thanks to @ github/hongyuan1306, Token Generation has been consolidated to use
-          Python3's stdlib (or reimplemented if not available). Tokens are also 32,
-          not 20, characters.
-        * Redis is supported in a LRU mode (see http://redis.io/topics/lru-cache) by
-          setting the option `set_redis_ttl` to `False` (by default, it is `True`).
-          This will eliminate calls to `EXPIRE` and will use `SET` instead of `SETEX`.
-        * In the 1.2.x branch, the created time can be set to an integer via
-          `use_int_time=True`. This will cast the `created` time via
-          `int(math.ceil(time.time()))`. This reduces a payload by several bits.
-        
-        Other Updates 1.4.x+
-        --------------------
-        
-        * Only `int()` time is supported; Fractional time wastes bytes.
-        * Sessions now have version control to support future upgrades via a "version"
-          `v` key.
-        * The format of the internal payload was rewritten, the encoded payload now
-          uses 1-letter keys instead of words. This should offset the addition of an
-          expires timestamp and version id.
-        * There was no logic for Python timeout control (whoops!) this has been fixed.
-          An "expires" `x` key now tracks the expiration.
-        * Added a `timeout_trigger` option.  This will defer expiry data updates to
-          lower usage on Redis.  This is explained below in more detail.
-        * In high load situations, Redis can have performance and storage issues because
-          in the original package Session IDs are created on every request (such as a
-          getting spidered by a botnet that does not respect Sessions). In this package,
-          a 'lazycreate' method is used: a session_id/cookie will not be generated
-          unless a session is needed in the callback routine. In order to generate
-          session_id/cookie beforehand, one can use the `RedisSession.ensure_id`
-          function.  To safely check if a session id exists, one can use the
-          `RedisSession.session_id_safecheck` method as well.
-        * Added `func_invalid_logger` to the constructor. This can be used to log
-          invalid Sessions. It is incredibly useful when integrated with a statsd
-          system. (see below)
-        * Added `set_redis_ttl_readheavy` to the factory and session constructors.
-          This option will optimize Sessions which have Redis-maintained TTLs by
-          executing a GET+EXPIRE together within a pipeline.
-        
-        
-        
-        Installation
-        ============
-        
-        Install via pypi:
-        
-            pip install pyramid_session_redis
-        
-        
-        Configuration
-        =============
-        
-        Configure `pyramid_session_redis` via your Paste config file or however you
-        prefer to configure Pyramid. Only `redis.sessions.secret` is required.
-        All other settings are optional.
-        
-        For complete documentation on the `RedisSessionFactory` that uses these
-        settings, see :doc:`api`. Otherwise, keep reading for the quick list:
-        
-        
-            # session settings
-            redis.sessions.secret = your_cookie_signing_secret
-            redis.sessions.timeout = 1200
-        
-            # session cookie settings
-            redis.sessions.cookie_name = session
-            redis.sessions.cookie_max_age = max_age_in_seconds
-            redis.sessions.cookie_path = /
-            redis.sessions.cookie_domain =
-            redis.sessions.cookie_secure = False
-            redis.sessions.cookie_httponly = False
-            redis.sessions.cookie_on_exception = True
-        
-            # you can supply a redis connection string as a URL
-            redis.sessions.url = redis://username:password@localhost:6379/0
-        
-            # or as individual settings (note: the URL gets preference if you do both)
-            redis.sessions.host = localhost
-            redis.sessions.port = 6379
-            redis.sessions.db = 0
-            redis.sessions.password = None
-        
-            # additional options can be supplied to redis-py's StrictRedis
-            redis.sessions.socket_timeout =
-            redis.sessions.connection_pool =
-            redis.sessions.charset = utf-8
-            redis.sessions.errors = strict
-            redis.sessions.unix_socket_path =
-        
-            # in the advanced section we'll cover how to instantiate your own client
-            redis.sessions.client_callable = my.dotted.python.callable
-        
-            # along with defining your own serialize and deserialize methods
-            redis.sessions.serialize = cPickle.dumps
-            redis.sessions.deserialize = cPickle.loads
-        
-            # you can specify a prefix to be used with session keys in redis
-            redis.sessions.prefix = mycoolprefix
-        
-            # or you can supply your own UID generator callable for session keys
-            redis.sessions.id_generator = niftyuid
-        
-        
-        Initialization
-        ==============
-        
-        Lastly, you need to tell Pyramid to use `pyramid_session_redis` as your
-        Session factory. The preferred way is adding it with `config.include`,
-        like this:
-        
-            def main(global_config, **settings):
-                config = Configurator(settings=settings)
-                config.include('pyramid_session_redis')
-        
-        Alternately, instead of using the Configurator's include method, you can
-        activate Pyramid by changing your application's ".ini" file, use the following
-        line:
-        
-            pyramid.includes = pyramid_session_redis
-        
-        The above method is recommended because it's simpler, idiomatic, and still fully
-        configurable. It even has the added benefit of automatically resolving dotted
-        python paths used in the advanced options.
-        
-        However, you can also explicitly pass a settings dict to the
-        `session_factory_from_settings` function. This can be helpful if you configure
-        or modify your settings in code:
-        
-            from pyramid_session_redis import session_factory_from_settings
-        
-            def main(global_config, **settings):
-                config = Configurator(settings=settings)
-                session_factory = pyramid_session_redis(settings)
-                config.set_session_factory(session_factory)
-        
-        
-        Timeout Notes
-        =============
-        
-        If ``set_redis_ttl`` is False, it does not imply there is no timeout at all --
-        only that Redis will not be sent timeout data via `SETEX` or `EXPIRE`.
-        Timeout data will still be stored in Python.
-        
-        If Redis is functioning as an LRU Cache, abandoned sessions will never be seen
-        by Python, but will eventually be cleared out to make room for new sessions by
-        the inherent Redis LRU logic.
-        
-        Timeout data stored in Python is relatively small when compared to the timeout
-        data stored in Redis.
-        
-        If you want to NEVER have sessions timeout, set the initial `timeout`
-        to "0" or "None".
-        
-        Setting a `timeout_trigger` will require Python to track the expiry.
-        
-        Enabling `set_redis_ttl_readheavy` requires a `timeout` and `set_redis_ttl`;
-        it also requires not enabling `timeout_trigger` or `python_expires`.
-        
-        
-        Timeout Examples
-        ----------------
-        
-        Timeout in Python, with Redis TTL via `SETEX`/`EXPIRE`:
-        
-            timeout = 60
-        
-        Timeout in Python, no Redis TTL (only `SET` used)
-        
-            timeout = 60
-            assume_redis_ttl = True
-        
-        No Timeout in Python, no Redis TTL (only `SET` used)
-        
-            timeout = 0  # or None
-            assume_redis_ttl = True
-        
-        
-        Warning: Session Locking and Race Conditions
-        ============================================
-        
-        This package does not incorporate any sort of locking for session updating or
-        handling of race conditions.
-        
-        This should not be a problem for the vast majority of users, and is a feature
-        not present on any known Pyramid Session providers.
-        
-        For more information, please see:
-        
-        * https://github.com/jvanasco/pyramid_session_redis/issues/9
-        * https://github.com/Pylons/pyramid/issues/3041
-        
-        
-        Feature - Timeout Triggers
-        ==========================
-        
-        A timeout trigger can be used to limit the amount of updates/writes.
-        It may be more beneficial to your usage pattern.
-        
-        For the sake of clarity, I'll use an oversimplification that Redis essentially
-        has two different internal data stores that are used independently: one for a
-        Key's payload and another for the Key's expiry.
-        
-        In the 'classic' behavior (project this was forked from): every time you access
-        an existing session, the GET is followed by sending Redis a new EXPIRE time;
-        essentially every "read" has a corresponding "write" for the Redis-tracked
-        expiry record.
-        
-        In order to minimize the writes via SETEX, I introduced the timeout trigger.
-        The trigger works by storing some timeout information in the Redis data payload,
-        and using that information to determine when to send a write. Instead of having
-        a GET+EXPIRE for every read, we only have a single GET and eliminate the write
-        caused by the EXPIRE. This has a maintenance cost though - once we hit the
-        timeout trigger, instead of just the GET we need to update the internal timeout
-        payload and issue a SET.
-        
-        Going back to your situation: when the user stops activity at 40 minutes in, if
-        the timeout trigger is enabled then there has never been an update to the
-        internal payload or Redis about the user activity since the session was first
-        created. The purpose of the trigger is to defer that "write" operation.
-        
-        In order to make a session valid for "reading" for around an hour, you should
-        do something like:
-        
-        * a two-hour session with a 10 minute trigger, or
-        * a one-hour session with a 50 minute trigger
-        
-        You can also disable the functionality by setting the trigger to 0. Up to a few
-        thousand daily users, you shouldn't have any issues with the overhead of the
-        "classic" mode. When you hit 10k users and/or start to have clustered web
-        servers communicating with dedicated Redis instances, setting a new EXPIRE after
-        every read operation becomes something you want to avoid.
-        
-        
-        Scenario 1 - Classic Redis
-        --------------------------
-        
-        In the typical "classic" Redis usage pattern, the session usage is refreshed via
-        an `EXPIRE` call on every session view.
-        
-        This is useful, but means many session operations will trigger two Redis calls
-        (`GET` + `EXPIRE`).  On a high performance system, this can be a lot.
-        
-        This is a typical scenario with refreshing:
-        
-            timeout = 200
-        
-        The following timeline would occur:
-        
-        | time | Redis calls    | timeout |
-        | ---- | -------------- | ------- |
-        | 0    | `GET`+`SETEX`  | 200     |
-        | 100  | `GET`+`EXPIRE` | 300     |
-        | 200  | `GET`+`EXPIRE` | 400     |
-        | 300  | `GET`+`EXPIRE` | 500     |
-        | 400  | `GET`+`EXPIRE` | 600     |
-        | 500  | `GET`+`EXPIRE` | 700     |
-        
-        
-        Scenario 2 - Timeout Trigger
-        --------------------------
-        
-        The 1.4.x branch introduces a `timeout_trigger` to augment the Session's
-        `timeout`.
-        
-        Whereas a `timeout` states how long a session is good for, a `timeout_trigger`
-        defers how long a Session's refresh should be deferred for:
-        
-        Given the following example, the package will use a 1200s timeout for requests,
-        but only trigger an update of the expiry time when the current time is within
-        600s of the expiry:
-        
-            timeout = 1200
-            timeout_trigger = 600
-        
-        The following timeline would occur:
-        
-        | time | Redis calls  | timeout | next threshold |
-        | ---- | ------------ | ------- | -------------- |
-        | 0    | `GET`+`SET`* | 1200    | 600            |
-        | 1    | `GET`        | 1200    | 600            |
-        | ...  |              |         |                |
-        | 599  | `GET`        | 1200    | 600            |
-        | 600  | `GET`+`SET`* | 1800    | 1200           |
-        | 601  | `GET`        | 1800    | 1200           |
-        | ...  |              |         |                |
-        | 1199 | `GET`        | 1800    | 1200           |
-        | 1200 | `GET`+`SET`* | 2400    | 1800           |
-        
-        * This method is compatible with setting a TTL in redis via `SETEX` or doing
-        everything within Python if Redis is in a LRU mode
-        
-        The removes all calls to `EXPIRE` before the threshold is reached, which can be
-         a considerable savings in read-heavy situations.
-        
-        The caveat to this method: an expiry timestamp must be stored within the payload
-        AND updating the timeout requires a `SET` operation.
-        
-        
-        Feature - set_redis_ttl_readheavy
-        =================================
-        
-        This is a new option in `1.4.2` which should improve performance on readheavy
-        installations BUT may degrade performance on writeheavy installations.  This
-        option will aggregate a GET+EXPIRE on every read.
-        
-        `set_redis_ttl_readheavy` requires the following:
-        
-        * a `timeout` value is set
-        * `set_redis_ttl` is `True`
-        * `timeout_trigger` is NOT set
-        * `python_expires` is NOT True
-        
-        The default behavior of this library during a read-only request is this:
-        
-        * On session access, query Redis via `redis.GET {session_id}`
-        * In a Pyramid callback, update Redis via `redis.EXPIRE {session_id} {expiry}`
-        
-        During a read-write:
-        
-        * On session access, query Redis via `redis.GET {session_id}`
-        * In a Pyramid callback, update Redis via
-          `redis.SETEX {session_id} {payload} {expiry}`
-        
-        The new `set_redis_ttl_readheavy` changes this. If enabled during a read-only
-        request, the behavior will be lighter on the Redis instance:
-        
-        * On session access, open a pipeline with two Redis commands:
-          `pipeline.GET {session_id}`,
-          `pipeline.EXPIRE {session_id} {expiry}`.
-        * In a Pyramid callback, the duplicate expire is suppressed.
-        
-        However during a read-write, the activity will be:
-        
-        * On session access, open a pipeline with two Redis commands:
-          `pipeline.GET {session_id}`,
-          `pipeline.EXPIRE {session_id} {expiry}`.
-        * In a Pyramid callback, update Redis via
-          `redis.SETEX {session_id} {payload} {expiry}`
-        
-        Read-heavy applications should see a slight performance bump via the pipeined
-        GET+EXPIRE, however write-heavy applications are likely to see a performance
-        degradation as it adds an extra EXPIRE to every request.
-        
-        
-        Invalid Logging
-        ================
-        
-        The default behavior of this library is to silently create new session when bad
-        session data is encountered, such as a cookie with an invalid id or corrupted
-        datastore.  A graceful "new session" is the ideal situation for end-users.
-        
-        The problem with that strategy is that problems in code or your application
-        stack can be hidden, and you might not know about a bad datastore.
-        
-        The 1.4 release introduces `func_invalid_logger` to the factory constructor.
-        This can be used to track the invalid sessions that are safely caught and
-        silently upgraded.
-        
-        How?  The package tracks why a session is invalid with variant classes of
-        `pyramid_session_redis.exceptions.InvalidSession`.
-        
-        Specifically there are the following classes:
-        
-        * ``InvalidSession(Exception)``
-          Catchall base class
-        * ``InvalidSession_NoSessionCookie(InvalidSession)``
-          The Session is invalid because there is no cookie.
-          This is the same as "new session".
-        * ``InvalidSession_NotInBackend(InvalidSession)``
-          The Session id was not in the backend.
-        * ``InvalidSession_DeserializationError(InvalidSession)``
-            Error deserializing.
-            This is raised if ``deserialized_fails_new`` is True. Otherwise the
-            exception is wrapped in a ``RawDeserializationError`` and raised without
-            being caught.
-        * ``InvalidSession_PayloadTimeout(InvalidSession)``
-            The inner Python payload timed out.
-        * ``InvalidSession_PayloadLegacy(InvalidSession)``
-            The Session is running on an earlier version.
-        
-        The factory accepts a `func_invalid_logger` callable argument. The input is the
-        raised exception BEFORE a new cookie is generated, and will be the request and
-        an instance of `InvalidSession`.
-        
-            from pyramid_session_redis.exceptions import *
-            from my_statsd import new_statsd_client()
-        
-            statsd_client = new_statsd_client()
-        
-            def my_logger(request, raised_exception):
-                """
-                raised_exception will be an instance of InvalidSession
-                log the exception to statsd for metrics
-                """
-                if isinstance(raised_exception, InvalidSession_NoSessionCookie):
-                    statsd_client.incr('invalid_session.NoSessionCookie')
-                elif isinstance(raised_exception, InvalidSession_NotInBackend):
-                    statsd_client.incr('invalid_session.NotInBackend')
-                elif isinstance(raised_exception, InvalidSession_DeserializationError):
-                    statsd_client.incr('invalid_session.DeserializationError')
-        
-            factory = RedisSessionFactory(...
-                                          func_invalid_logger=my_logger,
-                                          ...
-                                          )
-        
-        The `func_invalid_logger` argument may be provided as a dotted-notation string
-        in a configuration file.
-        
-        
-        Uncaught Errors
-        ================
-        
-        The exception `pyramid_session_redis.exceptions.RawDeserializationError` will be
-        raised if deserialization of a payload fails and `deserialized_fails_new` is not
-        `True`. The first arg will be the caught exception. This allows for a standard
-        error across multiple deserialization options.
-        
-        
-        FAQ:
-        =====
-        
-        Q. What serialization is used?
-        ------------------------------
-        
-        A. Serialization is used at two points
-        
-        * Serializing the Session data.
-          The server-side data serialization is handled by `pickle`. This Session data is
-          created on the server by your application and remains on the server. `pickle`
-          is safe to use in this context, as user-generated payloads can not be introduced
-          to these (de)serialization routines. If you wish to avoid `pickle`, or your
-          prefer to use another encoder, you can easily specify a different (de)serialization
-          routine such as a custom JSON, msgpack or pretty much anything else.
-        
-        * Serializing the `session_id` to encode into a signed cookie.
-          This library uses `WebOb.cookies.SignedSerializer` to securely manage a HMAC
-          signature of the `session_id` combined with a site-secret. The library allows
-          for a custom replacement to be provided as well.
-          
-          In the original library, the session id and signature were turned into a
-          cookie-safe value via `pickle` (de)serialization - a detail that remained in
-          this library through `<=v1.5.0`. This approach was identified as a security
-          risk, and was removed from this library starting in `v1.5.1`.  
-        
-        
-        Examples
-        ========
-        
-        There is an example of using this package in `pyramid_session_multi`
-        [examples/single_file_app.py](https://github.com/jvanasco/pyramid_session_multi/blob/main/examples/single_file_app.py).
-        
-        
-        Further Reading:
-        ================
-        
-        For more information about Redis performance under Python please see an
-        associated project:
-        
-        * https://github.com/jvanasco/dogpile_backend_redis_advanced
-        
-        To suport multiple Sessions under Pyramid
-        
-        * https://github.com/jvanasco/pyramid_session_multi
-        
-        Until Nov 2016 this was maintained as `jvanasco/pyramid_redis_sessions`
-        
-        * The main branch for `jvanasco/pyramid_redis_sessions` was "custom_deployment"
-        * The branched named "main" is the upstream source from ericrasmussen
-        
-        As of Nov 2016, this was forked into it's own project to allow for distribution
-        under PyPi.
-        
-        All support is handled via GitHub : https://github.com/jvanasco/pyramid_session_redis
-        
-        
-        ToDo
-        =====
-        
-        see `TODO.md`
-        
-        
-        Changelog
-        ==========
-        
-        see `CHANGES.md`
-        
-        
-        Support
-        =======
-        
-        You can report bugs or open feature/support requests via GitHub
-        
-        * https://github.com/jvanasco/pyramid_session_redis
-        
-        
-        License
-        =======
-        
-        `pyramid_session_redis` is available under a FreeBSD-derived license. See
-        `LICENSE.txt <https://github.com/jvanasco/pyramid_session_redis/blob/main/LICENSE.txt>`_
-        for details.
-        
 Keywords: pyramid session redis
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE.txt
+
+[![Build Status](https://travis-ci.org/jvanasco/pyramid_session_redis.png)](https://travis-ci.org/jvanasco/pyramid_session_redis)
+
+
+Overview
+========
+
+`pyramid_session_redis` is a mature, stable and actively maintained Server-Side
+Sessions plugin for the Pyramid web framework.
+
+Originally, this library was a fork of
+[`pyramid_redis_sessions`](https://github.com/ericrasmussen/pyramid_redis_sessions), focused on
+improvements and API changes designed for high performance (particularly with
+servers under load), and a slightly different API designed for developer
+convenience.
+
+Compatibility
+-------------
+
+`main` and `1.7` branches require:
+
+* Python 3.6+
+* Pyramid 2.0
+
+
+The `1.6` branch is designed to support both:
+
+* Python 2
+* Python 3
+
+and
+
+* Pyramid 1.x
+* Pyramid 2.0
+
+
+Breaking Changes
+----------------
+
+Starting in `1.7`, the NullSerializer will ensure data is serialized into a string.
+
+
+Prior Branches
+--------------
+
+The 1.6.x branch is in maintenance mode. This is the last branch to support
+Python2 and Pyramid1.
+
+The 1.5.x branch is EOL. No updates are expected, as 1.6 is backwards compatible.
+
+The 1.4.x branch is EOL. It led to the stable 1.5.0 API release.
+
+The 1.2.x branch is EOL as of 1.2.2. Previous plans were to support a final
+1.3.0 release.
+
+Prior Branch Details
+____________________
+
+The 1.2.x branch and earlier are largely a "drop-in-replacement" compatible with
+Eric Rasmussen's `pyramid_redis_sessions` as-is.  If you are migrating from that
+project and do not want to upgrade code, you should pin your install of this
+library to `pyramid_session_redis<=1.3.0` or `pyramid_session_redis<1.3`
+
+**Please be aware that you will be limited to using outdated versions of Pyramid 
+1.x if using the 1.2.x branch.**
+
+Starting with the 1.4.x branch, several design changes were made and this library
+is not a drop-in replacement, **HOWEVER** upgrading will only require minimal
+editing of your code: some editing for migration; some kwargs have changed;
+the structure of the package changed (imports); and advanced users who leverage
+the internal systems may need to upgrade. It should not take more than 5 minutes
+to convert.  The package is still a plug-and-play Pyramid ISessions interface, so
+there are very small changes.
+
+Prior Branch Incompatibilities
+______________________________
+
+IMPORTANT: The internal payload structure changed in the 1.4 branch, and is no
+longer compatible with sessions created under 1.2 - they will be invalid.
+
+PRs that can handle a graceful fallback are welcome.
+
+The 1.2 format guaranteed internal sessions to be in this format:
+
+    {'managed_dict': {},
+     'created': INT,
+     'timeout': INT,
+     }
+
+The 1.4 version streamlines the keys for a lighter footprint and generally
+looks like this:
+
+    {'m': {},  # managed_dict
+     'c': INT,  # created
+     'v': SESSION_API_VERSION,  # api version INT
+     # the following are optional and not guaranteed to be in a session
+     't': INT,  # timeout
+     'x': INT,  # expiry
+     }
+
+Key Takeaways:
+
+* Keys were shortened to 1 letter
+* An API Version is now used, to handle graceful changes in the future
+* The Timeout is no longer guaranteed to be present.
+  The library now supports the entire Timeout to be handled in Redis
+* An "Expiry Timeout" may also exist
+
+Key Concepts
+============================================
+
+
+Timeout vs Expires/MaxAge
+-------------------------
+
+This package allows you to set both *Timeout* and *Expiry* values.  The two
+concepts are closely related, but very different.
+
+A *Timeout* is an internal value and a moving target. It specifies how long a
+Session should last before it times out due to inactivity. The timeout is
+constantly refreshed when the session is accessed.
+
+For example, consider these settings:
+
+    timeout = 1800
+    timeout_trigger = 900
+
+The `timeout` setting is specifying the Session should remain active for 1800
+seconds since it's last activity.  The `timeout_trigger` setting is an
+optimization that defers modifying the Session's timeout on READ operations until
+at least 900 seconds have passed since the last modification. Modifications will
+always occur on WRITE operations.  Depending on your configuration, the timeout
+may be stored in Redis, as part of the Python Payload, or both.
+
+To illustrate how the above settings work, consider a timeline in which a User
+visits a website and then visits it again 2000 seconds later:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit N | 2000s | Session B (new)
+
+When the User makes the last visit, the Session would have timed out, because it
+exceeded the 1800 second mark in the timeout.
+
+Now assume the User makes 3 visits in this timeline, and a second visit happens
+at the 899 mark:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit 2 | 899s  | Session A
+> Visit N | 2000s | Session B (new)
+
+When the User makes the last visit, the Session would still
+have timed out, because the second visit did not meet the timeout_trigger
+threshold.
+
+But, if the second visit happens just 2 seconds later, at the 901 mark, the
+timeout_trigger is reached and the session's timeout will be extended:
+
+> Visit 1 | 0s    | Session A (new)
+> Visit 2 | 901s  | Session A (update timeout trigger)
+> Visit N | 2000s | Session A (update timeout trigger)
+
+When the User makes the last visit, it would still happen within the context of
+the original Session and the timeout will be extended even further.
+
+*Expires* and *Max-Age* are generally values that related to Cookie settings.
+
+*Expires* is created on a Cookie as either a specified Date, or a null value; if
+the value is null (explicit or unspecified), the Cookie will be set as a
+"Session" cookie and only last for the duration of the web browser application
+being open.
+
+*Max-Age* is created on a Cookie as the number of seconds until the Cookie
+expires.  A zero or negative value will expire (delete) the cookie immediately.
+If both Expires and Max-Age are set, Max-Age has precedence.
+
+
+The Confusion?
+--------------
+
+If Redis stores our Timeout info, it stores it in an "expiry" value via `SETEX`
+or similar calls.  
+
+
+Key Differences From pyramid_redis_sessions
+============================================
+
+Depending on your needs, this package is probably more desirable than the
+original project. This package was designed to significantly cut down on the
+communication between Redis and Pyramid. Some options are offered to minimize
+the size of Redis payloads as well.
+
+This package contains additional hooks and features to aid developers who are
+using Redis-based sessions in high-traffic situations.
+
+This package does not recommend any "best deployment" strategies, but supports a
+wide range of strategies to implement the "best deployment" under any given
+circumstance.
+
+Through 1.2.x
+-------------
+
+* The original package communicates with Redis on most attribute accesses and
+  writes within a given request. The traffic can be burdensome in some
+  implementations. `pyramid_session_redis` will queue a single `persist` or
+  `refresh` task per-request using Pyramid's `add_finished_callback` hook.
+* The original version used `EXISTS` to check if a Session existed or not, then
+  proceeded to `GET` or `SET` a new Session.  `pyramid_session_redis` will
+  immediately attempt a `GET`, and will `SET` a new Session on failure.
+  This approach eliminates a call.
+* Separate calls to `SET` and `EXPIRE` were replaced with a single `SETEX`.
+* A flag can be set to enable a LRU Cache (least recently used) mode. No expiry
+  data will be sent to Redis, allowing the Redis server to handle the LRU logic
+  itself.
+* The active Session is decoupled from the `request.session` attributs; this
+  allows for the Session to be set up on alternate attributes and supports
+  integration with
+  [pyramid_session_multi](https://github.com/jvanasco/pyramid_session_multi).
+* The original library does not detect changes in nested dictionaries. This
+  package uses `hashlib.md5` to fingerprint the serialized value on READ; if no
+  changes were detected, a failsafe will `Serialize+md5` the data to decide if a
+  WRITE should occur. This behavior can be disabled by setting `detect_changes`
+  to `False`.
+* The original library raises a fatal error if a Session can not be
+  deserialized. By passing in `deserialized_fails_new` to the constructor,
+  you can create a new Session on deserialization errors.
+* Support for disabling Sessions on CDN generated content via
+  `func_check_response_allow_cookies`
+* Thanks to @ github/hongyuan1306, Token Generation has been consolidated to use
+  Python3's stdlib (or reimplemented if not available). Tokens are also 32,
+  not 20, characters.
+* Redis is supported in a LRU mode (see http://redis.io/topics/lru-cache) by
+  setting the option `set_redis_ttl` to `False` (by default, it is `True`).
+  This will eliminate calls to `EXPIRE` and will use `SET` instead of `SETEX`.
+* In the 1.2.x branch, the created time can be set to an integer via
+  `use_int_time=True`. This will cast the `created` time via
+  `int(math.ceil(time.time()))`. This reduces a payload by several bits.
+
+Other Updates 1.4.x+
+--------------------
+
+* Only `int()` time is supported; Fractional time wastes bytes.
+* Sessions now have version control to support future upgrades via a "version"
+  `v` key.
+* The format of the internal payload was rewritten, the encoded payload now
+  uses 1-letter keys instead of words. This should offset the addition of an
+  expires timestamp and version id.
+* There was no logic for Python timeout control (whoops!) this has been fixed.
+  An "expires" `x` key now tracks the expiration.
+* Added a `timeout_trigger` option.  This will defer expiry data updates to
+  lower usage on Redis.  This is explained below in more detail.
+* In high load situations, Redis can have performance and storage issues because
+  in the original package Session IDs are created on every request (such as a
+  getting spidered by a botnet that does not respect Sessions). In this package,
+  a 'lazycreate' method is used: a session_id/cookie will not be generated
+  unless a session is needed in the callback routine. In order to generate
+  session_id/cookie beforehand, one can use the `RedisSession.ensure_id`
+  function.  To safely check if a session id exists, one can use the
+  `RedisSession.session_id_safecheck` method as well.
+* Added `func_invalid_logger` to the constructor. This can be used to log
+  invalid Sessions. It is incredibly useful when integrated with a statsd
+  system. (see below)
+* Added `set_redis_ttl_readheavy` to the factory and session constructors.
+  This option will optimize Sessions which have Redis-maintained TTLs by
+  executing a GET+EXPIRE together within a pipeline.
+
+
+
+Installation
+============
+
+Install via pypi:
+
+    pip install pyramid_session_redis
+
+
+Configuration
+=============
+
+Configure `pyramid_session_redis` via your Paste config file or however you
+prefer to configure Pyramid. Only `redis.sessions.secret` is required.
+All other settings are optional.
+
+For complete documentation on the `RedisSessionFactory` that uses these
+settings, see :doc:`api`. Otherwise, keep reading for the quick list:
+
+
+    # session settings
+    redis.sessions.secret = your_cookie_signing_secret
+    redis.sessions.timeout = 1200
+
+    # session cookie settings
+    redis.sessions.cookie_name = session
+    redis.sessions.cookie_max_age = max_age_in_seconds
+    redis.sessions.cookie_path = /
+    redis.sessions.cookie_domain =
+    redis.sessions.cookie_secure = False
+    redis.sessions.cookie_httponly = False
+    redis.sessions.cookie_on_exception = True
+
+    # you can supply a redis connection string as a URL
+    redis.sessions.url = redis://username:password@localhost:6379/0
+
+    # or as individual settings (note: the URL gets preference if you do both)
+    redis.sessions.host = localhost
+    redis.sessions.port = 6379
+    redis.sessions.db = 0
+    redis.sessions.password = None
+
+    # additional options can be supplied to redis-py's StrictRedis
+    redis.sessions.socket_timeout =
+    redis.sessions.connection_pool =
+    redis.sessions.charset = utf-8
+    redis.sessions.errors = strict
+    redis.sessions.unix_socket_path =
+
+    # in the advanced section we'll cover how to instantiate your own client
+    redis.sessions.client_callable = my.dotted.python.callable
+
+    # along with defining your own serialize and deserialize methods
+    redis.sessions.serialize = cPickle.dumps
+    redis.sessions.deserialize = cPickle.loads
+
+    # you can specify a prefix to be used with session keys in redis
+    redis.sessions.prefix = mycoolprefix
+
+    # or you can supply your own UID generator callable for session keys
+    redis.sessions.id_generator = niftyuid
+
+
+Initialization
+==============
+
+Lastly, you need to tell Pyramid to use `pyramid_session_redis` as your
+Session factory. The preferred way is adding it with `config.include`,
+like this:
+
+    def main(global_config, **settings):
+        config = Configurator(settings=settings)
+        config.include('pyramid_session_redis')
+
+Alternately, instead of using the Configurator's include method, you can
+activate Pyramid by changing your application's ".ini" file, use the following
+line:
+
+    pyramid.includes = pyramid_session_redis
+
+The above method is recommended because it's simpler, idiomatic, and still fully
+configurable. It even has the added benefit of automatically resolving dotted
+python paths used in the advanced options.
+
+However, you can also explicitly pass a settings dict to the
+`session_factory_from_settings` function. This can be helpful if you configure
+or modify your settings in code:
+
+    from pyramid_session_redis import session_factory_from_settings
+
+    def main(global_config, **settings):
+        config = Configurator(settings=settings)
+        session_factory = session_factory_from_settings(settings)
+        config.set_session_factory(session_factory)
+
+
+Timeout Notes
+=============
+
+If ``set_redis_ttl`` is False, it does not imply there is no timeout at all --
+only that Redis will not be sent timeout data via `SETEX` or `EXPIRE`.
+Timeout data will still be stored in Python.
+
+If Redis is functioning as an LRU Cache, abandoned sessions will never be seen
+by Python, but will eventually be cleared out to make room for new sessions by
+the inherent Redis LRU logic.
+
+Timeout data stored in Python is relatively small when compared to the timeout
+data stored in Redis.
+
+If you want to NEVER have sessions timeout, set the initial `timeout`
+to "0" or "None".
+
+Setting a `timeout_trigger` will require Python to track the expiry.
+
+Enabling `set_redis_ttl_readheavy` requires a `timeout` and `set_redis_ttl`;
+it also requires not enabling `timeout_trigger` or `python_expires`.
+
+
+Timeout Examples
+----------------
+
+Timeout in Python, with Redis TTL via `SETEX`/`EXPIRE`:
+
+    timeout = 60
+
+Timeout in Python, no Redis TTL (only `SET` used)
+
+    timeout = 60
+    assume_redis_ttl = True
+
+No Timeout in Python, no Redis TTL (only `SET` used)
+
+    timeout = 0  # or None
+    assume_redis_ttl = True
+
+
+Warning: Session Locking and Race Conditions
+============================================
+
+This package does not incorporate any sort of locking for session updating or
+handling of race conditions.
+
+This should not be a problem for the vast majority of users, and is a feature
+not present on any known Pyramid Session providers.
+
+For more information, please see:
+
+* https://github.com/jvanasco/pyramid_session_redis/issues/9
+* https://github.com/Pylons/pyramid/issues/3041
+
+
+Feature - Timeout Triggers
+==========================
+
+A timeout trigger can be used to limit the amount of updates/writes.
+It may be more beneficial to your usage pattern.
+
+For the sake of clarity, I'll use an oversimplification that Redis essentially
+has two different internal data stores that are used independently: one for a
+Key's payload and another for the Key's expiry.
+
+In the 'classic' behavior (project this was forked from): every time you access
+an existing session, the GET is followed by sending Redis a new EXPIRE time;
+essentially every "read" has a corresponding "write" for the Redis-tracked
+expiry record.
+
+In order to minimize the writes via SETEX, I introduced the timeout trigger.
+The trigger works by storing some timeout information in the Redis data payload,
+and using that information to determine when to send a write. Instead of having
+a GET+EXPIRE for every read, we only have a single GET and eliminate the write
+caused by the EXPIRE. This has a maintenance cost though - once we hit the
+timeout trigger, instead of just the GET we need to update the internal timeout
+payload and issue a SET.
+
+Going back to your situation: when the user stops activity at 40 minutes in, if
+the timeout trigger is enabled then there has never been an update to the
+internal payload or Redis about the user activity since the session was first
+created. The purpose of the trigger is to defer that "write" operation.
+
+In order to make a session valid for "reading" for around an hour, you should
+do something like:
+
+* a two-hour session with a 10 minute trigger, or
+* a one-hour session with a 50 minute trigger
+
+You can also disable the functionality by setting the trigger to 0. Up to a few
+thousand daily users, you shouldn't have any issues with the overhead of the
+"classic" mode. When you hit 10k users and/or start to have clustered web
+servers communicating with dedicated Redis instances, setting a new EXPIRE after
+every read operation becomes something you want to avoid.
+
+
+Scenario 1 - Classic Redis
+--------------------------
+
+In the typical "classic" Redis usage pattern, the session usage is refreshed via
+an `EXPIRE` call on every session view.
+
+This is useful, but means many session operations will trigger two Redis calls
+(`GET` + `EXPIRE`).  On a high performance system, this can be a lot.
+
+This is a typical scenario with refreshing:
+
+    timeout = 200
+
+The following timeline would occur:
+
+| time | Redis calls    | timeout |
+| ---- | -------------- | ------- |
+| 0    | `GET`+`SETEX`  | 200     |
+| 100  | `GET`+`EXPIRE` | 300     |
+| 200  | `GET`+`EXPIRE` | 400     |
+| 300  | `GET`+`EXPIRE` | 500     |
+| 400  | `GET`+`EXPIRE` | 600     |
+| 500  | `GET`+`EXPIRE` | 700     |
+
+
+Scenario 2 - Timeout Trigger
+--------------------------
+
+The 1.4.x branch introduces a `timeout_trigger` to augment the Session's
+`timeout`.
+
+Whereas a `timeout` states how long a session is good for, a `timeout_trigger`
+defers how long a Session's refresh should be deferred for:
+
+Given the following example, the package will use a 1200s timeout for requests,
+but only trigger an update of the expiry time when the current time is within
+600s of the expiry:
+
+    timeout = 1200
+    timeout_trigger = 600
+
+The following timeline would occur:
+
+| time | Redis calls  | timeout | next threshold |
+| ---- | ------------ | ------- | -------------- |
+| 0    | `GET`+`SET`* | 1200    | 600            |
+| 1    | `GET`        | 1200    | 600            |
+| ...  |              |         |                |
+| 599  | `GET`        | 1200    | 600            |
+| 600  | `GET`+`SET`* | 1800    | 1200           |
+| 601  | `GET`        | 1800    | 1200           |
+| ...  |              |         |                |
+| 1199 | `GET`        | 1800    | 1200           |
+| 1200 | `GET`+`SET`* | 2400    | 1800           |
+
+* This method is compatible with setting a TTL in redis via `SETEX` or doing
+everything within Python if Redis is in a LRU mode
+
+The removes all calls to `EXPIRE` before the threshold is reached, which can be
+ a considerable savings in read-heavy situations.
+
+The caveat to this method: an expiry timestamp must be stored within the payload
+AND updating the timeout requires a `SET` operation.
+
+
+Feature - set_redis_ttl_readheavy
+=================================
+
+This is a new option in `1.4.2` which should improve performance on readheavy
+installations BUT may degrade performance on writeheavy installations.  This
+option will aggregate a GET+EXPIRE on every read.
+
+`set_redis_ttl_readheavy` requires the following:
+
+* a `timeout` value is set
+* `set_redis_ttl` is `True`
+* `timeout_trigger` is NOT set
+* `python_expires` is NOT True
+
+The default behavior of this library during a read-only request is this:
+
+* On session access, query Redis via `redis.GET {session_id}`
+* In a Pyramid callback, update Redis via `redis.EXPIRE {session_id} {expiry}`
+
+During a read-write:
+
+* On session access, query Redis via `redis.GET {session_id}`
+* In a Pyramid callback, update Redis via
+  `redis.SETEX {session_id} {payload} {expiry}`
+
+The new `set_redis_ttl_readheavy` changes this. If enabled during a read-only
+request, the behavior will be lighter on the Redis instance:
+
+* On session access, open a pipeline with two Redis commands:
+  `pipeline.GET {session_id}`,
+  `pipeline.EXPIRE {session_id} {expiry}`.
+* In a Pyramid callback, the duplicate expire is suppressed.
+
+However during a read-write, the activity will be:
+
+* On session access, open a pipeline with two Redis commands:
+  `pipeline.GET {session_id}`,
+  `pipeline.EXPIRE {session_id} {expiry}`.
+* In a Pyramid callback, update Redis via
+  `redis.SETEX {session_id} {payload} {expiry}`
+
+Read-heavy applications should see a slight performance bump via the pipeined
+GET+EXPIRE, however write-heavy applications are likely to see a performance
+degradation as it adds an extra EXPIRE to every request.
+
+
+Invalid Logging
+================
+
+The default behavior of this library is to silently create new session when bad
+session data is encountered, such as a cookie with an invalid id or corrupted
+datastore.  A graceful "new session" is the ideal situation for end-users.
+
+The problem with that strategy is that problems in code or your application
+stack can be hidden, and you might not know about a bad datastore.
+
+The 1.4 release introduces `func_invalid_logger` to the factory constructor.
+This can be used to track the invalid sessions that are safely caught and
+silently upgraded.
+
+How?  The package tracks why a session is invalid with variant classes of
+`pyramid_session_redis.exceptions.InvalidSession`.
+
+Specifically there are the following classes:
+
+* ``InvalidSession(Exception)``
+  Catchall base class
+* ``InvalidSession_NoSessionCookie(InvalidSession)``
+  The Session is invalid because there is no cookie.
+  This is the same as "new session".
+* ``InvalidSession_NotInBackend(InvalidSession)``
+  The Session id was not in the backend.
+* ``InvalidSession_DeserializationError(InvalidSession)``
+    Error deserializing.
+    This is raised if ``deserialized_fails_new`` is True. Otherwise the
+    exception is wrapped in a ``RawDeserializationError`` and raised without
+    being caught.
+* ``InvalidSession_PayloadTimeout(InvalidSession)``
+    The inner Python payload timed out.
+* ``InvalidSession_PayloadLegacy(InvalidSession)``
+    The Session is running on an earlier version.
+
+The factory accepts a `func_invalid_logger` callable argument. The input is the
+raised exception BEFORE a new cookie is generated, and will be the request and
+an instance of `InvalidSession`.
+
+    from pyramid_session_redis.exceptions import *
+    from my_statsd import new_statsd_client()
+
+    statsd_client = new_statsd_client()
+
+    def my_logger(request, raised_exception):
+        """
+        raised_exception will be an instance of InvalidSession
+        log the exception to statsd for metrics
+        """
+        if isinstance(raised_exception, InvalidSession_NoSessionCookie):
+            statsd_client.incr('invalid_session.NoSessionCookie')
+        elif isinstance(raised_exception, InvalidSession_NotInBackend):
+            statsd_client.incr('invalid_session.NotInBackend')
+        elif isinstance(raised_exception, InvalidSession_DeserializationError):
+            statsd_client.incr('invalid_session.DeserializationError')
+
+    factory = RedisSessionFactory(...
+                                  func_invalid_logger=my_logger,
+                                  ...
+                                  )
+
+The `func_invalid_logger` argument may be provided as a dotted-notation string
+in a configuration file.
+
+
+Uncaught Errors
+================
+
+The exception `pyramid_session_redis.exceptions.RawDeserializationError` will be
+raised if deserialization of a payload fails and `deserialized_fails_new` is not
+`True`. The first arg will be the caught exception. This allows for a standard
+error across multiple deserialization options.
+
+
+FAQ:
+=====
+
+Q. What serialization is used?
+------------------------------
+
+A. Serialization is used at two points
+
+* Serializing the Session data.
+  The server-side data serialization is handled by `pickle`. This Session data is
+  created on the server by your application and remains on the server. `pickle`
+  is safe to use in this context, as user-generated payloads can not be introduced
+  to these (de)serialization routines. If you wish to avoid `pickle`, or your
+  prefer to use another encoder, you can easily specify a different (de)serialization
+  routine such as a custom JSON, msgpack or pretty much anything else.
+
+* Serializing the `session_id` to encode into a signed cookie.
+  This library uses `WebOb.cookies.SignedSerializer` to securely manage a HMAC
+  signature of the `session_id` combined with a site-secret. The library allows
+  for a custom replacement to be provided as well.
+  
+  In the original library, the session id and signature were turned into a
+  cookie-safe value via `pickle` (de)serialization - a detail that remained in
+  this library through `<=v1.5.0`. This approach was identified as a security
+  risk, and was removed from this library starting in `v1.5.1`.  
+
+
+Examples
+========
+
+There is an example of using this package in `pyramid_session_multi`
+[examples/single_file_app.py](https://github.com/jvanasco/pyramid_session_multi/blob/main/examples/single_file_app.py).
+
+
+Further Reading:
+================
+
+For more information about Redis performance under Python please see an
+associated project:
+
+* https://github.com/jvanasco/dogpile_backend_redis_advanced
+
+To suport multiple Sessions under Pyramid
+
+* https://github.com/jvanasco/pyramid_session_multi
+
+Until Nov 2016 this was maintained as `jvanasco/pyramid_redis_sessions`
+
+* The main branch for `jvanasco/pyramid_redis_sessions` was "custom_deployment"
+* The branched named "main" is the upstream source from ericrasmussen
+
+As of Nov 2016, this was forked into it's own project to allow for distribution
+under PyPi.
+
+All support is handled via GitHub : https://github.com/jvanasco/pyramid_session_redis
+
+
+ToDo
+=====
+
+see `TODO.md`
+
+
+Changelog
+==========
+
+see `CHANGES.md`
+
+
+Support
+=======
+
+You can report bugs or open feature/support requests via GitHub
+
+* https://github.com/jvanasco/pyramid_session_redis
+
+
+License
+=======
+
+`pyramid_session_redis` is available under a FreeBSD-derived license. See
+`LICENSE.txt <https://github.com/jvanasco/pyramid_session_redis/blob/main/LICENSE.txt>`_
+for details.
```

### Comparing `pyramid_session_redis-1.6.3/src/pyramid_session_redis.egg-info/SOURCES.txt` & `pyramid_session_redis-1.7.0rc1/src/pyramid_session_redis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.py
 tox.ini
 src/pyramid_session_redis/__init__.py
 src/pyramid_session_redis/compat.py
 src/pyramid_session_redis/connection.py
 src/pyramid_session_redis/exceptions.py
 src/pyramid_session_redis/legacy.py
+src/pyramid_session_redis/py.typed
 src/pyramid_session_redis/session.py
 src/pyramid_session_redis/util.py
 src/pyramid_session_redis.egg-info/PKG-INFO
 src/pyramid_session_redis.egg-info/SOURCES.txt
 src/pyramid_session_redis.egg-info/dependency_links.txt
 src/pyramid_session_redis.egg-info/not-zip-safe
 src/pyramid_session_redis.egg-info/requires.txt
@@ -32,8 +33,9 @@
 src/pyramid_session_redis/docs/redis.rst
 tests/__init__.py
 tests/test_config.py
 tests/test_connection.py
 tests/test_factory.py
 tests/test_serializers.py
 tests/test_session.py
+tests/test_support.py
 tests/test_util.py
```

### Comparing `pyramid_session_redis-1.6.3/tests/__init__.py` & `pyramid_session_redis-1.7.0rc1/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # -*- coding: utf-8 -*-
+# stdlib
+import pickle
 
 # pypi
 from redis.exceptions import WatchError
 
-# local
-from pyramid_session_redis.compat import pickle
-
 
 # ==============================================================================
 
 
 class DummySessionState(object):
     please_persist = None
     please_refresh = None
 
 
 class DummySession(object):
-    def __init__(self, session_id, redis, timeout=300, serialize=pickle.dumps):
+    def __init__(
+        self,
+        session_id,
+        redis,
+        timeout=300,
+        serialize=pickle.dumps,
+    ):
         self.session_id = session_id
         self.redis = redis
         self.timeout = timeout
         self.serialize = serialize
         self.managed_dict = {}
         self.created = float()
         self._set_redis_ttl = True
@@ -36,15 +41,17 @@
 class DummyRedis(object):
     def __init__(self, raise_watcherror=False, **kw):
         self.url = None
         self.timeouts = {}
         self.store = {}
         self.__dict__.update(kw)
         self._history = []
-        self.pipeline = lambda: DummyPipeline(self.store, self, raise_watcherror)
+        self.pipeline = lambda: DummyPipeline(
+            self.store, self, raise_watcherror
+        )  # noqa: E501
 
     def _history_reset(self):
         # test method. fake. used for tests against the actual redis operations
         self._history = []
 
     @classmethod
     def from_url(cls, url, **opts):
@@ -116,15 +123,17 @@
     def expire(self, key, timeout):
         self._history.append(("expire", key, timeout))
         self._redis_con._history.append(("pipeline.expire", key, timeout))
 
     def setex(self, key, timeout, value, debug=None):
         self.store[key] = value
         self._history.append(("setex", key, timeout, debug))
-        self._redis_con._history.append(("pipeline.setex", key, timeout, value, debug))
+        self._redis_con._history.append(
+            ("pipeline.setex", key, timeout, value, debug)
+        )  # noqa: E501
 
     def watch(self, key):
         if self.raise_watcherror:
             raise WatchError
 
     def execute(self):
         pass
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_config.py` & `pyramid_session_redis-1.7.0rc1/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 
 # stdlib
 import unittest
 
 # pypi
 from pyramid import testing
-from pyramid.threadlocal import get_current_request
 from pyramid.exceptions import ConfigurationError
+from pyramid.threadlocal import get_current_request
 
 # local
 from pyramid_session_redis.exceptions import InvalidSession
-from pyramid_session_redis.exceptions import InvalidSession_DeserializationError
+from pyramid_session_redis.exceptions import (
+    InvalidSession_DeserializationError,
+)  # noqa: E501
 
 
 # ==============================================================================
 
 
 # dotted paths to dummy callables
 _id_path = "tests.test_config.dummy_id_generator"
@@ -67,32 +69,32 @@
         self.config.include("pyramid_session_redis")
         self.settings = self.config.registry.settings
 
     def tearDown(self):
         testing.tearDown()
 
     def test_includeme_serialize_deserialize(self):
-        request = get_current_request()
+        request = get_current_request()  # noqa: F841
         serialize = self.settings["redis.sessions.serialize"]
         deserialize = self.settings["redis.sessions.deserialize"]
         result = deserialize(serialize("test"))
         self.assertEqual(result, "test")
 
     def test_includeme_id_generator(self):
-        request = get_current_request()
+        request = get_current_request()  # noqa: F841
         generator = self.settings["redis.sessions.id_generator"]
         self.assertEqual(generator(), 42)
 
     def test_includeme_client_callable(self):
         request = get_current_request()
         get_client = self.settings["redis.sessions.client_callable"]
         self.assertEqual(get_client(request), "client")
 
     def test_includeme_invalid_logger(self):
-        request = get_current_request()
+        request = get_current_request()  # noqa: F841
         logging_func = self.settings["redis.sessions.func_invalid_logger"]
         raised_error = InvalidSession_DeserializationError("foo")
         # check to ensure this is an InvalidSession instance
         self.assertTrue(logging_func(raised_error))
 
 
 class Test_includeme_advanced(unittest.TestCase):
@@ -109,15 +111,16 @@
             # "redis.sessions.secret": "supersecret",  # don't include!
             # "redis.sessions.cookie_signer": "",  # don't include!
         }
         with self.assertRaises(ConfigurationError) as cm:
             self.config.include("pyramid_session_redis")
         self.assertEqual(
             cm.exception.args[0],
-            "One, and only one, of `redis.sessions.secret` and `redis.sessions.cookie_signer` must be provided.",
+            "One, and only one, of `redis.sessions.secret` and "
+            "`redis.sessions.cookie_signer` must be provided.",
         )
 
     def test_fails__cookiesigner__secret(self):
         request = testing.DummyRequest()
         self.config = testing.setUp(request=request)
         self.config.registry.settings = {
             "redis.sessions.db": 9,
@@ -129,15 +132,16 @@
             "redis.sessions.secret": "supersecret",
             "redis.sessions.cookie_signer": CustomCookieSigner(),
         }
         with self.assertRaises(ConfigurationError) as cm:
             self.config.include("pyramid_session_redis")
         self.assertEqual(
             cm.exception.args[0],
-            "One, and only one, of `redis.sessions.secret` and `redis.sessions.cookie_signer` must be provided.",
+            "One, and only one, of `redis.sessions.secret` and "
+            "`redis.sessions.cookie_signer` must be provided.",
         )
 
     def test__cookiesigner__custom(self):
         request = testing.DummyRequest()
         self.config = testing.setUp(request=request)
         self.config.registry.settings = {
             "redis.sessions.db": 9,
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_connection.py` & `pyramid_session_redis-1.7.0rc1/tests/test_connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import unittest
 
 # pypi
 from pyramid import testing
 
 # local
 from pyramid_session_redis.connection import get_default_connection
-
-# local test suite
 from . import DummyRedis
 
 
 # ==============================================================================
 
 
 class TestConnection(unittest.TestCase):
@@ -22,27 +20,31 @@
         self.request = testing.DummyRequest()
 
     def tearDown(self):
         testing.tearDown(self)
 
     def test_get_default_connection(self):
         options = dict(host="localhost", port=999)
-        inst = get_default_connection(self.request, redis_client=DummyRedis, **options)
+        inst = get_default_connection(
+            self.request, client_class=DummyRedis, **options
+        )  # noqa: E501
         self.assertEqual(inst.host, "localhost")
         self.assertEqual(inst.port, 999)
 
     def test_get_default_connection_with_url(self):
         url = "redis://username:password@localhost:6379/0"
-        inst = get_default_connection(self.request, url=url, redis_client=DummyRedis)
+        inst = get_default_connection(
+            self.request, url=url, client_class=DummyRedis
+        )  # noqa: E501
         self.assertEqual(inst.url, url)
 
     def test_get_default_connection_url_removes_duplicates(self):
         options = dict(host="localhost", port=999, password="password", db=5)
         url = "redis://username:password@localhost:6379/0"
         inst = get_default_connection(
-            self.request, url=url, redis_client=DummyRedis, **options
+            self.request, url=url, client_class=DummyRedis, **options
         )
         self.assertEqual(inst.url, url)
         self.assertNotIn("password", inst.opts)
         self.assertNotIn("host", inst.opts)
         self.assertNotIn("port", inst.opts)
         self.assertNotIn("db", inst.opts)
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_factory.py` & `pyramid_session_redis-1.7.0rc1/tests/test_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function
 
 # stdlib
 import datetime
-import itertools
-import pdb
-import pprint
+import pickle
 import re
 import unittest
 
 # pypi
 from pyramid import testing
 from pyramid.interfaces import ISession
 import webob
 from webob.cookies import SignedSerializer
 from zope.interface.verify import verifyObject
 
 # local
-from pyramid_session_redis import RedisSessionFactory
 from pyramid_session_redis import check_response_allow_cookies
+from pyramid_session_redis import RedisSessionFactory
 from pyramid_session_redis import session_factory_from_settings
-from pyramid_session_redis.compat import pickle
 from pyramid_session_redis.exceptions import InvalidSession
 from pyramid_session_redis.exceptions import InvalidSession_DeserializationError
 from pyramid_session_redis.exceptions import InvalidSession_NoSessionCookie
 from pyramid_session_redis.exceptions import InvalidSession_NotInBackend
 from pyramid_session_redis.exceptions import InvalidSession_PayloadLegacy
 from pyramid_session_redis.exceptions import InvalidSession_PayloadTimeout
 from pyramid_session_redis.exceptions import RawDeserializationError
 from pyramid_session_redis.session import RedisSession
-from pyramid_session_redis.util import LAZYCREATE_SESSION
 from pyramid_session_redis.util import _NullSerializer
 from pyramid_session_redis.util import create_unique_session_id
 from pyramid_session_redis.util import encode_session_payload
 from pyramid_session_redis.util import int_time
-
-# local test suite
+from pyramid_session_redis.util import LazyCreateSession
 from . import DummyRedis
 from .test_config import dummy_id_generator
 
 
 # ==============================================================================
 
 
@@ -56,15 +51,14 @@
 
 class _TestRedisSessionFactoryCore(unittest.TestCase):
     def _makeOne(self, request, secret="secret", **kw):
         session = RedisSessionFactory(secret, **kw)(request)
         return session
 
     def _makeOneSession(self, redis, session_id, **kw):
-
         _set_redis_ttl_onexit = False
         if (kw.get("timeout") and kw.get("set_redis_ttl")) and (
             not kw.get("timeout_trigger")
             and not kw.get("python_expires")
             and not kw.get("set_redis_ttl_readheavy")
         ):
             _set_redis_ttl_onexit = True
@@ -99,15 +93,14 @@
     def _set_session_cookie(
         self, request, session_id, cookie_name="session", secret="secret"
     ):
         cookieval = self._serialize(session_id, secret=secret)
         request.cookies[cookie_name] = cookieval
 
     def _make_request(self, request_old=None):
-
         if request_old:
             # grab the registry data to persist, otherwise it gets discarded
             # and transfer it to a new request
             _redis_sessions = request_old.registry._redis_sessions
             request = testing.DummyRequest()
             request.registry._redis_sessions = _redis_sessions
         else:
@@ -725,15 +718,17 @@
         for _set in _test_matrix:
             with self.assertRaises(ValueError) as cm_expected_exception:
                 _settings = {
                     "redis.sessions.secret": "secret",  # required
                     "redis.sessions.%s" % _set[0]: _set[2],
                     "redis.sessions.%s" % _set[1]: _set[2],
                 }
-                session_using_old = session_factory_from_settings(_settings)
+                session_using_old = session_factory_from_settings(  # noqa: F841
+                    _settings
+                )
             exception_wrapper = cm_expected_exception.exception
             wrapped_exception = exception_wrapper.args[0]
             assert wrapped_exception == "Submit only one of `%s`, `%s`" % (
                 _set[0],
                 _set[1],
             )
 
@@ -950,15 +945,15 @@
 
         def _insert_new_session():
             """
             drop a session into our redis
             this requires a `request` but will only use a DummySession
             """
             request = self._make_request()
-            session_existing = self._set_up_session_in_Redis_and_makeOne(
+            session_existing = self._set_up_session_in_Redis_and_makeOne(  # noqa: F841
                 request, session_id, session_dict={"visited": True}, **session_args
             )
             return request
 
         # insert the session
         request1 = _insert_new_session()
         request = self._load_cookie_session_in_new_request(
@@ -989,15 +984,14 @@
         request.session.redis.store[_session_id] = _session_serialized
         request.session._resync()
 
 
 class TestRedisSessionFactory_expiries_v1_4_x(
     _TestRedisSessionFactoryCore, _TestRedisSessionFactoryCore_UtilsNew
 ):
-
     # args are used 2x: for NEW and EXISTING session tests
 
     _args_timeout_trigger_pythonExpires_setRedisTtl = {
         "timeout": 1200,
         "timeout_trigger": 600,
         "python_expires": True,
         "set_redis_ttl": True,
@@ -2172,28 +2166,28 @@
 
     def test_scenario_flow__noCookie_b(self):
         """no cookie created when accessing a session attrib"""
         # session_args should behave the same for all
         session_args = self._args_timeout_trigger_pythonExpires_setRedisTtl
         request = self._make_request()
         request.session = self._makeOne(request, **session_args)
-        v = request.session.get("foo", None)
+        v = request.session.get("foo", None)  # noqa: F841
         response = webob.Response()
         request._process_response_callbacks(response)
         request._process_finished_callbacks()
         set_cookie_headers = response.headers.getall("Set-Cookie")
         self.assertEqual(len(set_cookie_headers), 0)
 
     def test_scenario_flow__noCookie_c(self):
         """no cookie created when accessing a session_id"""
         # session_args should behave the same for all
         session_args = self._args_timeout_trigger_pythonExpires_setRedisTtl
         request = self._make_request()
         request.session = self._makeOne(request, **session_args)
-        session_id = request.session.session_id
+        session_id = request.session.session_id  # noqa: F841
         response = webob.Response()
         request._process_response_callbacks(response)
         request._process_finished_callbacks()
         set_cookie_headers = response.headers.getall("Set-Cookie")
         self.assertEqual(len(set_cookie_headers), 0)
 
     def test_scenario_flow__cookie_a(self):
@@ -2201,25 +2195,25 @@
         # session_args should behave the same for all
         session_args = self._args_timeout_trigger_pythonExpires_setRedisTtl
         request = self._make_request()
         request.session = self._makeOne(request, **session_args)
 
         # session_id is non-existant on create
         session_id = request.session.session_id
-        self.assertIs(session_id, LAZYCREATE_SESSION)
+        self.assertIs(session_id, LazyCreateSession)
         request.session["a"] = 1
 
         # session_id is non-existant until necessary
         session_id = request.session.session_id
-        self.assertIs(session_id, LAZYCREATE_SESSION)
+        self.assertIs(session_id, LazyCreateSession)
 
         # insist this is necessary
         request.session.ensure_id()
         session_id = request.session.session_id
-        self.assertIsNot(session_id, LAZYCREATE_SESSION)
+        self.assertIsNot(session_id, LazyCreateSession)
 
         response = webob.Response()
         request._process_response_callbacks(response)
         request._process_finished_callbacks()
         set_cookie_headers = response.headers.getall("Set-Cookie")
         self.assertEqual(len(set_cookie_headers), 1)
 
@@ -2228,28 +2222,28 @@
         # session_args should behave the same for all
         session_args = self._args_timeout_trigger_pythonExpires_setRedisTtl
         request = self._make_request()
         request.session = self._makeOne(request, **session_args)
 
         # session_id is non-existant on create
         session_id = request.session.session_id
-        self.assertIs(session_id, LAZYCREATE_SESSION)
+        self.assertIs(session_id, LazyCreateSession)
         request.session["a"] = 1
 
         # session_id is non-existant until necessary
         session_id = request.session.session_id
-        self.assertIs(session_id, LAZYCREATE_SESSION)
+        self.assertIs(session_id, LazyCreateSession)
 
         response = webob.Response()
         request._process_response_callbacks(response)
         request._process_finished_callbacks()
 
         # session_id should have created after callbacks
         session_id = request.session.session_id
-        self.assertIsNot(session_id, LAZYCREATE_SESSION)
+        self.assertIsNot(session_id, LazyCreateSession)
 
         set_cookie_headers = response.headers.getall("Set-Cookie")
         self.assertEqual(len(set_cookie_headers), 1)
 
 
 class TestRedisSessionFactory_loggedExceptions(
     _TestRedisSessionFactoryCore, _TestRedisSessionFactoryCore_UtilsNew
@@ -2279,55 +2273,53 @@
             "secret", func_invalid_logger=func_invalid_logger, **factory_args
         )
         return factory
 
     # -----
 
     def test_logger_InvalidSession_NoSessionCookie(self):
-
         func_invalid_logger_counts = self._new_loggerData()
 
         def func_invalid_logger(request, raised):
             assert isinstance(raised, InvalidSession)
             func_invalid_logger_counts["InvalidSession"] += 1
             assert isinstance(raised, InvalidSession_NoSessionCookie)
             func_invalid_logger_counts["InvalidSession_NoSessionCookie"] += 1
 
         factory = self._new_loggerFactory(func_invalid_logger=func_invalid_logger)
 
         request = self._make_request()
-        redis = request.registry._redis_sessions
-        session = factory(request)
+        redis = request.registry._redis_sessions  # noqa: F841
+        session = factory(request)  # noqa: F841
         # validate
         self.validate_loggerData(
             func_invalid_logger_counts,
             InvalidSession=1,
             InvalidSession_NoSessionCookie=1,
         )
 
     # -----
 
     def test_logger_InvalidSession_NotInBackend(self):
-
         func_invalid_logger_counts = self._new_loggerData()
 
         def func_invalid_logger(request, raised):
             assert isinstance(raised, InvalidSession)
             func_invalid_logger_counts["InvalidSession"] += 1
             assert isinstance(raised, InvalidSession_NotInBackend)
             func_invalid_logger_counts["InvalidSession_NotInBackend"] += 1
 
         factory = self._new_loggerFactory(func_invalid_logger=func_invalid_logger)
 
         # this session isn't tied to our factory.
         request = self._make_request()
-        redis = request.registry._redis_sessions
+        redis = request.registry._redis_sessions  # noqa: F841
 
         self._set_session_cookie(request=request, session_id="no_backend")
-        session = factory(request)
+        session = factory(request)  # noqa: F841
         # validate
         self.validate_loggerData(
             func_invalid_logger_counts, InvalidSession=1, InvalidSession_NotInBackend=1
         )
 
     # -----
 
@@ -2350,15 +2342,15 @@
         redis = request.registry._redis_sessions
         assert "existing_session" in redis.store
 
         # take of off the last 5 chars
         redis.store["existing_session"] = redis.store["existing_session"][:-5]
 
         # new request
-        session = factory(request)
+        session = factory(request)  # noqa: F841
         # validate
         self.validate_loggerData(
             func_invalid_logger_counts,
             InvalidSession=1,
             InvalidSession_DeserializationError=1,
         )
 
@@ -2388,15 +2380,15 @@
         # make it 10 seconds earlier
         deserialized["x"] = deserialized["x"] - 10
         deserialized["c"] = deserialized["c"] - 10
         reserialized = request.session.serialize(deserialized)
         redis.store["existing_session"] = reserialized
 
         # new request, which should trigger a timeout
-        session = factory(request)
+        session = factory(request)  # noqa: F841
 
         # validate
         self.validate_loggerData(
             func_invalid_logger_counts,
             InvalidSession=1,
             InvalidSession_PayloadTimeout=1,
         )
@@ -2427,23 +2419,23 @@
 
         # make it 1 version earlier
         deserialized["v"] = deserialized["v"] - 1
         reserialized = request.session.serialize(deserialized)
         redis.store["existing_session"] = reserialized
 
         # new request, which should trigger a legacy format issue
-        session = factory(request)
+        session = factory(request)  # noqa: F841
 
         # validate
         self.validate_loggerData(
             func_invalid_logger_counts, InvalidSession=1, InvalidSession_PayloadLegacy=1
         )
 
     def test_deserialized_error_raw(self):
-        func_invalid_logger_counts = self._new_loggerData()
+        func_invalid_logger_counts = self._new_loggerData()  # noqa: F841
 
         def func_invalid_logger(request, raised):
             raise ValueError("this should not be run")
 
         factory = self._new_loggerFactory(
             func_invalid_logger=func_invalid_logger,
             factory_args={"deserialized_fails_new": False},
@@ -2456,37 +2448,37 @@
         redis.store["existing_session"] = redis.store["existing_session"][:-5]
 
         # new request should raise a raw RawDeserializationError
         with self.assertRaises(RawDeserializationError) as cm_expected_exception:
             factory(request)
 
         exception_wrapper = cm_expected_exception.exception
-        wrapped_exception = exception_wrapper.args[0]
+        wrapped_exception = exception_wrapper.args[0]  # noqa: F841
 
         # we are using picke, so it should be:
         self.assertEqual(request.session.deserialize, pickle.loads)
         # py2.7-3.7: exceptions.EOFError
         # py3.8: pickle.UnpicklingError
         self.assertIsInstance(
             exception_wrapper.args[0], (EOFError, pickle.UnpicklingError)
         )
 
 
 class TestRedisSessionFactory_Invalid(unittest.TestCase):
     def test_fails__no_cookiesigner__no_secret(self):
         with self.assertRaises(ValueError) as cm:
-            factory = RedisSessionFactory(secret=None)
+            factory = RedisSessionFactory(secret=None)  # noqa: F841
         self.assertEqual(
             cm.exception.args[0],
             "One, and only one, of `secret` and `cookie_signer` must be provided.",
         )
 
     def test_fails__cookiesigner__secret(self):
         with self.assertRaises(ValueError) as cm:
-            factory = RedisSessionFactory(
+            factory = RedisSessionFactory(  # noqa: F841
                 secret="secret", cookie_signer=CustomCookieSigner()
             )
         self.assertEqual(
             cm.exception.args[0],
             "One, and only one, of `secret` and `cookie_signer` must be provided.",
         )
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_serializers.py` & `pyramid_session_redis-1.7.0rc1/tests/test_serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,97 +4,122 @@
 # stdlib
 import unittest
 
 # pypi
 from webob.cookies import SignedSerializer
 
 # local
+from pyramid_session_redis.exceptions import InvalidSessionId_Serialization
 from pyramid_session_redis.legacy import GracefulCookieSerializer
 from pyramid_session_redis.legacy import LegacyCookieSerializer
 from pyramid_session_redis.util import _NullSerializer
 
 
 # ==============================================================================
 
 
 class TestNullSerializer(unittest.TestCase):
-    def test_roundtrip_string(self):
+    def test_string(self):
+        "this should be a roundtrip"
         serializer = _NullSerializer()
-        data = "foo"
-        _serialized = serializer.dumps(data)
-        self.assertEqual(data, serializer.loads(_serialized))
+        data_in = "foo"
+        data_out = data_in
+        _serialized = serializer.dumps(data_in)
+        self.assertEqual(data_out, serializer.loads(_serialized))
 
-    def test_roundtrip_int(self):
+    def test_int(self):
+        "this should fail; _NullSerializer requires a str"
         serializer = _NullSerializer()
-        data = 100
-        _serialized = serializer.dumps(data)
-        self.assertEqual(data, serializer.loads(_serialized))
+        data_in = 100
+        self.assertRaises(InvalidSessionId_Serialization, serializer.dumps, data_in)
+
+    def test_bytes(self):
+        "this should fail; _NullSerializer requires a str"
+        serializer = _NullSerializer()
+        data_in = b"foo"
+        self.assertRaises(InvalidSessionId_Serialization, serializer.dumps, data_in)
 
 
 class TestCookieSerialization(unittest.TestCase):
     def _makeOne_default(self, secret):
         cookie_signer = SignedSerializer(
-            secret, "pyramid_session_redis.", "sha512", serializer=_NullSerializer()
+            secret,
+            "pyramid_session_redis.",
+            "sha512",
+            serializer=_NullSerializer(),
         )
         return cookie_signer
 
     def _makeOne_legacy(self, secret):
         cookie_signer = LegacyCookieSerializer(secret)
         return cookie_signer
 
     def _makeOne_graceful(self, secret, logging_hook=None):
-        cookie_signer = GracefulCookieSerializer(secret, logging_hook=logging_hook)
+        cookie_signer = GracefulCookieSerializer(
+            secret,
+            logging_hook=logging_hook,
+        )
         return cookie_signer
 
     def test_roundtrip_default(self):
         secret = "foo"
-        session_id = "123"
+        session_id = "session_id:123"
         cookie_signer = self._makeOne_default(secret)
         _serialized = cookie_signer.dumps(session_id)
         self.assertEqual(session_id, cookie_signer.loads(_serialized))
 
     def test_roundtrip_legacy(self):
         secret = "foo"
-        session_id = "123"
+        session_id = "session_id:123"
         cookie_signer = self._makeOne_legacy(secret)
         _serialized = cookie_signer.dumps(session_id)
         self.assertEqual(session_id, cookie_signer.loads(_serialized))
 
     def test_incompatible(self):
         secret = "foo"
-        session_id = "123"
+        session_id = "session_id:123"
         cookie_signer_current = self._makeOne_default(secret)
         cookie_signer_legacy = self._makeOne_legacy(secret)
         _serialized_current = cookie_signer_current.dumps(session_id)
         _serialized_legacy = cookie_signer_legacy.dumps(session_id)
         self.assertNotEqual(_serialized_current, _serialized_legacy)
-        self.assertRaises(ValueError, cookie_signer_legacy.loads, _serialized_current)
-        self.assertRaises(ValueError, cookie_signer_current.loads, _serialized_legacy)
+        self.assertRaises(
+            ValueError, cookie_signer_legacy.loads, _serialized_current
+        )  # noqa: E501
+        self.assertRaises(
+            ValueError, cookie_signer_current.loads, _serialized_legacy
+        )  # noqa: E501
 
     def test_graceful(self):
         secret = "foo"
-        session_id = "123"
+        session_id = "session_id:123"
         cookie_signer_current = self._makeOne_default(secret)
         cookie_signer_legacy = self._makeOne_legacy(secret)
         cookie_signer_graceful = self._makeOne_graceful(secret)
 
         _serialized_current = cookie_signer_current.dumps(session_id)
         _serialized_legacy = cookie_signer_legacy.dumps(session_id)
         _serialized_graceful = cookie_signer_graceful.dumps(session_id)
 
         self.assertEqual(_serialized_current, _serialized_graceful)
         self.assertNotEqual(_serialized_legacy, _serialized_graceful)
 
-        self.assertEqual(session_id, cookie_signer_graceful.loads(_serialized_current))
-        self.assertEqual(session_id, cookie_signer_graceful.loads(_serialized_graceful))
-        self.assertEqual(session_id, cookie_signer_graceful.loads(_serialized_legacy))
+        self.assertEqual(
+            session_id, cookie_signer_graceful.loads(_serialized_current)
+        )  # noqa: E501
+        self.assertEqual(
+            session_id, cookie_signer_graceful.loads(_serialized_graceful)
+        )  # noqa: E501
+        self.assertEqual(
+            session_id, cookie_signer_graceful.loads(_serialized_legacy)
+        )  # noqa: E501
 
     def test_graceful_hooks(self):
         secret = "foo"
-        session_id = "123"
+        session_id = "session_id:123"
 
         class LoggingHook(object):
             def __init__(self):
                 self._attempts_global = []
                 self._attempts = []
                 self._successes = []
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_session.py` & `pyramid_session_redis-1.7.0rc1/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function
 
 # stdlib
 import itertools
-import pdb
-import pprint
+import pickle
 import time
+from typing import Optional
 import unittest
 
 # local
-from pyramid_session_redis.compat import pickle
-from pyramid_session_redis.exceptions import InvalidSession
 from pyramid_session_redis.exceptions import InvalidSession_PayloadLegacy
 from pyramid_session_redis.exceptions import InvalidSession_PayloadTimeout
 from pyramid_session_redis.session import RedisSession
-from pyramid_session_redis.util import LAZYCREATE_SESSION
 from pyramid_session_redis.util import encode_session_payload
 from pyramid_session_redis.util import int_time
-
-# local test suite
+from pyramid_session_redis.util import LazyCreateSession
 from . import DummyRedis
 
 
 # ==============================================================================
 
 
 class TestRedisSession(unittest.TestCase):
@@ -400,30 +396,30 @@
     def test_session_id_access_after_invalidate_creates_new_session(self):
         inst = self._set_up_session_in_Redis_and_makeOne()
         first_session_id = inst.session_id
         inst.invalidate()
 
         # 1.4.x+| session_id defaults to a LAZYCREATE
         self.assertIs(inst.session_id_safecheck, None)
-        self.assertIs(inst.session_id, LAZYCREATE_SESSION)
+        self.assertIs(inst.session_id, LazyCreateSession)
 
         second_session_id = inst.session_id
         self.assertNotEqual(second_session_id, first_session_id)
         self.assertIs(bool(second_session_id), True)
 
     def test_managed_dict_access_after_invalidate_creates_new_session(self):
         inst = self._set_up_session_in_Redis_and_makeOne()
         first_session_id = inst.session_id
         inst.invalidate()
         inst.managed_dict  # access
 
         # 1.4.x+| session_id defaults to a LAZYCREATE
         # 1.4.x+| session_id is only created via ensure_id()
         self.assertIs(inst.session_id_safecheck, None)
-        self.assertIs(inst.session_id, LAZYCREATE_SESSION)
+        self.assertIs(inst.session_id, LazyCreateSession)
         inst.ensure_id()
 
         # ORIGINALLY
         # .session_id attribute access also creates a new session after
         # invalidate, so just asserting .session_id is not enough to prove that
         # a new session was created after .managed_dict access. Here we note
         # down the session_ids in Redis right after .managed_dict access for an
@@ -439,15 +435,15 @@
         first_session_id = inst.session_id
         inst.invalidate()
         inst.created  # access
 
         # 1.4.x+| session_id defaults to a LAZYCREATE
         # 1.4.x+| session_id is only created via ensure_id()
         self.assertIs(inst.session_id_safecheck, None)
-        self.assertIs(inst.session_id, LAZYCREATE_SESSION)
+        self.assertIs(inst.session_id, LazyCreateSession)
         inst.ensure_id()
 
         # ORIGINALLY
         # .session_id attribute access also creates a new session after
         # invalidate, so just asserting .session_id was not enough to prove that
         # a new session was created after .created access. Here we noted down
         # the session_ids in Redis right after .created access for an
@@ -463,15 +459,15 @@
         first_session_id = inst.session_id
         inst.invalidate()
         inst.timeout  # access
 
         # 1.4.x+| session_id defaults to a LAZYCREATE
         # 1.4.x+| session_id is only created via ensure_id()
         self.assertIs(inst.session_id_safecheck, None)
-        self.assertIs(inst.session_id, LAZYCREATE_SESSION)
+        self.assertIs(inst.session_id, LazyCreateSession)
         inst.ensure_id()
 
         # ORIGINALLY:
         # .session_id attribute access also creates a new session after
         # invalidate, so just asserting .session_id is not enough to prove that
         # a new session was created after .timeout access. Here we note down
         # the session_ids in Redis right after .timeout access for an
@@ -487,15 +483,15 @@
         first_session_id = inst.session_id
         inst.invalidate()
         inst.new  # access
 
         # 1.4.x+| session_id defaults to a LAZYCREATE
         # 1.4.x+| session_id is only created via ensure_id()
         self.assertIs(inst.session_id_safecheck, None)
-        self.assertIs(inst.session_id, LAZYCREATE_SESSION)
+        self.assertIs(inst.session_id, LazyCreateSession)
         inst.ensure_id()
 
         # ORIGINALLY
         # .session_id attribute access also creates a new session after
         # invalidate, so just asserting .session_id is not enough to prove that
         # a new session was created after .created access. Here we note down
         # session_ids in Redis right after .new access for an additional check.
@@ -634,15 +630,14 @@
         set_redis_ttl=True,
         deserialized_fails_new=None,
         timeout_trigger=None,
         timeout=1200,
         python_expires=True,
         set_redis_ttl_readheavy=None,
     ):
-
         _set_redis_ttl_onexit = False
         if (timeout and set_redis_ttl) and (
             not timeout_trigger and not python_expires and not set_redis_ttl_readheavy
         ):
             _set_redis_ttl_onexit = True
 
         return RedisSession(
@@ -757,21 +752,21 @@
         _session_id = session.session_id
         _session_data = session.redis.store[_session_id]
         _session_serialized = deserialize(_session_data)
         return _session_serialized
 
 
 class _TestRedisSessionNew__MIXIN_A(object):
-    PYTHON_EXPIRES = None
-    set_redis_ttl = None
-    set_redis_ttl_readheavy = None
-    session_id = "session_id"
-    timeout = 3
-    timeout_trigger = 6
-    adjusted_timeout = 6
+    PYTHON_EXPIRES: Optional[bool] = None
+    set_redis_ttl: Optional[bool] = None
+    set_redis_ttl_readheavy: Optional[bool] = None
+    session_id: str = "session_id"
+    timeout: Optional[int] = 3
+    timeout_trigger: Optional[int] = 6
+    adjusted_timeout: Optional[int] = 6
 
     def _session_new(self):
         session = self._set_up_session_in_Redis_and_makeOne(
             session_id=self.session_id,
             new=True,
             timeout=self.timeout,
             set_redis_ttl=self.set_redis_ttl,
@@ -977,15 +972,15 @@
         check that ``exceptions.InvalidSession_PayloadLegacy`` is raised if a previous version is detected
         """
         new = True
         timeout = 60
         set_redis_ttl = False
         session_version = -1
         with self.assertRaises(InvalidSession_PayloadLegacy):
-            session = self._set_up_session_in_Redis_and_makeOne(
+            session = self._set_up_session_in_Redis_and_makeOne(  # noqa: F841
                 session_id=self.session_id,
                 new=new,
                 timeout=timeout,
                 set_redis_ttl=set_redis_ttl,
                 session_version=session_version,
             )
         return
@@ -995,15 +990,15 @@
         check that ``exceptions.InvalidSession_PayloadTimeout`` is raised if we timed out
         """
         new = True
         timeout = 60
         set_redis_ttl = False
         expires = int_time() - timeout - 1
         with self.assertRaises(InvalidSession_PayloadTimeout):
-            session = self._set_up_session_in_Redis_and_makeOne(
+            session = self._set_up_session_in_Redis_and_makeOne(  # noqa: F841
                 session_id=self.session_id,
                 new=new,
                 timeout=timeout,
                 set_redis_ttl=set_redis_ttl,
                 expires=expires,
             )
 
@@ -1035,15 +1030,15 @@
         serialized_1 = (
             session.from_redis()
         )  # this executes a second get, the session doesn't save the raw value
 
         timeout_1 = serialized_1["t"]
         self.assertEqual(timeout_1, self.timeout)
         timestamp_created = serialized_1["c"]
-        timestamp_expiry_initial = serialized_1["x"]
+        timestamp_expiry_initial = serialized_1["x"]  # noqa: F841
         if not variant:
             session.adjust_session_timeout(self.adjusted_timeout)
         else:
             getattr(session, variant)(self.adjusted_timeout)
         session._deferred_callback(None)  # trigger the real session's set/setex
         self.assertEqual(len(session.redis._history), 3)
         self.assertEqual(session.redis._history[0][0], "get")
@@ -1096,15 +1091,15 @@
         session["FOO"] = "1"
         session._deferred_callback(None)  # trigger the real session's set/setex
 
         serialized_1 = session.from_redis()
         timeout_1 = serialized_1["t"]
         self.assertEqual(timeout_1, self.timeout)
         timestamp_created = serialized_1["c"]
-        timestamp_expiry_initial = serialized_1["x"]
+        timestamp_expiry_initial = serialized_1["x"]  # noqa: F841
         if not variant:
             session.adjust_session_timeout(self.adjusted_timeout)
         else:
             getattr(session, variant)(self.adjusted_timeout)
         session._deferred_callback(None)  # trigger the real session's set/setex
 
         serialized_2 = session.from_redis()
@@ -1153,15 +1148,15 @@
         )
 
         sleeptime = session2_redis["x"] - int(time.time()) + 1
         print("sleeping for ", sleeptime)
         time.sleep(sleeptime)
 
         with self.assertRaises(InvalidSession_PayloadTimeout):
-            session3 = self._makeOne(
+            session3 = self._makeOne(  # noqa: F841
                 session.redis,
                 self.session_id,
                 True,  # new
                 func_new_session,
                 set_redis_ttl=self.set_redis_ttl,
                 timeout_trigger=self.timeout_trigger,
                 timeout=self.timeout,
```

### Comparing `pyramid_session_redis-1.6.3/tests/test_util.py` & `pyramid_session_redis-1.7.0rc1/tests/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # stdlib
 import itertools
-import time
 import unittest
 
 # local
-from pyramid_session_redis.compat import pickle
 from pyramid_session_redis.util import _generate_session_id
 from pyramid_session_redis.util import _insert_session_id_if_unique
 from pyramid_session_redis.util import _parse_settings
 from pyramid_session_redis.util import create_unique_session_id
 from pyramid_session_redis.util import int_time
 from pyramid_session_redis.util import persist
 from pyramid_session_redis.util import prefixed_id
 from pyramid_session_redis.util import refresh
-
-# local test suite
-from . import DummyRedis, DummySession
+from . import DummyRedis
+from . import DummySession
 
 
 # ==============================================================================
 
 
 class Test_parse_settings(unittest.TestCase):
     def _makeOne(self, settings):
@@ -123,15 +120,20 @@
 
 
 class Test_create_unique_session_id(unittest.TestCase):
     def _makeOne(self, redis=DummyRedis(), timeout=300):
         serialize = lambda x: x
         ids = itertools.count(start=1, step=1)
         generator = lambda: next(ids)
-        return create_unique_session_id(redis, timeout, serialize, generator=generator)
+        return create_unique_session_id(
+            redis,
+            timeout,
+            serialize,
+            generator=generator,
+        )
 
     def test_id_is_unique(self):
         result = self._makeOne()
         self.assertEqual(result, 1)
 
     def test_id_not_unique(self):
         redis = DummyRedis()
```

