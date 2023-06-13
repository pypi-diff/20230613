# Comparing `tmp/acapela_downloader_py-0.0.9.tar.gz` & `tmp/acapela_downloader_py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.0.9.tar", last modified: Mon Jun 12 21:53:35 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.0.tar", last modified: Tue Jun 13 11:31:36 2023, max compression
```

## Comparing `acapela_downloader_py-0.0.9.tar` & `acapela_downloader_py-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.085016 acapela_downloader_py-0.0.9/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/src/utils.py
```

### Comparing `acapela_downloader_py-0.0.9/LICENSE` & `acapela_downloader_py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.0.9/PKG-INFO` & `acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acapela_downloader_py
-Version: 0.0.9
+Name: acapela-downloader-py
+Version: 0.1.0
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acapela-downloader-py
-Version: 0.0.9
+Name: acapela_downloader_py
+Version: 0.1.0
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.0.9/src/utils.py` & `acapela_downloader_py-0.1.0/src/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 import random
 import string
 import re
 from datetime import time
+from time import sleep
 
 from requests import post
 
 NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
 SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
 cached_nonce = ""
 cached_email = ""
 
 
 def update_nonce_token():
     global NONCE_ENDPOINT
     global cached_nonce
     global cached_email
     global last_failed
-    EMAIL_LENGTH = random.randint(10, 20)
-    fake_email = ""
-    for i in range(EMAIL_LENGTH):
-        fake_email += random.choice(string.ascii_letters)
-    fake_email += "@gmail.com"
-    nonce_response = post(NONCE_ENDPOINT, json={
-        "googleid": fake_email
-    })
-    if len(nonce_response.json()["nonce"]) > 1:
-        cached_nonce = nonce_response.json()["nonce"]
-        cached_email = fake_email
+
+    finished = False
+
+    while not finished:
+        EMAIL_LENGTH = random.randint(10, 20)
+        fake_email = ""
+        for i in range(EMAIL_LENGTH):
+            fake_email += random.choice(string.ascii_letters)
+        fake_email += "@gmail.com"
+        nonce_response = post(NONCE_ENDPOINT, json={
+            "googleid": fake_email
+        })
+        if len(nonce_response.json()["nonce"]) > 1:
+            cached_nonce = nonce_response.json()["nonce"]
+            cached_email = fake_email
+            finished = True
+
 
 
 def get_sound_link(text, voice_id):
-    update_nonce_token()
     finished = False
     while not finished:
+        update_nonce_token()
         try:
             synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
             synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
             headers = {'Content-type': 'application/x-www-form-urlencoded',
                        'Content-Length': str(len(synthesizer_request_bytes))}
             synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
             split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
             finished = True
             return split_res[1]
         except:
+            update_nonce_token()
             print("one minute delay...")
-            time.sleep(60)
+            sleep(60)
     return ""
```

