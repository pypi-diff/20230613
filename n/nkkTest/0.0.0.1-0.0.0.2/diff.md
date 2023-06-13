# Comparing `tmp/nkkTest-0.0.0.1-py3-none-any.whl.zip` & `tmp/nkkTest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1602 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      108 b- defN 23-Jun-12 08:25 nkkTest/test1.py
--rw-rw-rw-  2.0 fat      136 b- defN 23-Jun-12 08:18 nkkTest/test2.py
--rw-rw-rw-  2.0 fat      213 b- defN 23-Jun-12 08:25 nkkTest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:25 nkkTest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-12 08:25 nkkTest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      448 b- defN 23-Jun-12 08:25 nkkTest-0.0.0.1.dist-info/RECORD
-6 files, 1010 bytes uncompressed, 788 bytes compressed:  22.0%
+Zip file size: 1638 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-13 00:14 nkkTest/test1.py
+-rw-rw-rw-  2.0 fat      167 b- defN 23-Jun-13 00:14 nkkTest/test2.py
+-rw-rw-rw-  2.0 fat      213 b- defN 23-Jun-13 00:16 nkkTest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:16 nkkTest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-13 00:16 nkkTest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      448 b- defN 23-Jun-13 00:16 nkkTest-0.0.0.2.dist-info/RECORD
+6 files, 1072 bytes uncompressed, 824 bytes compressed:  23.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: nkkTest/test1.py
 Comment: 
 
 Filename: nkkTest/test2.py
 Comment: 
 
-Filename: nkkTest-0.0.0.1.dist-info/METADATA
+Filename: nkkTest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: nkkTest-0.0.0.1.dist-info/WHEEL
+Filename: nkkTest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: nkkTest-0.0.0.1.dist-info/top_level.txt
+Filename: nkkTest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nkkTest-0.0.0.1.dist-info/RECORD
+Filename: nkkTest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nkkTest/test1.py

```diff
@@ -1,3 +1,4 @@
 def print_test1():
     '''테스트 문장을 출력합니다'''
     print('Hi, This is test1.py page!')
+    print('version up 0.0.0.2')
```

## nkkTest/test2.py

```diff
@@ -1,3 +1,4 @@
 def print_test2():
     '''테스트 문장을 출력합니다'''
     print('안녕하세요, 이것은 test2.py 페이지입니다')
+    print('버전 업 0.0.0.2')
```

