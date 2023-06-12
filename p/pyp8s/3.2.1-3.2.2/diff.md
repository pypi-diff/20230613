# Comparing `tmp/pyp8s-3.2.1-py3-none-any.whl.zip` & `tmp/pyp8s-3.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19296 bytes, number of entries: 10
--rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 22:20 pyp8s/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-Jun-12 22:20 pyp8s/_version.py
--rw-r--r--  2.0 unx    11753 b- defN 23-Jun-12 22:20 pyp8s/metrics.py
--rw-r--r--  2.0 unx      226 b- defN 23-Jun-12 22:20 tests/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 23-Jun-12 22:20 tests/test_import.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2935 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/RECORD
-10 files, 52762 bytes uncompressed, 18042 bytes compressed:  65.8%
+Zip file size: 19297 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 22:34 pyp8s/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-12 22:34 pyp8s/_version.py
+-rw-r--r--  2.0 unx    11747 b- defN 23-Jun-12 22:34 pyp8s/metrics.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-12 22:34 tests/__init__.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-Jun-12 22:34 tests/test_import.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-12 22:35 pyp8s-3.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2935 b- defN 23-Jun-12 22:35 pyp8s-3.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 22:35 pyp8s-3.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 22:35 pyp8s-3.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 23-Jun-12 22:35 pyp8s-3.2.2.dist-info/RECORD
+10 files, 52756 bytes uncompressed, 18043 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_import.py
 Comment: 
 
-Filename: pyp8s-3.2.1.dist-info/LICENSE
+Filename: pyp8s-3.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyp8s-3.2.1.dist-info/METADATA
+Filename: pyp8s-3.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pyp8s-3.2.1.dist-info/WHEEL
+Filename: pyp8s-3.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyp8s-3.2.1.dist-info/top_level.txt
+Filename: pyp8s-3.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyp8s-3.2.1.dist-info/RECORD
+Filename: pyp8s-3.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyp8s/_version.py

```diff
@@ -1,8 +1,8 @@
 #!/usr/bin/env python3
 # pylint: disable=line-too-long, missing-function-docstring, logging-fstring-interpolation
 # pylint: disable=too-many-locals, broad-except, too-many-arguments, raise-missing-from
 """
     pyp8s module
 """
 
-__version__ = "3.2.1"
+__version__ = "3.2.2"
```

## pyp8s/metrics.py

```diff
@@ -197,25 +197,25 @@
 
     @staticmethod
     def render():
         self = MetricsHandler()
         result = []
         for metric_name, metric_item in self.get_metrics().items():
 
-            help_header = f"""# HELP {metric_name} {metric_item.get_help()}\n"""
+            help_header = f"""# HELP {metric_name} {metric_item.get_help()}"""
             result.append(help_header)
 
-            type_header = f"""# TYPE {metric_name} {metric_item.get_type()}\n"""
+            type_header = f"""# TYPE {metric_name} {metric_item.get_type()}"""
             result.append(type_header)
 
             for _, labelset in metric_item.get_labelsets().items():
                 metric_value = labelset['value']
                 metric_labels_formatted_joined = ",".join(labelset['labels_formatted'])
 
-                metric_line = f"""{metric_name}{{{metric_labels_formatted_joined}}} {metric_value}\n"""
+                metric_line = f"""{metric_name}{{{metric_labels_formatted_joined}}} {metric_value}"""
                 result.append(metric_line)
 
         return "\n".join(result)
 
     @staticmethod
     def get_metrics():
         self = MetricsHandler()
```

## Comparing `pyp8s-3.2.1.dist-info/LICENSE` & `pyp8s-3.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyp8s-3.2.1.dist-info/METADATA` & `pyp8s-3.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp8s
-Version: 3.2.1
+Version: 3.2.2
 Summary: Customisable prometheus exporter for your python application
 Home-page: https://github.com/pyp8s/pyp8s
 Author: Pavel Kim
 Author-email: hello@pavelkim.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

