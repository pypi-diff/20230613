# Comparing `tmp/acapela_downloader_py-0.1.0.tar.gz` & `tmp/acapela_downloader_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.1.0.tar", last modified: Tue Jun 13 11:31:36 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.1.tar", last modified: Tue Jun 13 12:33:09 2023, max compression
```

## Comparing `acapela_downloader_py-0.1.0.tar` & `acapela_downloader_py-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:31:36.074068 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 11:31:36.000000 acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 11:31:23.000000 acapela_downloader_py-0.1.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.599919 acapela_downloader_py-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:33:09.603919 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 12:33:09.000000 acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-13 12:32:55.000000 acapela_downloader_py-0.1.1/src/utils.py
```

### Comparing `acapela_downloader_py-0.1.0/LICENSE` & `acapela_downloader_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.1.0/PKG-INFO` & `acapela_downloader_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.0/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.1/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.0/src/utils.py` & `acapela_downloader_py-0.1.1/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
             headers = {'Content-type': 'application/x-www-form-urlencoded',
                        'Content-Length': str(len(synthesizer_request_bytes))}
             synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
             split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
             finished = True
             return split_res[1]
-        except:
+        except Exception as msg:
+            print(msg)
             update_nonce_token()
-            print("one minute delay...")
-            sleep(60)
     return ""
```

