# Comparing `tmp/example_wise_f1_maximizer-0.1.1-py3-none-any.whl.zip` & `tmp/example_wise_f1_maximizer-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7834 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer/__init__.py
--rw-r--r--  2.0 unx    11802 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer/example_wise_f1_maximizer.py
--rw-r--r--  2.0 unx     6574 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      677 b- defN 23-Jun-13 14:41 example_wise_f1_maximizer-0.1.1.dist-info/RECORD
-7 files, 19172 bytes uncompressed, 6598 bytes compressed:  65.6%
+Zip file size: 7890 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer/__init__.py
+-rw-r--r--  2.0 unx    11802 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer/example_wise_f1_maximizer.py
+-rw-r--r--  2.0 unx     6574 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer-0.1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer-0.1.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      678 b- defN 23-Jun-13 14:48 example_wise_f1_maximizer-0.1.2.dist-info/RECORD
+7 files, 19234 bytes uncompressed, 6654 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: example_wise_f1_maximizer/__init__.py
 Comment: 
 
 Filename: example_wise_f1_maximizer/example_wise_f1_maximizer.py
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.1.dist-info/METADATA
+Filename: example_wise_f1_maximizer-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.1.dist-info/WHEEL
+Filename: example_wise_f1_maximizer-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.1.dist-info/top_level.txt
+Filename: example_wise_f1_maximizer-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.1.dist-info/zip-safe
+Filename: example_wise_f1_maximizer-0.1.2.dist-info/zip-safe
 Comment: 
 
-Filename: example_wise_f1_maximizer-0.1.1.dist-info/RECORD
+Filename: example_wise_f1_maximizer-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## example_wise_f1_maximizer/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 2065 7861 6d70 6c65 5f77 6973  from example_wis
+00000010: 655f 6631 5f6d 6178 696d 697a 6572 2069  e_f1_maximizer i
+00000020: 6d70 6f72 7420 4578 616d 706c 6557 6973  mport ExampleWis
+00000030: 6546 314d 6178 696d 697a 6572 0a         eF1Maximizer.
```

## Comparing `example_wise_f1_maximizer-0.1.1.dist-info/METADATA` & `example_wise_f1_maximizer-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-wise-f1-maximizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A scikit-learn meta-estimator for multi-label classification that aims to maximize the example-wise F1 measure
 Home-page: https://github.com/mrapp-ke/ExampleWiseF1Maximizer
 Download-URL: https://github.com/mrapp-ke/ExampleWiseF1Maximizer/releases
 Author: Michael Rapp
 Author-email: michael.rapp.ml@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/mrapp-ke/ExampleWiseF1Maximizer/issues
```

## Comparing `example_wise_f1_maximizer-0.1.1.dist-info/RECORD` & `example_wise_f1_maximizer-0.1.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-example_wise_f1_maximizer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+example_wise_f1_maximizer/__init__.py,sha256=WwOW1pGPtu8sBAncu7jt9oowVxHNKZqtoqRVaaMB_dk,61
 example_wise_f1_maximizer/example_wise_f1_maximizer.py,sha256=n2a56fwEW3WdJoSFxNs4LhKI3hEjd3ajW8NacXx4a1w,11802
-example_wise_f1_maximizer-0.1.1.dist-info/METADATA,sha256=yDNUpGDagfeC4PEE3B2CM20j7E_Gf95UMrgyOJBmoMc,6574
-example_wise_f1_maximizer-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-example_wise_f1_maximizer-0.1.1.dist-info/top_level.txt,sha256=Y3_hRTvgv8_1Vtj4I0HcBsiANUAJuFfeC2v0x06eRqo,26
-example_wise_f1_maximizer-0.1.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-example_wise_f1_maximizer-0.1.1.dist-info/RECORD,,
+example_wise_f1_maximizer-0.1.2.dist-info/METADATA,sha256=vlaEFlcYgJxXyJO5HXvvM6ekJS-R-cFWGvcR3kCj55E,6574
+example_wise_f1_maximizer-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+example_wise_f1_maximizer-0.1.2.dist-info/top_level.txt,sha256=Y3_hRTvgv8_1Vtj4I0HcBsiANUAJuFfeC2v0x06eRqo,26
+example_wise_f1_maximizer-0.1.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+example_wise_f1_maximizer-0.1.2.dist-info/RECORD,,
```

