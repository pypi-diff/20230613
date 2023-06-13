# Comparing `tmp/BMIckwrlTest001-0.0.0.1-py3-none-any.whl.zip` & `tmp/BMIckwrlTest001-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1579 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      446 b- defN 23-Jun-13 00:25 BMIckwrlTest001/BMI_test.py
--rw-rw-rw-  2.0 fat      209 b- defN 23-Jun-13 00:28 BMIckwrlTest001-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:28 BMIckwrlTest001-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-13 00:28 BMIckwrlTest001-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      420 b- defN 23-Jun-13 00:28 BMIckwrlTest001-0.0.0.1.dist-info/RECORD
-5 files, 1197 bytes uncompressed, 787 bytes compressed:  34.3%
+Zip file size: 1627 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-13 00:33 BMIckwrlTest001/BMI_test.py
+-rw-rw-rw-  2.0 fat      209 b- defN 23-Jun-13 00:33 BMIckwrlTest001-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:33 BMIckwrlTest001-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-13 00:33 BMIckwrlTest001-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      420 b- defN 23-Jun-13 00:33 BMIckwrlTest001-0.0.0.2.dist-info/RECORD
+5 files, 1296 bytes uncompressed, 835 bytes compressed:  35.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: BMIckwrlTest001/BMI_test.py
 Comment: 
 
-Filename: BMIckwrlTest001-0.0.0.1.dist-info/METADATA
+Filename: BMIckwrlTest001-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: BMIckwrlTest001-0.0.0.1.dist-info/WHEEL
+Filename: BMIckwrlTest001-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: BMIckwrlTest001-0.0.0.1.dist-info/top_level.txt
+Filename: BMIckwrlTest001-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: BMIckwrlTest001-0.0.0.1.dist-info/RECORD
+Filename: BMIckwrlTest001-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BMIckwrlTest001/BMI_test.py

```diff
@@ -1,8 +1,10 @@
-def BMI_check(weight, height):
+def BMI_check():
+    weight = int(input('체중을 입력하세요 : ',))
+    height = int(input('키를 입력하세요 : ',))
     BMI = weight/((height*0.01)**2)
     list = ['저체중', '최적 범위', '과체중', '1급 비만', '2급 비만', '3급 비만']
     if BMI < 18.5:
         i = 0
     elif BMI < 25:
         i = 1
     elif BMI < 30:
```

