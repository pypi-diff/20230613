# Comparing `tmp/check_requirements_txt-1.1.6-py3-none-any.whl.zip` & `tmp/check_requirements_txt-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5535 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7153 b- defN 23-Jun-13 04:41 check_requirements_txt.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2213 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      653 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/RECORD
-7 files, 11257 bytes uncompressed, 4353 bytes compressed:  61.3%
+Zip file size: 5666 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7702 b- defN 23-Jun-13 05:52 check_requirements_txt.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2213 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      653 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/RECORD
+7 files, 11806 bytes uncompressed, 4484 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: check_requirements_txt.py
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/LICENSE
+Filename: check_requirements_txt-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/METADATA
+Filename: check_requirements_txt-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/WHEEL
+Filename: check_requirements_txt-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/entry_points.txt
+Filename: check_requirements_txt-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/top_level.txt
+Filename: check_requirements_txt-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.6.dist-info/RECORD
+Filename: check_requirements_txt-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_requirements_txt.py

```diff
@@ -45,24 +45,39 @@
         requires.update(find_depends(req.name))
     return list(requires)
 
 
 @functools.lru_cache()
 def find_real_modules(package_name: str) -> List[str]:
     try:
-        metadata_dir = pkg_resources.get_distribution(package_name).egg_info
+        egg_dir = Path(pkg_resources.get_distribution(package_name).egg_info)
     except pkg_resources.DistributionNotFound:
         return [package_name]
-    top_level_file = Path(metadata_dir) / "top_level.txt"
+    top_level_file = egg_dir / "top_level.txt"
     if top_level_file.exists() and top_level_file.is_file():
         real_modules = []
         with open(top_level_file) as file_obj:
             for line in file_obj:
                 real_modules.append(line.strip().lower())
         return real_modules
+
+    # Some packages do not have "top_level.txt", such as "attrs".
+    # We can use "RECORD" file to find the possible modules.
+    record = egg_dir / "RECORD"
+    if record.exists() and record.is_file():
+        real_modules = []
+        with open(record) as file_obj:
+            for line in file_obj:
+                path = line.split(",", 1)[0].strip()
+                if egg_dir.name in path:
+                    continue
+                if '__init__.' in path:
+                    real_modules.append(os.path.dirname(path))
+        return real_modules
+
     return [package_name]
 
 
 def parse_requirements(path: Path) -> Iterable[str]:
     with open(path) as req_file:
         for line in req_file:
             if line.startswith("-r"):
```

## Comparing `check_requirements_txt-1.1.6.dist-info/LICENSE` & `check_requirements_txt-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `check_requirements_txt-1.1.6.dist-info/METADATA` & `check_requirements_txt-1.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-requirements-txt
-Version: 1.1.6
+Version: 1.1.7
 Summary: Check the missing packages in requirements.txt
 Home-page: https://github.com/ferstar/check-requirements-txt
 Author: ferstar
 Author-email: zhangjianfei3@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

