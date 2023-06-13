# Comparing `tmp/jsfuzz-0.1.1.tar.gz` & `tmp/jsfuzz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsfuzz-0.1.1.tar", max compression
+gzip compressed data, was "jsfuzz-1.0.0.tar", max compression
```

## Comparing `jsfuzz-0.1.1.tar` & `jsfuzz-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/LICENSE
--rw-r--r--   0        0        0     1754 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/README.md
--rw-r--r--   0        0        0     2068 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/jsfuzz/inspector.py
--rw-r--r--   0        0        0      430 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 jsfuzz-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 08:18:09.902000 jsfuzz-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1807 2023-06-13 08:18:09.902000 jsfuzz-1.0.0/README.md
+-rw-r--r--   0        0        0     2060 2023-06-13 08:18:09.902000 jsfuzz-1.0.0/jsfuzz/inspector.py
+-rw-r--r--   0        0        0      479 2023-06-13 08:18:09.902000 jsfuzz-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 jsfuzz-1.0.0/PKG-INFO
```

### Comparing `jsfuzz-0.1.1/LICENSE` & `jsfuzz-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsfuzz-0.1.1/README.md` & `jsfuzz-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Fuzzy matching for JSON payload. Find json_path that matches best for your provided value
 
+## Demo: https://huggingface.co/spaces/3cham/jsfuzz
+
 ## Install
 ```bash
 $ pip install jsfuzz
 ```
 
 ## Examples:
```

### Comparing `jsfuzz-0.1.1/jsfuzz/inspector.py` & `jsfuzz-1.0.0/jsfuzz/inspector.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def similarity_score(node_path: str, node_value: str, value: str) -> float:
     parts = node_path.split(".")
     # iterate through all the node names along the path and calculate the best match
     node_path_score = max([fuzz.partial_ratio(part.lower(), value.lower()) for part in parts])
 
     node_value_score = fuzz.partial_ratio(node_value.lower(), value.lower())
-    return 0.7 * node_path_score + 0.3 * node_value_score
+    return max(node_path_score, node_value_score)
 
 
 def traverse(obj: object, path: str, candidates: list, value: str, top_k: int) -> list:
     if type(obj) == dict:
         for key in obj:
             candidates = traverse(obj[key], path=f"{path}.{key}", candidates=candidates, value=value, top_k=top_k)
         return candidates
```

### Comparing `jsfuzz-0.1.1/PKG-INFO` & `jsfuzz-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: jsfuzz
-Version: 0.1.1
+Version: 1.0.0
 Summary: Inspect json data and fuzzy search for values or key names
+Home-page: https://github.com/3cham/jsfuzz.git
 License: MIT
 Author: Tung Dang
 Author-email: tung.dang@otto.de
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rapidfuzz (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Fuzzy matching for JSON payload. Find json_path that matches best for your provided value
 
+## Demo: https://huggingface.co/spaces/3cham/jsfuzz
+
 ## Install
 ```bash
 $ pip install jsfuzz
 ```
 
 ## Examples:
```

