# Comparing `tmp/JpegIPTC-1.4.tar.gz` & `tmp/JpegIPTC-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JpegIPTC-1.4.tar", last modified: Mon Mar 13 17:12:43 2023, max compression
+gzip compressed data, was "JpegIPTC-1.5.tar", last modified: Tue Jun 13 12:23:18 2023, max compression
```

## Comparing `JpegIPTC-1.4.tar` & `JpegIPTC-1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-03-13 17:12:43.590852 JpegIPTC-1.4/
-drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-03-13 17:12:43.590852 JpegIPTC-1.4/JpegIPTC.egg-info/
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    10191 2023-03-13 17:12:43.000000 JpegIPTC-1.4/JpegIPTC.egg-info/PKG-INFO
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      177 2023-03-13 17:12:43.000000 JpegIPTC-1.4/JpegIPTC.egg-info/SOURCES.txt
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        1 2023-03-13 17:12:43.000000 JpegIPTC-1.4/JpegIPTC.egg-info/dependency_links.txt
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        9 2023-03-13 17:12:43.000000 JpegIPTC-1.4/JpegIPTC.egg-info/top_level.txt
--rwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)    17845 2023-03-13 17:12:23.000000 JpegIPTC-1.4/JpegIPTC.py
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1075 2023-03-12 16:17:47.000000 JpegIPTC-1.4/LICENSE
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    10191 2023-03-13 17:12:43.590852 JpegIPTC-1.4/PKG-INFO
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      547 2023-03-12 16:25:31.000000 JpegIPTC-1.4/README.rst
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      170 2023-03-13 17:12:43.590852 JpegIPTC-1.4/setup.cfg
--rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1977 2023-03-13 17:05:39.000000 JpegIPTC-1.4/setup.py
+drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-06-13 12:23:18.380879 JpegIPTC-1.5/
+drwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)        0 2023-06-13 12:23:18.380879 JpegIPTC-1.5/JpegIPTC.egg-info/
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    10240 2023-06-13 12:23:18.000000 JpegIPTC-1.5/JpegIPTC.egg-info/PKG-INFO
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      176 2023-06-13 12:23:18.000000 JpegIPTC-1.5/JpegIPTC.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        1 2023-06-13 12:23:18.000000 JpegIPTC-1.5/JpegIPTC.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)        9 2023-06-13 12:23:18.000000 JpegIPTC-1.5/JpegIPTC.egg-info/top_level.txt
+-rwxrwxr-x   0 gdegoulet  (1000) gdegoulet  (1000)    18165 2023-06-13 12:17:08.000000 JpegIPTC-1.5/JpegIPTC.py
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1075 2023-03-12 16:17:47.000000 JpegIPTC-1.5/LICENSE
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)    10240 2023-06-13 12:23:18.380879 JpegIPTC-1.5/PKG-INFO
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     9443 2023-03-13 17:34:16.000000 JpegIPTC-1.5/README.md
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)      170 2023-06-13 12:23:18.380879 JpegIPTC-1.5/setup.cfg
+-rw-rw-r--   0 gdegoulet  (1000) gdegoulet  (1000)     1957 2023-03-13 17:34:16.000000 JpegIPTC-1.5/setup.py
```

### Comparing `JpegIPTC-1.4/JpegIPTC.egg-info/PKG-INFO` & `JpegIPTC-1.5/JpegIPTC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: JpegIPTC
-Version: 1.4
+Version: 1.5
 Summary: Jpeg Iptc data raw extract/copy
 Home-page: https://github.com/gdegoulet/JpegIPTC
-Download-URL: https://github.com/gdegoulet/JpegIPTC/archive/v1.3.tar.gz
+Download-URL: https://github.com/gdegoulet/JpegIPTC
 Author: Guillaume Degoulet
 Author-email: jpegiptc@degoulet.net
 Maintainer: Guillaume Degoulet
 Maintainer-email: jpegiptc@degoulet.net
 License: http://www.opensource.org/licenses/gpl-license.php
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -50,14 +50,19 @@
 # All rights reserved.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the same terms as Python itself.
 
 ```
 
+###
+```
+pip install JpegIPTC
+```
+
 ## Functions:
 
 - load_from_file(filename) : initialize object from file location (return booleans)
 - load_from_binarydata(rawdata) : initialize object from binary string (return booleans) **(for thumbor integration)**
 - save() : for object initialized with load_from_file : overwrite with new content (return booleans)
 - save_as(output_filename) : write/overwrite new content to output_filename (return booleans)
 - get_raw_iptc() : return raw iptc as binary string **(for thumbor integration)**
@@ -176,7 +181,9 @@
 ```
 
 As you can see, IPTC Envelope has vanished .. :( for now ..
 
 **since 0.3 : ALL IPTC data (record 1 and 2 from APP13) are raw copied**
 
 **since 1.0 : Searching for IPTC data only if input is regular jpeg file**
+
+**since 1.4 : available on Pypip"
```

### Comparing `JpegIPTC-1.4/JpegIPTC.py` & `JpegIPTC-1.5/JpegIPTC.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os
 import shutil
 import sys
 import tempfile
 from struct import pack, unpack
 import json
 
-__version__ = '1.4'
+__version__ = '1.5'
 __author__ = 'Guillaume Degoulet'
 __updated_by__ = 'Guillaume Degoulet'
 
 class EOFException(Exception):
     def __init__(self, *args):
         super().__init__(self)
         self._str = '\n'.join(args)
@@ -200,22 +200,27 @@
         # IPTC code: record 2, dataset 0.
         bio = BytesIO()
         while True:
             try:
                 header = self._read_exactly(bytesio_obj, 5)
             except EOFException:
                 return bio
-            bio.write(header)
 
             (tag, record, dataset, length) = unpack("!BBBH", header)
             if record > 2:
+                #print(bio.getvalue())
                 return bio
-            value = bytesio_obj.read(length)
-            bio.write(value)
+            if tag == 28:
+                value = bytesio_obj.read(length)
+                #print(tag,record,length)
+                #print(value)
+                bio.write(header)
+                bio.write(value)
 
+        #print(bio.getvalue())
         return bio
 
     def _collect_adobe_parts(self,data):
         """Part APP13 contains yet another markup format, one defined by
         Adobe.  See"File Formats Specification" in the Photoshop SDK
         (avail from www.adobe.com). We must take
         everything but the IPTC data so that way we can write the file back
@@ -385,17 +390,19 @@
         # Pad with a blank if not even size
         if len(data) % 2 != 0:
             resourceBlock.append(pack("B", 0))
         # Finally tack on other data
         if otherparts is not None:
             resourceBlock.append(otherparts)
         resourceBlock = b''.join(resourceBlock)
-        out.append(pack("BB", 0xff, APP13))  # Jpeg start of block, APP13
-        out.append(pack("!H", len(resourceBlock) + 2))  # length
-        out.append(resourceBlock)
+        #print(len(resourceBlock) + 2)
+        if (len(resourceBlock) + 2) <= 65535:
+            out.append(pack("BB", 0xff, APP13))  # Jpeg start of block, APP13
+            out.append(pack("!H", len(resourceBlock) + 2))  # length
+            out.append(resourceBlock)
         return b''.join(out)
 
     def __del__(self):
         self.error = None
         self.is_jpeg = False
         self.bytesio_obj = None
         self.finename = None
@@ -417,14 +424,15 @@
     def load_from_file(self,filename):
         self.finename = filename
         try:
             with open(filename, "rb") as file:
                 bytesio_obj = file.read()
                 self.bytesio_obj = bytesio_obj
                 self._fetch_iptc(bytesio_obj)
+                #print(len(self.raw_iptc))
                 return True
         except:
             return False
 
     def load_from_binarydata(self,data):
         bytesio_obj = BytesIO()
         bytesio_obj.write(data)
```

### Comparing `JpegIPTC-1.4/LICENSE` & `JpegIPTC-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JpegIPTC-1.4/PKG-INFO` & `JpegIPTC-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: JpegIPTC
-Version: 1.4
+Version: 1.5
 Summary: Jpeg Iptc data raw extract/copy
 Home-page: https://github.com/gdegoulet/JpegIPTC
-Download-URL: https://github.com/gdegoulet/JpegIPTC/archive/v1.3.tar.gz
+Download-URL: https://github.com/gdegoulet/JpegIPTC
 Author: Guillaume Degoulet
 Author-email: jpegiptc@degoulet.net
 Maintainer: Guillaume Degoulet
 Maintainer-email: jpegiptc@degoulet.net
 License: http://www.opensource.org/licenses/gpl-license.php
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -50,14 +50,19 @@
 # All rights reserved.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the same terms as Python itself.
 
 ```
 
+###
+```
+pip install JpegIPTC
+```
+
 ## Functions:
 
 - load_from_file(filename) : initialize object from file location (return booleans)
 - load_from_binarydata(rawdata) : initialize object from binary string (return booleans) **(for thumbor integration)**
 - save() : for object initialized with load_from_file : overwrite with new content (return booleans)
 - save_as(output_filename) : write/overwrite new content to output_filename (return booleans)
 - get_raw_iptc() : return raw iptc as binary string **(for thumbor integration)**
@@ -176,7 +181,9 @@
 ```
 
 As you can see, IPTC Envelope has vanished .. :( for now ..
 
 **since 0.3 : ALL IPTC data (record 1 and 2 from APP13) are raw copied**
 
 **since 1.0 : Searching for IPTC data only if input is regular jpeg file**
+
+**since 1.4 : available on Pypip"
```

### Comparing `JpegIPTC-1.4/setup.py` & `JpegIPTC-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 version = next((row.split('=', 1)[-1].strip().strip("'").strip('"')
                 for row in open('JpegIPTC.py', 'r')
                 if row.startswith('__version__')))
 setup(  # cmdclass={'sdist': sdist},
     name='JpegIPTC',
     version=version,
     url='https://github.com/gdegoulet/JpegIPTC',
-    download_url='https://github.com/gdegoulet/JpegIPTC/archive/v1.3.tar.gz',
+    download_url='https://github.com/gdegoulet/JpegIPTC',
     author='Guillaume Degoulet',
     author_email='jpegiptc@degoulet.net',
     maintainer='Guillaume Degoulet',
     maintainer_email='jpegiptc@degoulet.net',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license='http://www.opensource.org/licenses/gpl-license.php',
```

