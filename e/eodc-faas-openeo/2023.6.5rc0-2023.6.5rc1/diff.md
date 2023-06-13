# Comparing `tmp/eodc_faas_openeo-2023.6.5rc0.tar.gz` & `tmp/eodc_faas_openeo-2023.6.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_openeo-2023.6.5rc0.tar", max compression
+gzip compressed data, was "eodc_faas_openeo-2023.6.5rc1.tar", max compression
```

## Comparing `eodc_faas_openeo-2023.6.5rc0.tar` & `eodc_faas_openeo-2023.6.5rc1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       11 2023-06-11 06:50:07.525102 eodc_faas_openeo-2023.6.5rc0/README.md
--rw-r--r--   0        0        0      107 2023-06-11 07:04:15.038030 eodc_faas_openeo-2023.6.5rc0/openeo_executor_bindings/__init__.py
--rw-r--r--   0        0        0      272 2023-06-11 06:50:07.525102 eodc_faas_openeo-2023.6.5rc0/openeo_executor_bindings/model.py
--rw-r--r--   0        0        0     4827 2023-06-11 06:50:07.525102 eodc_faas_openeo-2023.6.5rc0/openeo_executor_bindings/workflow.py
--rw-r--r--   0        0        0      699 2023-06-11 07:04:19.403862 eodc_faas_openeo-2023.6.5rc0/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.5rc0/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/README.md
+-rw-r--r--   0        0        0      107 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/__init__.py
+-rw-r--r--   0        0        0      272 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/model.py
+-rw-r--r--   0        0        0     4827 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/workflow.py
+-rw-r--r--   0        0        0      699 2023-06-13 15:22:25.655253 eodc_faas_openeo-2023.6.5rc1/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 eodc_faas_openeo-2023.6.5rc1/PKG-INFO
```

### Comparing `eodc_faas_openeo-2023.6.5rc0/openeo_executor_bindings/workflow.py` & `eodc_faas_openeo-2023.6.5rc1/openeo_executor_bindings/workflow.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_openeo-2023.6.5rc0/PKG-INFO` & `eodc_faas_openeo-2023.6.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-openeo
-Version: 2023.6.5rc0
+Version: 2023.6.5rc1
 Summary: Bindings for the OpenEO processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

