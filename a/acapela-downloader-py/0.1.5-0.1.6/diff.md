# Comparing `tmp/acapela_downloader_py-0.1.5.tar.gz` & `tmp/acapela_downloader_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.1.5.tar", last modified: Tue Jun 13 15:49:54 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.6.tar", last modified: Tue Jun 13 17:13:39 2023, max compression
```

## Comparing `acapela_downloader_py-0.1.5.tar` & `acapela_downloader_py-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:49:54.493212 acapela_downloader_py-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 15:49:44.000000 acapela_downloader_py-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:49:54.489212 acapela_downloader_py-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 15:49:44.000000 acapela_downloader_py-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 15:49:44.000000 acapela_downloader_py-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:49:54.493212 acapela_downloader_py-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:49:54.489212 acapela_downloader_py-0.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 15:49:44.000000 acapela_downloader_py-0.1.5/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:49:54.489212 acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:49:54.000000 acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:49:54.000000 acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:49:54.000000 acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 15:49:54.000000 acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-13 15:49:44.000000 acapela_downloader_py-0.1.5/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:13:39.711011 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:13:39.000000 acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-13 17:13:17.000000 acapela_downloader_py-0.1.6/src/utils.py
```

### Comparing `acapela_downloader_py-0.1.5/LICENSE` & `acapela_downloader_py-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.1.5/PKG-INFO` & `acapela_downloader_py-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.5/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.6/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.5/src/utils.py` & `acapela_downloader_py-0.1.6/src/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,28 +14,34 @@
 def set_debug_mode(active):
     global debug_mode
     debug_mode = active
 
 def update_nonce_token():
     global NONCE_ENDPOINT
     global cached_nonce
+    global debug_mode
     global cached_email
     global last_failed
 
     finished = False
 
     while not finished:
         EMAIL_LENGTH = random.randint(10, 20)
         fake_email = ""
         for i in range(EMAIL_LENGTH):
             fake_email += random.choice(string.ascii_letters)
         fake_email += "@gmail.com"
+        fake_email = fake_email.replace(" ", "")
         nonce_response = post(NONCE_ENDPOINT, json={
             "googleid": fake_email
         })
+
+        if debug_mode:
+            print("DEBUG: " + fake_email)
+
         if len(nonce_response.json()["nonce"]) > 1:
             cached_nonce = nonce_response.json()["nonce"]
             cached_email = fake_email
             finished = True
```

