# Comparing `tmp/nkkbmiTest-0.0.0.1-py3-none-any.whl.zip` & `tmp/nkkbmiTest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1571 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      715 b- defN 23-Jun-13 00:59 nkkbmiTest/bmitest.py
--rw-rw-rw-  2.0 fat      214 b- defN 23-Jun-13 01:04 nkkbmiTest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 01:04 nkkbmiTest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 01:04 nkkbmiTest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      394 b- defN 23-Jun-13 01:04 nkkbmiTest-0.0.0.1.dist-info/RECORD
-5 files, 1431 bytes uncompressed, 831 bytes compressed:  41.9%
+Zip file size: 1565 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      706 b- defN 23-Jun-13 01:09 nkkbmiTest/bmitest.py
+-rw-rw-rw-  2.0 fat      214 b- defN 23-Jun-13 01:10 nkkbmiTest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 01:10 nkkbmiTest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 01:10 nkkbmiTest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      394 b- defN 23-Jun-13 01:10 nkkbmiTest-0.0.0.2.dist-info/RECORD
+5 files, 1422 bytes uncompressed, 825 bytes compressed:  42.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: nkkbmiTest/bmitest.py
 Comment: 
 
-Filename: nkkbmiTest-0.0.0.1.dist-info/METADATA
+Filename: nkkbmiTest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: nkkbmiTest-0.0.0.1.dist-info/WHEEL
+Filename: nkkbmiTest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: nkkbmiTest-0.0.0.1.dist-info/top_level.txt
+Filename: nkkbmiTest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nkkbmiTest-0.0.0.1.dist-info/RECORD
+Filename: nkkbmiTest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nkkbmiTest/bmitest.py

```diff
@@ -11,10 +11,8 @@
   if my_bmi <= 18.5:
     print(f'나의 BMI(신체질량지수)는 {my_bmi} 이고, 저체중입니다.')
   elif my_bmi <= 22.9 and my_bmi > 18.5:
     print(f'나의 BMI(신체질량지수)는 {my_bmi} 이고, 정상입니다.')
   elif my_bmi <= 24.9 and my_bmi > 22.9:
     print(f'나의 BMI(신체질량지수)는 {my_bmi} 이고, 과체중입니다.')
   elif my_bmi > 25.0:
-    print(f'나의 BMI(신체질량지수)는 {my_bmi} 이고, 비만입니다.')
-
-bmi()
+    print(f'나의 BMI(신체질량지수)는 {my_bmi} 이고, 비만입니다.')
```

