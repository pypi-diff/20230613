# Comparing `tmp/example_wise_f1_maximizer-0.1.0-py3-none-any.whl.zip` & `tmp/example_wise_f1_maximizer-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 4028 bytes, number of entries: 5
--rw-r--r--  2.0 unx     6574 b- defN 23-Jun-13 14:16 example_wise_f1_maximizer-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:16 example_wise_f1_maximizer-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:16 example_wise_f1_maximizer-0.1.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:16 example_wise_f1_maximizer-0.1.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx      473 b- defN 23-Jun-13 14:16 example_wise_f1_maximizer-0.1.0.dist-info/RECORD
-5 files, 7141 bytes uncompressed, 3126 bytes compressed:  56.2%
+Zip file size: 7834 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer/__init__.py
+-rw-r--r--  2.0 unx    11802 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer/example_wise_f1_maximizer.py
+-rw-r--r--  2.0 unx     6574 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      677 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/RECORD
+7 files, 19172 bytes uncompressed, 6598 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: example_wise_f1_maximizer-0.1.0.dist-info/METADATA
+Filename: example_wise_f1_maximizer/__init__.py
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.0.dist-info/WHEEL
+Filename: example_wise_f1_maximizer/example_wise_f1_maximizer.py
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.0.dist-info/top_level.txt
+Filename: example_wise_f1_maximizer-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.0.dist-info/zip-safe
+Filename: example_wise_f1_maximizer-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.0.dist-info/RECORD
+Filename: example_wise_f1_maximizer-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: example_wise_f1_maximizer-0.1.1.dist-info/zip-safe
+Comment: 
+
+Filename: example_wise_f1_maximizer-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `example_wise_f1_maximizer-0.1.0.dist-info/METADATA` & `example_wise_f1_maximizer-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-wise-f1-maximizer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A scikit-learn meta-estimator for multi-label classification that aims to maximize the example-wise F1 measure
 Home-page: https://github.com/mrapp-ke/ExampleWiseF1Maximizer
 Download-URL: https://github.com/mrapp-ke/ExampleWiseF1Maximizer/releases
 Author: Michael Rapp
 Author-email: michael.rapp.ml@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/mrapp-ke/ExampleWiseF1Maximizer/issues
```

