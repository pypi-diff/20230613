# Comparing `tmp/themule-0.1.0.tar.gz` & `tmp/themule-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themule-0.1.0.tar", last modified: Mon Jun 12 19:39:27 2023, max compression
+gzip compressed data, was "themule-0.1.1.tar", last modified: Tue Jun 13 12:47:10 2023, max compression
```

## Comparing `themule-0.1.0.tar` & `themule-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:27.186340 themule-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 19:39:09.000000 themule-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-12 19:39:27.186340 themule-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 19:39:09.000000 themule-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 19:39:09.000000 themule-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:27.182340 themule-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 19:39:09.000000 themule-0.1.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 19:39:09.000000 themule-0.1.0/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:09.000000 themule-0.1.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:39:27.186340 themule-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-12 19:39:09.000000 themule-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:27.186340 themule-0.1.0/themule/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:39:15.000000 themule-0.1.0/themule/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 19:39:09.000000 themule-0.1.0/themule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 19:39:09.000000 themule-0.1.0/themule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-12 19:39:09.000000 themule-0.1.0/themule/boto_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-12 19:39:09.000000 themule-0.1.0/themule/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 19:39:09.000000 themule-0.1.0/themule/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-12 19:39:09.000000 themule-0.1.0/themule/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 19:39:09.000000 themule-0.1.0/themule/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-12 19:39:09.000000 themule-0.1.0/themule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 19:39:09.000000 themule-0.1.0/themule/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:27.186340 themule-0.1.0/themule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:39:26.000000 themule-0.1.0/themule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 19:39:27.000000 themule-0.1.0/themule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:47:10.313370 themule-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 12:47:00.000000 themule-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 12:47:10.313370 themule-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 12:47:00.000000 themule-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 12:47:00.000000 themule-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:47:10.313370 themule-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 12:47:00.000000 themule-0.1.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 12:47:00.000000 themule-0.1.1/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:47:00.000000 themule-0.1.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:47:10.313370 themule-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 12:47:00.000000 themule-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:47:10.313370 themule-0.1.1/themule/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 12:47:03.000000 themule-0.1.1/themule/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 12:47:00.000000 themule-0.1.1/themule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 12:47:00.000000 themule-0.1.1/themule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 12:47:00.000000 themule-0.1.1/themule/boto_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 12:47:00.000000 themule-0.1.1/themule/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 12:47:00.000000 themule-0.1.1/themule/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 12:47:00.000000 themule-0.1.1/themule/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 12:47:00.000000 themule-0.1.1/themule/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-13 12:47:00.000000 themule-0.1.1/themule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 12:47:00.000000 themule-0.1.1/themule/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:47:10.313370 themule-0.1.1/themule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 12:47:10.000000 themule-0.1.1/themule.egg-info/top_level.txt
```

### Comparing `themule-0.1.0/PKG-INFO` & `themule-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themule
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Mule - run arbitrary python function on AWS Batch
 Home-page: http://github.com/wlatanowicz/themule
 Author: Wiktor Latanowicz
 Author-email: wiktor@latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `themule-0.1.0/setup.py` & `themule-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.0/themule/boto_client.py` & `themule-0.1.1/themule/boto_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
         self.client.submit_job(
             jobName=str(job.id),
             jobQueue=queue_name,
             jobDefinition=job_definition,
             containerOverrides={
                 "command": [
                     "themule",
-                    "executejob",
+                    "execute-job",
                     "--serializer",
                     serializer.get_path(),
                     serialized_job,
                 ],
             },
         )
```

### Comparing `themule-0.1.0/themule/cli.py` & `themule-0.1.1/themule/cli.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.0/themule/job.py` & `themule-0.1.1/themule/job.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.0/themule/serializers.py` & `themule-0.1.1/themule/serializers.py`

 * *Files identical despite different names*

### Comparing `themule-0.1.0/themule.egg-info/PKG-INFO` & `themule-0.1.1/themule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themule
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Mule - run arbitrary python function on AWS Batch
 Home-page: http://github.com/wlatanowicz/themule
 Author: Wiktor Latanowicz
 Author-email: wiktor@latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `themule-0.1.0/themule.egg-info/SOURCES.txt` & `themule-0.1.1/themule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

