# Comparing `tmp/check_requirements_txt-1.1.5-py3-none-any.whl.zip` & `tmp/check_requirements_txt-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5729 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7557 b- defN 23-Apr-06 06:25 check_requirements_txt.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2215 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      653 b- defN 23-Apr-06 06:25 check_requirements_txt-1.1.5.dist-info/RECORD
-7 files, 11662 bytes uncompressed, 4547 bytes compressed:  61.0%
+Zip file size: 5535 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7153 b- defN 23-Jun-13 04:41 check_requirements_txt.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2213 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      653 b- defN 23-Jun-13 04:56 check_requirements_txt-1.1.6.dist-info/RECORD
+7 files, 11257 bytes uncompressed, 4353 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: check_requirements_txt.py
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/LICENSE
+Filename: check_requirements_txt-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/METADATA
+Filename: check_requirements_txt-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/WHEEL
+Filename: check_requirements_txt-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/entry_points.txt
+Filename: check_requirements_txt-1.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/top_level.txt
+Filename: check_requirements_txt-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: check_requirements_txt-1.1.5.dist-info/RECORD
+Filename: check_requirements_txt-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## check_requirements_txt.py

```diff
@@ -1,9 +1,9 @@
 import argparse
-import logging
+import functools
 import os
 import re
 import sys
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict
 from typing import Generator
@@ -15,47 +15,42 @@
 from typing import Union
 
 import pkg_resources
 
 MODULE_IMPORT_P = re.compile(r"^\s*?import\s+(?P<module>[a-zA-Z0-9_]+)")
 MODULE_FROM_P = re.compile(r"^\s*?from\s+(?P<module>[a-zA-Z0-9_]+).*?\simport")
 DROP_LINE_P = re.compile(r"^\w+:/+", re.I)
-P_QUOTE = re.compile(r'\(\s*[>=<].*?\)')
-P_EMPTY = re.compile(r'\s')
 project_modules = set()
 
 
 def stdlibs() -> List[str]:
     ver = sys.version_info
     if ver < (3, 10):
         from stdlib_list import stdlib_list
         return stdlib_list(f"{ver.major}.{ver.minor}")
     else:
         return list(set(list(sys.stdlib_module_names) + list(sys.builtin_module_names)))
 
 
+@functools.lru_cache()
 def find_depends(package_name: str) -> List[str]:
-    package = pkg_resources.working_set.by_key.get(package_name)
-    if not package:
-        return [package_name]
-    headers = []
+    requires = set()
     try:
-        headers.extend(package._parsed_pkg_info._headers)
-    except Exception as e:
-        logging.warning("package %s has no header, error: %s", headers, e)
-    for i, header in enumerate(headers):
-        if header[0] == "Requires-Dist":
-            matched = P_QUOTE.search(header[1])
-            if matched and not P_EMPTY.sub('', matched.group())[-2].isdigit():
-                logging.warning("wrong format for version `%s`", header[1])
-            new_version = P_QUOTE.sub('', header[1]).rstrip()
-            package._parsed_pkg_info._headers[i] = header[0], new_version
-    return [r.key for r in package.requires()]
+        dist_obj = pkg_resources.get_distribution(package_name)
+    except pkg_resources.DistributionNotFound:
+        return [package_name]
+    for req in dist_obj.requires():
+        if req.marker and not req.marker.evaluate():
+            continue
+        requires.add(req.name)
+        requires.update(find_depends(req.name))
+    return list(requires)
 
 
+@functools.lru_cache()
 def find_real_modules(package_name: str) -> List[str]:
     try:
         metadata_dir = pkg_resources.get_distribution(package_name).egg_info
     except pkg_resources.DistributionNotFound:
         return [package_name]
     top_level_file = Path(metadata_dir) / "top_level.txt"
     if top_level_file.exists() and top_level_file.is_file():
```

## Comparing `check_requirements_txt-1.1.5.dist-info/LICENSE` & `check_requirements_txt-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `check_requirements_txt-1.1.5.dist-info/METADATA` & `check_requirements_txt-1.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: check-requirements-txt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Check the missing packages in requirements.txt
 Home-page: https://github.com/ferstar/check-requirements-txt
 Author: ferstar
 Author-email: zhangjianfei3@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: stdlib-list ; python_version < "3.10"
 
 check-requirements-txt
 ==================
 
 A tool (and also a pre-commit hook) to automatically check the missing packages in requirements.txt.
 
@@ -64,7 +64,9 @@
 Bad import detected: "requests"
 /Users/ferstar/PycharmProjects/xxx_demo/xxx_handler.py:17
 "numpy" required by: {'numpy', 'scikit-learn', 'tensorflow', 'pandas'}
 # NOTE: the output of cli is the total bad import count
 ~ echo $?
 ~ 2
 ```
+
+
```

## Comparing `check_requirements_txt-1.1.5.dist-info/RECORD` & `check_requirements_txt-1.1.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-check_requirements_txt.py,sha256=JyVtdV-xrnRKPaGjykFpLo7Six1BcKY179dvV1t0A_0,7557
-check_requirements_txt-1.1.5.dist-info/LICENSE,sha256=AUFJbQy786XqddWpNjpaZbNhx8j9sVq9E19FJQSNO9Y,1051
-check_requirements_txt-1.1.5.dist-info/METADATA,sha256=Ha_pmvE9LTys4FL7xQR-UsqZWgIGOMrMCCnqj64pDnk,2215
-check_requirements_txt-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-check_requirements_txt-1.1.5.dist-info/entry_points.txt,sha256=pidlhoCUlqNGu1jjeIsyVRxnvJwBhzpnFOLDqXzsumY,71
-check_requirements_txt-1.1.5.dist-info/top_level.txt,sha256=DzFwRy-Yd5omS8dGMMRQzf7ME4NfhptpxUUCRY_NdrI,23
-check_requirements_txt-1.1.5.dist-info/RECORD,,
+check_requirements_txt.py,sha256=3rh84Ow2yEhLyUvFXLmRMEUQpltwHNURog5BiOIjRwY,7153
+check_requirements_txt-1.1.6.dist-info/LICENSE,sha256=AUFJbQy786XqddWpNjpaZbNhx8j9sVq9E19FJQSNO9Y,1051
+check_requirements_txt-1.1.6.dist-info/METADATA,sha256=oE1NnMy27rrD1DysfGgEyGUmm6Ltx_r1iJF-n-UkCCU,2213
+check_requirements_txt-1.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+check_requirements_txt-1.1.6.dist-info/entry_points.txt,sha256=tunVRL-rMH7vmFBhqrnqiZibs9_6T-5b0uJZxeg7aMg,72
+check_requirements_txt-1.1.6.dist-info/top_level.txt,sha256=DzFwRy-Yd5omS8dGMMRQzf7ME4NfhptpxUUCRY_NdrI,23
+check_requirements_txt-1.1.6.dist-info/RECORD,,
```

