# Comparing `tmp/proj00-0.0.0.4-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3631 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     3250 b- defN 23-Jun-13 00:18 proj00/baek.py
--rw-rw-rw-  2.0 fat      640 b- defN 23-Jun-13 00:31 proj00/bmi.py
+Zip file size: 3677 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     3264 b- defN 23-Jun-13 00:35 proj00/baek.py
+-rw-rw-rw-  2.0 fat      650 b- defN 23-Jun-13 00:35 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
--rw-rw-rw-  2.0 fat      179 b- defN 23-Jun-13 00:11 proj00/test2.py
--rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:32 proj00-0.0.0.4.dist-info/RECORD
-8 files, 5061 bytes uncompressed, 2623 bytes compressed:  48.2%
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-13 00:35 proj00/test2.py
+-rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:35 proj00-0.0.0.5.dist-info/RECORD
+8 files, 5155 bytes uncompressed, 2669 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.4.dist-info/METADATA
+Filename: proj00-0.0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.4.dist-info/WHEEL
+Filename: proj00-0.0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.4.dist-info/top_level.txt
+Filename: proj00-0.0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.4.dist-info/RECORD
+Filename: proj00-0.0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/baek.py

```diff
@@ -46,28 +46,26 @@
 NO
 힌트
 1234567 -> 28 -> 10 -> 1 (NO)
 '''
 
 n = input()
 
-
-sum = 0
 count = 0
-while True:
-    if sum > 9:
-        count += 1
-        for i in range(len(n)):
-            sum += int(n[i])
-    else:
-        if sum != 0:
-            n = sum
+if len(n) > 1:
+    sum = 0
+    while True:
+        if sum > 9:
+            count += 1
+            for i in range(len(n)):
+                sum += int(n[i])
         else:
-            n = int(n)
-        break
+            if count >= 1:
+                n ==
+            break
 
 if n % 3 == 0:
     print(count)
     print('YES')
     
 else:
     print(count)
```

## proj00/bmi.py

```diff
@@ -10,14 +10,17 @@
         string = '정상'
     elif bmi <= 24.9:
         string = '과체중'
     else:
         string = '비만'
     return string
 
+
+def printMessage(bmi):
+    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
+
+    
 def printMessage(height, weight):
     bmi = calculateBMI(height, weight)
     print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
 
-def printMessage(bmi):
-    print(f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi}이고, {BMItoString(bmi)}입니다.')
```

## proj00/test2.py

```diff
@@ -2,8 +2,14 @@
     '''테스트 문장을 출력합니다.'''
     print('Hi, This is Test2')
 
 from proj00 import test1, test2
 
 test1.print_test1()
 
-test2.print_test2()
+test2.print_test2()
+
+from proj00 import bmi
+
+h, w = 175, 66
+
+bmi.printMessage(h, w)
```

