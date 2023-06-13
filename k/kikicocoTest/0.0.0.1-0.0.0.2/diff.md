# Comparing `tmp/kikicocoTest-0.0.0.1-py3-none-any.whl.zip` & `tmp/kikicocoTest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1691 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      106 b- defN 23-Jun-12 07:48 kikicocoTest/test1.py
--rw-rw-rw-  2.0 fat      135 b- defN 23-Jun-12 07:49 kikicocoTest/test2.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-Jun-12 08:58 kikicocoTest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:58 kikicocoTest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-12 08:58 kikicocoTest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      479 b- defN 23-Jun-12 08:58 kikicocoTest-0.0.0.1.dist-info/RECORD
-6 files, 1068 bytes uncompressed, 817 bytes compressed:  23.5%
+Zip file size: 1701 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      114 b- defN 23-Jun-13 00:15 kikicocoTest/test1.py
+-rw-rw-rw-  2.0 fat      143 b- defN 23-Jun-13 00:15 kikicocoTest/test2.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-Jun-13 00:16 kikicocoTest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:16 kikicocoTest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-13 00:16 kikicocoTest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      479 b- defN 23-Jun-13 00:16 kikicocoTest-0.0.0.2.dist-info/RECORD
+6 files, 1084 bytes uncompressed, 827 bytes compressed:  23.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kikicocoTest/test1.py
 Comment: 
 
 Filename: kikicocoTest/test2.py
 Comment: 
 
-Filename: kikicocoTest-0.0.0.1.dist-info/METADATA
+Filename: kikicocoTest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: kikicocoTest-0.0.0.1.dist-info/WHEEL
+Filename: kikicocoTest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: kikicocoTest-0.0.0.1.dist-info/top_level.txt
+Filename: kikicocoTest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kikicocoTest-0.0.0.1.dist-info/RECORD
+Filename: kikicocoTest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kikicocoTest/test1.py

```diff
@@ -1,3 +1,3 @@
 def print_test1():
     '''테스트 문장을 출력합니다'''
-    print("Hi, This is test1.py page!")
+    print("Hi, This is 0.0.0.2 test1.py page!")
```

## kikicocoTest/test2.py

```diff
@@ -1,3 +1,3 @@
 def print_test2():
     '''테스트 문장을 출력합니다'''
-    print("안녕하세요? 이것은 test2.py 페이지입니다!")
+    print("안녕하세요? 이것은 0.0.0.2 test2.py 페이지입니다!")
```

