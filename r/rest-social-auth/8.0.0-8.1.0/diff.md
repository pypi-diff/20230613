# Comparing `tmp/rest_social_auth-8.0.0.tar.gz` & `tmp/rest_social_auth-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_social_auth-8.0.0.tar", last modified: Sat Nov 19 13:28:30 2022, max compression
+gzip compressed data, was "rest_social_auth-8.1.0.tar", last modified: Tue Jun 13 21:01:13 2023, max compression
```

## Comparing `rest_social_auth-8.0.0.tar` & `rest_social_auth-8.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 stalk      (501) staff       (20)        0 2022-11-19 13:28:30.429772 rest_social_auth-8.0.0/
--rw-r--r--   0 stalk      (501) staff       (20)     1072 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/LICENSE
--rw-r--r--   0 stalk      (501) staff       (20)       68 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/MANIFEST.in
--rw-r--r--   0 stalk      (501) staff       (20)    29731 2022-11-19 13:28:30.430050 rest_social_auth-8.0.0/PKG-INFO
--rw-r--r--   0 stalk      (501) staff       (20)    18480 2022-11-19 13:24:37.000000 rest_social_auth-8.0.0/README.md
--rw-r--r--   0 stalk      (501) staff       (20)     4143 2022-11-19 13:24:33.000000 rest_social_auth-8.0.0/RELEASE_NOTES.md
--rw-r--r--   0 stalk      (501) staff       (20)      101 2022-11-19 00:52:06.000000 rest_social_auth-8.0.0/requirements.txt
-drwxr-xr-x   0 stalk      (501) staff       (20)        0 2022-11-19 13:28:30.428972 rest_social_auth-8.0.0/rest_social_auth/
--rw-r--r--   0 stalk      (501) staff       (20)       43 2022-11-19 13:26:36.000000 rest_social_auth-8.0.0/rest_social_auth/__init__.py
--rw-r--r--   0 stalk      (501) staff       (20)     4354 2022-11-19 00:52:06.000000 rest_social_auth-8.0.0/rest_social_auth/serializers.py
--rw-r--r--   0 stalk      (501) staff       (20)      634 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/strategy.py
--rw-r--r--   0 stalk      (501) staff       (20)      476 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/urls_jwt_pair.py
--rw-r--r--   0 stalk      (501) staff       (20)      494 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/urls_jwt_sliding.py
--rw-r--r--   0 stalk      (501) staff       (20)      465 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/urls_knox.py
--rw-r--r--   0 stalk      (501) staff       (20)      234 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/urls_session.py
--rw-r--r--   0 stalk      (501) staff       (20)      460 2022-11-18 17:05:12.000000 rest_social_auth-8.0.0/rest_social_auth/urls_token.py
--rw-r--r--   0 stalk      (501) staff       (20)    12139 2022-11-19 13:24:07.000000 rest_social_auth-8.0.0/rest_social_auth/views.py
-drwxr-xr-x   0 stalk      (501) staff       (20)        0 2022-11-19 13:28:30.429672 rest_social_auth-8.0.0/rest_social_auth.egg-info/
--rw-r--r--   0 stalk      (501) staff       (20)    29731 2022-11-19 13:28:30.000000 rest_social_auth-8.0.0/rest_social_auth.egg-info/PKG-INFO
--rw-r--r--   0 stalk      (501) staff       (20)      562 2022-11-19 13:28:30.000000 rest_social_auth-8.0.0/rest_social_auth.egg-info/SOURCES.txt
--rw-r--r--   0 stalk      (501) staff       (20)        1 2022-11-19 13:28:30.000000 rest_social_auth-8.0.0/rest_social_auth.egg-info/dependency_links.txt
--rw-r--r--   0 stalk      (501) staff       (20)      101 2022-11-19 13:28:30.000000 rest_social_auth-8.0.0/rest_social_auth.egg-info/requires.txt
--rw-r--r--   0 stalk      (501) staff       (20)       17 2022-11-19 13:28:30.000000 rest_social_auth-8.0.0/rest_social_auth.egg-info/top_level.txt
--rw-r--r--   0 stalk      (501) staff       (20)      199 2022-11-19 13:28:30.430369 rest_social_auth-8.0.0/setup.cfg
--rw-r--r--   0 stalk      (501) staff       (20)     2265 2022-11-19 13:28:17.000000 rest_social_auth-8.0.0/setup.py
+drwxr-xr-x   0 stalk      (501) staff       (20)        0 2023-06-13 21:01:13.260977 rest_social_auth-8.1.0/
+-rw-r--r--   0 stalk      (501) staff       (20)     1072 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/LICENSE
+-rw-r--r--   0 stalk      (501) staff       (20)       68 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/MANIFEST.in
+-rw-r--r--   0 stalk      (501) staff       (20)    23650 2023-06-13 21:01:13.261064 rest_social_auth-8.1.0/PKG-INFO
+-rw-r--r--   0 stalk      (501) staff       (20)    18491 2023-06-13 20:56:40.000000 rest_social_auth-8.1.0/README.md
+-rw-r--r--   0 stalk      (501) staff       (20)     4215 2023-06-13 20:58:02.000000 rest_social_auth-8.1.0/RELEASE_NOTES.md
+-rw-r--r--   0 stalk      (501) staff       (20)      101 2023-06-13 20:56:40.000000 rest_social_auth-8.1.0/requirements.txt
+drwxr-xr-x   0 stalk      (501) staff       (20)        0 2023-06-13 21:01:13.259904 rest_social_auth-8.1.0/rest_social_auth/
+-rw-r--r--   0 stalk      (501) staff       (20)       43 2023-06-13 20:58:30.000000 rest_social_auth-8.1.0/rest_social_auth/__init__.py
+-rw-r--r--   0 stalk      (501) staff       (20)     4354 2022-11-19 00:52:06.000000 rest_social_auth-8.1.0/rest_social_auth/serializers.py
+-rw-r--r--   0 stalk      (501) staff       (20)      634 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/strategy.py
+-rw-r--r--   0 stalk      (501) staff       (20)      476 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/urls_jwt_pair.py
+-rw-r--r--   0 stalk      (501) staff       (20)      494 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/urls_jwt_sliding.py
+-rw-r--r--   0 stalk      (501) staff       (20)      465 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/urls_knox.py
+-rw-r--r--   0 stalk      (501) staff       (20)      234 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/urls_session.py
+-rw-r--r--   0 stalk      (501) staff       (20)      460 2022-11-18 17:05:12.000000 rest_social_auth-8.1.0/rest_social_auth/urls_token.py
+-rw-r--r--   0 stalk      (501) staff       (20)    12139 2022-11-19 13:24:07.000000 rest_social_auth-8.1.0/rest_social_auth/views.py
+drwxr-xr-x   0 stalk      (501) staff       (20)        0 2023-06-13 21:01:13.260852 rest_social_auth-8.1.0/rest_social_auth.egg-info/
+-rw-r--r--   0 stalk      (501) staff       (20)    23650 2023-06-13 21:01:13.000000 rest_social_auth-8.1.0/rest_social_auth.egg-info/PKG-INFO
+-rw-r--r--   0 stalk      (501) staff       (20)      562 2023-06-13 21:01:13.000000 rest_social_auth-8.1.0/rest_social_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 stalk      (501) staff       (20)        1 2023-06-13 21:01:13.000000 rest_social_auth-8.1.0/rest_social_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 stalk      (501) staff       (20)      101 2023-06-13 21:01:13.000000 rest_social_auth-8.1.0/rest_social_auth.egg-info/requires.txt
+-rw-r--r--   0 stalk      (501) staff       (20)       17 2023-06-13 21:01:13.000000 rest_social_auth-8.1.0/rest_social_auth.egg-info/top_level.txt
+-rw-r--r--   0 stalk      (501) staff       (20)      199 2023-06-13 21:01:13.261326 rest_social_auth-8.1.0/setup.cfg
+-rw-r--r--   0 stalk      (501) staff       (20)     2315 2023-06-13 20:56:40.000000 rest_social_auth-8.1.0/setup.py
```

### Comparing `rest_social_auth-8.0.0/LICENSE` & `rest_social_auth-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_social_auth-8.0.0/README.md` & `rest_social_auth-8.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 OAuth signin with django rest framework.
 
 
 Requirements
 -----------
 
-- python (3.7, 3.8, 3.9, 3.10)
-- django (3.2, 4.1)
+- python (3.7, 3.8, 3.9, 3.10, 3.11)
+- django (3.2, 4.1, 4.2)
 - djangorestframework (>=3.9, <4.0)
 - social-auth-core (>=4.3, <5.0)
 - social-auth-app-django (>=5.0, <6.0)
 - [optional] djangorestframework-simplejwt (>=5.0.0)
 - [optional] django-rest-knox (>=4.0.0, <5.0.0)
 
 Release notes
```

### Comparing `rest_social_auth-8.0.0/RELEASE_NOTES.md` & `rest_social_auth-8.1.0/RELEASE_NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 rest_social_auth release notes
 ==============================
 
+v8.1.0
+------
+- Add support of Django 4.2
+- Add support of Python 3.11
+
 v8.0.0
 ------
 - Drop support of Python 3.6
 - Drop support of Django 3.0, 3.1
 - Add support of Django 4.1
 - Add support of Python 3.10
 - Allow customized implementations of djangorestframework-simplejwt token class
```

### Comparing `rest_social_auth-8.0.0/rest_social_auth/serializers.py` & `rest_social_auth-8.1.0/rest_social_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `rest_social_auth-8.0.0/rest_social_auth/strategy.py` & `rest_social_auth-8.1.0/rest_social_auth/strategy.py`

 * *Files identical despite different names*

### Comparing `rest_social_auth-8.0.0/rest_social_auth/views.py` & `rest_social_auth-8.1.0/rest_social_auth/views.py`

 * *Files identical despite different names*

### Comparing `rest_social_auth-8.0.0/rest_social_auth.egg-info/SOURCES.txt` & `rest_social_auth-8.1.0/rest_social_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rest_social_auth-8.0.0/setup.py` & `rest_social_auth-8.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,10 +61,11 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Utilities',
     ],
 )
```

