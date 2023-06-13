# Comparing `tmp/proj00-0.0.0.3-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3497 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     3170 b- defN 23-Jun-13 00:12 proj00/baek.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-12 08:53 proj00/bmi.py
+Zip file size: 3631 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     3250 b- defN 23-Jun-13 00:18 proj00/baek.py
+-rw-rw-rw-  2.0 fat      640 b- defN 23-Jun-13 00:31 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
 -rw-rw-rw-  2.0 fat      179 b- defN 23-Jun-13 00:11 proj00/test2.py
--rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:15 proj00-0.0.0.3.dist-info/RECORD
-8 files, 4671 bytes uncompressed, 2489 bytes compressed:  46.7%
+-rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/RECORD
+8 files, 5061 bytes uncompressed, 2623 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.3.dist-info/METADATA
+Filename: proj00-0.0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.3.dist-info/WHEEL
+Filename: proj00-0.0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.3.dist-info/top_level.txt
+Filename: proj00-0.0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.3.dist-info/RECORD
+Filename: proj00-0.0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/baek.py

```diff
@@ -55,17 +55,21 @@
 count = 0
 while True:
     if sum > 9:
         count += 1
         for i in range(len(n)):
             sum += int(n[i])
     else:
+        if sum != 0:
+            n = sum
+        else:
+            n = int(n)
         break
 
-if sum % 3 == 0:
+if n % 3 == 0:
     print(count)
     print('YES')
     
 else:
     print(count)
     print('NO')
```

## proj00/bmi.py

```diff
@@ -1,16 +1,23 @@
 
-
-def bmi(height, weight):
+def calculateBMI(height, weight):
     return (weight/((height/100)**2))
 
-def message(bmi):
-    message = ''
+def BMItoString(bmi):
+    string = ''
     if bmi <= 18.5:
-        message = '저체중'
+        string = '저체중'
     elif bmi <= 22.9:
-        message = '정상'
+        string = '정상'
     elif bmi <= 24.9:
-        message = '과체중'
+        string = '과체중'
     else:
-        message = '비만'
-    return message
+        string = '비만'
+    return string
+
+def printMessage(height, weight):
+    bmi = calculateBMI(height, weight)
+    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
+
+def printMessage(bmi):
+    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
+
```

