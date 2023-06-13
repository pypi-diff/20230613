# Comparing `tmp/kkw2401_bmi-0.0.0.1-py3-none-any.whl.zip` & `tmp/kkw2401_bmi-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1912 bytes, number of entries: 6
+Zip file size: 1811 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      549 b- defN 23-Jun-13 00:52 kkw2401_bmi/bmi_class.py
--rw-rw-rw-  2.0 fat      394 b- defN 23-Jun-13 00:54 kkw2401_bmi/bmi_module.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-Jun-13 00:55 kkw2401_bmi-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 00:55 kkw2401_bmi-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-13 00:55 kkw2401_bmi-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      482 b- defN 23-Jun-13 00:55 kkw2401_bmi-0.0.0.1.dist-info/RECORD
-6 files, 1776 bytes uncompressed, 1032 bytes compressed:  41.9%
+-rw-rw-rw-  2.0 fat      162 b- defN 23-Jun-13 01:02 kkw2401_bmi/bmi_module.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-Jun-13 01:03 kkw2401_bmi-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 01:03 kkw2401_bmi-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-13 01:03 kkw2401_bmi-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      482 b- defN 23-Jun-13 01:03 kkw2401_bmi-0.0.0.2.dist-info/RECORD
+6 files, 1544 bytes uncompressed, 931 bytes compressed:  39.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kkw2401_bmi/bmi_class.py
 Comment: 
 
 Filename: kkw2401_bmi/bmi_module.py
 Comment: 
 
-Filename: kkw2401_bmi-0.0.0.1.dist-info/METADATA
+Filename: kkw2401_bmi-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: kkw2401_bmi-0.0.0.1.dist-info/WHEEL
+Filename: kkw2401_bmi-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: kkw2401_bmi-0.0.0.1.dist-info/top_level.txt
+Filename: kkw2401_bmi-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kkw2401_bmi-0.0.0.1.dist-info/RECORD
+Filename: kkw2401_bmi-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kkw2401_bmi/bmi_module.py

```diff
@@ -1,15 +1,5 @@
+import bmi_class
 def bmi_input():
-    weight = int(input())
-    height = int(input())
-    return round(weight/(height*height)*10000, 2)
-def bmi_text(x):
-    result = ""
-    if x > 25.0:
-        result = "비만"
-    elif x > 23.0 and x < 24.9:
-        result = "과체중"
-    elif x > 18.5 and x < 22.9:
-        result = "정상"
-    elif x < 18.5:
-        result =  "저체중"
-    return result
+    x = bmi_class.bmi_class.bmi_calcula1tor(int(input()), int(input()))
+    y = bmi_class.bmi_class.bmi_text(x)
+    return y
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

