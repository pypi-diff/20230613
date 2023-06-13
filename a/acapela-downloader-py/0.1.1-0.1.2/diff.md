# Comparing `tmp/acapela_downloader_py-0.1.1.tar.gz` & `tmp/acapela_downloader_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.1.1.tar", last modified: Tue Jun 13 12:33:09 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.2.tar", last modified: Tue Jun 13 15:34:33 2023, max compression
```

## Comparing `acapela_downloader_py-0.1.1.tar` & `acapela_downloader_py-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.599919 acapela_downloader_py-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:34:33.009865 acapela_downloader_py-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 15:34:17.000000 acapela_downloader_py-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:34:33.009865 acapela_downloader_py-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 15:34:17.000000 acapela_downloader_py-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 15:34:17.000000 acapela_downloader_py-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:34:33.009865 acapela_downloader_py-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:34:33.009865 acapela_downloader_py-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 15:34:17.000000 acapela_downloader_py-0.1.2/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:34:33.009865 acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:34:33.000000 acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:34:33.000000 acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:34:33.000000 acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 15:34:33.000000 acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 15:34:17.000000 acapela_downloader_py-0.1.2/src/utils.py
```

### Comparing `acapela_downloader_py-0.1.1/LICENSE` & `acapela_downloader_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.1.1/PKG-INFO` & `acapela_downloader_py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.2/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.1/src/utils.py` & `acapela_downloader_py-0.1.2/src/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import string
 import re
 from datetime import time
 from time import sleep
 
 from requests import post
 
+debug_mode = False
+
+def set_debug_mode(active):
+    global debug_mode
+    debug_mode = active
+
 NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
 SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
 cached_nonce = ""
 cached_email = ""
 
 
 def update_nonce_token():
@@ -33,26 +39,30 @@
             cached_nonce = nonce_response.json()["nonce"]
             cached_email = fake_email
             finished = True
 
 
 
 def get_sound_link(text, voice_id):
+    global debug_mode
     finished = False
     while not finished:
         update_nonce_token()
         try:
             synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
             synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
             headers = {'Content-type': 'application/x-www-form-urlencoded',
                        'Content-Length': str(len(synthesizer_request_bytes))}
             synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
             split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
-            finished = True
-            return split_res[1]
+            if debug_mode:
+                print("DEBUG: " + str(synthesizer_request.content))
+            if len(split_res) > 1:
+                finished = True
+                return split_res[1]
         except Exception as msg:
             print(msg)
             update_nonce_token()
     return ""
```

