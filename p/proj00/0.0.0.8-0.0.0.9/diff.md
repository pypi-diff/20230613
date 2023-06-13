# Comparing `tmp/proj00-0.0.0.8-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3691 bytes, number of entries: 8
+Zip file size: 3777 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3264 b- defN 23-Jun-13 00:35 proj00/baek.py
--rw-rw-rw-  2.0 fat      659 b- defN 23-Jun-13 00:50 proj00/bmi.py
+-rw-rw-rw-  2.0 fat      914 b- defN 23-Jun-13 00:58 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-Jun-13 00:48 proj00/test2.py
--rw-rw-rw-  2.0 fat      222 b- defN 23-Jun-13 00:56 proj00-0.0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:56 proj00-0.0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:56 proj00-0.0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:56 proj00-0.0.0.8.dist-info/RECORD
-8 files, 5098 bytes uncompressed, 2683 bytes compressed:  47.4%
+-rw-rw-rw-  2.0 fat      222 b- defN 23-Jun-13 00:58 proj00-0.0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:58 proj00-0.0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:58 proj00-0.0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:58 proj00-0.0.0.9.dist-info/RECORD
+8 files, 5353 bytes uncompressed, 2769 bytes compressed:  48.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.8.dist-info/METADATA
+Filename: proj00-0.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.8.dist-info/WHEEL
+Filename: proj00-0.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.8.dist-info/top_level.txt
+Filename: proj00-0.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.8.dist-info/RECORD
+Filename: proj00-0.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/bmi.py

```diff
@@ -14,15 +14,26 @@
         string = '비만'
     return string
 
 def returnMessage(bmi):
     return f'MY BMI: {bmi:f=.1f}\n나의BMI(신체질량지수)는 {bmi:f=.1f}이고, {BMItoString(bmi)}입니다.'
 
 def printBMIMessage(bmi):
+    '''
+    bmi 바로 입력 시에 메시지 출력.
+    bmi: weight/((height/100)**2)
+    height = 키
+    weight = 몸무게
+    '''
     print(returnMessage(bmi))
 
 
 def printHeightWeightMessage(height, weight):
+    '''
+    height, weight 입력 시에 메시지 출력.
+    height = 키
+    weight = 몸무게
+    '''
     bmi = calculateBMI(height, weight)
     print(returnMessage(bmi))
```

