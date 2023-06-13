# Comparing `tmp/check-jsonschema-0.9.0.tar.gz` & `tmp/check-jsonschema-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check-jsonschema-0.9.0.tar", last modified: Mon Dec 13 19:01:22 2021, max compression
+gzip compressed data, was "check-jsonschema-0.9.1.tar", last modified: Thu Dec 16 20:42:37 2021, max compression
```

## Comparing `check-jsonschema-0.9.0.tar` & `check-jsonschema-0.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.368586 check-jsonschema-0.9.0/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      583 2021-01-08 05:26:01.000000 check-jsonschema-0.9.0/LICENSE
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      113 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/MANIFEST.in
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5899 2021-12-13 19:01:22.368586 check-jsonschema-0.9.0/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5314 2021-12-13 19:00:14.000000 check-jsonschema-0.9.0/README.md
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1113 2021-12-13 19:01:22.372586 check-jsonschema-0.9.0/setup.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       38 2021-01-08 04:02:34.000000 check-jsonschema-0.9.0/setup.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.360586 check-jsonschema-0.9.0/src/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.364586 check-jsonschema-0.9.0/src/check_jsonschema/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      669 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.364586 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1236 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.364586 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/custom/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/custom/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1237 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/custom/github-workflows-require-timeout.json
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.368586 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1162 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.azure-pipelines
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1083 2021-12-10 22:21:44.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.readthedocs
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    35973 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.renovate
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11358 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.schemastore
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      758 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/README.md
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)   941405 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    29111 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-actions.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-actions.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    93868 2021-12-13 18:37:21.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-workflows.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:37:21.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-workflows.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9914 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/readthedocs.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/readthedocs.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    75784 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/renovate.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/renovate.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    65341 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/travis.json
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-13 18:37:22.000000 check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/travis.sha256
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3737 2021-12-09 19:32:11.000000 check-jsonschema-0.9.0/src/check_jsonschema/cachedownloader.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2964 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/checker.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1477 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/formats.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.368586 check-jsonschema-0.9.0/src/check_jsonschema/loaders/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      444 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/loaders/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      143 2021-10-29 16:27:48.000000 check-jsonschema-0.9.0/src/check_jsonschema/loaders/errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1244 2021-12-09 22:07:05.000000 check-jsonschema-0.9.0/src/check_jsonschema/loaders/instance.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5633 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/loaders/schema.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4041 2021-12-13 18:51:15.000000 check-jsonschema-0.9.0/src/check_jsonschema/parse_cli.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2051 2021-11-10 19:07:02.000000 check-jsonschema-0.9.0/src/check_jsonschema/utils.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-13 19:01:22.364586 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5899 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1981 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/SOURCES.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/dependency_links.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       60 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/entry_points.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      144 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/requires.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       17 2021-12-13 19:01:22.000000 check-jsonschema-0.9.0/src/check_jsonschema.egg-info/top_level.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.752498 check-jsonschema-0.9.1/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      583 2021-01-08 05:26:01.000000 check-jsonschema-0.9.1/LICENSE
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      113 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/MANIFEST.in
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5899 2021-12-16 20:42:37.752498 check-jsonschema-0.9.1/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5314 2021-12-13 19:00:14.000000 check-jsonschema-0.9.1/README.md
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1113 2021-12-16 20:42:37.752498 check-jsonschema-0.9.1/setup.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       38 2021-01-08 04:02:34.000000 check-jsonschema-0.9.1/setup.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.732499 check-jsonschema-0.9.1/src/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.736498 check-jsonschema-0.9.1/src/check_jsonschema/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      669 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.740498 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1236 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.740498 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/custom/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/custom/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1237 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/custom/github-workflows-require-timeout.json
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.748499 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1162 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.azure-pipelines
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1083 2021-12-10 22:21:44.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.readthedocs
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    35973 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.renovate
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11358 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.schemastore
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      758 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/README.md
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)   967276 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    29111 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-actions.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-actions.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    93868 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-workflows.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-workflows.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9914 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/readthedocs.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/readthedocs.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    75784 2021-12-16 20:15:52.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/renovate.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:52.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/renovate.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    65341 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/travis.json
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       64 2021-12-16 20:15:51.000000 check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/travis.sha256
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3737 2021-12-09 19:32:11.000000 check-jsonschema-0.9.1/src/check_jsonschema/cachedownloader.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2964 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/checker.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1477 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/formats.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.748499 check-jsonschema-0.9.1/src/check_jsonschema/loaders/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      444 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/loaders/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      143 2021-10-29 16:27:48.000000 check-jsonschema-0.9.1/src/check_jsonschema/loaders/errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1244 2021-12-09 22:07:05.000000 check-jsonschema-0.9.1/src/check_jsonschema/loaders/instance.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5633 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/loaders/schema.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4041 2021-12-13 18:51:15.000000 check-jsonschema-0.9.1/src/check_jsonschema/parse_cli.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2051 2021-11-10 19:07:02.000000 check-jsonschema-0.9.1/src/check_jsonschema/utils.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2021-12-16 20:42:37.736498 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5899 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1981 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       60 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/entry_points.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      144 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/requires.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       17 2021-12-16 20:42:37.000000 check-jsonschema-0.9.1/src/check_jsonschema.egg-info/top_level.txt
```

### Comparing `check-jsonschema-0.9.0/LICENSE` & `check-jsonschema-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/PKG-INFO` & `check-jsonschema-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-jsonschema
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pre-commit hook for validating files against jsonschemas.
 Home-page: https://github.com/sirosen/check-jsonschema
 Author: Stephen Rosen
 Author-email: sirosen@uchicago.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `check-jsonschema-0.9.0/README.md` & `check-jsonschema-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/setup.cfg` & `check-jsonschema-0.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = check-jsonschema
-version = 0.9.0
+version = 0.9.1
 description = A pre-commit hook for validating files against jsonschemas.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sirosen/check-jsonschema
 author = Stephen Rosen
 author_email = sirosen@uchicago.edu
 classifiers =
```

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/__init__.py` & `check-jsonschema-0.9.1/src/check_jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/__init__.py` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/custom/github-workflows-require-timeout.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/custom/github-workflows-require-timeout.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.azure-pipelines` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.azure-pipelines`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.readthedocs` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.readthedocs`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.renovate` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.renovate`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/LICENSE.schemastore` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/LICENSE.schemastore`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/README.md` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/README.md`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/azure-pipelines.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8564776739968846%*

 * *Differences: {"'$comment'": "'v1.195.0'",*

 * * "'$id'": "'https://github.com/Microsoft/azure-pipelines-vscode/blob/main/service-schema.json'",*

 * * "'definitions'": "{'pipeline': {'anyOf': {0: {'properties': {'lockBehavior': "*

 * *                  "OrderedDict([('description', 'Behavior lock requests from this stage should "*

 * *                  "exhibit in relation to other exclusive lock requests'), ('$ref', "*

 * *                  "'#/definitions/lockBehavior')])}}, 1: {'properties': {'lockBehavior': "*

 * *                  "OrderedDict([ […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "$comment": "v1.187.0",
-    "$id": "https://github.com/microsoft/azure-pipelines-vscode/blob/main/service-schema.json",
+    "$comment": "v1.195.0",
+    "$id": "https://github.com/Microsoft/azure-pipelines-vscode/blob/main/service-schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "any": {
             "anyOf": [
                 {
                     "type": "string"
                 },
@@ -949,14 +949,26 @@
                 },
                 "repo": {
                     "$ref": "#/definitions/legacyRepoResourceAlias"
                 }
             },
             "type": "object"
         },
+        "lockBehavior": {
+            "anyOf": [
+                {
+                    "pattern": "^sequential$",
+                    "type": "string"
+                },
+                {
+                    "pattern": "^runLatest$",
+                    "type": "string"
+                }
+            ]
+        },
         "mapping": {
             "additionalProperties": true,
             "type": "object"
         },
         "mappingOfStringString": {
             "additionalProperties": true,
             "type": "object"
@@ -1371,14 +1383,18 @@
             "type": "array"
         },
         "pipeline": {
             "anyOf": [
                 {
                     "additionalProperties": false,
                     "properties": {
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1419,14 +1435,18 @@
                 {
                     "additionalProperties": false,
                     "properties": {
                         "extends": {
                             "$ref": "#/definitions/extends",
                             "description": "Extends a template"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1463,14 +1483,18 @@
                 {
                     "additionalProperties": false,
                     "properties": {
                         "jobs": {
                             "$ref": "#/definitions/jobs",
                             "description": "Jobs represent units of work which can be assigned to a single agent or server"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1503,14 +1527,18 @@
                         "jobs"
                     ],
                     "type": "object"
                 },
                 {
                     "additionalProperties": false,
                     "properties": {
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1553,14 +1581,18 @@
                             "$ref": "#/definitions/jobContainer",
                             "description": "Container resource name"
                         },
                         "continueOnError": {
                             "$ref": "#/definitions/jobContinueOnError",
                             "description": "Continue running even on failure?"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1612,14 +1644,18 @@
                     "additionalProperties": false,
                     "deprecationMessage": "This option is deprecated, use `job` (inside `jobs`) instead",
                     "properties": {
                         "continueOnError": {
                             "$ref": "#/definitions/jobContinueOnError",
                             "description": "Continue running even on failure?"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1663,14 +1699,18 @@
                     "additionalProperties": false,
                     "deprecationMessage": "This option is deprecated, use `job` (inside `jobs`) instead",
                     "properties": {
                         "continueOnError": {
                             "$ref": "#/definitions/jobContinueOnError",
                             "description": "Continue running even on failure?"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "name": {
                             "$ref": "#/definitions/string_allowExpressions",
                             "description": "Pipeline name"
                         },
                         "parameters": {
                             "$ref": "#/definitions/pipelineTemplateParameters",
                             "description": "Pipeline template parameters"
@@ -1727,14 +1767,18 @@
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Extends a template"
                 },
                 "jobs": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Jobs which make up the pipeline"
                 },
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline template parameters"
@@ -1799,14 +1843,18 @@
                 }
             },
             "type": "object"
         },
         "pipelineBase": {
             "additionalProperties": false,
             "properties": {
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/string_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/pipelineTemplateParameters",
                     "description": "Pipeline template parameters"
@@ -1848,14 +1896,18 @@
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Extends a template"
                 },
                 "jobs": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Jobs which make up the pipeline"
                 },
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline template parameters"
@@ -1936,14 +1988,18 @@
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Extends a template"
                 },
                 "jobs": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Jobs which make up the pipeline"
                 },
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/pipelineTemplateParameters",
                     "description": "Pipeline template parameters"
@@ -2094,14 +2150,18 @@
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Extends a template"
                 },
                 "jobs": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Jobs which make up the pipeline"
                 },
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline template parameters"
@@ -2293,14 +2353,18 @@
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Extends a template"
                 },
                 "jobs": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Jobs which make up the pipeline"
                 },
+                "lockBehavior": {
+                    "$ref": "#/definitions/lockBehavior",
+                    "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                },
                 "name": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline name"
                 },
                 "parameters": {
                     "$ref": "#/definitions/any_allowExpressions",
                     "description": "Pipeline template parameters"
@@ -2724,14 +2788,18 @@
                             "$ref": "#/definitions/string",
                             "description": "Human-readable name for the stage"
                         },
                         "jobs": {
                             "$ref": "#/definitions/jobs",
                             "description": "Jobs which make up the stage"
                         },
+                        "lockBehavior": {
+                            "$ref": "#/definitions/lockBehavior",
+                            "description": "Behavior lock requests from this stage should exhibit in relation to other exclusive lock requests"
+                        },
                         "pool": {
                             "$ref": "#/definitions/pool",
                             "description": "Pool where jobs in this stage will run unless otherwise specified"
                         },
                         "stage": {
                             "$ref": "#/definitions/string",
                             "description": "ID of the stage"
@@ -2816,14 +2884,18 @@
                             "$ref": "#/definitions/string",
                             "description": "Fail the task if output is sent to Stderr?"
                         },
                         "name": {
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "script": {
                             "$ref": "#/definitions/string",
                             "description": "An inline script"
                         },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
@@ -2883,14 +2955,18 @@
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "powershell": {
                             "$ref": "#/definitions/string",
                             "description": "Inline PowerShell or reference to a PowerShell file"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -2946,14 +3022,18 @@
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "pwsh": {
                             "$ref": "#/definitions/string",
                             "description": "Inline PowerShell or reference to a PowerShell file"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3002,14 +3082,18 @@
                             "$ref": "#/definitions/string",
                             "description": "Fail the task if output is sent to Stderr?"
                         },
                         "name": {
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3078,14 +3162,18 @@
                             "$ref": "#/definitions/string",
                             "description": "Path of the repository to check out"
                         },
                         "persistCredentials": {
                             "$ref": "#/definitions/string",
                             "description": "Keep credentials available for later use?"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "submodules": {
                             "$ref": "#/definitions/string",
                             "description": "Check out Git submodules?"
                         },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
@@ -3135,14 +3223,18 @@
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "patterns": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Pattern to download files from artifact"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3195,14 +3287,18 @@
                             "$ref": "#/definitions/string",
                             "description": "Path to download the artifact into"
                         },
                         "patterns": {
                             "$ref": "#/definitions/string",
                             "description": "Downloads the files which matches the patterns"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3244,14 +3340,18 @@
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "path": {
                             "$ref": "#/definitions/string",
                             "description": "Path to download the package into"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3288,14 +3388,18 @@
                             "$ref": "#/definitions/mappingOfStringString",
                             "description": "Variables to map into the process's environment"
                         },
                         "name": {
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3340,14 +3444,18 @@
                         "name": {
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "publish": {
                             "$ref": "#/definitions/string"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3406,14 +3514,18 @@
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "The folder path to download the cache to. This can be a fully-qualified path or a path relative to the root of the repository. Wildcards are not supported."
                         },
                         "restoreCache": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "The name of the key"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
                         "timeoutInMinutes": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "Time to wait for this task to complete before the server kills it"
@@ -3455,14 +3567,18 @@
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
                         "path": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "The folder or file path to publish. This can be a fully-qualified path or a path relative to the root of the repository. Wildcards are not supported."
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "saveCache": {
                             "$ref": "#/definitions/nonEmptyString",
                             "description": "The name of the key"
                         },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
@@ -3504,14 +3620,18 @@
                             "$ref": "#/definitions/mappingOfStringString",
                             "description": "Variables to map into the process's environment"
                         },
                         "name": {
                             "$ref": "#/definitions/referenceName",
                             "description": "ID of the step"
                         },
+                        "retryCountOnTaskFailure": {
+                            "$ref": "#/definitions/string",
+                            "description": "Number of retries if the task fails"
+                        },
                         "reviewApp": {
                             "$ref": "#/definitions/string"
                         },
                         "target": {
                             "$ref": "#/definitions/stepTarget",
                             "description": "Environment in which to run this task"
                         },
@@ -3594,17 +3714,28 @@
                             "description": "PowerShell inputs",
                             "properties": {
                                 "arguments": {
                                     "description": "Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "debugPreference": {
+                                    "description": "DebugPreference",
+                                    "enum": [
+                                        "default",
+                                        "stop",
+                                        "continue",
+                                        "silentlyContinue"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "errorActionPreference": {
                                     "description": "ErrorActionPreference",
                                     "enum": [
+                                        "default",
                                         "stop",
                                         "continue",
                                         "silentlyContinue"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "failOnStderr": {
@@ -3618,14 +3749,24 @@
                                     "type": "string"
                                 },
                                 "ignoreLASTEXITCODE": {
                                     "description": "Ignore $LASTEXITCODE",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "informationPreference": {
+                                    "description": "InformationPreference",
+                                    "enum": [
+                                        "default",
+                                        "stop",
+                                        "continue",
+                                        "silentlyContinue"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "pwsh": {
                                     "description": "Use PowerShell Core",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "runScriptInSeparateScope": {
                                     "description": "Run script in the separate scope",
@@ -3646,14 +3787,34 @@
                                     "description": "Type",
                                     "enum": [
                                         "filePath",
                                         "inline"
                                     ],
                                     "ignoreCase": "all"
                                 },
+                                "verbosePreference": {
+                                    "description": "VerbosePreference",
+                                    "enum": [
+                                        "default",
+                                        "stop",
+                                        "continue",
+                                        "silentlyContinue"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "warningPreference": {
+                                    "description": "WarningPreference",
+                                    "enum": [
+                                        "default",
+                                        "stop",
+                                        "continue",
+                                        "silentlyContinue"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "workingDirectory": {
                                     "description": "Working Directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": []
@@ -4418,22 +4579,14 @@
                                     "enum": [
                                         "None",
                                         "Cobertura",
                                         "JaCoCo"
                                     ],
                                     "ignoreCase": "all"
                                 },
-                                "effectivePomSkip": {
-                                    "aliases": [
-                                        "skipEffectivePom"
-                                    ],
-                                    "description": "Skip generating effective POM while authenticating built-in feeds",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
                                 "findBugsRunAnalysis": {
                                     "aliases": [
                                         "findbugsAnalysisEnabled"
                                     ],
                                     "description": "Run FindBugs",
                                     "ignoreCase": "key",
                                     "type": "boolean"
@@ -4588,15 +4741,15 @@
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Maven\n\nBuild, test, and deploy with Apache Maven",
                             "ignoreCase": "value",
-                            "pattern": "^Maven@3$"
+                            "pattern": "^Maven@2$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -4969,14 +5122,22 @@
                                     "enum": [
                                         "None",
                                         "Cobertura",
                                         "JaCoCo"
                                     ],
                                     "ignoreCase": "all"
                                 },
+                                "effectivePomSkip": {
+                                    "aliases": [
+                                        "skipEffectivePom"
+                                    ],
+                                    "description": "Skip generating effective POM while authenticating built-in feeds",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "findBugsRunAnalysis": {
                                     "aliases": [
                                         "findbugsAnalysisEnabled"
                                     ],
                                     "description": "Run FindBugs",
                                     "ignoreCase": "key",
                                     "type": "boolean"
@@ -5131,15 +5292,15 @@
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Maven\n\nBuild, test, and deploy with Apache Maven",
                             "ignoreCase": "value",
-                            "pattern": "^Maven@2$"
+                            "pattern": "^Maven@3$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -6770,86 +6931,86 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Install Apple Provisioning Profile inputs",
+                            "description": "Install Apple provisioning profile inputs",
                             "properties": {
                                 "provProfileSecureFile": {
-                                    "description": "Provisioning Profile",
+                                    "description": "Provisioning profile",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "provProfileSourceRepository": {
+                                    "description": "Provisioning profile",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "provisioningProfileLocation": {
+                                    "description": "Provisioning profile location",
+                                    "enum": [
+                                        "secureFiles",
+                                        "sourceRepository"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "removeProfile": {
-                                    "description": "Remove Profile After Build",
+                                    "description": "Remove profile after build",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 }
                             },
-                            "required": [
-                                "provProfileSecureFile"
-                            ]
+                            "required": []
                         },
                         "task": {
-                            "description": "Install Apple Provisioning Profile\n\nInstall an Apple provisioning profile required to build on a macOS agent",
+                            "description": "Install Apple provisioning profile\n\nInstall an Apple provisioning profile required to build on a macOS agent machine",
                             "ignoreCase": "value",
-                            "pattern": "^InstallAppleProvisioningProfile@0$"
+                            "pattern": "^InstallAppleProvisioningProfile@1$"
                         }
                     },
                     "required": [
-                        "task",
-                        "inputs"
+                        "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Install Apple provisioning profile inputs",
+                            "description": "Install Apple Provisioning Profile inputs",
                             "properties": {
                                 "provProfileSecureFile": {
-                                    "description": "Provisioning profile",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "provProfileSourceRepository": {
-                                    "description": "Provisioning profile",
+                                    "description": "Provisioning Profile",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "provisioningProfileLocation": {
-                                    "description": "Provisioning profile location",
-                                    "enum": [
-                                        "secureFiles",
-                                        "sourceRepository"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
                                 "removeProfile": {
-                                    "description": "Remove profile after build",
+                                    "description": "Remove Profile After Build",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 }
                             },
-                            "required": []
+                            "required": [
+                                "provProfileSecureFile"
+                            ]
                         },
                         "task": {
-                            "description": "Install Apple provisioning profile\n\nInstall an Apple provisioning profile required to build on a macOS agent machine",
+                            "description": "Install Apple Provisioning Profile\n\nInstall an Apple provisioning profile required to build on a macOS agent",
                             "ignoreCase": "value",
-                            "pattern": "^InstallAppleProvisioningProfile@1$"
+                            "pattern": "^InstallAppleProvisioningProfile@0$"
                         }
                     },
                     "required": [
-                        "task"
+                        "task",
+                        "inputs"
                     ]
                 },
                 {
                     "deprecationMessage": "SonarQubePostTest is deprecated - [DEPRECATED] Finish the analysis and upload the results to SonarQube",
                     "doNotSuggest": true,
                     "firstProperty": [
                         "task"
@@ -7136,95 +7297,14 @@
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
                             "description": "Docker inputs",
                             "properties": {
-                                "Dockerfile": {
-                                    "description": "Dockerfile",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "addBaseImageData": {
-                                    "description": "Add base image metadata to image(s)",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "addPipelineData": {
-                                    "description": "Add Pipeline metadata to image(s)",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "arguments": {
-                                    "description": "Arguments",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "buildContext": {
-                                    "description": "Build context",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "command": {
-                                    "description": "Command",
-                                    "enum": [
-                                        "buildAndPush",
-                                        "build",
-                                        "push",
-                                        "login",
-                                        "logout",
-                                        "start",
-                                        "stop"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "container": {
-                                    "description": "Container",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "containerRegistry": {
-                                    "description": "Container registry",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "repository": {
-                                    "description": "Container repository",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "tags": {
-                                    "description": "Tags",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                }
-                            },
-                            "required": []
-                        },
-                        "task": {
-                            "description": "Docker\n\nBuild or push Docker images, login or logout, start or stop containers, or run a Docker command",
-                            "ignoreCase": "value",
-                            "pattern": "^Docker@2$"
-                        }
-                    },
-                    "required": [
-                        "task"
-                    ]
-                },
-                {
-                    "doNotSuggest": false,
-                    "firstProperty": [
-                        "task"
-                    ],
-                    "properties": {
-                        "inputs": {
-                            "additionalProperties": false,
-                            "description": "Docker inputs",
-                            "properties": {
                                 "action": {
                                     "description": "Action",
                                     "enum": [
                                         "Build an image",
                                         "Tag images",
                                         "Push an image",
                                         "Push images",
@@ -7424,14 +7504,95 @@
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
                             "description": "Docker inputs",
                             "properties": {
+                                "Dockerfile": {
+                                    "description": "Dockerfile",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "addBaseImageData": {
+                                    "description": "Add base image metadata to image(s)",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "addPipelineData": {
+                                    "description": "Add Pipeline metadata to image(s)",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "arguments": {
+                                    "description": "Arguments",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "buildContext": {
+                                    "description": "Build context",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "command": {
+                                    "description": "Command",
+                                    "enum": [
+                                        "buildAndPush",
+                                        "build",
+                                        "push",
+                                        "login",
+                                        "logout",
+                                        "start",
+                                        "stop"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "container": {
+                                    "description": "Container",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "containerRegistry": {
+                                    "description": "Container registry",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "repository": {
+                                    "description": "Container repository",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "tags": {
+                                    "description": "Tags",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                }
+                            },
+                            "required": []
+                        },
+                        "task": {
+                            "description": "Docker\n\nBuild or push Docker images, login or logout, start or stop containers, or run a Docker command",
+                            "ignoreCase": "value",
+                            "pattern": "^Docker@2$"
+                        }
+                    },
+                    "required": [
+                        "task"
+                    ]
+                },
+                {
+                    "doNotSuggest": false,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
+                            "description": "Docker inputs",
+                            "properties": {
                                 "addBaseImageData": {
                                     "description": "Add base image metadata to image(s)",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "addDefaultLabels": {
                                     "description": "Add default labels",
@@ -7704,14 +7865,24 @@
                                     "type": "boolean"
                                 },
                                 "capturePipeline": {
                                     "description": "Capture pipeline output and wait for pipeline completion",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "delayBetweenRetries": {
+                                    "description": "Time between retries",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "failOnUnstableResult": {
+                                    "description": "Fail on unstable result",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "isMultibranchJob": {
                                     "description": "Job is of multibranch pipeline type",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "isParameterizedJob": {
                                     "aliases": [
@@ -7732,14 +7903,19 @@
                                     "type": "string"
                                 },
                                 "multibranchPipelineBranch": {
                                     "description": "Multibranch pipeline branch",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "retryCount": {
+                                    "description": "Number of retries for failed connection",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "serverEndpoint": {
                                     "description": "Jenkins service connection",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": [
@@ -8878,14 +9054,19 @@
                                     "type": "string"
                                 },
                                 "cleanDestinationDirectory": {
                                     "description": "Clean destination directory",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "createExtractDirectory": {
+                                    "description": "Create directory for extracting",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "jdkArchitectureOption": {
                                     "description": "JDK architecture",
                                     "enum": [
                                         "x64",
                                         "x86"
                                     ],
                                     "ignoreCase": "all"
@@ -9200,14 +9381,15 @@
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "msbuildVersion": {
                                     "description": "MSBuild Version",
                                     "enum": [
                                         "latest",
+                                        "17.0",
                                         "16.0",
                                         "15.0",
                                         "14.0",
                                         "12.0",
                                         "4.0"
                                     ],
                                     "ignoreCase": "all"
@@ -10782,387 +10964,374 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Xcode inputs",
+                            "description": "Xcode Build inputs",
                             "properties": {
                                 "actions": {
                                     "description": "Actions",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "archivePath": {
-                                    "description": "Archive path",
+                                    "description": "Archive Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "args": {
                                     "description": "Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "configuration": {
                                     "description": "Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "destinationDevices": {
-                                    "description": "Device",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "destinationPlatform": {
-                                    "description": "Custom destination platform",
+                                "cwd": {
+                                    "description": "Working Directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "destinationPlatformOption": {
-                                    "description": "Destination platform",
-                                    "enum": [
-                                        "default",
-                                        "iOS",
-                                        "tvOS",
-                                        "macOS",
-                                        "custom"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "destinationSimulators": {
-                                    "description": "Simulator",
+                                "defaultKeychainPassword": {
+                                    "description": "Default Keychain Password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "destinationTypeOption": {
-                                    "description": "Destination type",
-                                    "enum": [
-                                        "simulators",
-                                        "devices"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
                                 "exportArgs": {
-                                    "description": "Export arguments",
+                                    "description": "Export Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportMethod": {
-                                    "description": "Export method",
+                                    "description": "Export Method",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportOptions": {
-                                    "description": "Export options",
+                                    "description": "Export Options",
                                     "enum": [
                                         "auto",
                                         "plist",
                                         "specify"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "exportOptionsPlist": {
-                                    "description": "Export options plist",
+                                    "description": "Export Options Plist",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportPath": {
-                                    "description": "Export path",
+                                    "description": "Export Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportTeamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "iosSigningIdentity": {
+                                    "description": "Signing Identity",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "outputPattern": {
+                                    "description": "Output Directory",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "p12": {
+                                    "description": "P12 Certificate File",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "p12pwd": {
+                                    "description": "P12 Password",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "packageApp": {
-                                    "description": "Create app package",
+                                    "description": "Create App Package",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "provisioningProfileName": {
-                                    "description": "Provisioning profile name",
+                                "provProfile": {
+                                    "description": "Provisioning Profile File",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "provisioningProfileUuid": {
-                                    "description": "Provisioning profile UUID",
+                                "provProfileUuid": {
+                                    "description": "Provisioning Profile UUID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "publishJUnitResults": {
-                                    "description": "Publish test results to Azure Pipelines",
+                                    "description": "Publish to VSTS/TFS",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "removeProfile": {
+                                    "description": "Remove Profile After Build",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "scheme": {
                                     "description": "Scheme",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "sdk": {
                                     "description": "SDK",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "signingIdentity": {
-                                    "description": "Signing identity",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "signingOption": {
-                                    "description": "Signing style",
+                                "signMethod": {
+                                    "description": "Override Using",
                                     "enum": [
-                                        "nosign",
-                                        "default",
-                                        "manual",
-                                        "auto"
+                                        "file",
+                                        "id"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "teamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "testRunTitle": {
-                                    "description": "Test run title",
+                                "unlockDefaultKeychain": {
+                                    "description": "Unlock Default Keychain",
                                     "ignoreCase": "key",
-                                    "type": "string"
+                                    "type": "boolean"
                                 },
                                 "useXcpretty": {
                                     "description": "Use xcpretty",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "workingDirectory": {
-                                    "aliases": [
-                                        "cwd"
-                                    ],
-                                    "description": "Working directory",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
                                 "xcWorkspacePath": {
-                                    "description": "Workspace or project path",
+                                    "description": "Workspace/Project Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "xcodeDeveloperDir": {
-                                    "description": "Xcode developer path",
+                                "xcode8AutomaticSigning": {
+                                    "description": "Automatic Signing",
                                     "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "xcodeVersion": {
-                                    "description": "Xcode version",
-                                    "enum": [
-                                        "8",
-                                        "9",
-                                        "10",
-                                        "11",
-                                        "12",
-                                        "default",
-                                        "specifyPath"
-                                    ],
-                                    "ignoreCase": "all"
+                                    "type": "boolean"
                                 },
-                                "xcprettyArgs": {
-                                    "description": "Xcpretty arguments",
+                                "xcodeDeveloperDir": {
+                                    "description": "Xcode Developer Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Xcode\n\nBuild, test, or archive an Xcode workspace on macOS. Optionally package an app.",
+                            "description": "Xcode Build\n\nBuild an Xcode workspace on macOS",
                             "ignoreCase": "value",
-                            "pattern": "^Xcode@5$"
+                            "pattern": "^Xcode@3$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Xcode Build inputs",
+                            "description": "Xcode inputs",
                             "properties": {
                                 "actions": {
                                     "description": "Actions",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "archivePath": {
-                                    "description": "Archive Path",
+                                    "description": "Archive path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "args": {
                                     "description": "Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "configuration": {
                                     "description": "Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "cwd": {
-                                    "description": "Working Directory",
+                                "destinationDevices": {
+                                    "description": "Device",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "defaultKeychainPassword": {
-                                    "description": "Default Keychain Password",
+                                "destinationPlatform": {
+                                    "description": "Custom destination platform",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "destinationPlatformOption": {
+                                    "description": "Destination platform",
+                                    "enum": [
+                                        "default",
+                                        "iOS",
+                                        "tvOS",
+                                        "macOS",
+                                        "custom"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "destinationSimulators": {
+                                    "description": "Simulator",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "destinationTypeOption": {
+                                    "description": "Destination type",
+                                    "enum": [
+                                        "simulators",
+                                        "devices"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "exportArgs": {
-                                    "description": "Export Arguments",
+                                    "description": "Export arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportMethod": {
-                                    "description": "Export Method",
+                                    "description": "Export method",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportOptions": {
-                                    "description": "Export Options",
+                                    "description": "Export options",
                                     "enum": [
                                         "auto",
                                         "plist",
                                         "specify"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "exportOptionsPlist": {
-                                    "description": "Export Options Plist",
+                                    "description": "Export options plist",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportPath": {
-                                    "description": "Export Path",
+                                    "description": "Export path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "exportTeamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "iosSigningIdentity": {
-                                    "description": "Signing Identity",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
                                 "outputPattern": {
-                                    "description": "Output Directory",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "p12": {
-                                    "description": "P12 Certificate File",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "p12pwd": {
-                                    "description": "P12 Password",
+                                    "description": "Output directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "packageApp": {
-                                    "description": "Create App Package",
+                                    "description": "Create app package",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "provProfile": {
-                                    "description": "Provisioning Profile File",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "provProfileUuid": {
-                                    "description": "Provisioning Profile UUID",
+                                "provisioningProfileUuid": {
+                                    "description": "Provisioning profile UUID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "publishJUnitResults": {
-                                    "description": "Publish to VSTS/TFS",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "removeProfile": {
-                                    "description": "Remove Profile After Build",
+                                    "description": "Publish test results to VSTS/TFS",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "scheme": {
                                     "description": "Scheme",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "sdk": {
                                     "description": "SDK",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "signMethod": {
-                                    "description": "Override Using",
+                                "signingIdentity": {
+                                    "description": "Signing identity",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "signingOption": {
+                                    "description": "Signing style",
                                     "enum": [
-                                        "file",
-                                        "id"
+                                        "nosign",
+                                        "default",
+                                        "manual",
+                                        "auto"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "teamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "unlockDefaultKeychain": {
-                                    "description": "Unlock Default Keychain",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
                                 "useXcpretty": {
                                     "description": "Use xcpretty",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "xcWorkspacePath": {
-                                    "description": "Workspace/Project Path",
+                                "workingDirectory": {
+                                    "aliases": [
+                                        "cwd"
+                                    ],
+                                    "description": "Working directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "xcode8AutomaticSigning": {
-                                    "description": "Automatic Signing",
+                                "xcWorkspacePath": {
+                                    "description": "Workspace or project path",
                                     "ignoreCase": "key",
-                                    "type": "boolean"
+                                    "type": "string"
                                 },
                                 "xcodeDeveloperDir": {
-                                    "description": "Xcode Developer Path",
+                                    "description": "Xcode developer path",
                                     "ignoreCase": "key",
                                     "type": "string"
+                                },
+                                "xcodeVersion": {
+                                    "description": "Xcode version",
+                                    "enum": [
+                                        "8",
+                                        "9",
+                                        "default",
+                                        "specifyPath"
+                                    ],
+                                    "ignoreCase": "all"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Xcode Build\n\nBuild an Xcode workspace on macOS",
+                            "description": "Xcode\n\nBuild, test, or archive an Xcode workspace on macOS. Optionally package an app.",
                             "ignoreCase": "value",
-                            "pattern": "^Xcode@3$"
+                            "pattern": "^Xcode@4$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -11259,31 +11428,31 @@
                                     "type": "string"
                                 },
                                 "exportTeamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "outputPattern": {
-                                    "description": "Output directory",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
                                 "packageApp": {
                                     "description": "Create app package",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "provisioningProfileName": {
+                                    "description": "Provisioning profile name",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "provisioningProfileUuid": {
                                     "description": "Provisioning profile UUID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "publishJUnitResults": {
-                                    "description": "Publish test results to VSTS/TFS",
+                                    "description": "Publish test results to Azure Pipelines",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "scheme": {
                                     "description": "Scheme",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -11309,14 +11478,19 @@
                                     "ignoreCase": "all"
                                 },
                                 "teamId": {
                                     "description": "Team ID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "testRunTitle": {
+                                    "description": "Test run title",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "useXcpretty": {
                                     "description": "Use xcpretty",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "workingDirectory": {
                                     "aliases": [
@@ -11337,26 +11511,34 @@
                                     "type": "string"
                                 },
                                 "xcodeVersion": {
                                     "description": "Xcode version",
                                     "enum": [
                                         "8",
                                         "9",
+                                        "10",
+                                        "11",
+                                        "12",
                                         "default",
                                         "specifyPath"
                                     ],
                                     "ignoreCase": "all"
+                                },
+                                "xcprettyArgs": {
+                                    "description": "Xcpretty arguments",
+                                    "ignoreCase": "key",
+                                    "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Xcode\n\nBuild, test, or archive an Xcode workspace on macOS. Optionally package an app.",
                             "ignoreCase": "value",
-                            "pattern": "^Xcode@4$"
+                            "pattern": "^Xcode@5$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -13965,27 +14147,37 @@
                                     "aliases": [
                                         "forSimulator"
                                     ],
                                     "description": "Build for iOS Simulator",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "buildToolOption": {
+                                    "aliases": [
+                                        "buildTool"
+                                    ],
+                                    "description": "Build tool",
+                                    "enum": [
+                                        "xbuild",
+                                        "msbuild"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
                                 "clean": {
                                     "description": "Clean",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "configuration": {
                                     "description": "Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "mdtoolFile": {
                                     "aliases": [
-                                        "buildToolLocation",
                                         "mdtoolLocation"
                                     ],
                                     "description": "Build tool path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "packageApp": {
@@ -13994,30 +14186,89 @@
                                     "type": "boolean"
                                 },
                                 "runNugetRestore": {
                                     "description": "Run NuGet restore",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "signingDefaultKeychainPassword": {
+                                    "aliases": [
+                                        "defaultKeychainPassword"
+                                    ],
+                                    "description": "Default keychain password",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "signingIdentity": {
                                     "aliases": [
                                         "iosSigningIdentity"
                                     ],
                                     "description": "Signing identity",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "signingOption": {
+                                    "aliases": [
+                                        "signMethod"
+                                    ],
+                                    "description": "Override using",
+                                    "enum": [
+                                        "file",
+                                        "id"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "signingP12File": {
+                                    "aliases": [
+                                        "p12"
+                                    ],
+                                    "description": "P12 certificate file",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "signingP12Password": {
+                                    "aliases": [
+                                        "p12pwd"
+                                    ],
+                                    "description": "P12 password",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "signingProvisioningProfileFile": {
+                                    "aliases": [
+                                        "provProfile"
+                                    ],
+                                    "description": "Provisioning profile file",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "signingProvisioningProfileID": {
                                     "aliases": [
                                         "provProfileUuid"
                                     ],
                                     "description": "Provisioning profile UUID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "signingRemoveProfile": {
+                                    "aliases": [
+                                        "removeProfile"
+                                    ],
+                                    "description": "Remove profile after build",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "signingUnlockDefaultKeychain": {
+                                    "aliases": [
+                                        "unlockDefaultKeychain"
+                                    ],
+                                    "description": "Unlock default keychain",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "solutionFile": {
                                     "aliases": [
                                         "solution"
                                     ],
                                     "description": "Solution",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -14032,15 +14283,15 @@
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Xamarin.iOS\n\nBuild an iOS app with Xamarin on macOS",
                             "ignoreCase": "value",
-                            "pattern": "^XamariniOS@2$"
+                            "pattern": "^XamariniOS@1$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -14062,37 +14313,27 @@
                                     "aliases": [
                                         "forSimulator"
                                     ],
                                     "description": "Build for iOS Simulator",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "buildToolOption": {
-                                    "aliases": [
-                                        "buildTool"
-                                    ],
-                                    "description": "Build tool",
-                                    "enum": [
-                                        "xbuild",
-                                        "msbuild"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
                                 "clean": {
                                     "description": "Clean",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "configuration": {
                                     "description": "Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "mdtoolFile": {
                                     "aliases": [
+                                        "buildToolLocation",
                                         "mdtoolLocation"
                                     ],
                                     "description": "Build tool path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "packageApp": {
@@ -14101,89 +14342,30 @@
                                     "type": "boolean"
                                 },
                                 "runNugetRestore": {
                                     "description": "Run NuGet restore",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "signingDefaultKeychainPassword": {
-                                    "aliases": [
-                                        "defaultKeychainPassword"
-                                    ],
-                                    "description": "Default keychain password",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
                                 "signingIdentity": {
                                     "aliases": [
                                         "iosSigningIdentity"
                                     ],
                                     "description": "Signing identity",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "signingOption": {
-                                    "aliases": [
-                                        "signMethod"
-                                    ],
-                                    "description": "Override using",
-                                    "enum": [
-                                        "file",
-                                        "id"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "signingP12File": {
-                                    "aliases": [
-                                        "p12"
-                                    ],
-                                    "description": "P12 certificate file",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "signingP12Password": {
-                                    "aliases": [
-                                        "p12pwd"
-                                    ],
-                                    "description": "P12 password",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "signingProvisioningProfileFile": {
-                                    "aliases": [
-                                        "provProfile"
-                                    ],
-                                    "description": "Provisioning profile file",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
                                 "signingProvisioningProfileID": {
                                     "aliases": [
                                         "provProfileUuid"
                                     ],
                                     "description": "Provisioning profile UUID",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "signingRemoveProfile": {
-                                    "aliases": [
-                                        "removeProfile"
-                                    ],
-                                    "description": "Remove profile after build",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "signingUnlockDefaultKeychain": {
-                                    "aliases": [
-                                        "unlockDefaultKeychain"
-                                    ],
-                                    "description": "Unlock default keychain",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
                                 "solutionFile": {
                                     "aliases": [
                                         "solution"
                                     ],
                                     "description": "Solution",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -14198,161 +14380,161 @@
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Xamarin.iOS\n\nBuild an iOS app with Xamarin on macOS",
                             "ignoreCase": "value",
-                            "pattern": "^XamariniOS@1$"
+                            "pattern": "^XamariniOS@2$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Publish Test Results inputs",
+                            "description": "Publish test results inputs",
                             "properties": {
-                                "buildConfiguration": {
-                                    "aliases": [
-                                        "configuration"
-                                    ],
-                                    "description": "Build Configuration",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "buildPlatform": {
-                                    "aliases": [
-                                        "platform"
-                                    ],
-                                    "description": "Build Platform",
+                                "configuration": {
+                                    "description": "Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "failTaskOnFailedTests": {
-                                    "description": "Fail if there are test failures",
+                                "mergeTestResults": {
+                                    "description": "Merge Test Results",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "mergeTestResults": {
-                                    "description": "Merge test results",
+                                "platform": {
+                                    "description": "Platform",
                                     "ignoreCase": "key",
-                                    "type": "boolean"
+                                    "type": "string"
                                 },
                                 "publishRunAttachments": {
-                                    "description": "Upload test results files",
+                                    "description": "Upload Test Attachments",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "searchFolder": {
-                                    "description": "Search folder",
+                                "testResultsFiles": {
+                                    "description": "Test Results Files",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "testResultsFiles": {
-                                    "description": "Test results files",
+                                "testRunTitle": {
+                                    "description": "Test Run Title",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "testResultsFormat": {
-                                    "aliases": [
-                                        "testRunner"
-                                    ],
-                                    "description": "Test result format",
+                                "testRunner": {
+                                    "description": "Test Result Format",
                                     "enum": [
                                         "JUnit",
                                         "NUnit",
                                         "VSTest",
-                                        "XUnit",
-                                        "CTest"
+                                        "XUnit"
                                     ],
                                     "ignoreCase": "all"
-                                },
-                                "testRunTitle": {
-                                    "description": "Test run title",
-                                    "ignoreCase": "key",
-                                    "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Publish Test Results\n\nPublish test results to Azure Pipelines",
+                            "description": "Publish test results\n\nPublish test results to Azure Pipelines",
                             "ignoreCase": "value",
-                            "pattern": "^PublishTestResults@2$"
+                            "pattern": "^PublishTestResults@1$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Publish test results inputs",
+                            "description": "Publish Test Results inputs",
                             "properties": {
-                                "configuration": {
-                                    "description": "Configuration",
+                                "buildConfiguration": {
+                                    "aliases": [
+                                        "configuration"
+                                    ],
+                                    "description": "Build Configuration",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "mergeTestResults": {
-                                    "description": "Merge Test Results",
+                                "buildPlatform": {
+                                    "aliases": [
+                                        "platform"
+                                    ],
+                                    "description": "Build Platform",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "failTaskOnFailedTests": {
+                                    "description": "Fail if there are test failures",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "platform": {
-                                    "description": "Platform",
+                                "mergeTestResults": {
+                                    "description": "Merge test results",
                                     "ignoreCase": "key",
-                                    "type": "string"
+                                    "type": "boolean"
                                 },
                                 "publishRunAttachments": {
-                                    "description": "Upload Test Attachments",
+                                    "description": "Upload test results files",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "testResultsFiles": {
-                                    "description": "Test Results Files",
+                                "searchFolder": {
+                                    "description": "Search folder",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "testRunTitle": {
-                                    "description": "Test Run Title",
+                                "testResultsFiles": {
+                                    "description": "Test results files",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "testRunner": {
-                                    "description": "Test Result Format",
+                                "testResultsFormat": {
+                                    "aliases": [
+                                        "testRunner"
+                                    ],
+                                    "description": "Test result format",
                                     "enum": [
                                         "JUnit",
                                         "NUnit",
                                         "VSTest",
-                                        "XUnit"
+                                        "XUnit",
+                                        "CTest"
                                     ],
                                     "ignoreCase": "all"
+                                },
+                                "testRunTitle": {
+                                    "description": "Test run title",
+                                    "ignoreCase": "key",
+                                    "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Publish test results\n\nPublish test results to Azure Pipelines",
+                            "description": "Publish Test Results\n\nPublish test results to Azure Pipelines",
                             "ignoreCase": "value",
-                            "pattern": "^PublishTestResults@1$"
+                            "pattern": "^PublishTestResults@2$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -14996,49 +15178,25 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Index sources and publish symbols inputs",
+                            "description": "Index Sources & Publish Symbols inputs",
                             "properties": {
-                                "CompressSymbols": {
-                                    "description": "Compress symbols",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "DetailedLog": {
-                                    "description": "Verbose logging",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "IndexSources": {
-                                    "description": "Index sources",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "PublishSymbols": {
-                                    "description": "Publish symbols",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
                                 "SearchPattern": {
                                     "description": "Search pattern",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "SymbolServerType": {
-                                    "description": "Symbol server type",
-                                    "enum": [
-                                        " ",
-                                        "TeamServices",
-                                        "FileShare"
-                                    ],
-                                    "ignoreCase": "all"
+                                "SkipIndexing": {
+                                    "description": "Skip indexing",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
                                 },
                                 "SymbolsArtifactName": {
                                     "description": "Artifact name",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "SymbolsFolder": {
@@ -15071,42 +15229,76 @@
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Index sources and publish symbols\n\nIndex your source code and publish symbols to a file share or Azure Artifacts symbol server",
+                            "description": "Index Sources & Publish Symbols\n\nIndex your source code and publish symbols to a file share",
                             "ignoreCase": "value",
-                            "pattern": "^PublishSymbols@2$"
+                            "pattern": "^PublishSymbols@1$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Index Sources & Publish Symbols inputs",
+                            "description": "Index sources and publish symbols inputs",
                             "properties": {
+                                "CompressSymbols": {
+                                    "description": "Compress symbols",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "DetailedLog": {
+                                    "description": "Verbose logging",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "IndexSources": {
+                                    "description": "Index sources",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "IndexableFileFormats": {
+                                    "description": "Symbol file formats to publish",
+                                    "enum": [
+                                        "Default",
+                                        "Pdb",
+                                        "SourceMap",
+                                        "All"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "PublishSymbols": {
+                                    "description": "Publish symbols",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "SearchPattern": {
                                     "description": "Search pattern",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "SkipIndexing": {
-                                    "description": "Skip indexing",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
+                                "SymbolServerType": {
+                                    "description": "Symbol server type",
+                                    "enum": [
+                                        " ",
+                                        "TeamServices",
+                                        "FileShare"
+                                    ],
+                                    "ignoreCase": "all"
                                 },
                                 "SymbolsArtifactName": {
                                     "description": "Artifact name",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "SymbolsFolder": {
@@ -15139,17 +15331,17 @@
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Index Sources & Publish Symbols\n\nIndex your source code and publish symbols to a file share",
+                            "description": "Index sources and publish symbols\n\nIndex your source code and publish symbols to a file share or Azure Artifacts symbol server",
                             "ignoreCase": "value",
-                            "pattern": "^PublishSymbols@1$"
+                            "pattern": "^PublishSymbols@2$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -15738,131 +15930,238 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "App Center distribute inputs",
+                            "description": "Gradle inputs",
                             "properties": {
-                                "appFile": {
+                                "checkStyleRunAnalysis": {
                                     "aliases": [
-                                        "app"
+                                        "checkstyleAnalysisEnabled"
                                     ],
-                                    "description": "Binary file path",
+                                    "description": "Run Checkstyle",
                                     "ignoreCase": "key",
-                                    "type": "string"
+                                    "type": "boolean"
                                 },
-                                "appSlug": {
-                                    "description": "App slug",
+                                "codeCoverageClassFilesDirectories": {
+                                    "aliases": [
+                                        "classFilesDirectories"
+                                    ],
+                                    "description": "Class files directories",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "distributionGroupId": {
+                                "codeCoverageClassFilter": {
                                     "aliases": [
-                                        "destinationId"
+                                        "classFilter"
                                     ],
-                                    "description": "Destination ID",
+                                    "description": "Class inclusion/exclusion filters",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "isMandatory": {
-                                    "description": "Require users to update to this release",
+                                "codeCoverageFailIfEmpty": {
+                                    "aliases": [
+                                        "failIfCoverageEmpty"
+                                    ],
+                                    "description": "Fail when code coverage results are missing",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "releaseNotesFile": {
-                                    "description": "Release notes file",
+                                "codeCoverageGradle5xOrHigher": {
+                                    "aliases": [
+                                        "gradle5xOrHigher"
+                                    ],
+                                    "description": "Gradle version >= 5.x",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "codeCoverageToolOption": {
+                                    "aliases": [
+                                        "codeCoverageTool"
+                                    ],
+                                    "description": "Code coverage tool",
+                                    "enum": [
+                                        "None",
+                                        "Cobertura",
+                                        "JaCoCo"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "findBugsRunAnalysis": {
+                                    "aliases": [
+                                        "findbugsAnalysisEnabled"
+                                    ],
+                                    "description": "Run FindBugs",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "gradleOptions": {
+                                    "aliases": [
+                                        "gradleOpts"
+                                    ],
+                                    "description": "Set GRADLE_OPTS",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "releaseNotesInput": {
-                                    "description": "Release notes",
+                                "gradleWrapperFile": {
+                                    "aliases": [
+                                        "wrapperScript"
+                                    ],
+                                    "description": "Gradle wrapper",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "releaseNotesOption": {
+                                "javaHomeOption": {
                                     "aliases": [
-                                        "releaseNotesSelection"
+                                        "javaHomeSelection"
                                     ],
-                                    "description": "Create release notes",
+                                    "description": "Set JAVA_HOME by",
                                     "enum": [
-                                        "input",
-                                        "file"
+                                        "JDKVersion",
+                                        "Path"
                                     ],
                                     "ignoreCase": "all"
                                 },
-                                "serverEndpoint": {
-                                    "description": "App Center service connection",
+                                "jdkArchitectureOption": {
+                                    "aliases": [
+                                        "jdkArchitecture"
+                                    ],
+                                    "description": "JDK architecture",
+                                    "enum": [
+                                        "x86",
+                                        "x64"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "jdkDirectory": {
+                                    "aliases": [
+                                        "jdkUserInputPath"
+                                    ],
+                                    "description": "JDK path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "symbolsDsymFiles": {
+                                "jdkVersionOption": {
                                     "aliases": [
-                                        "dsymPath"
+                                        "jdkVersion"
                                     ],
-                                    "description": "dSYM path",
+                                    "description": "JDK version",
+                                    "enum": [
+                                        "default",
+                                        "1.11",
+                                        "1.10",
+                                        "1.9",
+                                        "1.8",
+                                        "1.7",
+                                        "1.6"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "options": {
+                                    "description": "Options",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "symbolsIncludeParentDirectory": {
+                                "pmdRunAnalysis": {
                                     "aliases": [
-                                        "packParentFolder"
+                                        "pmdAnalysisEnabled"
                                     ],
-                                    "description": "Include all items in parent folder",
+                                    "description": "Run PMD",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "symbolsMappingTxtFile": {
+                                "publishJUnitResults": {
+                                    "description": "Publish to Azure Pipelines",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "sonarQubeGradlePluginVersion": {
                                     "aliases": [
-                                        "mappingTxtPath"
+                                        "sqGradlePluginVersion"
                                     ],
-                                    "description": "Mapping file",
+                                    "description": "SonarQube scanner for Gradle plugin version",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "symbolsOption": {
+                                "sonarQubeRunAnalysis": {
                                     "aliases": [
-                                        "symbolsType"
+                                        "sqAnalysisEnabled"
                                     ],
-                                    "description": "Symbols type",
+                                    "description": "Run SonarQube or SonarCloud Analysis",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "spotBugsAnalysis": {
+                                    "aliases": [
+                                        "spotBugsAnalysisEnabled"
+                                    ],
+                                    "description": "Run SpotBugs",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "spotBugsGradlePluginVersionChoice": {
+                                    "description": "Spotbugs plugin version",
                                     "enum": [
-                                        "Apple"
+                                        "specify",
+                                        "build"
                                     ],
                                     "ignoreCase": "all"
                                 },
-                                "symbolsPath": {
-                                    "description": "Symbols path",
+                                "spotbugsGradlePluginVersion": {
+                                    "aliases": [
+                                        "spotbugsGradlePluginVersion"
+                                    ],
+                                    "description": "Version number",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "symbolsPdbFiles": {
+                                "sqGradlePluginVersionChoice": {
+                                    "description": "SonarQube scanner for Gradle version",
+                                    "enum": [
+                                        "specify",
+                                        "build"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "tasks": {
+                                    "description": "Tasks",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "testResultsFiles": {
+                                    "description": "Test results files",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "testRunTitle": {
+                                    "description": "Test run title",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "workingDirectory": {
                                     "aliases": [
-                                        "pdbPath"
+                                        "cwd"
                                     ],
-                                    "description": "Symbols path (*.pdb)",
+                                    "description": "Working directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
-                            "required": [
-                                "serverEndpoint",
-                                "appSlug",
-                                "appFile"
-                            ]
+                            "required": []
                         },
                         "task": {
-                            "description": "App Center distribute\n\nDistribute app builds to testers and users via Visual Studio App Center",
+                            "description": "Gradle\n\nBuild using a Gradle wrapper script",
                             "ignoreCase": "value",
-                            "pattern": "^AppCenterDistribute@1$"
+                            "pattern": "^Gradle@3$"
                         }
                     },
                     "required": [
-                        "task",
-                        "inputs"
+                        "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
@@ -16147,14 +16446,141 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
+                            "description": "App Center distribute inputs",
+                            "properties": {
+                                "appFile": {
+                                    "aliases": [
+                                        "app"
+                                    ],
+                                    "description": "Binary file path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "appSlug": {
+                                    "description": "App slug",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "distributionGroupId": {
+                                    "aliases": [
+                                        "destinationId"
+                                    ],
+                                    "description": "Destination ID",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "isMandatory": {
+                                    "description": "Require users to update to this release",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "releaseNotesFile": {
+                                    "description": "Release notes file",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "releaseNotesInput": {
+                                    "description": "Release notes",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "releaseNotesOption": {
+                                    "aliases": [
+                                        "releaseNotesSelection"
+                                    ],
+                                    "description": "Create release notes",
+                                    "enum": [
+                                        "input",
+                                        "file"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "serverEndpoint": {
+                                    "description": "App Center service connection",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "symbolsDsymFiles": {
+                                    "aliases": [
+                                        "dsymPath"
+                                    ],
+                                    "description": "dSYM path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "symbolsIncludeParentDirectory": {
+                                    "aliases": [
+                                        "packParentFolder"
+                                    ],
+                                    "description": "Include all items in parent folder",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "symbolsMappingTxtFile": {
+                                    "aliases": [
+                                        "mappingTxtPath"
+                                    ],
+                                    "description": "Mapping file",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "symbolsOption": {
+                                    "aliases": [
+                                        "symbolsType"
+                                    ],
+                                    "description": "Symbols type",
+                                    "enum": [
+                                        "Apple"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "symbolsPath": {
+                                    "description": "Symbols path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "symbolsPdbFiles": {
+                                    "aliases": [
+                                        "pdbPath"
+                                    ],
+                                    "description": "Symbols path (*.pdb)",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                }
+                            },
+                            "required": [
+                                "serverEndpoint",
+                                "appSlug",
+                                "appFile"
+                            ]
+                        },
+                        "task": {
+                            "description": "App Center distribute\n\nDistribute app builds to testers and users via Visual Studio App Center",
+                            "ignoreCase": "value",
+                            "pattern": "^AppCenterDistribute@1$"
+                        }
+                    },
+                    "required": [
+                        "task",
+                        "inputs"
+                    ]
+                },
+                {
+                    "doNotSuggest": false,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
                             "description": "App Center Distribute inputs",
                             "properties": {
                                 "appFile": {
                                     "aliases": [
                                         "app"
                                     ],
                                     "description": "Binary file path",
@@ -16909,69 +17335,69 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Install Apple Certificate inputs",
+                            "description": "Install Apple certificate inputs",
                             "properties": {
                                 "certPwd": {
-                                    "description": "Certificate (P12) Password",
+                                    "description": "Certificate (P12) password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "certSecureFile": {
                                     "description": "Certificate (P12)",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "customKeychainPath": {
-                                    "description": "Custom Keychain Path",
+                                    "description": "Custom keychain path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "deleteCert": {
-                                    "description": "Delete Certificate from Keychain",
+                                    "description": "Delete certificate from keychain",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "deleteCustomKeychain": {
-                                    "description": "Delete Custom Keychain",
+                                    "description": "Delete custom keychain",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "keychain": {
                                     "description": "Keychain",
                                     "enum": [
                                         "default",
                                         "temp",
                                         "custom"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "keychainPassword": {
-                                    "description": "Keychain Password",
+                                    "description": "Keychain password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "signingIdentity": {
-                                    "description": "Certificate Signing Identity",
+                                    "description": "Certificate signing identity",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": [
                                 "certSecureFile"
                             ]
                         },
                         "task": {
-                            "description": "Install Apple Certificate\n\nInstall an Apple certificate required to build on a macOS agent",
+                            "description": "Install Apple certificate\n\nInstall an Apple certificate required to build on a macOS agent machine",
                             "ignoreCase": "value",
-                            "pattern": "^InstallAppleCertificate@0$"
+                            "pattern": "^InstallAppleCertificate@2$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -16979,69 +17405,69 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Install Apple certificate inputs",
+                            "description": "Install Apple Certificate inputs",
                             "properties": {
                                 "certPwd": {
-                                    "description": "Certificate (P12) password",
+                                    "description": "Certificate (P12) Password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "certSecureFile": {
                                     "description": "Certificate (P12)",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "customKeychainPath": {
-                                    "description": "Custom keychain path",
+                                    "description": "Custom Keychain Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "deleteCert": {
-                                    "description": "Delete certificate from keychain",
+                                    "description": "Delete Certificate from Keychain",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "deleteCustomKeychain": {
-                                    "description": "Delete custom keychain",
+                                    "description": "Delete Custom Keychain",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "keychain": {
                                     "description": "Keychain",
                                     "enum": [
                                         "default",
                                         "temp",
                                         "custom"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "keychainPassword": {
-                                    "description": "Keychain password",
+                                    "description": "Keychain Password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "signingIdentity": {
-                                    "description": "Certificate signing identity",
+                                    "description": "Certificate Signing Identity",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": [
                                 "certSecureFile"
                             ]
                         },
                         "task": {
-                            "description": "Install Apple certificate\n\nInstall an Apple certificate required to build on a macOS agent machine",
+                            "description": "Install Apple Certificate\n\nInstall an Apple certificate required to build on a macOS agent",
                             "ignoreCase": "value",
-                            "pattern": "^InstallAppleCertificate@2$"
+                            "pattern": "^InstallAppleCertificate@0$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -18265,179 +18691,161 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Android signing inputs",
+                            "description": "Android Signing inputs",
                             "properties": {
-                                "apkFiles": {
-                                    "aliases": [
-                                        "files"
-                                    ],
-                                    "description": "APK files",
+                                "files": {
+                                    "description": "APK Files",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "apksign": {
+                                "jarsign": {
                                     "description": "Sign the APK",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "apksignerArguments": {
-                                    "description": "apksigner arguments",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "apksignerFile": {
-                                    "aliases": [
-                                        "apksignerLocation"
-                                    ],
-                                    "description": "apksigner location",
+                                "jarsignerArguments": {
+                                    "description": "Jarsigner Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "apksignerKeyPassword": {
-                                    "aliases": [
-                                        "keyPass"
-                                    ],
-                                    "description": "Key password",
+                                "keyPass": {
+                                    "description": "Key Password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "apksignerKeystoreAlias": {
-                                    "aliases": [
-                                        "keystoreAlias"
-                                    ],
+                                "keystoreAlias": {
                                     "description": "Alias",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "apksignerKeystoreFile": {
-                                    "aliases": [
-                                        "keystoreFile"
-                                    ],
-                                    "description": "Keystore file",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "apksignerKeystorePassword": {
-                                    "aliases": [
-                                        "keystorePass"
-                                    ],
-                                    "description": "Keystore password",
+                                "keystoreFile": {
+                                    "description": "Keystore File",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "apksignerVersion": {
-                                    "description": "apksigner version",
+                                "keystorePass": {
+                                    "description": "Keystore Password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "zipalign": {
                                     "description": "Zipalign",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "zipalignFile": {
-                                    "aliases": [
-                                        "zipalignLocation"
-                                    ],
-                                    "description": "Zipalign location",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "zipalignVersion": {
-                                    "description": "Zipalign version",
+                                "zipalignLocation": {
+                                    "description": "Zipalign Location",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
-                            "required": []
+                            "required": [
+                                "files"
+                            ]
                         },
                         "task": {
-                            "description": "Android signing\n\nSign and align Android APK files",
+                            "description": "Android Signing\n\nSign and align Android APK files",
                             "ignoreCase": "value",
-                            "pattern": "^AndroidSigning@3$"
+                            "pattern": "^AndroidSigning@1$"
                         }
                     },
                     "required": [
-                        "task"
+                        "task",
+                        "inputs"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Android Signing inputs",
+                            "description": "Android signing inputs",
                             "properties": {
-                                "files": {
-                                    "description": "APK Files",
+                                "apkFiles": {
+                                    "aliases": [
+                                        "files"
+                                    ],
+                                    "description": "APK files",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "jarsign": {
                                     "description": "Sign the APK",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "jarsignerArguments": {
-                                    "description": "Jarsigner Arguments",
+                                    "description": "Jarsigner arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "keyPass": {
-                                    "description": "Key Password",
+                                "jarsignerKeyPassword": {
+                                    "aliases": [
+                                        "keyPass"
+                                    ],
+                                    "description": "Key password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "keystoreAlias": {
+                                "jarsignerKeystoreAlias": {
+                                    "aliases": [
+                                        "keystoreAlias"
+                                    ],
                                     "description": "Alias",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "keystoreFile": {
-                                    "description": "Keystore File",
+                                "jarsignerKeystoreFile": {
+                                    "aliases": [
+                                        "keystoreFile"
+                                    ],
+                                    "description": "Keystore file",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "keystorePass": {
-                                    "description": "Keystore Password",
+                                "jarsignerKeystorePassword": {
+                                    "aliases": [
+                                        "keystorePass"
+                                    ],
+                                    "description": "Keystore password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "zipalign": {
                                     "description": "Zipalign",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "zipalignLocation": {
-                                    "description": "Zipalign Location",
+                                "zipalignFile": {
+                                    "aliases": [
+                                        "zipalignLocation"
+                                    ],
+                                    "description": "Zipalign location",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
-                            "required": [
-                                "files"
-                            ]
+                            "required": []
                         },
                         "task": {
-                            "description": "Android Signing\n\nSign and align Android APK files",
+                            "description": "Android signing\n\nSign and align Android APK files",
                             "ignoreCase": "value",
-                            "pattern": "^AndroidSigning@1$"
+                            "pattern": "^AndroidSigning@2$"
                         }
                     },
                     "required": [
-                        "task",
-                        "inputs"
+                        "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
@@ -18450,76 +18858,94 @@
                                     "aliases": [
                                         "files"
                                     ],
                                     "description": "APK files",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "jarsign": {
+                                "apksign": {
                                     "description": "Sign the APK",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "jarsignerArguments": {
-                                    "description": "Jarsigner arguments",
+                                "apksignerArguments": {
+                                    "description": "apksigner arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "jarsignerKeyPassword": {
+                                "apksignerFile": {
+                                    "aliases": [
+                                        "apksignerLocation"
+                                    ],
+                                    "description": "apksigner location",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "apksignerKeyPassword": {
                                     "aliases": [
                                         "keyPass"
                                     ],
                                     "description": "Key password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "jarsignerKeystoreAlias": {
+                                "apksignerKeystoreAlias": {
                                     "aliases": [
                                         "keystoreAlias"
                                     ],
                                     "description": "Alias",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "jarsignerKeystoreFile": {
+                                "apksignerKeystoreFile": {
                                     "aliases": [
                                         "keystoreFile"
                                     ],
                                     "description": "Keystore file",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "jarsignerKeystorePassword": {
+                                "apksignerKeystorePassword": {
                                     "aliases": [
                                         "keystorePass"
                                     ],
                                     "description": "Keystore password",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "apksignerVersion": {
+                                    "description": "apksigner version",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "zipalign": {
                                     "description": "Zipalign",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "zipalignFile": {
                                     "aliases": [
                                         "zipalignLocation"
                                     ],
                                     "description": "Zipalign location",
                                     "ignoreCase": "key",
                                     "type": "string"
+                                },
+                                "zipalignVersion": {
+                                    "description": "Zipalign version",
+                                    "ignoreCase": "key",
+                                    "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Android signing\n\nSign and align Android APK files",
                             "ignoreCase": "value",
-                            "pattern": "^AndroidSigning@2$"
+                            "pattern": "^AndroidSigning@3$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -18828,14 +19254,112 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
+                            "description": "Accessibility Insights Azure DevOps Task inputs",
+                            "properties": {
+                                "baselineFile": {
+                                    "description": "Baseline File Path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "chromePath": {
+                                    "description": "Chrome Path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "discoveryPatterns": {
+                                    "description": "Discovery Patterns",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "failOnAccessibilityError": {
+                                    "description": "Fail on Accessibility Error",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "inputFile": {
+                                    "description": "Input File",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "inputUrls": {
+                                    "description": "Input URLs",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "localhostPort": {
+                                    "description": "Localhost Port",
+                                    "ignoreCase": "key",
+                                    "type": "integer"
+                                },
+                                "maxUrls": {
+                                    "description": "Maximum number of URLs",
+                                    "ignoreCase": "key",
+                                    "type": "integer"
+                                },
+                                "outputDir": {
+                                    "description": "Output Directory",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "repoServiceConnectionName": {
+                                    "description": "Azure Repos Connection",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "scanTimeout": {
+                                    "description": "Scan Timeout",
+                                    "ignoreCase": "key",
+                                    "type": "integer"
+                                },
+                                "scanUrlRelativePath": {
+                                    "description": "Scan URL Relative Path",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "singleWorker": {
+                                    "description": "Uses a single crawler worker.",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "siteDir": {
+                                    "description": "Site Directory",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "url": {
+                                    "description": "Website URL",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                }
+                            },
+                            "required": []
+                        },
+                        "task": {
+                            "description": "Accessibility Insights Azure DevOps Task\n\nScan accessibility issues in an Azure DevOps pipeline",
+                            "ignoreCase": "value",
+                            "pattern": "^accessibility-insights@1$"
+                        }
+                    },
+                    "required": [
+                        "task"
+                    ]
+                },
+                {
+                    "doNotSuggest": false,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
                             "description": "Service Fabric PowerShell inputs",
                             "properties": {
                                 "Inline": {
                                     "description": "Inline Script",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
@@ -18887,14 +19411,119 @@
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
                             "description": "Visual Studio Test inputs",
                             "properties": {
+                                "codeCoverageEnabled": {
+                                    "description": "Code Coverage Enabled",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "configuration": {
+                                    "description": "Configuration",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "otherConsoleOptions": {
+                                    "description": "Other console options",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "overrideTestrunParameters": {
+                                    "description": "Override TestRun Parameters",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "pathtoCustomTestAdapters": {
+                                    "description": "Path to Custom Test Adapters",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "platform": {
+                                    "description": "Platform",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "publishRunAttachments": {
+                                    "description": "Upload Test Attachments",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "runInParallel": {
+                                    "description": "Run In Parallel",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "runSettingsFile": {
+                                    "description": "Run Settings File",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "testAssembly": {
+                                    "description": "Test Assembly",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "testFiltercriteria": {
+                                    "description": "Test Filter criteria",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "testRunTitle": {
+                                    "description": "Test Run Title",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "vsTestVersion": {
+                                    "description": "VSTest version",
+                                    "enum": [
+                                        "latest",
+                                        "14.0",
+                                        "12.0"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "vstestLocation": {
+                                    "description": "Path to vstest.console.exe",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "vstestLocationMethod": {
+                                    "description": "VSTest",
+                                    "enum": [
+                                        "version",
+                                        "location"
+                                    ],
+                                    "ignoreCase": "all"
+                                }
+                            },
+                            "required": []
+                        },
+                        "task": {
+                            "description": "Visual Studio Test\n\nRun tests with Visual Studio test runner",
+                            "ignoreCase": "value",
+                            "pattern": "^VSTest@1$"
+                        }
+                    },
+                    "required": [
+                        "task"
+                    ]
+                },
+                {
+                    "doNotSuggest": false,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
+                            "description": "Visual Studio Test inputs",
+                            "properties": {
                                 "batchingBasedOnAgentsOption": {
                                     "description": "Batch options",
                                     "enum": [
                                         "autoBatchSize",
                                         "customBatchSize"
                                     ],
                                     "ignoreCase": "all"
@@ -19143,119 +19772,14 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Visual Studio Test inputs",
-                            "properties": {
-                                "codeCoverageEnabled": {
-                                    "description": "Code Coverage Enabled",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "configuration": {
-                                    "description": "Configuration",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "otherConsoleOptions": {
-                                    "description": "Other console options",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "overrideTestrunParameters": {
-                                    "description": "Override TestRun Parameters",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "pathtoCustomTestAdapters": {
-                                    "description": "Path to Custom Test Adapters",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "platform": {
-                                    "description": "Platform",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "publishRunAttachments": {
-                                    "description": "Upload Test Attachments",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "runInParallel": {
-                                    "description": "Run In Parallel",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "runSettingsFile": {
-                                    "description": "Run Settings File",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "testAssembly": {
-                                    "description": "Test Assembly",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "testFiltercriteria": {
-                                    "description": "Test Filter criteria",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "testRunTitle": {
-                                    "description": "Test Run Title",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "vsTestVersion": {
-                                    "description": "VSTest version",
-                                    "enum": [
-                                        "latest",
-                                        "14.0",
-                                        "12.0"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "vstestLocation": {
-                                    "description": "Path to vstest.console.exe",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "vstestLocationMethod": {
-                                    "description": "VSTest",
-                                    "enum": [
-                                        "version",
-                                        "location"
-                                    ],
-                                    "ignoreCase": "all"
-                                }
-                            },
-                            "required": []
-                        },
-                        "task": {
-                            "description": "Visual Studio Test\n\nRun tests with Visual Studio test runner",
-                            "ignoreCase": "value",
-                            "pattern": "^VSTest@1$"
-                        }
-                    },
-                    "required": [
-                        "task"
-                    ]
-                },
-                {
-                    "doNotSuggest": false,
-                    "firstProperty": [
-                        "task"
-                    ],
-                    "properties": {
-                        "inputs": {
-                            "additionalProperties": false,
                             "description": "Manual validation inputs",
                             "properties": {
                                 "instructions": {
                                     "description": "Instructions",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
@@ -19874,14 +20398,19 @@
                                     "type": "string"
                                 },
                                 "createLogFile": {
                                     "description": "Create Log File",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "customVersion": {
+                                    "description": "Custom Version",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "enableDefaultLogger": {
                                     "description": "Enable Default Logger",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "logFileVerbosity": {
                                     "description": "Log File Verbosity",
@@ -19932,14 +20461,15 @@
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "vsVersion": {
                                     "description": "Visual Studio Version",
                                     "enum": [
                                         "latest",
+                                        "17.0",
                                         "16.0",
                                         "15.0",
                                         "14.0",
                                         "12.0",
                                         "11.0"
                                     ],
                                     "ignoreCase": "all"
@@ -20622,14 +21152,16 @@
                                 "msbuildVersionOption": {
                                     "aliases": [
                                         "msbuildVersion"
                                     ],
                                     "description": "MSBuild version",
                                     "enum": [
                                         "latest",
+                                        "17.0",
+                                        "16.0",
                                         "15.0",
                                         "14.0",
                                         "12.0",
                                         "4.0"
                                     ],
                                     "ignoreCase": "all"
                                 },
@@ -20673,14 +21205,19 @@
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
                             "description": "Manifest Generator Task inputs",
                             "properties": {
+                                "BuildComponentPath": {
+                                    "description": "The folder that contains the build's components/packages.",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "BuildDropPath": {
                                     "description": "The root folder for which the manifest has to be generated.",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "ConfigFilePath": {
                                     "description": "The json file that contains the configuration for the Manifest Tool.",
@@ -20896,14 +21433,155 @@
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
                 {
+                    "deprecationMessage": "AzureResourceGroupDeployment is deprecated - Deploy, start, stop, delete Azure Resource Groups",
+                    "doNotSuggest": true,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
+                            "description": "Azure Resource Group Deployment inputs",
+                            "properties": {
+                                "ConnectedServiceName": {
+                                    "description": "Azure Subscription",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "ConnectedServiceNameClassic": {
+                                    "description": "Azure Classic Subscription",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "ConnectedServiceNameSelector": {
+                                    "description": "Azure Connection Type",
+                                    "enum": [
+                                        "ConnectedServiceName",
+                                        "ConnectedServiceNameClassic"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "action": {
+                                    "description": "Action",
+                                    "enum": [
+                                        "Create Or Update Resource Group",
+                                        "Select Resource Group",
+                                        "Start",
+                                        "Stop",
+                                        "Restart",
+                                        "Delete",
+                                        "DeleteRG"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "actionClassic": {
+                                    "description": "Action",
+                                    "enum": [
+                                        "Select Resource Group"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "cloudService": {
+                                    "description": "Cloud Service",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "csmFile": {
+                                    "description": "Template",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "csmParametersFile": {
+                                    "description": "Template Parameters",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "deploymentMode": {
+                                    "description": "Deployment Mode",
+                                    "enum": [
+                                        "Validation",
+                                        "Incremental",
+                                        "Complete"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "enableDeploymentPrerequisitesForCreate": {
+                                    "description": "Enable Deployment Prerequisites",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "enableDeploymentPrerequisitesForSelect": {
+                                    "description": "Enable Deployment Prerequisites",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "location": {
+                                    "description": "Location",
+                                    "enum": [
+                                        "Australia East",
+                                        "Australia Southeast",
+                                        "Brazil South",
+                                        "Canada Central",
+                                        "Canada East",
+                                        "Central India",
+                                        "Central US",
+                                        "East Asia",
+                                        "East US",
+                                        "East US 2 ",
+                                        "Japan East",
+                                        "Japan West",
+                                        "North Central US",
+                                        "North Europe",
+                                        "South Central US",
+                                        "South India",
+                                        "Southeast Asia",
+                                        "UK South",
+                                        "UK West",
+                                        "West Central US",
+                                        "West Europe",
+                                        "West India",
+                                        "West US",
+                                        "West US 2"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "outputVariable": {
+                                    "description": "Resource Group",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "overrideParameters": {
+                                    "description": "Override Template Parameters",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "resourceGroupName": {
+                                    "description": "Resource Group",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                }
+                            },
+                            "required": []
+                        },
+                        "task": {
+                            "description": "Azure Resource Group Deployment\n\nDeploy, start, stop, delete Azure Resource Groups",
+                            "ignoreCase": "value",
+                            "pattern": "^AzureResourceGroupDeployment@1$"
+                        }
+                    },
+                    "required": [
+                        "task"
+                    ]
+                },
+                {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
@@ -21193,155 +21871,14 @@
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
                 {
-                    "deprecationMessage": "AzureResourceGroupDeployment is deprecated - Deploy, start, stop, delete Azure Resource Groups",
-                    "doNotSuggest": true,
-                    "firstProperty": [
-                        "task"
-                    ],
-                    "properties": {
-                        "inputs": {
-                            "additionalProperties": false,
-                            "description": "Azure Resource Group Deployment inputs",
-                            "properties": {
-                                "ConnectedServiceName": {
-                                    "description": "Azure Subscription",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "ConnectedServiceNameClassic": {
-                                    "description": "Azure Classic Subscription",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "ConnectedServiceNameSelector": {
-                                    "description": "Azure Connection Type",
-                                    "enum": [
-                                        "ConnectedServiceName",
-                                        "ConnectedServiceNameClassic"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "action": {
-                                    "description": "Action",
-                                    "enum": [
-                                        "Create Or Update Resource Group",
-                                        "Select Resource Group",
-                                        "Start",
-                                        "Stop",
-                                        "Restart",
-                                        "Delete",
-                                        "DeleteRG"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "actionClassic": {
-                                    "description": "Action",
-                                    "enum": [
-                                        "Select Resource Group"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "cloudService": {
-                                    "description": "Cloud Service",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "csmFile": {
-                                    "description": "Template",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "csmParametersFile": {
-                                    "description": "Template Parameters",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "deploymentMode": {
-                                    "description": "Deployment Mode",
-                                    "enum": [
-                                        "Validation",
-                                        "Incremental",
-                                        "Complete"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "enableDeploymentPrerequisitesForCreate": {
-                                    "description": "Enable Deployment Prerequisites",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "enableDeploymentPrerequisitesForSelect": {
-                                    "description": "Enable Deployment Prerequisites",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "location": {
-                                    "description": "Location",
-                                    "enum": [
-                                        "Australia East",
-                                        "Australia Southeast",
-                                        "Brazil South",
-                                        "Canada Central",
-                                        "Canada East",
-                                        "Central India",
-                                        "Central US",
-                                        "East Asia",
-                                        "East US",
-                                        "East US 2 ",
-                                        "Japan East",
-                                        "Japan West",
-                                        "North Central US",
-                                        "North Europe",
-                                        "South Central US",
-                                        "South India",
-                                        "Southeast Asia",
-                                        "UK South",
-                                        "UK West",
-                                        "West Central US",
-                                        "West Europe",
-                                        "West India",
-                                        "West US",
-                                        "West US 2"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "outputVariable": {
-                                    "description": "Resource Group",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "overrideParameters": {
-                                    "description": "Override Template Parameters",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "resourceGroupName": {
-                                    "description": "Resource Group",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                }
-                            },
-                            "required": []
-                        },
-                        "task": {
-                            "description": "Azure Resource Group Deployment\n\nDeploy, start, stop, delete Azure Resource Groups",
-                            "ignoreCase": "value",
-                            "pattern": "^AzureResourceGroupDeployment@1$"
-                        }
-                    },
-                    "required": [
-                        "task"
-                    ]
-                },
-                {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
@@ -21705,15 +22242,15 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Copy Files inputs",
+                            "description": "Copy files inputs",
                             "properties": {
                                 "CleanTargetFolder": {
                                     "description": "Clean Target Folder",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "Contents": {
@@ -21732,28 +22269,48 @@
                                     "type": "string"
                                 },
                                 "TargetFolder": {
                                     "description": "Target Folder",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
+                                "delayBetweenRetries": {
+                                    "description": "Delay between two retries.",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
                                 "flattenFolders": {
                                     "description": "Flatten Folders",
                                     "ignoreCase": "key",
                                     "type": "boolean"
+                                },
+                                "ignoreMakeDirErrors": {
+                                    "description": "Ignore errors during creation of target folder.",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "preserveTimestamp": {
+                                    "description": "Preserve Target Timestamp",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "retryCount": {
+                                    "description": "Retry count to copy the file",
+                                    "ignoreCase": "key",
+                                    "type": "string"
                                 }
                             },
                             "required": [
                                 "TargetFolder"
                             ]
                         },
                         "task": {
-                            "description": "Copy Files\n\nCopy files from source folder to target folder using minimatch patterns (The minimatch patterns will only match file paths, not folder paths)",
+                            "description": "Copy files\n\nCopy files from a source folder to a target folder using patterns matching file paths (not folder paths)",
                             "ignoreCase": "value",
-                            "pattern": "^CopyFiles@1$"
+                            "pattern": "^CopyFiles@2$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -21761,15 +22318,15 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Copy files inputs",
+                            "description": "Copy Files inputs",
                             "properties": {
                                 "CleanTargetFolder": {
                                     "description": "Clean Target Folder",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "Contents": {
@@ -21792,34 +22349,24 @@
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "flattenFolders": {
                                     "description": "Flatten Folders",
                                     "ignoreCase": "key",
                                     "type": "boolean"
-                                },
-                                "preserveTimestamp": {
-                                    "description": "Preserve Target Timestamp",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "retryCount": {
-                                    "description": "Retry count to copy the file",
-                                    "ignoreCase": "key",
-                                    "type": "string"
                                 }
                             },
                             "required": [
                                 "TargetFolder"
                             ]
                         },
                         "task": {
-                            "description": "Copy files\n\nCopy files from a source folder to a target folder using patterns matching file paths (not folder paths)",
+                            "description": "Copy Files\n\nCopy files from source folder to target folder using minimatch patterns (The minimatch patterns will only match file paths, not folder paths)",
                             "ignoreCase": "value",
-                            "pattern": "^CopyFiles@2$"
+                            "pattern": "^CopyFiles@1$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -22168,14 +22715,23 @@
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "skip_app_build": {
                                     "description": "Skip App Build",
                                     "ignoreCase": "key",
                                     "type": "boolean"
+                                },
+                                "workingDirectory": {
+                                    "aliases": [
+                                        "cwd",
+                                        "rootDirectory"
+                                    ],
+                                    "description": "Working directory",
+                                    "ignoreCase": "key",
+                                    "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
                             "description": "Deploy Azure Static Web App\n\n[PREVIEW] Build and deploy an Azure Static Web App",
                             "ignoreCase": "value",
@@ -22190,76 +22746,76 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Use Node.js ecosystem inputs",
+                            "description": "Node.js tool installer inputs",
                             "properties": {
                                 "checkLatest": {
                                     "description": "Check for Latest Version",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "force32bit": {
                                     "description": "Use 32 bit version on x64 agents",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "version": {
-                                    "description": "Version",
+                                "versionSpec": {
+                                    "description": "Version Spec",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Use Node.js ecosystem\n\nSet up a Node.js environment and add it to the PATH, additionally providing proxy support",
+                            "description": "Node.js tool installer\n\nFinds or downloads and caches the specified version spec of Node.js and adds it to the PATH",
                             "ignoreCase": "value",
-                            "pattern": "^UseNode@1$"
+                            "pattern": "^NodeTool@0$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Node.js tool installer inputs",
+                            "description": "Use Node.js ecosystem inputs",
                             "properties": {
                                 "checkLatest": {
                                     "description": "Check for Latest Version",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
                                 "force32bit": {
                                     "description": "Use 32 bit version on x64 agents",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "versionSpec": {
-                                    "description": "Version Spec",
+                                "version": {
+                                    "description": "Version",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
                             "required": []
                         },
                         "task": {
-                            "description": "Node.js tool installer\n\nFinds or downloads and caches the specified version spec of Node.js and adds it to the PATH",
+                            "description": "Use Node.js ecosystem\n\nSet up a Node.js environment and add it to the PATH, additionally providing proxy support",
                             "ignoreCase": "value",
-                            "pattern": "^NodeTool@0$"
+                            "pattern": "^UseNode@1$"
                         }
                     },
                     "required": [
                         "task"
                     ]
                 },
                 {
@@ -22813,14 +23369,19 @@
                                     "ignoreCase": "all"
                                 },
                                 "checkDownloadedFiles": {
                                     "description": "Check downloaded files",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
+                                "cleanDestinationFolder": {
+                                    "description": "Clean destination folder",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
                                 "downloadPath": {
                                     "description": "Destination directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "downloadType": {
                                     "description": "Download type",
@@ -22890,14 +23451,130 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
+                            "description": "Download build artifacts inputs",
+                            "properties": {
+                                "allowPartiallySucceededBuilds": {
+                                    "description": "Download artifacts even from partially succeeded builds.",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "artifactName": {
+                                    "description": "Artifact name",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "branchName": {
+                                    "description": "Branch name",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "buildId": {
+                                    "description": "Build",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "buildType": {
+                                    "description": "Download artifacts produced by",
+                                    "enum": [
+                                        "current",
+                                        "specific"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "buildVersionToDownload": {
+                                    "description": "Build version to download",
+                                    "enum": [
+                                        "latest",
+                                        "latestFromBranch",
+                                        "specific"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "checkDownloadedFiles": {
+                                    "description": "Check downloaded files",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "downloadPath": {
+                                    "description": "Destination directory",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "downloadType": {
+                                    "description": "Download type",
+                                    "enum": [
+                                        "single",
+                                        "specific"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "itemPattern": {
+                                    "description": "Matching pattern",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "parallelizationLimit": {
+                                    "description": "Parallelization limit",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "pipeline": {
+                                    "aliases": [
+                                        "definition"
+                                    ],
+                                    "description": "Build pipeline",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "project": {
+                                    "description": "Project",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "retryDownloadCount": {
+                                    "description": "Retry count",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "specificBuildWithTriggering": {
+                                    "description": "When appropriate, download artifacts from the triggering build.",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "tags": {
+                                    "description": "Build Tags",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                }
+                            },
+                            "required": []
+                        },
+                        "task": {
+                            "description": "Download build artifacts\n\nDownload files that were saved as artifacts of a completed build",
+                            "ignoreCase": "value",
+                            "pattern": "^DownloadBuildArtifacts@1$"
+                        }
+                    },
+                    "required": [
+                        "task"
+                    ]
+                },
+                {
+                    "doNotSuggest": false,
+                    "firstProperty": [
+                        "task"
+                    ],
+                    "properties": {
+                        "inputs": {
+                            "additionalProperties": false,
                             "description": "CocoaPods inputs",
                             "properties": {
                                 "forceRepoUpdate": {
                                     "description": "Force repo update",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
@@ -23476,29 +24153,29 @@
                                     "type": "boolean"
                                 },
                                 "isPreRelease": {
                                     "description": "Pre-release",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "releaseNotes": {
-                                    "description": "Release notes",
+                                "releaseNotesFilePath": {
+                                    "description": "Release notes file path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "releaseNotesFile": {
-                                    "description": "Release notes file path",
+                                "releaseNotesInline": {
+                                    "description": "Release notes",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "releaseNotesSource": {
                                     "description": "Release notes source",
                                     "enum": [
-                                        "file",
-                                        "input"
+                                        "filePath",
+                                        "inline"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "repositoryName": {
                                     "description": "Repository",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -23512,16 +24189,16 @@
                                     "description": "Tag Pattern",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "tagSource": {
                                     "description": "Tag source",
                                     "enum": [
-                                        "auto",
-                                        "manual"
+                                        "gitTag",
+                                        "userSpecifiedTag"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "target": {
                                     "description": "Target",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -23535,15 +24212,15 @@
                             "required": [
                                 "gitHubConnection"
                             ]
                         },
                         "task": {
                             "description": "GitHub Release\n\nCreate, edit, or delete a GitHub release",
                             "ignoreCase": "value",
-                            "pattern": "^GitHubRelease@0$"
+                            "pattern": "^GitHubRelease@1$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -23622,29 +24299,29 @@
                                     "type": "boolean"
                                 },
                                 "isPreRelease": {
                                     "description": "Pre-release",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "releaseNotesFilePath": {
-                                    "description": "Release notes file path",
+                                "releaseNotes": {
+                                    "description": "Release notes",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "releaseNotesInline": {
-                                    "description": "Release notes",
+                                "releaseNotesFile": {
+                                    "description": "Release notes file path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "releaseNotesSource": {
                                     "description": "Release notes source",
                                     "enum": [
-                                        "filePath",
-                                        "inline"
+                                        "file",
+                                        "input"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "repositoryName": {
                                     "description": "Repository",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -23658,16 +24335,16 @@
                                     "description": "Tag Pattern",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
                                 "tagSource": {
                                     "description": "Tag source",
                                     "enum": [
-                                        "gitTag",
-                                        "userSpecifiedTag"
+                                        "auto",
+                                        "manual"
                                     ],
                                     "ignoreCase": "all"
                                 },
                                 "target": {
                                     "description": "Target",
                                     "ignoreCase": "key",
                                     "type": "string"
@@ -23681,15 +24358,15 @@
                             "required": [
                                 "gitHubConnection"
                             ]
                         },
                         "task": {
                             "description": "GitHub Release\n\nCreate, edit, or delete a GitHub release",
                             "ignoreCase": "value",
-                            "pattern": "^GitHubRelease@1$"
+                            "pattern": "^GitHubRelease@0$"
                         }
                     },
                     "required": [
                         "task",
                         "inputs"
                     ]
                 },
@@ -24207,121 +24884,121 @@
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Bash inputs",
+                            "description": "Shell script inputs",
                             "properties": {
-                                "arguments": {
+                                "args": {
                                     "description": "Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "failOnStderr": {
-                                    "description": "Fail on Standard Error",
-                                    "ignoreCase": "key",
-                                    "type": "boolean"
-                                },
-                                "filePath": {
-                                    "description": "Script Path",
+                                "cwd": {
+                                    "description": "Working Directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "noProfile": {
-                                    "description": "Don't load the profile startup/initialization files",
+                                "disableAutoCwd": {
+                                    "description": "Specify Working Directory",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "noRc": {
-                                    "description": "Don't read the `~/.bashrc' initialization file",
+                                "failOnStandardError": {
+                                    "description": "Fail on Standard Error",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "script": {
-                                    "description": "Script",
-                                    "ignoreCase": "key",
-                                    "type": "string"
-                                },
-                                "targetType": {
-                                    "description": "Type",
-                                    "enum": [
-                                        "filePath",
-                                        "inline"
-                                    ],
-                                    "ignoreCase": "all"
-                                },
-                                "workingDirectory": {
-                                    "description": "Working Directory",
+                                "scriptPath": {
+                                    "description": "Script Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
-                            "required": []
+                            "required": [
+                                "scriptPath"
+                            ]
                         },
                         "task": {
-                            "description": "Bash\n\nRun a Bash script on macOS, Linux, or Windows",
+                            "description": "Shell script\n\nRun a shell script using Bash",
                             "ignoreCase": "value",
-                            "pattern": "^Bash@3$"
+                            "pattern": "^ShellScript@2$"
                         }
                     },
                     "required": [
-                        "task"
+                        "task",
+                        "inputs"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
                     "properties": {
                         "inputs": {
                             "additionalProperties": false,
-                            "description": "Shell script inputs",
+                            "description": "Bash inputs",
                             "properties": {
-                                "args": {
+                                "arguments": {
                                     "description": "Arguments",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "cwd": {
-                                    "description": "Working Directory",
+                                "failOnStderr": {
+                                    "description": "Fail on Standard Error",
+                                    "ignoreCase": "key",
+                                    "type": "boolean"
+                                },
+                                "filePath": {
+                                    "description": "Script Path",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 },
-                                "disableAutoCwd": {
-                                    "description": "Specify Working Directory",
+                                "noProfile": {
+                                    "description": "Don't load the profile startup/initialization files",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "failOnStandardError": {
-                                    "description": "Fail on Standard Error",
+                                "noRc": {
+                                    "description": "Don't read the `~/.bashrc' initialization file",
                                     "ignoreCase": "key",
                                     "type": "boolean"
                                 },
-                                "scriptPath": {
-                                    "description": "Script Path",
+                                "script": {
+                                    "description": "Script",
+                                    "ignoreCase": "key",
+                                    "type": "string"
+                                },
+                                "targetType": {
+                                    "description": "Type",
+                                    "enum": [
+                                        "filePath",
+                                        "inline"
+                                    ],
+                                    "ignoreCase": "all"
+                                },
+                                "workingDirectory": {
+                                    "description": "Working Directory",
                                     "ignoreCase": "key",
                                     "type": "string"
                                 }
                             },
-                            "required": [
-                                "scriptPath"
-                            ]
+                            "required": []
                         },
                         "task": {
-                            "description": "Shell script\n\nRun a shell script using Bash",
+                            "description": "Bash\n\nRun a Bash script on macOS, Linux, or Windows",
                             "ignoreCase": "value",
-                            "pattern": "^ShellScript@2$"
+                            "pattern": "^Bash@3$"
                         }
                     },
                     "required": [
-                        "task",
-                        "inputs"
+                        "task"
                     ]
                 },
                 {
                     "doNotSuggest": false,
                     "firstProperty": [
                         "task"
                     ],
@@ -25542,14 +26219,18 @@
                     "type": "object"
                 },
                 "name": {
                     "description": "ID of the task instance",
                     "pattern": "^[_A-Za-z0-9]*$",
                     "type": "string"
                 },
+                "retryCountOnTaskFailure": {
+                    "description": "Number of retries if the task fails",
+                    "type": "integer"
+                },
                 "task": {
                     "anyOf": [
                         {
                             "description": "Run a PowerShell script on Linux, macOS, or Windows",
                             "doNotSuggest": false,
                             "enum": [
                                 "PowerShell@2"
@@ -25628,15 +26309,15 @@
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build, test, and deploy with Apache Maven",
                             "doNotSuggest": false,
                             "enum": [
-                                "Maven@3"
+                                "Maven@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build with Apache Maven",
                             "doNotSuggest": false,
                             "enum": [
@@ -25644,15 +26325,15 @@
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build, test, and deploy with Apache Maven",
                             "doNotSuggest": false,
                             "enum": [
-                                "Maven@2"
+                                "Maven@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build, test, package, or publish a dotnet application, or run a custom dotnet command",
                             "doNotSuggest": false,
                             "enum": [
@@ -25764,26 +26445,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "ManualIntervention@8"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Install an Apple provisioning profile required to build on a macOS agent",
+                            "description": "Install an Apple provisioning profile required to build on a macOS agent machine",
                             "doNotSuggest": false,
                             "enum": [
-                                "InstallAppleProvisioningProfile@0"
+                                "InstallAppleProvisioningProfile@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Install an Apple provisioning profile required to build on a macOS agent machine",
+                            "description": "Install an Apple provisioning profile required to build on a macOS agent",
                             "doNotSuggest": false,
                             "enum": [
-                                "InstallAppleProvisioningProfile@1"
+                                "InstallAppleProvisioningProfile@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "deprecationMessage": "SonarQubePostTest is deprecated - [DEPRECATED] Finish the analysis and upload the results to SonarQube",
                             "description": "[DEPRECATED] Finish the analysis and upload the results to SonarQube",
                             "doNotSuggest": true,
@@ -25839,26 +26520,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "PublishPipelineMetadata@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Build or push Docker images, login or logout, start or stop containers, or run a Docker command",
+                            "description": "Build, tag, push, or run Docker images, or run a Docker command",
                             "doNotSuggest": false,
                             "enum": [
-                                "Docker@2"
+                                "Docker@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Build, tag, push, or run Docker images, or run a Docker command",
+                            "description": "Build or push Docker images, login or logout, start or stop containers, or run a Docker command",
                             "doNotSuggest": false,
                             "enum": [
-                                "Docker@0"
+                                "Docker@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build, tag, push, or run Docker images, or run a Docker command",
                             "doNotSuggest": false,
                             "enum": [
@@ -26173,34 +26854,34 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "ServiceFabricDeploy@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Build, test, or archive an Xcode workspace on macOS. Optionally package an app.",
+                            "description": "Build an Xcode workspace on macOS",
                             "doNotSuggest": false,
                             "enum": [
-                                "Xcode@5"
+                                "Xcode@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Build an Xcode workspace on macOS",
+                            "description": "Build, test, or archive an Xcode workspace on macOS. Optionally package an app.",
                             "doNotSuggest": false,
                             "enum": [
-                                "Xcode@3"
+                                "Xcode@4"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build, test, or archive an Xcode workspace on macOS. Optionally package an app.",
                             "doNotSuggest": false,
                             "enum": [
-                                "Xcode@4"
+                                "Xcode@5"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build an Xcode workspace on Mac OS",
                             "doNotSuggest": false,
                             "enum": [
@@ -26420,39 +27101,39 @@
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build an iOS app with Xamarin on macOS",
                             "doNotSuggest": false,
                             "enum": [
-                                "XamariniOS@2"
+                                "XamariniOS@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Build an iOS app with Xamarin on macOS",
                             "doNotSuggest": false,
                             "enum": [
-                                "XamariniOS@1"
+                                "XamariniOS@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Publish test results to Azure Pipelines",
                             "doNotSuggest": false,
                             "enum": [
-                                "PublishTestResults@2"
+                                "PublishTestResults@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Publish test results to Azure Pipelines",
                             "doNotSuggest": false,
                             "enum": [
-                                "PublishTestResults@1"
+                                "PublishTestResults@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Copy files to Azure Blob Storage or virtual machines",
                             "doNotSuggest": false,
                             "enum": [
@@ -26481,26 +27162,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "AzureFileCopy@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Index your source code and publish symbols to a file share or Azure Artifacts symbol server",
+                            "description": "Index your source code and publish symbols to a file share",
                             "doNotSuggest": false,
                             "enum": [
-                                "PublishSymbols@2"
+                                "PublishSymbols@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Index your source code and publish symbols to a file share",
+                            "description": "Index your source code and publish symbols to a file share or Azure Artifacts symbol server",
                             "doNotSuggest": false,
                             "enum": [
-                                "PublishSymbols@1"
+                                "PublishSymbols@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Copy files or build artifacts to a remote machine over SSH",
                             "doNotSuggest": false,
                             "enum": [
@@ -26521,18 +27202,18 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "Gradle@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Distribute app builds to testers and users via Visual Studio App Center",
+                            "description": "Build using a Gradle wrapper script",
                             "doNotSuggest": false,
                             "enum": [
-                                "AppCenterDistribute@1"
+                                "Gradle@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Distribute app builds to testers and users via Visual Studio App Center",
                             "doNotSuggest": false,
                             "enum": [
@@ -26545,14 +27226,22 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "AppCenterDistribute@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
+                            "description": "Distribute app builds to testers and users via Visual Studio App Center",
+                            "doNotSuggest": false,
+                            "enum": [
+                                "AppCenterDistribute@1"
+                            ],
+                            "ignoreCase": "value"
+                        },
+                        {
                             "description": "Distribute app builds to testers and users via App Center",
                             "doNotSuggest": false,
                             "enum": [
                                 "AppCenterDistribute@0"
                             ],
                             "ignoreCase": "value"
                         },
@@ -26609,26 +27298,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "InstallAppleCertificate@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Install an Apple certificate required to build on a macOS agent",
+                            "description": "Install an Apple certificate required to build on a macOS agent machine",
                             "doNotSuggest": false,
                             "enum": [
-                                "InstallAppleCertificate@0"
+                                "InstallAppleCertificate@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Install an Apple certificate required to build on a macOS agent machine",
+                            "description": "Install an Apple certificate required to build on a macOS agent",
                             "doNotSuggest": false,
                             "enum": [
-                                "InstallAppleCertificate@2"
+                                "InstallAppleCertificate@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Invoke Azure function as a part of your process.",
                             "doNotSuggest": false,
                             "enum": [
@@ -26734,31 +27423,31 @@
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Sign and align Android APK files",
                             "doNotSuggest": false,
                             "enum": [
-                                "AndroidSigning@3"
+                                "AndroidSigning@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Sign and align Android APK files",
                             "doNotSuggest": false,
                             "enum": [
-                                "AndroidSigning@1"
+                                "AndroidSigning@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Sign and align Android APK files",
                             "doNotSuggest": false,
                             "enum": [
-                                "AndroidSigning@2"
+                                "AndroidSigning@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "deprecationMessage": "DownloadPipelineArtifact is deprecated - Downloads an artifact associated with a pipeline",
                             "description": "Downloads an artifact associated with a pipeline",
                             "doNotSuggest": true,
@@ -26789,38 +27478,46 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "UsePythonVersion@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Run a PowerShell script in the context of an Azure Service Fabric cluster connection",
+                            "description": "Scan accessibility issues in an Azure DevOps pipeline",
                             "doNotSuggest": false,
                             "enum": [
-                                "ServiceFabricPowerShell@1"
+                                "accessibility-insights@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Run unit and functional tests (Selenium, Appium, Coded UI test, etc.) using the Visual Studio Test (VsTest) runner. Test frameworks that have a Visual Studio test adapter such as MsTest, xUnit, NUnit, Chutzpah (for JavaScript tests using QUnit, Mocha and Jasmine), etc. can be run. Tests can be distributed on multiple agents using this task (version 2).",
+                            "description": "Run a PowerShell script in the context of an Azure Service Fabric cluster connection",
                             "doNotSuggest": false,
                             "enum": [
-                                "VSTest@2"
+                                "ServiceFabricPowerShell@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Run tests with Visual Studio test runner",
                             "doNotSuggest": false,
                             "enum": [
                                 "VSTest@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
+                            "description": "Run unit and functional tests (Selenium, Appium, Coded UI test, etc.) using the Visual Studio Test (VsTest) runner. Test frameworks that have a Visual Studio test adapter such as MsTest, xUnit, NUnit, Chutzpah (for JavaScript tests using QUnit, Mocha and Jasmine), etc. can be run. Tests can be distributed on multiple agents using this task (version 2).",
+                            "doNotSuggest": false,
+                            "enum": [
+                                "VSTest@2"
+                            ],
+                            "ignoreCase": "value"
+                        },
+                        {
                             "description": "[PREVIEW] Pause a pipeline run to wait for manual interaction. Works only with YAML pipelines.",
                             "doNotSuggest": false,
                             "enum": [
                                 "ManualValidation@0"
                             ],
                             "ignoreCase": "value"
                         },
@@ -27009,35 +27706,35 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "DownloadPackage@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Deploy an Azure Resource Manager (ARM) template to a resource group and manage virtual machines",
-                            "doNotSuggest": false,
+                            "deprecationMessage": "AzureResourceGroupDeployment is deprecated - Deploy, start, stop, delete Azure Resource Groups",
+                            "description": "Deploy, start, stop, delete Azure Resource Groups",
+                            "doNotSuggest": true,
                             "enum": [
-                                "AzureResourceGroupDeployment@2"
+                                "AzureResourceGroupDeployment@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Deploy an Azure Resource Manager (ARM) template to all the deployment scopes",
+                            "description": "Deploy an Azure Resource Manager (ARM) template to a resource group and manage virtual machines",
                             "doNotSuggest": false,
                             "enum": [
-                                "AzureResourceManagerTemplateDeployment@3"
+                                "AzureResourceGroupDeployment@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "deprecationMessage": "AzureResourceGroupDeployment is deprecated - Deploy, start, stop, delete Azure Resource Groups",
-                            "description": "Deploy, start, stop, delete Azure Resource Groups",
-                            "doNotSuggest": true,
+                            "description": "Deploy an Azure Resource Manager (ARM) template to all the deployment scopes",
+                            "doNotSuggest": false,
                             "enum": [
-                                "AzureResourceGroupDeployment@1"
+                                "AzureResourceManagerTemplateDeployment@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Invoke REST API as a part of your process.",
                             "doNotSuggest": false,
                             "enum": [
@@ -27074,26 +27771,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "GitHubComment@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Copy files from source folder to target folder using minimatch patterns (The minimatch patterns will only match file paths, not folder paths)",
+                            "description": "Copy files from a source folder to a target folder using patterns matching file paths (not folder paths)",
                             "doNotSuggest": false,
                             "enum": [
-                                "CopyFiles@1"
+                                "CopyFiles@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Copy files from a source folder to a target folder using patterns matching file paths (not folder paths)",
+                            "description": "Copy files from source folder to target folder using minimatch patterns (The minimatch patterns will only match file paths, not folder paths)",
                             "doNotSuggest": false,
                             "enum": [
-                                "CopyFiles@2"
+                                "CopyFiles@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Run your scripts and make changes to your Azure Database for MySQL",
                             "doNotSuggest": false,
                             "enum": [
@@ -27130,26 +27827,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "AzureStaticWebApp@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Set up a Node.js environment and add it to the PATH, additionally providing proxy support",
+                            "description": "Finds or downloads and caches the specified version spec of Node.js and adds it to the PATH",
                             "doNotSuggest": false,
                             "enum": [
-                                "UseNode@1"
+                                "NodeTool@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Finds or downloads and caches the specified version spec of Node.js and adds it to the PATH",
+                            "description": "Set up a Node.js environment and add it to the PATH, additionally providing proxy support",
                             "doNotSuggest": false,
                             "enum": [
-                                "NodeTool@0"
+                                "UseNode@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "deprecationMessage": "SqlServerDacpacDeployment is deprecated - Deploy a SQL Server database using DACPAC",
                             "description": "Deploy a SQL Server database using DACPAC",
                             "doNotSuggest": true,
@@ -27195,14 +27892,22 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "DownloadBuildArtifacts@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
+                            "description": "Download files that were saved as artifacts of a completed build",
+                            "doNotSuggest": false,
+                            "enum": [
+                                "DownloadBuildArtifacts@1"
+                            ],
+                            "ignoreCase": "value"
+                        },
+                        {
                             "description": "Install CocoaPods dependencies for Swift and Objective-C Cocoa projects",
                             "doNotSuggest": false,
                             "enum": [
                                 "CocoaPods@0"
                             ],
                             "ignoreCase": "value"
                         },
@@ -27246,23 +27951,23 @@
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Create, edit, or delete a GitHub release",
                             "doNotSuggest": false,
                             "enum": [
-                                "GitHubRelease@0"
+                                "GitHubRelease@1"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Create, edit, or delete a GitHub release",
                             "doNotSuggest": false,
                             "enum": [
-                                "GitHubRelease@1"
+                                "GitHubRelease@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Use cURL to upload files with FTP, FTPS, SFTP, HTTP, and more.",
                             "doNotSuggest": false,
                             "enum": [
@@ -27307,26 +28012,26 @@
                             "doNotSuggest": false,
                             "enum": [
                                 "AzureFunctionOnKubernetes@0"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Run a Bash script on macOS, Linux, or Windows",
+                            "description": "Run a shell script using Bash",
                             "doNotSuggest": false,
                             "enum": [
-                                "Bash@3"
+                                "ShellScript@2"
                             ],
                             "ignoreCase": "value"
                         },
                         {
-                            "description": "Run a shell script using Bash",
+                            "description": "Run a Bash script on macOS, Linux, or Windows",
                             "doNotSuggest": false,
                             "enum": [
-                                "ShellScript@2"
+                                "Bash@3"
                             ],
                             "ignoreCase": "value"
                         },
                         {
                             "description": "Publish build artifacts to Azure Pipelines or a Windows file share",
                             "doNotSuggest": false,
                             "enum": [
@@ -27448,14 +28153,18 @@
                     "$ref": "#/definitions/mappingOfStringString",
                     "description": "Variables to map into the process's environment"
                 },
                 "name": {
                     "$ref": "#/definitions/referenceName",
                     "description": "ID of the step"
                 },
+                "retryCountOnTaskFailure": {
+                    "$ref": "#/definitions/string",
+                    "description": "Number of retries if the task fails"
+                },
                 "target": {
                     "$ref": "#/definitions/stepTarget",
                     "description": "Environment in which to run this task"
                 },
                 "timeoutInMinutes": {
                     "$ref": "#/definitions/nonEmptyString",
                     "description": "Time to wait for this task to complete before the server kills it"
```

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-actions.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-actions.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/github-workflows.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/github-workflows.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/readthedocs.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/readthedocs.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/renovate.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/renovate.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/builtin_schemas/vendor/travis.json` & `check-jsonschema-0.9.1/src/check_jsonschema/builtin_schemas/vendor/travis.json`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/cachedownloader.py` & `check-jsonschema-0.9.1/src/check_jsonschema/cachedownloader.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/checker.py` & `check-jsonschema-0.9.1/src/check_jsonschema/checker.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/formats.py` & `check-jsonschema-0.9.1/src/check_jsonschema/formats.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/loaders/instance.py` & `check-jsonschema-0.9.1/src/check_jsonschema/loaders/instance.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/loaders/schema.py` & `check-jsonschema-0.9.1/src/check_jsonschema/loaders/schema.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/parse_cli.py` & `check-jsonschema-0.9.1/src/check_jsonschema/parse_cli.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema/utils.py` & `check-jsonschema-0.9.1/src/check_jsonschema/utils.py`

 * *Files identical despite different names*

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema.egg-info/PKG-INFO` & `check-jsonschema-0.9.1/src/check_jsonschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-jsonschema
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pre-commit hook for validating files against jsonschemas.
 Home-page: https://github.com/sirosen/check-jsonschema
 Author: Stephen Rosen
 Author-email: sirosen@uchicago.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `check-jsonschema-0.9.0/src/check_jsonschema.egg-info/SOURCES.txt` & `check-jsonschema-0.9.1/src/check_jsonschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

