# Comparing `tmp/pyp8s-3.2.0-py3-none-any.whl.zip` & `tmp/pyp8s-3.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19299 bytes, number of entries: 10
--rw-r--r--  2.0 unx      298 b- defN 23-Jun-11 02:56 pyp8s/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-Jun-11 02:56 pyp8s/_version.py
--rw-r--r--  2.0 unx    11751 b- defN 23-Jun-11 02:56 pyp8s/metrics.py
--rw-r--r--  2.0 unx      226 b- defN 23-Jun-11 02:56 tests/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 23-Jun-11 02:56 tests/test_import.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2937 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 23-Jun-11 02:56 pyp8s-3.2.0.dist-info/RECORD
-10 files, 52762 bytes uncompressed, 18045 bytes compressed:  65.8%
+Zip file size: 19296 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      298 b- defN 23-Jun-12 22:20 pyp8s/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-12 22:20 pyp8s/_version.py
+-rw-r--r--  2.0 unx    11753 b- defN 23-Jun-12 22:20 pyp8s/metrics.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-12 22:20 tests/__init__.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-Jun-12 22:20 tests/test_import.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2935 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 23-Jun-12 22:20 pyp8s-3.2.1.dist-info/RECORD
+10 files, 52762 bytes uncompressed, 18042 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_import.py
 Comment: 
 
-Filename: pyp8s-3.2.0.dist-info/LICENSE
+Filename: pyp8s-3.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyp8s-3.2.0.dist-info/METADATA
+Filename: pyp8s-3.2.1.dist-info/METADATA
 Comment: 
 
-Filename: pyp8s-3.2.0.dist-info/WHEEL
+Filename: pyp8s-3.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyp8s-3.2.0.dist-info/top_level.txt
+Filename: pyp8s-3.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyp8s-3.2.0.dist-info/RECORD
+Filename: pyp8s-3.2.1.dist-info/RECORD
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
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
```

## pyp8s/metrics.py

```diff
@@ -210,15 +210,15 @@
             for _, labelset in metric_item.get_labelsets().items():
                 metric_value = labelset['value']
                 metric_labels_formatted_joined = ",".join(labelset['labels_formatted'])
 
                 metric_line = f"""{metric_name}{{{metric_labels_formatted_joined}}} {metric_value}\n"""
                 result.append(metric_line)
 
-        return "".join(result)
+        return "\n".join(result)
 
     @staticmethod
     def get_metrics():
         self = MetricsHandler()
         return self.metrics
 
     @staticmethod
```

## Comparing `pyp8s-3.2.0.dist-info/LICENSE` & `pyp8s-3.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyp8s-3.2.0.dist-info/METADATA` & `pyp8s-3.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp8s
-Version: 3.2.0
+Version: 3.2.1
 Summary: Customisable prometheus exporter for your python application
 Home-page: https://github.com/pyp8s/pyp8s
 Author: Pavel Kim
 Author-email: hello@pavelkim.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -78,15 +78,15 @@
 yawns{satisfying="yes"} 8
 yawns{satisfying="no",loud="yes"} 1
 # HELP mood How do I feel myself from 1 to good enough
 # TYPE mood gauge
 mood{} 6
 # HELP giggles Measurement of the joke power.
 # TYPE giggles counter
-giggles{} -50
+giggles{} 0
 ```
 
 ## Usage without starting a server
 
 When you only need this thing to collect and render metrics:
 
 ```python
```

