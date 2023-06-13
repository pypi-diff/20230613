# Comparing `tmp/mypackagelicenseprototype-3.0.1-py3-none-any.whl.zip` & `tmp/mypackagelicenseprototype-3.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5274 bytes, number of entries: 7
+Zip file size: 256401 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx     5455 b- defN 23-Jun-13 07:44 parent/PackageContent.py
 -rw-rw-r--  2.0 unx     1364 b- defN 23-Jun-13 07:44 parent/__init__.py
 -rw-rw-r--  2.0 unx      101 b- defN 23-Jun-13 07:44 parent/pyarmor_runtime_000000/__init__.py
--rw-rw-r--  2.0 unx       91 b- defN 23-Jun-13 07:51 mypackagelicenseprototype-3.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 07:51 mypackagelicenseprototype-3.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-13 07:51 mypackagelicenseprototype-3.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      620 b- defN 23-Jun-13 07:51 mypackagelicenseprototype-3.0.1.dist-info/RECORD
-7 files, 7730 bytes uncompressed, 4154 bytes compressed:  46.3%
+-rwxrwxr-x  2.0 unx   788232 b- defN 23-Jun-13 07:44 parent/pyarmor_runtime_000000/pyarmor_runtime.so
+-rw-rw-r--  2.0 unx      112 b- defN 23-Jun-13 08:05 mypackagelicenseprototype-3.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 08:05 mypackagelicenseprototype-3.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-13 08:05 mypackagelicenseprototype-3.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      728 b- defN 23-Jun-13 08:05 mypackagelicenseprototype-3.0.2.dist-info/RECORD
+8 files, 796091 bytes uncompressed, 255109 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: parent/__init__.py
 Comment: 
 
 Filename: parent/pyarmor_runtime_000000/__init__.py
 Comment: 
 
-Filename: mypackagelicenseprototype-3.0.1.dist-info/METADATA
+Filename: parent/pyarmor_runtime_000000/pyarmor_runtime.so
 Comment: 
 
-Filename: mypackagelicenseprototype-3.0.1.dist-info/WHEEL
+Filename: mypackagelicenseprototype-3.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mypackagelicenseprototype-3.0.1.dist-info/top_level.txt
+Filename: mypackagelicenseprototype-3.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mypackagelicenseprototype-3.0.1.dist-info/RECORD
+Filename: mypackagelicenseprototype-3.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: mypackagelicenseprototype-3.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

