# Comparing `tmp/maccarone-0.1.0.tar.gz` & `tmp/maccarone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.1.0.tar", last modified: Sun Jun 11 00:08:16 2023, max compression
+gzip compressed data, was "maccarone-0.1.1.tar", last modified: Mon Jun 12 23:23:24 2023, max compression
```

## Comparing `maccarone-0.1.0.tar` & `maccarone-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.668154 maccarone-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-11 00:07:48.000000 maccarone-0.1.0/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-11 00:07:48.000000 maccarone-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-11 00:07:48.000000 maccarone-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 00:08:16.676154 maccarone-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 00:07:48.000000 maccarone-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-11 00:07:48.000000 maccarone-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/add.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/file_sizes.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/file_sizes.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/fizzbuzz.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/todo.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-11 00:07:48.000000 maccarone-0.1.0/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 00:07:48.000000 maccarone-0.1.0/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-11 00:07:48.000000 maccarone-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:08:16.676154 maccarone-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.668154 maccarone-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/caching.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/caching.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/loader.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/loader.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.json
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-11 00:08:08.000000 maccarone-0.1.0/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-11 00:07:48.000000 maccarone-0.1.0/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.672154 maccarone-0.1.0/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 00:08:16.000000 maccarone-0.1.0/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:08:16.676154 maccarone-0.1.0/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-11 00:07:48.000000 maccarone-0.1.0/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.525112 maccarone-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.529112 maccarone-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-12 23:22:45.000000 maccarone-0.1.1/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-12 23:22:45.000000 maccarone-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 23:22:45.000000 maccarone-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 23:23:24.537113 maccarone-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-12 23:22:45.000000 maccarone-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-12 23:22:45.000000 maccarone-0.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.533112 maccarone-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/add.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes_inlined.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/file_sizes_inlined.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/fizzbuzz.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/todo.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 23:22:45.000000 maccarone-0.1.1/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 23:22:45.000000 maccarone-0.1.1/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-12 23:22:45.000000 maccarone-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:23:24.537113 maccarone-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.525112 maccarone-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.533112 maccarone-0.1.1/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/caching.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/caching.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/loader.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/loader.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-12 23:23:13.000000 maccarone-0.1.1/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 23:22:45.000000 maccarone-0.1.1/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 23:23:24.000000 maccarone-0.1.1/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:23:24.537113 maccarone-0.1.1/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-12 23:22:45.000000 maccarone-0.1.1/support/rename_to_stale.sh
```

### Comparing `maccarone-0.1.0/.github/workflows/publish-to-pypi-stale.yml` & `maccarone-0.1.1/.github/workflows/publish-to-pypi-stale.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/.github/workflows/publish-to-pypi.yml` & `maccarone-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/.github/workflows/run-pytest.yml` & `maccarone-0.1.1/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/.gitignore` & `maccarone-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/LICENSE` & `maccarone-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/PKG-INFO` & `maccarone-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.0/README.md` & `maccarone-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/dev-requirements.txt` & `maccarone-0.1.1/dev-requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     # via
     #   maccarone (pyproject.toml)
     #   stale-maccarone
 packaging==23.1
     # via
     #   build
     #   pytest
+parsimonious==0.10.0
+    # via maccarone (pyproject.toml)
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
@@ -85,14 +87,16 @@
     #   maccarone (pyproject.toml)
     #   pytest-asyncio
     #   stale-maccarone
 pytest-asyncio==0.21.0
     # via
     #   maccarone (pyproject.toml)
     #   stale-maccarone
+regex==2023.6.3
+    # via parsimonious
 requests==2.30.0
     # via openai
 six==1.16.0
     # via asttokens
 stack-data==0.6.2
     # via ipython
 stale-maccarone==0.0.12
```

### Comparing `maccarone-0.1.0/examples/fizzbuzz.mn.json` & `maccarone-0.1.1/examples/fizzbuzz.mn.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'tagged_input_to_tagged_output'": "{'inputs_hash': "*

 * *                                    "'965706d855ac76c4bfd0514cb183871fc3230955a7220236d5f965603f6cb4d3'}"}*

```diff
@@ -1,6 +1,6 @@
 {
     "tagged_input_to_tagged_output": {
-        "inputs_hash": "350fe4a27767d6574b2d53e8dc5d16e9f9c6a97e14e1e5a565680c687afd3c2c",
+        "inputs_hash": "965706d855ac76c4bfd0514cb183871fc3230955a7220236d5f965603f6cb4d3",
         "value": "<completed id=\"0\">\nfor i in range(1, n + 1):\n    if i % 3 == 0 and i % 5 == 0:\n        print(\"FizzBuzz\")\n    elif i % 3 == 0:\n        print(\"Fizz\")\n    elif i % 5 == 0:\n        print(\"Buzz\")\n    else:\n        print(i)\n</>\n<completed id=\"1\">\nimport argparse\nparser = argparse.ArgumentParser()\nparser.add_argument(\"n\", type=int)\nargs = parser.parse_args()\nmain(args.n)\n</>"
     }
 }
```

### Comparing `maccarone-0.1.0/pyproject.toml` & `maccarone-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
     "stale_maccarone==0.0.12",
+    "parsimonious",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `maccarone-0.1.0/src/maccarone/caching.mn.py` & `maccarone-0.1.1/src/maccarone/caching.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/caching.py` & `maccarone-0.1.1/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/loader.mn.py` & `maccarone-0.1.1/src/maccarone/loader.mn.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/loader.py` & `maccarone-0.1.1/src/maccarone/loader.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/openai.py` & `maccarone-0.1.1/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.json` & `maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'tagged_input_to_tagged_output'": "{'inputs_hash': "*

 * *                                    "'f6eb8c528beaad4c1cdd702662650244e10726dcb97093968930adb4ff6f13e1', "*

 * *                                    '\'value\': \'<completed id="0">\\nmn_source = open(mn_path, '*

 * *                                    '"r").read()\\n</>\\n<completed id="1">\\nimport re\\npy_path '*

 * *                                    '= re.sub(f"{suffix}$", ".py", mn_path)\\n</>\\n<completed '*

 * *                                    'id="2">\\nif py_p […]*

```diff
@@ -1,6 +1,6 @@
 {
     "tagged_input_to_tagged_output": {
-        "inputs_hash": "204d447bb2a6752254bea6d4c7f7b52697a40b0d2c25729aa77938d06e1eb57c",
-        "value": "<completed id=\"0\">\nwith open(mn_path, \"r\") as f:\n    mn_source = f.read()\n</>\n<completed id=\"1\">\nimport re\npy_path = re.sub(f\"{suffix}$\", \".py\", mn_path)\n</>\n<completed id=\"2\">\nwith open(py_path, \"w\") as f:\n    f.write(py_source)\n</>\n<completed id=\"3\">\nfor mn_file in mn_files:\n    preprocess(mn_file, print_, write, suffix)\n</>\n<completed id=\"4\">\nimport argparse\nparser = argparse.ArgumentParser()\nparser.add_argument(\"path\", help=\"Path to the file or directory containing Maccarone snippets\")\nparser.add_argument(\"--print\", dest=\"print_\", action=\"store_true\", help=\"Print the preprocessed Python source\")\nparser.add_argument(\"--write\", action=\"store_true\", help=\"Write the preprocessed Python source to a file\")\nparser.add_argument(\"--suffix\", default=\".mn.py\", help=\"Suffix for files containing Maccarone snippets (default: .mn.py)\")\nargs = parser.parse_args()\nreturn args\n</>"
+        "inputs_hash": "f6eb8c528beaad4c1cdd702662650244e10726dcb97093968930adb4ff6f13e1",
+        "value": "<completed id=\"0\">\nmn_source = open(mn_path, \"r\").read()\n</>\n<completed id=\"1\">\nimport re\npy_path = re.sub(f\"{suffix}$\", \".py\", mn_path)\n</>\n<completed id=\"2\">\nif py_path is not None:\n    with open(py_path, \"w\") as f:\n        f.write(py_source)\n</>\n<completed id=\"3\">\nfor mn_file in mn_files:\n    preprocess(mn_file, print_, write, rewrite, suffix)\n</>\n<completed id=\"4\">\nimport argparse\nparser = argparse.ArgumentParser()\nparser.add_argument(\"path\", help=\"Path to the file or directory containing Maccarone snippets\")\nparser.add_argument(\"--print\", dest=\"print_\", action=\"store_true\", help=\"Print the preprocessed Python source\")\nparser.add_argument(\"--write\", action=\"store_true\", help=\"Write the preprocessed Python source to a new file\")\nparser.add_argument(\"--rewrite\", action=\"store_true\", help=\"Overwrite the input file with the preprocessed Python source\")\nparser.add_argument(\"--suffix\", default=\".mn.py\", help=\"Suffix for Maccarone snippet files (default: .mn.py)\")\nargs = parser.parse_args()\nreturn args\n</>"
     }
 }
```

### Comparing `maccarone-0.1.0/src/maccarone/scripts/preprocess.mn.py` & `maccarone-0.1.1/src/maccarone/scripts/preprocess.mn.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from argparse import Namespace
 
 from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
 logger = logging.getLogger(__name__)
 
-def preprocess(mn_path: str, print_: bool, write: bool, suffix: str) -> None:
+def preprocess(
+        mn_path: str,
+        print_: bool,
+        write: bool,
+        rewrite: bool,
+        suffix: str,
+    ) -> None:
     # produce Python source
     logger.info("preprocessing %s", mn_path)
 
     cache_path = mn_path.replace(suffix, ".mn.json")
     chat_api = CachedChatAPI(cache_path)
 
     #<<mn_source = read mn_path>>
@@ -23,21 +29,25 @@
     if write:
         #<<py_path = regex replace mn_path: f"{suffix}$" -> ".py">>
 
         logger.info("writing %s", py_path)
 
         if py_path == mn_path:
             raise ValueError("won't overwrite input file", mn_path)
+    elif rewrite:
+        py_path = mn_path
+    else:
+        py_path = None
 
-        #<<write py_source to py_path>>
+    #<<write py_source to py_path if not None>>
 
     if print_:
-        print(py_source)
+        print(py_source, end="")
 
-def main(path: str, print_: bool, write: bool, suffix: str) -> None:
+def main(path: str, print_: bool, write: bool, rewrite: bool, suffix: str) -> None:
     """Preprocess files with Maccarone snippets."""
 
     if os.path.isdir(path):
         mn_files = glob.glob(
             os.path.join(path, f"**/*{suffix}"),
             recursive=True,
         )
@@ -45,14 +55,15 @@
         mn_files = [path]
 
     #<<preprocess mn_files>>
 
 def parse_args() -> Namespace:
     #<<
     # get args for main() and return; use argparse
+    # set the `print_` var for `--print`
     # default suffix: ".mn.py"
     #>>
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
```

### Comparing `maccarone-0.1.0/src/maccarone/scripts/preprocess.py` & `maccarone-0.1.1/src/maccarone/scripts/preprocess.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,66 +5,77 @@
 from argparse import Namespace
 
 from maccarone.openai import CachedChatAPI
 from maccarone.preprocessor import preprocess_maccarone
 
 logger = logging.getLogger(__name__)
 
-def preprocess(mn_path: str, print_: bool, write: bool, suffix: str) -> None:
+def preprocess(
+        mn_path: str,
+        print_: bool,
+        write: bool,
+        rewrite: bool,
+        suffix: str,
+    ) -> None:
     # produce Python source
     logger.info("preprocessing %s", mn_path)
 
     cache_path = mn_path.replace(suffix, ".mn.json")
     chat_api = CachedChatAPI(cache_path)
 
-    with open(mn_path, "r") as f:
-        mn_source = f.read()
+    mn_source = open(mn_path, "r").read()
 
 
     py_source = preprocess_maccarone(mn_source, chat_api)
 
     if write:
         import re
         py_path = re.sub(f"{suffix}$", ".py", mn_path)
 
 
         logger.info("writing %s", py_path)
 
         if py_path == mn_path:
             raise ValueError("won't overwrite input file", mn_path)
+    elif rewrite:
+        py_path = mn_path
+    else:
+        py_path = None
 
+    if py_path is not None:
         with open(py_path, "w") as f:
             f.write(py_source)
 
 
     if print_:
-        print(py_source)
+        print(py_source, end="")
 
-def main(path: str, print_: bool, write: bool, suffix: str) -> None:
+def main(path: str, print_: bool, write: bool, rewrite: bool, suffix: str) -> None:
     """Preprocess files with Maccarone snippets."""
 
     if os.path.isdir(path):
         mn_files = glob.glob(
             os.path.join(path, f"**/*{suffix}"),
             recursive=True,
         )
     else:
         mn_files = [path]
 
     for mn_file in mn_files:
-        preprocess(mn_file, print_, write, suffix)
+        preprocess(mn_file, print_, write, rewrite, suffix)
 
 
 def parse_args() -> Namespace:
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument("path", help="Path to the file or directory containing Maccarone snippets")
     parser.add_argument("--print", dest="print_", action="store_true", help="Print the preprocessed Python source")
-    parser.add_argument("--write", action="store_true", help="Write the preprocessed Python source to a file")
-    parser.add_argument("--suffix", default=".mn.py", help="Suffix for files containing Maccarone snippets (default: .mn.py)")
+    parser.add_argument("--write", action="store_true", help="Write the preprocessed Python source to a new file")
+    parser.add_argument("--rewrite", action="store_true", help="Overwrite the input file with the preprocessed Python source")
+    parser.add_argument("--suffix", default=".mn.py", help="Suffix for Maccarone snippet files (default: .mn.py)")
     args = parser.parse_args()
     return args
 
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
```

### Comparing `maccarone-0.1.0/src/maccarone/test/test_caching.py` & `maccarone-0.1.1/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.1.0/src/maccarone/test/test_preprocessor.py` & `maccarone-0.1.1/src/maccarone/test/test_preprocessor.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,42 +8,81 @@
     raw_source_to_pieces,
     raw_pieces_to_tagged_input,
     tagged_output_to_completed_pieces,
 )
 
 @pytest.mark.parametrize("input, expected", [
     (
-        "",
-        [PresentPiece("")],
+        """
+        this source has
+        #<<a missing piece>>
+        above
+        """,
+        [
+            PresentPiece("\nthis source has\n"),
+            MissingPiece("", "a missing piece"),
+            PresentPiece("above\n"),
+        ],
     ),
     (
-        "This is a normal string",
-        [PresentPiece("This is a normal string")],
+        """
+        this source has
+        #<<a missing piece>>
+        with inline source
+        #<</>>
+        above
+        """,
+        [
+            PresentPiece("\nthis source has\n"),
+            MissingPiece("", "a missing piece", "with inline source\n"),
+            PresentPiece("above\n"),
+        ],
     ),
     (
-        "This string has #<<one>> missing piece",
+        """
+        this source has
+        #<<
+        # a missing piece
+        # with multiline guidance
+        #>>
+        and inline source
+        #<</>>
+        above
+        """,
         [
-            PresentPiece("This string has "),
-            MissingPiece("", "one"),
-            PresentPiece(" missing piece"),
+            PresentPiece("\nthis source has\n"),
+            MissingPiece(
+                "",
+                " a missing piece\n with multiline guidance",
+                "and inline source\n",
+            ),
+            PresentPiece("above\n"),
         ],
     ),
     (
-        "This string has #<<one>> and #<<two>> missing pieces",
+        """
+        this source has...*
+        #<<various special chars, (like this)>>
+        and inline source with more chars _-%$
+        #<</>>
+        `and more!`
+        """,
         [
-            PresentPiece("This string has "),
-            MissingPiece("", "one"),
-            PresentPiece(" and "),
-            MissingPiece("", "two"),
-            PresentPiece(" missing pieces"),
+            PresentPiece("\nthis source has...*\n"),
+            MissingPiece(
+                "",
+                "various special chars, (like this)",
+                "and inline source with more chars _-%$\n",
+            ),
+            PresentPiece("`and more!`\n"),
         ],
     ),
 ])
 def test_raw_source_to_pieces(input, expected):
-    assert list(raw_source_to_pieces(input)) == expected
+    assert list(raw_source_to_pieces(dedent(input))) == expected
 
 @pytest.mark.parametrize("raw_pieces, expected", [
     (
         [
             PresentPiece("\ndef add_two_numbers(x, y):\n    "),
             MissingPiece("    ", "add the args"),
             PresentPiece("\n\n"),
```

### Comparing `maccarone-0.1.0/src/maccarone.egg-info/PKG-INFO` & `maccarone-0.1.1/src/maccarone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maccarone
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mix natural language into your Python code
 Project-URL: Homepage, https://github.com/bsilverthorn/maccarone
 Project-URL: Repository, https://github.com/bsilverthorn/maccarone
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `maccarone-0.1.0/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.1.1/src/maccarone.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run-pytest.yml
 examples/__init__.py
 examples/add.mn.json
 examples/add.mn.py
 examples/file_sizes.mn.json
 examples/file_sizes.mn.py
+examples/file_sizes_inlined.mn.json
+examples/file_sizes_inlined.mn.py
 examples/fizzbuzz.mn.json
 examples/fizzbuzz.mn.py
 examples/todo.mn.json
 examples/todo.mn.py
 src/maccarone/__init__.py
 src/maccarone/caching.mn.json
 src/maccarone/caching.mn.py
```

### Comparing `maccarone-0.1.0/support/rename_to_stale.sh` & `maccarone-0.1.1/support/rename_to_stale.sh`

 * *Files identical despite different names*

