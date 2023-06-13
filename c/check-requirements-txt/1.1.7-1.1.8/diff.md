# Comparing `tmp/check_requirements_txt-1.1.7-py3-none-any.whl.zip` & `tmp/check_requirements_txt-1.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 5666 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7702 b- defN 23-Jun-13 05:52 check_requirements_txt.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2213 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      653 b- defN 23-Jun-13 05:53 check_requirements_txt-1.1.7.dist-info/RECORD
-7 files, 11806 bytes uncompressed, 4484 bytes compressed:  62.0%
+-rw-r--r--  2.0 unx     7661 b- defN 23-Jun-13 06:03 check_requirements_txt.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2213 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      653 b- defN 23-Jun-13 06:05 check_requirements_txt-1.1.8.dist-info/RECORD
+7 files, 11765 bytes uncompressed, 4484 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: check_requirements_txt.py
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/LICENSE
+Filename: check_requirements_txt-1.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/METADATA
+Filename: check_requirements_txt-1.1.8.dist-info/METADATA
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/WHEEL
+Filename: check_requirements_txt-1.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/entry_points.txt
+Filename: check_requirements_txt-1.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/top_level.txt
+Filename: check_requirements_txt-1.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.7.dist-info/RECORD
+Filename: check_requirements_txt-1.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_requirements_txt.py

```diff
@@ -48,37 +48,37 @@
 
 @functools.lru_cache()
 def find_real_modules(package_name: str) -> List[str]:
     try:
         egg_dir = Path(pkg_resources.get_distribution(package_name).egg_info)
     except pkg_resources.DistributionNotFound:
         return [package_name]
+
+    modules = set()
     top_level_file = egg_dir / "top_level.txt"
     if top_level_file.exists() and top_level_file.is_file():
-        real_modules = []
         with open(top_level_file) as file_obj:
             for line in file_obj:
-                real_modules.append(line.strip().lower())
-        return real_modules
+                modules.add(line.strip().lower())
 
     # Some packages do not have "top_level.txt", such as "attrs".
     # We can use "RECORD" file to find the possible modules.
     record = egg_dir / "RECORD"
     if record.exists() and record.is_file():
-        real_modules = []
         with open(record) as file_obj:
             for line in file_obj:
                 path = line.split(",", 1)[0].strip()
                 if egg_dir.name in path:
                     continue
                 if '__init__.' in path:
-                    real_modules.append(os.path.dirname(path))
-        return real_modules
+                    modules.add(Path(path).parent.name.lower())
 
-    return [package_name]
+    if not modules:
+        modules.add(package_name)
+    return list(modules)
 
 
 def parse_requirements(path: Path) -> Iterable[str]:
     with open(path) as req_file:
         for line in req_file:
             if line.startswith("-r"):
                 # nested requirements path: "-r another-path.txt"
```

## Comparing `check_requirements_txt-1.1.7.dist-info/LICENSE` & `check_requirements_txt-1.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `check_requirements_txt-1.1.7.dist-info/METADATA` & `check_requirements_txt-1.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-requirements-txt
-Version: 1.1.7
+Version: 1.1.8
 Summary: Check the missing packages in requirements.txt
 Home-page: https://github.com/ferstar/check-requirements-txt
 Author: ferstar
 Author-email: zhangjianfei3@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `check_requirements_txt-1.1.7.dist-info/RECORD` & `check_requirements_txt-1.1.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-check_requirements_txt.py,sha256=MAk1aNdzlo-GTBpJju5qOxuiZXKQpp8g5blK7ETaAws,7702
-check_requirements_txt-1.1.7.dist-info/LICENSE,sha256=AUFJbQy786XqddWpNjpaZbNhx8j9sVq9E19FJQSNO9Y,1051
-check_requirements_txt-1.1.7.dist-info/METADATA,sha256=H1HRAS_XVzji2u4rDoh2DyxQzH3Vgi1KNyB6LSJVMyk,2213
-check_requirements_txt-1.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-check_requirements_txt-1.1.7.dist-info/entry_points.txt,sha256=tunVRL-rMH7vmFBhqrnqiZibs9_6T-5b0uJZxeg7aMg,72
-check_requirements_txt-1.1.7.dist-info/top_level.txt,sha256=DzFwRy-Yd5omS8dGMMRQzf7ME4NfhptpxUUCRY_NdrI,23
-check_requirements_txt-1.1.7.dist-info/RECORD,,
+check_requirements_txt.py,sha256=7XIbXSeDHqwPbNF2R1EUKfmtW3UGYJ_vYVCpBN-XUh8,7661
+check_requirements_txt-1.1.8.dist-info/LICENSE,sha256=AUFJbQy786XqddWpNjpaZbNhx8j9sVq9E19FJQSNO9Y,1051
+check_requirements_txt-1.1.8.dist-info/METADATA,sha256=rt1Gl0qZeEl2yXJNuqJ0U-XGo3QB7MnFIow68ALAZ0w,2213
+check_requirements_txt-1.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+check_requirements_txt-1.1.8.dist-info/entry_points.txt,sha256=tunVRL-rMH7vmFBhqrnqiZibs9_6T-5b0uJZxeg7aMg,72
+check_requirements_txt-1.1.8.dist-info/top_level.txt,sha256=DzFwRy-Yd5omS8dGMMRQzf7ME4NfhptpxUUCRY_NdrI,23
+check_requirements_txt-1.1.8.dist-info/RECORD,,
```

