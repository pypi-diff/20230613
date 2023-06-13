# Comparing `tmp/themule-0.1.2.tar.gz` & `tmp/themule-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themule-0.1.2.tar", last modified: Tue Jun 13 18:21:30 2023, max compression
+gzip compressed data, was "themule-0.1.3.tar", last modified: Tue Jun 13 21:25:14 2023, max compression
```

## Comparing `themule-0.1.2.tar` & `themule-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:21:30.145569 themule-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 18:21:20.000000 themule-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 18:21:30.145569 themule-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 18:21:20.000000 themule-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 18:21:20.000000 themule-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:21:30.141569 themule-0.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 18:21:20.000000 themule-0.1.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 18:21:20.000000 themule-0.1.2/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 18:21:20.000000 themule-0.1.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:21:30.145569 themule-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 18:21:20.000000 themule-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:21:30.145569 themule-0.1.2/themule/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 18:21:22.000000 themule-0.1.2/themule/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 18:21:20.000000 themule-0.1.2/themule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 18:21:20.000000 themule-0.1.2/themule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 18:21:20.000000 themule-0.1.2/themule/boto_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-13 18:21:20.000000 themule-0.1.2/themule/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 18:21:20.000000 themule-0.1.2/themule/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 18:21:20.000000 themule-0.1.2/themule/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 18:21:20.000000 themule-0.1.2/themule/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-13 18:21:20.000000 themule-0.1.2/themule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 18:21:20.000000 themule-0.1.2/themule/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:21:30.145569 themule-0.1.2/themule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:21:29.000000 themule-0.1.2/themule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 18:21:30.000000 themule-0.1.2/themule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.644984 themule-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 21:25:04.000000 themule-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 21:25:14.640984 themule-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 21:25:04.000000 themule-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 21:25:04.000000 themule-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:25:14.644984 themule-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 21:25:04.000000 themule-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/themule/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:25:07.000000 themule-0.1.3/themule/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 21:25:04.000000 themule-0.1.3/themule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 21:25:04.000000 themule-0.1.3/themule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 21:25:04.000000 themule-0.1.3/themule/boto_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:25:04.000000 themule-0.1.3/themule/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:25:04.000000 themule-0.1.3/themule/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 21:25:04.000000 themule-0.1.3/themule/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 21:25:04.000000 themule-0.1.3/themule/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-13 21:25:04.000000 themule-0.1.3/themule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 21:25:04.000000 themule-0.1.3/themule/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/themule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/top_level.txt
```

### Comparing `themule-0.1.2/PKG-INFO` & `themule-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themule
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Mule - run arbitrary python function on AWS Batch
 Home-page: http://github.com/wlatanowicz/themule
 Author: Wiktor Latanowicz
 Author-email: wiktor@latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `themule-0.1.2/setup.py` & `themule-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.2/themule/boto_client.py` & `themule-0.1.3/themule/boto_client.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.2/themule/cli.py` & `themule-0.1.3/themule/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,30 @@
 
 @click.group()
 def cli():
     pass
 
 
 @cli.command("execute-job")
-@click.option("-s", "--serializer", "serializer_path", type=str, help="Path to serializer's class")
+@click.option(
+    "-s",
+    "--serializer",
+    "serializer_path",
+    type=str,
+    help="Path to serializer's class",
+)
 @click.argument("job-spec", type=str)
 def execute_job_cli(serializer_path, job_spec):
+    setup = os.environ.get("THEMULE_SETUP_CALLBACK")
+    if setup:
+        setup_func = import_by_path(setup)
+        setup_func()
+
     if not serializer_path:
         serializer_path = os.environ.get(
             "THEMULE_JOB_SERIALIZER", default=DEFAULT_SERIALIZER
         )
     serializer_class: Type[BaseSerializer] = import_by_path(serializer_path)
     serializer = serializer_class()
     job = serializer.unserialize(job_spec)
+
     execute_job(job)
```

### Comparing `themule-0.1.2/themule/job.py` & `themule-0.1.3/themule/job.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.2/themule/serializers.py` & `themule-0.1.3/themule/serializers.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.2/themule.egg-info/PKG-INFO` & `themule-0.1.3/themule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themule
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Mule - run arbitrary python function on AWS Batch
 Home-page: http://github.com/wlatanowicz/themule
 Author: Wiktor Latanowicz
 Author-email: wiktor@latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `themule-0.1.2/themule.egg-info/SOURCES.txt` & `themule-0.1.3/themule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

