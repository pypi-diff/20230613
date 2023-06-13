# Comparing `tmp/yoTestfile01-0.0.0.1-py3-none-any.whl.zip` & `tmp/yoTestfile01-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1722 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      117 b- defN 23-Jun-12 08:14 yoTestfile01/test1.py
--rw-rw-rw-  2.0 fat      138 b- defN 23-Jun-12 08:19 yoTestfile01/test2.py
--rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-12 08:25 yoTestfile01-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:25 yoTestfile01-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-12 08:25 yoTestfile01-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      479 b- defN 23-Jun-12 08:25 yoTestfile01-0.0.0.1.dist-info/RECORD
-6 files, 1097 bytes uncompressed, 848 bytes compressed:  22.7%
+Zip file size: 1746 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-13 00:16 yoTestfile01/test1.py
+-rw-rw-rw-  2.0 fat      151 b- defN 23-Jun-13 00:16 yoTestfile01/test2.py
+-rw-rw-rw-  2.0 fat      241 b- defN 23-Jun-13 00:20 yoTestfile01-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:20 yoTestfile01-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-13 00:20 yoTestfile01-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      479 b- defN 23-Jun-13 00:20 yoTestfile01-0.0.0.2.dist-info/RECORD
+6 files, 1124 bytes uncompressed, 872 bytes compressed:  22.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: yoTestfile01/test1.py
 Comment: 
 
 Filename: yoTestfile01/test2.py
 Comment: 
 
-Filename: yoTestfile01-0.0.0.1.dist-info/METADATA
+Filename: yoTestfile01-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: yoTestfile01-0.0.0.1.dist-info/WHEEL
+Filename: yoTestfile01-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: yoTestfile01-0.0.0.1.dist-info/top_level.txt
+Filename: yoTestfile01-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: yoTestfile01-0.0.0.1.dist-info/RECORD
+Filename: yoTestfile01-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yoTestfile01/test1.py

```diff
@@ -1,3 +1,3 @@
 def print_test() :
     '''테스트 문장을 출력하는 것입니다.'''
-    print("Hi, This is test1.py page!")
+    print("Hi, This is test1.py page. good morning!")
```

## yoTestfile01/test2.py

```diff
@@ -1,3 +1,3 @@
 def print_test2() :
     '''테스트 문장을 출력합니다'''
-    print("안녕하세요, 이것은 test2.py 페이지입니다.")
+    print("안녕하세요, 이것은 test2.py 페이지입니다. 환영해요")
```

