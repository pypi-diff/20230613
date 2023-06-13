# Comparing `tmp/cerebrium-1.1.0.tar.gz` & `tmp/cerebrium-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.0.tar", max compression
+gzip compressed data, was "cerebrium-1.1.1.tar", max compression
```

## Comparing `cerebrium-1.1.0.tar` & `cerebrium-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-09 13:01:37.533263 cerebrium-1.1.0/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-09 13:01:37.533263 cerebrium-1.1.0/README.md
--rw-r--r--   0        0        0      330 2023-06-09 13:05:25.573181 cerebrium-1.1.0/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     8671 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/cli.py
--rw-r--r--   0        0        0    31667 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/conduit.py
--rw-r--r--   0        0        0     5049 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/errors.py
--rw-r--r--   0        0        0    11299 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8540 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-09 13:01:37.533263 cerebrium-1.1.0/cerebrium/utils.py
--rw-r--r--   0        0        0     2546 2023-06-09 13:05:25.569181 cerebrium-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-13 21:26:20.075493 cerebrium-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-13 21:26:20.075493 cerebrium-1.1.1/README.md
+-rw-r--r--   0        0        0      330 2023-06-13 21:31:24.282792 cerebrium-1.1.1/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     9110 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/cli.py
+-rw-r--r--   0        0        0    31667 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5049 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-13 21:26:20.075493 cerebrium-1.1.1/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8540 2023-06-13 21:26:20.079493 cerebrium-1.1.1/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-13 21:26:20.079493 cerebrium-1.1.1/cerebrium/utils.py
+-rw-r--r--   0        0        0     2546 2023-06-13 21:31:24.282792 cerebrium-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.1/PKG-INFO
```

### Comparing `cerebrium-1.1.0/LICENSE` & `cerebrium-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/README.md` & `cerebrium-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/cli.py` & `cerebrium-1.1.1/cerebrium/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,26 @@
     Deploy a builder deployment to Cerebrium
     """
     print(f"Deploying {name} with {hardware} hardware to Cerebrium...")
 
     requirements_hash = "REQUIREMENTS_FILE_DOESNT_EXIST"
     pkglist_hash = "PKGLIST_FILE_DOESNT_EXIST"
 
+    # Check if main.py exists
+    if not os.path.exists("./main.py"):
+        print("main.py not found in current directory. This file is required.")
+        sys.exit(1)
+
+    # Check main.py for a predict function
+    with open("./main.py", "r") as f:
+        main_py = f.read()
+        if "def predict(" not in main_py:
+            print("main.py does not contain a predict function. This function is required.")
+            sys.exit(1)
+
     # Calc MD5 hash of ./requirements.txt
     if os.path.exists("./requirements.txt"):
         with open("./requirements.txt", "rb") as f:
             requirements_hash = hashlib.md5(f.read()).hexdigest()
 
     # Calc MD5 hash of ./pkglist.txt if it exists
     if os.path.exists("./pkglist.txt"):
```

### Comparing `cerebrium-1.1.0/cerebrium/conduit.py` & `cerebrium-1.1.1/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/core.py` & `cerebrium-1.1.1/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/errors.py` & `cerebrium-1.1.1/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/flow.py` & `cerebrium-1.1.1/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/logging/arize.py` & `cerebrium-1.1.1/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/logging/base.py` & `cerebrium-1.1.1/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/logging/censius.py` & `cerebrium-1.1.1/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/models/base.py` & `cerebrium-1.1.1/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/models/sklearn.py` & `cerebrium-1.1.1/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/cerebrium/requests.py` & `cerebrium-1.1.1/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.0/pyproject.toml` & `cerebrium-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.1.0/PKG-INFO` & `cerebrium-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

