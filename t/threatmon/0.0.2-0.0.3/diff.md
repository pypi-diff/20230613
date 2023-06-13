# Comparing `tmp/threatmon-0.0.2-py3-none-any.whl.zip` & `tmp/threatmon-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3076 bytes, number of entries: 8
+Zip file size: 3517 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 19:03 threatmon/__init__.py
--rw-r--r--  2.0 unx      753 b- defN 23-Jun-05 19:08 threatmon/ioc.py
+-rw-r--r--  2.0 unx     1978 b- defN 23-Jun-13 12:00 threatmon/ioc.py
 -rw-r--r--  2.0 unx      597 b- defN 23-Jun-05 16:51 threatmon/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-05 19:18 threatmon-0.0.2.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-05 19:18 threatmon-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 19:18 threatmon-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 19:18 threatmon-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-05 19:18 threatmon-0.0.2.dist-info/RECORD
-8 files, 3606 bytes uncompressed, 1990 bytes compressed:  44.8%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-13 12:03 threatmon-0.0.3.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-13 12:03 threatmon-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 12:03 threatmon-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-13 12:03 threatmon-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 23-Jun-13 12:03 threatmon-0.0.3.dist-info/RECORD
+8 files, 4832 bytes uncompressed, 2431 bytes compressed:  49.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: threatmon/ioc.py
 Comment: 
 
 Filename: threatmon/utils.py
 Comment: 
 
-Filename: threatmon-0.0.2.dist-info/LICENCE.txt
+Filename: threatmon-0.0.3.dist-info/LICENCE.txt
 Comment: 
 
-Filename: threatmon-0.0.2.dist-info/METADATA
+Filename: threatmon-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: threatmon-0.0.2.dist-info/WHEEL
+Filename: threatmon-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: threatmon-0.0.2.dist-info/top_level.txt
+Filename: threatmon-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: threatmon-0.0.2.dist-info/RECORD
+Filename: threatmon-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## threatmon/ioc.py

```diff
@@ -1,26 +1,58 @@
 import requests
+import time
+import re
+import socket
 
-class IOC_API():
+class ioc():
     def __init__(self, api_token = "", limit = 10):
         self.api_token = api_token
         self.headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
         }
         self.limit = limit
         self.json_data = {
             'api_token': self.api_token,
             'limit': self.limit,
         }
-        
+
     def daily_ioc(self,):
         if self.api_token == "":
             return print("Please Use Your API Token")
         if self.limit > 100:
             return print("Limit can not exceed 100")
 
         return requests.post(
             'https://ioc.threatmonit.io/api/daily-ioc/',
             headers=self.headers,
             json=self.json_data,
-        )
+        ).json()
+
+    def QRadarIntegrator(self, 
+                        import_data,
+                        qradar_auth_key,
+                        qradar_server,
+                        qradar_ref_set
+                        ):
+        
+        # self.qradar_auth_key = "811aacf9-jh68-444h-98f4-5d25b7a94844"
+        self.qradar_ref_set = "THREATMON_Event_IOC"
+
+        QRadar_POST_url = f"https://{qradar_server}/api/reference_data/sets/bulk_load/{qradar_ref_set}"
+
+        self.QRadar_headers = {
+            'sec': qradar_auth_key,
+            'content-type': "application/json",
+        }
+
+        print(time.strftime("%H:%M:%S") + " -- " + "Initiating, IOC POST to QRadar ")
+        files = []
+
+        for key in import_data["entities"]:
+            files.extend(ioc["hash"] for ioc in key["hashes"])
+            
+        qradar_response = requests.request("POST", QRadar_POST_url, data=files, headers=self.QRadar_headers, verify=False)
+        if qradar_response.status_code == 200:
+            print(time.strftime("%H:%M:%S") + " -- " + " (Finished) Imported IOCs to QRadar (Success)" )
+        else:
+            print(time.strftime("%H:%M:%S") + " -- " + "Could not POST IOCs to QRadar (Failure)")
```

## Comparing `threatmon-0.0.2.dist-info/LICENCE.txt` & `threatmon-0.0.3.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `threatmon-0.0.2.dist-info/RECORD` & `threatmon-0.0.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 threatmon/__init__.py,sha256=nXlXBoxbxeXzEDK0JXVCkIi47kcoch2e0GirpfTyquU,42
-threatmon/ioc.py,sha256=Er5h3dcmNvwZu0-01nK61X6hxa6bTnDOpeJgPMH1Wl8,753
+threatmon/ioc.py,sha256=mUKz0RGHi3jNpIWcE2Tmoj8J-h4c9oTzu48jsFYfftw,1978
 threatmon/utils.py,sha256=SydslOhqSkZo6ppgSiYrDyP7ZIJd7h4pNXD3Gu6_9Tc,597
-threatmon-0.0.2.dist-info/LICENCE.txt,sha256=Kj1QsVeBn9NHAhuxP4DmX8ksX3OHTCzMVVV8NG6nW1o,1069
-threatmon-0.0.2.dist-info/METADATA,sha256=8k-Pdx55FhpKkcacv4mgN3rLGQ7ZttEFDdxsFEY_3og,422
-threatmon-0.0.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-threatmon-0.0.2.dist-info/top_level.txt,sha256=0m-UKHGwuR6fmNQ5DZTLtl7jOOC9RJjh0nqy91Dm6oE,10
-threatmon-0.0.2.dist-info/RECORD,,
+threatmon-0.0.3.dist-info/LICENCE.txt,sha256=Kj1QsVeBn9NHAhuxP4DmX8ksX3OHTCzMVVV8NG6nW1o,1069
+threatmon-0.0.3.dist-info/METADATA,sha256=Uh5bbmJfG5BootNFVV601O-ie3IBwMDI_2v3RWKpSq0,422
+threatmon-0.0.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+threatmon-0.0.3.dist-info/top_level.txt,sha256=0m-UKHGwuR6fmNQ5DZTLtl7jOOC9RJjh0nqy91Dm6oE,10
+threatmon-0.0.3.dist-info/RECORD,,
```

