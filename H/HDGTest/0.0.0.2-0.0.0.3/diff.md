# Comparing `tmp/HDGTest-0.0.0.2-py3-none-any.whl.zip` & `tmp/HDGTest-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1602 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      109 b- defN 23-Jun-13 00:18 HDGTest/test1.py
--rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-13 00:18 HDGTest/test2.py
--rw-rw-rw-  2.0 fat      220 b- defN 23-Jun-13 00:19 HDGTest-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:19 HDGTest-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-13 00:19 HDGTest-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      449 b- defN 23-Jun-13 00:19 HDGTest-0.0.0.2.dist-info/RECORD
-6 files, 1031 bytes uncompressed, 788 bytes compressed:  23.6%
+Zip file size: 1648 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      161 b- defN 23-Jun-13 01:30 HDGTest/test1.py
+-rw-rw-rw-  2.0 fat      191 b- defN 23-Jun-13 01:30 HDGTest/test2.py
+-rw-rw-rw-  2.0 fat      220 b- defN 23-Jun-13 01:31 HDGTest-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 01:31 HDGTest-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jun-13 01:31 HDGTest-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      449 b- defN 23-Jun-13 01:31 HDGTest-0.0.0.3.dist-info/RECORD
+6 files, 1138 bytes uncompressed, 834 bytes compressed:  26.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: HDGTest/test1.py
 Comment: 
 
 Filename: HDGTest/test2.py
 Comment: 
 
-Filename: HDGTest-0.0.0.2.dist-info/METADATA
+Filename: HDGTest-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: HDGTest-0.0.0.2.dist-info/WHEEL
+Filename: HDGTest-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: HDGTest-0.0.0.2.dist-info/top_level.txt
+Filename: HDGTest-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: HDGTest-0.0.0.2.dist-info/RECORD
+Filename: HDGTest-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HDGTest/test1.py

```diff
@@ -1,4 +1,5 @@
 def print_test1():
 
     print("Hi, This is test1.py page!")
-    print("\n 버전 업글 엽습입니다.")
+    print("\n 버전 업글 연습입니다.")
+    print("\n BMI 를 만들어 보았습니다.")
```

## HDGTest/test2.py

```diff
@@ -1,4 +1,5 @@
 def print_test2():
 
-    print("안녕하세요, 이것은 test2.py 페이지입니다")
-    print("\n 잘됬으면 좋겠습니다.")
+    print("안녕하세요, 이것은 test2.py 페이지입니다.")
+    print("\n 잘됬으면 좋겠습니다.")
+    print("\n 오류만 안뜨면 좋겠습니다.")
```

