# Comparing `tmp/seq-json-schema-1.0.8.tar.gz` & `tmp/seq-json-schema-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seq-json-schema-1.0.8.tar", last modified: Mon Jan 23 19:22:41 2023, max compression
+gzip compressed data, was "seq-json-schema-1.0.9.tar", last modified: Tue Jan 24 16:44:02 2023, max compression
```

## Comparing `seq-json-schema-1.0.8.tar` & `seq-json-schema-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ccamargo   (502) staff       (20)        0 2023-01-23 19:22:41.696552 seq-json-schema-1.0.8/
--rw-r--r--   0 ccamargo   (502) staff       (20)     1074 2023-01-19 04:38:09.000000 seq-json-schema-1.0.8/LICENSE
--rw-r--r--   0 ccamargo   (502) staff       (20)       36 2023-01-19 04:34:48.000000 seq-json-schema-1.0.8/MANIFEST.in
--rw-r--r--   0 ccamargo   (502) staff       (20)     1181 2023-01-23 19:22:41.696247 seq-json-schema-1.0.8/PKG-INFO
--rw-r--r--   0 ccamargo   (502) staff       (20)      865 2023-01-19 17:56:16.000000 seq-json-schema-1.0.8/README.md
-drwxr-xr-x   0 ccamargo   (502) staff       (20)        0 2023-01-23 19:22:41.693995 seq-json-schema-1.0.8/seq-json-schema/
--rw-r--r--   0 ccamargo   (502) staff       (20)        0 2020-08-24 22:14:55.000000 seq-json-schema-1.0.8/seq-json-schema/__init__.py
--rw-r--r--   0 ccamargo   (502) staff       (20)    16375 2023-01-23 19:19:36.000000 seq-json-schema-1.0.8/seq-json-schema/schema.json
-drwxr-xr-x   0 ccamargo   (502) staff       (20)        0 2023-01-23 19:22:41.695746 seq-json-schema-1.0.8/seq_json_schema.egg-info/
--rw-r--r--   0 ccamargo   (502) staff       (20)     1181 2023-01-23 19:22:41.000000 seq-json-schema-1.0.8/seq_json_schema.egg-info/PKG-INFO
--rw-r--r--   0 ccamargo   (502) staff       (20)      250 2023-01-23 19:22:41.000000 seq-json-schema-1.0.8/seq_json_schema.egg-info/SOURCES.txt
--rw-r--r--   0 ccamargo   (502) staff       (20)        1 2023-01-23 19:22:41.000000 seq-json-schema-1.0.8/seq_json_schema.egg-info/dependency_links.txt
--rw-r--r--   0 ccamargo   (502) staff       (20)       16 2023-01-23 19:22:41.000000 seq-json-schema-1.0.8/seq_json_schema.egg-info/top_level.txt
--rw-r--r--   0 ccamargo   (502) staff       (20)       38 2023-01-23 19:22:41.696642 seq-json-schema-1.0.8/setup.cfg
--rw-r--r--   0 ccamargo   (502) staff       (20)      565 2023-01-23 19:22:15.000000 seq-json-schema-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:44:02.139035 seq-json-schema-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-01-24 16:44:02.139035 seq-json-schema-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:44:02.139035 seq-json-schema-1.0.9/seq-json-schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/seq-json-schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/seq-json-schema/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:44:02.139035 seq-json-schema-1.0.9/seq_json_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-01-24 16:44:02.000000 seq-json-schema-1.0.9/seq_json_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-24 16:44:02.000000 seq-json-schema-1.0.9/seq_json_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 16:44:02.000000 seq-json-schema-1.0.9/seq_json_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 16:44:02.000000 seq-json-schema-1.0.9/seq_json_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 16:44:02.139035 seq-json-schema-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-24 16:44:01.000000 seq-json-schema-1.0.9/setup.py
```

### Comparing `seq-json-schema-1.0.8/LICENSE` & `seq-json-schema-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seq-json-schema-1.0.8/seq-json-schema/schema.json` & `seq-json-schema-1.0.9/seq-json-schema/schema.json`

 * *Files identical despite different names*

### Comparing `seq-json-schema-1.0.8/setup.py` & `seq-json-schema-1.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from setuptools import setup
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / 'README.md').read_text()
 
 setup(
   author='camargo',
   author_email='Christopher.A.Camargo@jpl.nasa.gov',
   description='Standardized JSON Schema for authoring multi-mission sequences',
   include_package_data=True,
   long_description=long_description,
   long_description_content_type='text/markdown',
   name='seq-json-schema',
   packages=['seq-json-schema'],
   url='https://github.com/NASA-AMMOS/seq-json-schema',
-  version='1.0.8'
+  version='1.0.9'
 )
```

