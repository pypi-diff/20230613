# Comparing `tmp/gauth-1.0.7.tar.gz` & `tmp/gauth-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth-1.0.7.tar", last modified: Wed May 31 10:37:41 2023, max compression
+gzip compressed data, was "gauth-1.0.8.tar", last modified: Tue Jun 13 02:45:38 2023, max compression
```

## Comparing `gauth-1.0.7.tar` & `gauth-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.801763 gauth-1.0.7/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.7/LICENSE.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       24 2023-05-31 10:08:04.000000 gauth-1.0.7/MANIFEST.in
--rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:37:41.801548 gauth-1.0.7/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)     1465 2023-05-31 09:47:37.000000 gauth-1.0.7/README.md
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.798003 gauth-1.0.7/gauth/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/__init__.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.800075 gauth-1.0.7/gauth/extract/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/extract/__init__.py
--rw-r--r--   0 damonyuan   (501) staff       (20)    38669 2023-05-31 09:50:16.000000 gauth-1.0.7/gauth/extract/extract_otp_secrets.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.801129 gauth-1.0.7/gauth/extract/protobuf_generated_python/
--rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.7/gauth/extract/protobuf_generated_python/__init__.py
--rw-r--r--   0 damonyuan   (501) staff       (20)     2171 2023-05-31 09:14:07.000000 gauth-1.0.7/gauth/extract/protobuf_generated_python/google_auth_pb2.py
--rw-r--r--   0 damonyuan   (501) staff       (20)     2075 2023-05-31 10:36:23.000000 gauth-1.0.7/gauth/main.py
-drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-05-31 10:37:41.799586 gauth-1.0.7/gauth.egg-info/
--rw-r--r--   0 damonyuan   (501) staff       (20)     1893 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/PKG-INFO
--rw-r--r--   0 damonyuan   (501) staff       (20)      441 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/SOURCES.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/dependency_links.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/entry_points.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      263 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/requires.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-05-31 10:37:41.000000 gauth-1.0.7/gauth.egg-info/top_level.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)      274 2023-05-31 09:06:17.000000 gauth-1.0.7/requirements.txt
--rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-05-31 10:37:41.801815 gauth-1.0.7/setup.cfg
--rw-r--r--   0 damonyuan   (501) staff       (20)      933 2023-05-31 10:36:54.000000 gauth-1.0.7/setup.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-06-13 02:45:38.313164 gauth-1.0.8/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1066 2023-05-31 06:54:54.000000 gauth-1.0.8/LICENSE.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       24 2023-05-31 10:08:04.000000 gauth-1.0.8/MANIFEST.in
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2078 2023-06-13 02:45:38.312992 gauth-1.0.8/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)     1650 2023-06-12 10:33:21.000000 gauth-1.0.8/README.md
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-06-13 02:45:38.309773 gauth-1.0.8/gauth/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.8/gauth/__init__.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-06-13 02:45:38.312120 gauth-1.0.8/gauth/extract/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.8/gauth/extract/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)    38669 2023-05-31 09:50:16.000000 gauth-1.0.8/gauth/extract/extract_otp_secrets.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-06-13 02:45:38.312670 gauth-1.0.8/gauth/extract/protobuf_generated_python/
+-rw-r--r--   0 damonyuan   (501) staff       (20)        0 2023-05-31 09:45:35.000000 gauth-1.0.8/gauth/extract/protobuf_generated_python/__init__.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2171 2023-05-31 09:14:07.000000 gauth-1.0.8/gauth/extract/protobuf_generated_python/google_auth_pb2.py
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2621 2023-06-13 02:43:21.000000 gauth-1.0.8/gauth/main.py
+drwxr-xr-x   0 damonyuan   (501) staff       (20)        0 2023-06-13 02:45:38.311666 gauth-1.0.8/gauth.egg-info/
+-rw-r--r--   0 damonyuan   (501) staff       (20)     2078 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/PKG-INFO
+-rw-r--r--   0 damonyuan   (501) staff       (20)      441 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/SOURCES.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        1 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/dependency_links.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       42 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/entry_points.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      275 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/requires.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)        6 2023-06-13 02:45:38.000000 gauth-1.0.8/gauth.egg-info/top_level.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)      286 2023-06-12 10:37:12.000000 gauth-1.0.8/requirements.txt
+-rw-r--r--   0 damonyuan   (501) staff       (20)       38 2023-06-13 02:45:38.313205 gauth-1.0.8/setup.cfg
+-rw-r--r--   0 damonyuan   (501) staff       (20)      933 2023-06-13 02:45:26.000000 gauth-1.0.8/setup.py
```

### Comparing `gauth-1.0.7/LICENSE.txt` & `gauth-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gauth-1.0.7/PKG-INFO` & `gauth-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,12 +57,27 @@
 # Release
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
+# YAML example
+
+```
+---
+keys:
+  - Name:    TEST1
+    Secret:  1234567
+    Issuer:  ABC
+    Type:    totp
+
+  - Name:    TEST2
+    Secret:  1234455
+    Issuer:  CDE
+    Type:    totp
+```
 
 # Reference
 
 [extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
```

### Comparing `gauth-1.0.7/README.md` & `gauth-1.0.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -43,12 +43,27 @@
 # Release
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
+# YAML example
+
+```
+---
+keys:
+  - Name:    TEST1
+    Secret:  1234567
+    Issuer:  ABC
+    Type:    totp
+
+  - Name:    TEST2
+    Secret:  1234455
+    Issuer:  CDE
+    Type:    totp
+```
 
 # Reference
 
 [extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
```

### Comparing `gauth-1.0.7/gauth/extract/extract_otp_secrets.py` & `gauth-1.0.8/gauth/extract/extract_otp_secrets.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.7/gauth/extract/protobuf_generated_python/google_auth_pb2.py` & `gauth-1.0.8/gauth/extract/protobuf_generated_python/google_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `gauth-1.0.7/gauth/main.py` & `gauth-1.0.8/gauth/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import os
 import argparse
 import pyotp
 import tempfile
 import json
+import yaml
 from PIL import Image
 from contextlib import contextmanager
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), '../'))
 
 
 def check_img(filename):
     try:
@@ -18,14 +19,21 @@
         im.transpose(Image.FLIP_LEFT_RIGHT)
         im.close()
         return True
     except:
         return False
 
 
+def check_yaml(filename):
+    if filename.endswith('.yaml') or filename.endswith('.yml'):
+        return True
+    else:
+        return False
+
+
 @contextmanager
 def silence_stdout():
     old_target = sys.stdout
     old_stderr = sys.stderr
     try:
         with open(os.devnull, "w") as new_target:
             sys.stdout = new_target
@@ -34,27 +42,34 @@
     finally:
         sys.stdout = old_target
         sys.stderr = old_stderr
 
 
 def main():
     parser = argparse.ArgumentParser(description='Tool to help migrate Google Authenticator from phone to desktop')
-    parser.add_argument('-p', '--path', help='file path to the exported qr code or text file', required=True)
+    parser.add_argument('-p', '--path', help='file path to the exported qr code or text file, or yaml file', required=True)
     parser.add_argument('-n', '--name', help='otp name', required=False)
     args = parser.parse_args()
     if args.path:
-        if check_img(args.path):
-            from gauth.extract import extract_otp_secrets
+        if check_yaml(args.path):
+            with open(args.path, "r") as yaml_file:
+                config = yaml.safe_load(yaml_file)
+                for e in config['keys']:
+                    totp = pyotp.TOTP(e['Secret'].strip())
+                    print(f"{e['Issuer'].ljust(15)} {e['Name'].ljust(38)}: {totp.now()}")
         else:
-            with silence_stdout():
+            if check_img(args.path):
                 from gauth.extract import extract_otp_secrets
-        with tempfile.NamedTemporaryFile() as tmp:
-            params = [args.path, '--json', tmp.name, '--quiet', '--ignore']
-            extract_otp_secrets.main(params)
-            otps(json.load(tmp), args.name)
+            else:
+                with silence_stdout():
+                    from gauth.extract import extract_otp_secrets
+            with tempfile.NamedTemporaryFile() as tmp:
+                params = [args.path, '--json', tmp.name, '--quiet', '--ignore']
+                extract_otp_secrets.main(params)
+                otps(json.load(tmp), args.name)
 
 
 def otps(config, name):
     for e in config:
         if name is not None and name == e['name']:
             otp(e['name'], e['issuer'], e['secret'].strip())
         elif name is None:
```

### Comparing `gauth-1.0.7/gauth.egg-info/PKG-INFO` & `gauth-1.0.8/gauth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tool to help migrate Google Authenticator from phone to desktop
 Home-page: https://github.com/damonYuan/gauth
 Author: Damon Yuan
 Author-email: damon.yuan.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,12 +57,27 @@
 # Release
 
 ```
 pip install --upgrade twine
 python setup.py sdist
 twine upload dist/*
 ```
+# YAML example
+
+```
+---
+keys:
+  - Name:    TEST1
+    Secret:  1234567
+    Issuer:  ABC
+    Type:    totp
+
+  - Name:    TEST2
+    Secret:  1234455
+    Issuer:  CDE
+    Type:    totp
+```
 
 # Reference
 
 [extract_otp_secrets v2.4.3](https://github.com/scito/extract_otp_secrets)
```

### Comparing `gauth-1.0.7/setup.py` & `gauth-1.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 with open("requirements.txt", "r") as f:
     REQUIREMENTS = f.read().splitlines()
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gauth",
-    version="1.0.7",
+    version="1.0.8",
     license='MIT',
     description="Tool to help migrate Google Authenticator from phone to desktop",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Damon Yuan",
     author_email="damon.yuan.dev@gmail.com",
     url="https://github.com/damonYuan/gauth",
```

