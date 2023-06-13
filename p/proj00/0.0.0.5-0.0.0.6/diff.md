# Comparing `tmp/proj00-0.0.0.5-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3677 bytes, number of entries: 8
+Zip file size: 3700 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3264 b- defN 23-Jun-13 00:35 proj00/baek.py
--rw-rw-rw-  2.0 fat      650 b- defN 23-Jun-13 00:35 proj00/bmi.py
+-rw-rw-rw-  2.0 fat      651 b- defN 23-Jun-13 00:45 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-13 00:35 proj00/test2.py
--rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/RECORD
-8 files, 5155 bytes uncompressed, 2669 bytes compressed:  48.2%
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-13 00:36 proj00/test2.py
+-rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/RECORD
+8 files, 5156 bytes uncompressed, 2692 bytes compressed:  47.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.5.dist-info/METADATA
+Filename: proj00-0.0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.5.dist-info/WHEEL
+Filename: proj00-0.0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.5.dist-info/top_level.txt
+Filename: proj00-0.0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.5.dist-info/RECORD
+Filename: proj00-0.0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/bmi.py

```diff
@@ -10,17 +10,19 @@
         string = '정상'
     elif bmi <= 24.9:
         string = '과체중'
     else:
         string = '비만'
     return string
 
+def returnMessage(bmi):
+    return f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi:f=.1f}이고, {BMItoString(bmi)}입니다.'
 
-def printMessage(bmi):
-    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
+def printBMIMessage(bmi):
+    print(returnMessage(bmi))
 
-    
-def printMessage(height, weight):
+
+def printHeightWeightMessage(height, weight):
     bmi = calculateBMI(height, weight)
-    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
+    print(returnMessage(bmi))
```

