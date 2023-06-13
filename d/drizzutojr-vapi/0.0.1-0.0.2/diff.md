# Comparing `tmp/drizzutojr_vapi-0.0.1-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3679 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-12 10:02 vapi/__init__.py
--rw-r--r--  2.0 unx      367 b- defN 23-Jun-12 10:02 vapi/exceptions.py
--rw-r--r--  2.0 unx     4760 b- defN 23-Jun-12 10:02 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-12 10:04 drizzutojr_vapi-0.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-12 10:04 drizzutojr_vapi-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 10:04 drizzutojr_vapi-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-12 10:04 drizzutojr_vapi-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Jun-12 10:04 drizzutojr_vapi-0.0.1.dist-info/RECORD
-8 files, 7175 bytes uncompressed, 2553 bytes compressed:  64.4%
+Zip file size: 3692 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-13 07:14 vapi/__init__.py
+-rw-r--r--  2.0 unx      367 b- defN 23-Jun-13 07:14 vapi/exceptions.py
+-rw-r--r--  2.0 unx     4775 b- defN 23-Jun-13 07:14 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jun-13 07:15 drizzutojr_vapi-0.0.2.dist-info/RECORD
+8 files, 7190 bytes uncompressed, 2566 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.1.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.1.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.1.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.1.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.1.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/vapi.py

```diff
@@ -102,15 +102,15 @@
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
 
     def list(self, path, raw=False, accepted_status_codes=[204, 200]):
         headers = self._set_headers()
-        url = self._format_url(path)
+        url = f"{self._format_url(path)}?list=true"
         response = requests.get(url, headers=headers, verify=self.cacert)
 
         if raw:
             return response
         else:
             return self._format_response(response, accepted_status_codes)
```

## Comparing `drizzutojr_vapi-0.0.1.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

