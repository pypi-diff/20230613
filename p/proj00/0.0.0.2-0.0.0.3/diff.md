# Comparing `tmp/proj00-0.0.0.2-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 1549 bytes, number of entries: 6
+Zip file size: 3497 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     3170 b- defN 23-Jun-13 00:12 proj00/baek.py
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-12 08:53 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
--rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test2.py
--rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-12 08:44 proj00-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:44 proj00-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-12 08:44 proj00-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      441 b- defN 23-Jun-12 08:44 proj00-0.0.0.2.dist-info/RECORD
-6 files, 957 bytes uncompressed, 747 bytes compressed:  21.9%
+-rw-rw-rw-  2.0 fat      179 b- defN 23-Jun-13 00:11 proj00/test2.py
+-rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/RECORD
+8 files, 4671 bytes uncompressed, 2489 bytes compressed:  46.7%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
+Filename: proj00/baek.py
+Comment: 
+
+Filename: proj00/bmi.py
+Comment: 
+
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.2.dist-info/METADATA
+Filename: proj00-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.2.dist-info/WHEEL
+Filename: proj00-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.2.dist-info/top_level.txt
+Filename: proj00-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.2.dist-info/RECORD
+Filename: proj00-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/test2.py

```diff
@@ -1,3 +1,9 @@
 def print_test2():
     '''테스트 문장을 출력합니다.'''
-    print('Hi, This is Test2')
+    print('Hi, This is Test2')
+
+from proj00 import test1, test2
+
+test1.print_test1()
+
+test2.print_test2()
```

