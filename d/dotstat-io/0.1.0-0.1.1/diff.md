# Comparing `tmp/dotstat_io-0.1.0.tar.gz` & `tmp/dotstat_io-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstat_io-0.1.0.tar", max compression
+gzip compressed data, was "dotstat_io-0.1.1.tar", max compression
```

## Comparing `dotstat_io-0.1.0.tar` & `dotstat_io-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.0/dotstat_io/__init__.py
--rw-r--r--   0        0        0     7420 2023-05-10 16:00:57.233534 dotstat_io-0.1.0/dotstat_io/authentication.py
--rw-r--r--   0        0        0     7059 2023-05-10 08:51:25.981071 dotstat_io-0.1.0/dotstat_io/download_upload.py
--rw-r--r--   0        0        0      613 2023-05-12 06:53:07.260647 dotstat_io-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3404 2023-05-11 13:29:36.082806 dotstat_io-0.1.0/README.md
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 dotstat_io-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 17:04:57.103457 dotstat_io-0.1.1/dotstat_io/__init__.py
+-rw-r--r--   0        0        0     7420 2023-05-10 16:00:57.233534 dotstat_io-0.1.1/dotstat_io/authentication.py
+-rw-r--r--   0        0        0     9499 2023-06-12 11:17:52.891576 dotstat_io-0.1.1/dotstat_io/download_upload.py
+-rw-r--r--   0        0        0      633 2023-06-13 13:32:43.783357 dotstat_io-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3666 2023-06-08 12:29:56.582671 dotstat_io-0.1.1/README.md
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 dotstat_io-0.1.1/PKG-INFO
```

### Comparing `dotstat_io-0.1.0/dotstat_io/authentication.py` & `dotstat_io-0.1.1/dotstat_io/authentication.py`

 * *Files identical despite different names*

### Comparing `dotstat_io-0.1.0/dotstat_io/download_upload.py` & `dotstat_io-0.1.1/dotstat_io/download_upload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import os
 import requests
+import chardet
+import xml.etree.ElementTree as ET
 
 from pathlib import Path
 from time import sleep
 
 
 # class to download or upload data from/to .Stat Suite
 class Download_upload():
 
     # Declare constants
     __ERROR  = "An error occurred: "
     __EXECUTION_IN_PROGRESS = "InProgress"
-    __SUCCESS = "Successful download"
+    __DOWNLOAD_SUCCESS = "Successful download"
+    __UPLOAD_SUCCESS = "The request was successfully processed"
 
+    __NAMESPACE_MESSAGE = "{http://www.sdmx.org/resources/sdmxml/schemas/v2_1/message}"
+    __NAMESPACE_COMMON = "{http://www.sdmx.org/resources/sdmxml/schemas/v2_1/common}"
+  
     # Initialise Download_upload
     def __init__(self, token):
         self.token = token
 
     def __enter__(self):
         return self
 
@@ -50,15 +56,15 @@
                 if len(response.text) > 0:
                     Returned_Message += os.linesep + 'Text: ' + response.text
             else:
                 if os.path.isfile(file_path):
                     os.remove(file_path)
                 with open(file_path, "wb") as file:
                     file.write(response.content)
-                    Returned_Message = self.__SUCCESS
+                    Returned_Message = self.__DOWNLOAD_SUCCESS
                 file.close()
         finally:
             return Returned_Message
 
 
     # Download streamed content from .STAT
     def download_stream(self, dotstat_url: str, content_format: str):
@@ -66,16 +72,16 @@
             Returned_Message = ""
 
             if (self.token == None):
                 Returned_Message = self.__ERROR  + "No token" + os.linesep
             else:
                 headers = {
                     'accept': content_format,
-                   'Transfer-Encoding': 'chunked',
-                   'authorization': 'Bearer '+self.token
+                    'Transfer-Encoding': 'chunked',
+                    'authorization': 'Bearer '+self.token
                 }
 
                 #
                 return requests.get(dotstat_url, verify=True, headers=headers, stream=True)
 
         except Exception as err:
             Returned_Message = self.__ERROR  + str(err) + os.linesep
@@ -88,24 +94,24 @@
             Returned_Message = ""
 
             if (self.token == None):
                 Returned_Message = self.__ERROR  + "No token" + os.linesep
             else:
                 headers = {
                     'accept': 'application/json',
-                   'authorization': "Bearer "+self.token
+                    'authorization': "Bearer "+self.token
                 }
 
                 payload = {
                     "dataspace": space,
                 }
 
                 files = {
                     'dataspace': (None, payload['dataspace']),
-                   'file': (os.path.realpath(file_path), open(os.path.realpath(file_path), 'rb'), 'text/csv', '')
+                    'file': (os.path.realpath(file_path), open(os.path.realpath(file_path), 'rb'), 'text/csv', '')
                 }
 
                 #
                 response = requests.post(
                     transfer_url, verify=True, headers=headers, files=files)
 
         except Exception as err:
@@ -139,28 +145,77 @@
                 except Exception as err:
                     if len(response.text) > 0:
                         Returned_Message = self.__ERROR  + 'Text: ' + response.text
         finally:
             return Returned_Message
 
 
+    # Upload a structure to .STAT
+    def upload_structure(self, transfer_url: str, file_path: Path):
+        try:
+            Returned_Message = ""
+
+            # Detect the encoding used in file 
+            file = open(file=file_path, mode="rb")
+            detected_encoding = chardet.detect(file.read(10000))
+            file.close()
+
+            # Read file as a string "r+" with the detected encoding
+            file = open(file=file_path, mode="r+", encoding=detected_encoding.get("encoding"))
+            xml_data = file.read()
+            file.close()
+
+            # Make sure the encoding is "utf-8"
+            tree = ET.fromstring(xml_data)
+            xml_data = ET.tostring(tree, encoding="utf-8", method='xml', xml_declaration=True)
+
+            if (self.token == None):
+                Returned_Message = self.__ERROR  + "No token" + os.linesep
+            else:
+                headers = {
+                    'Content-Type': 'application/xml',
+                    'authorization': "Bearer "+self.token
+                }
+
+                #
+                response = requests.post(
+                    transfer_url, verify=True, headers=headers, data=xml_data)
+        except Exception as err:
+            Returned_Message = self.__ERROR  + str(err)
+        else:
+            try:
+                response.raise_for_status()
+            except requests.exceptions.HTTPError as e:
+                Returned_Message = f'Request failed with status code {response.status_code}: {e}'
+            else:
+                response_tree = ET.XML(response.content)
+                for error_message in response_tree.findall("./{0}ErrorMessage".format(self.__NAMESPACE_MESSAGE)):
+                    text_element = error_message.find("./{0}Text".format(self.__NAMESPACE_COMMON))
+                    if (text_element is not None):
+                        if Returned_Message == "":
+                            Returned_Message = self.__UPLOAD_SUCCESS + os.linesep
+                        Returned_Message = Returned_Message + text_element.text + os.linesep
+        finally:
+            return Returned_Message
+        
+
     # Check request sent to .STAT status
     # This is a recursive function to check the execution status
     def __check_request_status(self, transfer_url, requestId, space):
         try:
             Returned_Message = ""
 
             headers = {
                 'accept': 'application/json',
-               'authorization': "Bearer "+self.token
+                'authorization': "Bearer "+self.token
             }
 
             payload = {
                 'dataspace': space,
-               'id': requestId
+                'id': requestId
             }
 
             transfer_url = transfer_url.replace("import", "status")
             transfer_url = transfer_url.replace("sdmxFile", "request")
 
             response = requests.post(
                 transfer_url, verify=False, headers=headers, data=payload)
```

### Comparing `dotstat_io-0.1.0/pyproject.toml` & `dotstat_io-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "dotstat_io"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it"
 license = "MIT"
 authors = ["Gyorgy Gyomai <gyorgy.gyomai@oecd.org>", "Abdel Aliaoui <abdel.aliaoui@oecd.org>"]
 readme = "README.md"
 packages = [{include = "dotstat_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.29.0"
 requests-kerberos = "^0.14.0"
 msal = "^1.22.0"
+chardet = "^5.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dotstat_io-0.1.0/README.md` & `dotstat_io-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# DotStat_IO: 
+## DotStat_IO: 
 A generic python package which could be integrated with other end-user applications and Gitlab runner to perform basic io with .Stat Suite. 
 Its role is to mask the complexities of authentication to connect to .Stat Suite.
 The user needs to provide a set of parameters and the package exposes a couple of methods which will download or upload data from/to .Stat Suite.
 
-## This package contains two modules:
+### This package contains two modules:
 - ADFS-authentication module
 - Download-upload module
 
 ## In ADFS-authentication module, four methods are available:
 ### 1. To initialise the module for interactive use:
 ```python 
 interactive(client_id: str, sdmx_resource_id: str, scopes: list[str], authority_url: str, redirect_port: int)
@@ -37,15 +37,15 @@
 * `token_url:` URL of the authentication service
 
 ### 4. To get a token after initialisation: 
 ```python
 get_token()
 ```
 
-## In Download-upload module, three methods are available:
+### In Download-upload module, four methods are available:
 ### 1. To download a file from .Stat:
 ```python
 download_file(self, dotstat_url: str, content_format: str, file_path: Path)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 * `file_path:` The full path where the file will downloaded
@@ -53,16 +53,23 @@
 ### 2. To download streamed content from .Stat:
 ```python
 download_stream(self, dotstat_url: str, content_format: str)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 
-### 3. To upload a file to .Stat:
+### 3. To upload a data file to .Stat:
 ```python
 upload_file(self, transfer_url: str, file_path: Path, space: str)
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-CSV file, which will be uploaded to .Stat Suite
 * `space:` Data space where the file will be uploaded
 
-## For more information about how to use this package, all test cases can be accessed from this [`link`](https://gitlab.algobank.oecd.org/sdd-legacy/dotstat_io/-/blob/main/tests/test_cases.py)
+### 4. To upload a structure to .Stat:
+```python
+upload_structure(self, transfer_url: str, file_path: Path)
+```
+* `transfer_url:` URL of the transfer service
+* `file_path:` The full path of the SDMX-ML file, which will be uploaded to .Stat Suite
+
+### For more information about how to use this package, all test cases can be accessed from this [`link`](https://gitlab.algobank.oecd.org/sdd-legacy/dotstat_io/-/blob/main/tests/test_cases.py)
```

### Comparing `dotstat_io-0.1.0/PKG-INFO` & `dotstat_io-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: dotstat-io
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility to download or upload data from/to .Stat Suite using ADFS authentication to connect to it
 License: MIT
 Author: Gyorgy Gyomai
 Author-email: gyorgy.gyomai@oecd.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: msal (>=1.22.0,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: requests-kerberos (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
-# DotStat_IO: 
+## DotStat_IO: 
 A generic python package which could be integrated with other end-user applications and Gitlab runner to perform basic io with .Stat Suite. 
 Its role is to mask the complexities of authentication to connect to .Stat Suite.
 The user needs to provide a set of parameters and the package exposes a couple of methods which will download or upload data from/to .Stat Suite.
 
-## This package contains two modules:
+### This package contains two modules:
 - ADFS-authentication module
 - Download-upload module
 
 ## In ADFS-authentication module, four methods are available:
 ### 1. To initialise the module for interactive use:
 ```python 
 interactive(client_id: str, sdmx_resource_id: str, scopes: list[str], authority_url: str, redirect_port: int)
@@ -54,15 +55,15 @@
 * `token_url:` URL of the authentication service
 
 ### 4. To get a token after initialisation: 
 ```python
 get_token()
 ```
 
-## In Download-upload module, three methods are available:
+### In Download-upload module, four methods are available:
 ### 1. To download a file from .Stat:
 ```python
 download_file(self, dotstat_url: str, content_format: str, file_path: Path)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 * `file_path:` The full path where the file will downloaded
@@ -70,17 +71,24 @@
 ### 2. To download streamed content from .Stat:
 ```python
 download_stream(self, dotstat_url: str, content_format: str)
 ```
 * `dotstat_url:` URL of data to be downloaded from .Stat Suite
 * `content_format:` Format of the downloaded content
 
-### 3. To upload a file to .Stat:
+### 3. To upload a data file to .Stat:
 ```python
 upload_file(self, transfer_url: str, file_path: Path, space: str)
 ```
 * `transfer_url:` URL of the transfer service
 * `file_path:` The full path of the SDMX-CSV file, which will be uploaded to .Stat Suite
 * `space:` Data space where the file will be uploaded
 
-## For more information about how to use this package, all test cases can be accessed from this [`link`](https://gitlab.algobank.oecd.org/sdd-legacy/dotstat_io/-/blob/main/tests/test_cases.py)
+### 4. To upload a structure to .Stat:
+```python
+upload_structure(self, transfer_url: str, file_path: Path)
+```
+* `transfer_url:` URL of the transfer service
+* `file_path:` The full path of the SDMX-ML file, which will be uploaded to .Stat Suite
+
+### For more information about how to use this package, all test cases can be accessed from this [`link`](https://gitlab.algobank.oecd.org/sdd-legacy/dotstat_io/-/blob/main/tests/test_cases.py)
```

