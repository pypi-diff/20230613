# Comparing `tmp/BMIpsyTest-0.0.0.2-py3-none-any.whl.zip` & `tmp/BMIpsyTest-0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1809 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      910 b- defN 23-Jun-13 01:12 BMIpsyTest/BMIpsyTest.py
--rw-rw-rw-  2.0 fat      253 b- defN 23-Jun-13 01:14 BMIpsyTest-0.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 01:14 BMIpsyTest-0.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 01:14 BMIpsyTest-0.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      397 b- defN 23-Jun-13 01:14 BMIpsyTest-0.0.0.2.dist-info/RECORD
-5 files, 1668 bytes uncompressed, 1063 bytes compressed:  36.3%
+Zip file size: 1807 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      901 b- defN 23-Jun-13 01:16 BMIpsyTest/BMIpsyTest.py
+-rw-rw-rw-  2.0 fat      253 b- defN 23-Jun-13 01:17 BMIpsyTest-0.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 01:17 BMIpsyTest-0.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 01:17 BMIpsyTest-0.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      397 b- defN 23-Jun-13 01:17 BMIpsyTest-0.0.0.3.dist-info/RECORD
+5 files, 1659 bytes uncompressed, 1061 bytes compressed:  36.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: BMIpsyTest/BMIpsyTest.py
 Comment: 
 
-Filename: BMIpsyTest-0.0.0.2.dist-info/METADATA
+Filename: BMIpsyTest-0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: BMIpsyTest-0.0.0.2.dist-info/WHEEL
+Filename: BMIpsyTest-0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: BMIpsyTest-0.0.0.2.dist-info/top_level.txt
+Filename: BMIpsyTest-0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: BMIpsyTest-0.0.0.2.dist-info/RECORD
+Filename: BMIpsyTest-0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BMIpsyTest/BMIpsyTest.py

```diff
@@ -1,8 +1,8 @@
-def BMIcheck(height,weight):
+def BMIcheck():
     print("비만도 측정(BMI지수")
     print()
     print("BMI를 이용한 비만도 계산은 자신의 몸무게를 키의 제곱으로 나누는 것으로 공식은 Kg/m^.'''"
           "BMI가 18.5 이하면 저체중 / 18.2 ~ 22.9 사이면 정상 / 23.0 ~ 24.9 사이면 과체중 / 25.0 이상부터는 비만으로 판정")
     print("ex)키 170cm에 몸무게 73kg에면, 계산식: 73 / (1.7*1.7) = 25.26 -> 과체중")
     height = int(input("신장?"))
     weight = int(input("체중?"))
@@ -13,7 +13,9 @@
     elif BMI<=22.9:
         BMIstate = "정상"
     elif BMI<=24.9:
         BMIstate = "과체중"
     else:
         BMIstate = "비만"
     print("MY BMI: {:.1f}\n나의BMI(신체질량지수)는 {:.1f}이고, {}입니다".format(BMI,BMI,BMIstate))
+
+
```

