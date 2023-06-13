# Comparing `tmp/yamlres-0.1.2-py3-none-any.whl.zip` & `tmp/yamlres-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5915 bytes, number of entries: 8
+Zip file size: 5927 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       70 b- defN 23-Feb-10 10:40 yamlres/__init__.py
 -rw-rw-rw-  2.0 fat      266 b- defN 23-Feb-11 11:29 yamlres/functional.py
 -rw-rw-rw-  2.0 fat     2211 b- defN 23-Feb-27 12:26 yamlres/loader.py
--rw-rw-rw-  2.0 fat     4141 b- defN 23-Feb-11 11:33 yamlres/runner.py
--rw-rw-rw-  2.0 fat     6543 b- defN 23-Feb-27 12:32 yamlres-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-27 12:32 yamlres-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Feb-27 12:32 yamlres-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      596 b- defN 23-Feb-27 12:32 yamlres-0.1.2.dist-info/RECORD
-8 files, 13927 bytes uncompressed, 4881 bytes compressed:  65.0%
+-rw-rw-rw-  2.0 fat     4339 b- defN 23-Jun-13 09:54 yamlres/runner.py
+-rw-rw-rw-  2.0 fat     6534 b- defN 23-Jun-13 09:54 yamlres-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 09:54 yamlres-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-13 09:54 yamlres-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      596 b- defN 23-Jun-13 09:54 yamlres-0.1.3.dist-info/RECORD
+8 files, 14116 bytes uncompressed, 4893 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: yamlres/loader.py
 Comment: 
 
 Filename: yamlres/runner.py
 Comment: 
 
-Filename: yamlres-0.1.2.dist-info/METADATA
+Filename: yamlres-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: yamlres-0.1.2.dist-info/WHEEL
+Filename: yamlres-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: yamlres-0.1.2.dist-info/top_level.txt
+Filename: yamlres-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: yamlres-0.1.2.dist-info/RECORD
+Filename: yamlres-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yamlres/runner.py

```diff
@@ -13,14 +13,18 @@
             for part in parts[1:]:
                 obj = getattr(obj, part)
             return obj
         if isinstance(name, str) and name in values:
             name = values[name]
         if isinstance(name, dict) and "method" in name:
             return self.exec(name, values)
+        if isinstance(name, list):
+            return [self.get(values, v) for v in name]
+        if isinstance(name, dict):
+            return {k: self.get(values, v) for k, v in name.items()}
         return name
 
     def exec(self, specs, values: dict = None):
         assert isinstance(specs, dict)
         values = dict() if values is None else values
         for k, v in self.globals.items():
             if k not in values:
```

## Comparing `yamlres-0.1.2.dist-info/METADATA` & `yamlres-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlres
-Version: 0.1.2
+Version: 0.1.3
 Summary: A yaml-based declarative programming interface
 Home-page: https://github.com/maniospas/yamlres
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,23 +17,23 @@
 # yamlres
 
 *Retrieving algorithm component combinations from online (or local) yaml resources.*
 
 This project extends the *yaml* prototype with web-based resource fields
 and creates a declarative algorithm interface. This can help share algorithms
 based on existing *Python* libraries via a continuous deployment pipeline
-where you only update web resources. Thus, algorithm declarations are
+where you only update web resources. Thus, algorithm declarations
 are separated from the update cycles of building components.
 
 **Development:** Emmanouil (Manios) Krasanakis<br>
 **Dependencies:** `pyyaml`,`wget`
 
 ## Loading yaml from the web
 `yamlres` parses normal *yaml* files, but also goes through their fields
-in search of strings with containing the *.yaml* file extension and recursively
+in search of strings containing the *.yaml* file extension and recursively
 replaces such fields from files. Recursive loading throws an exception.
 You can reference online web resources to automatically download and parse.
 
 For example, you can download and load an online *yaml* resource with 
 the following code:
 
 ```python
```

## Comparing `yamlres-0.1.2.dist-info/RECORD` & `yamlres-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 yamlres/__init__.py,sha256=WSYdc1X8ct04mUVNcPbGrnlHjeG3ZhEA8sqw1wOTOZE,70
 yamlres/functional.py,sha256=IC8svabU_PygIGrMZiYDQ_phEQKhhrBBITDuPMcZUNI,266
 yamlres/loader.py,sha256=d-zesSx8Nk0-kNk6_TyeERI15A4W7ZgFgDLKLutHvhk,2211
-yamlres/runner.py,sha256=8lVhxsHo40QoLIS_8muA3pY3te0TkGvfxGSIgUftYEk,4141
-yamlres-0.1.2.dist-info/METADATA,sha256=NoJnxsACt71uJJEMK0Xih0xDj61h6cld1Jf735tsq0o,6543
-yamlres-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-yamlres-0.1.2.dist-info/top_level.txt,sha256=5OifXjvr0S9TmtwNt9XLht_86CWVo7u7RaMW2crkrG8,8
-yamlres-0.1.2.dist-info/RECORD,,
+yamlres/runner.py,sha256=VR-eZH0kX3jTD30KsLaXAC-GJgB4Fqw_pOTHUnDoZzc,4339
+yamlres-0.1.3.dist-info/METADATA,sha256=UCtvtwtuSlh73xY-HlEDg7pldY3IXRaKHl7NMQNymds,6534
+yamlres-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+yamlres-0.1.3.dist-info/top_level.txt,sha256=5OifXjvr0S9TmtwNt9XLht_86CWVo7u7RaMW2crkrG8,8
+yamlres-0.1.3.dist-info/RECORD,,
```

