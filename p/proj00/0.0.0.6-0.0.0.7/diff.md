# Comparing `tmp/proj00-0.0.0.6-py3-none-any.whl.zip` & `tmp/proj00-0.0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3700 bytes, number of entries: 8
+Zip file size: 3671 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3264 b- defN 23-Jun-13 00:35 proj00/baek.py
--rw-rw-rw-  2.0 fat      651 b- defN 23-Jun-13 00:45 proj00/bmi.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-Jun-13 00:48 proj00/bmi.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jun-12 08:18 proj00/test1.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-13 00:36 proj00/test2.py
--rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:45 proj00-0.0.0.6.dist-info/RECORD
-8 files, 5156 bytes uncompressed, 2692 bytes compressed:  47.8%
+-rw-rw-rw-  2.0 fat      165 b- defN 23-Jun-13 00:48 proj00/test2.py
+-rw-rw-rw-  2.0 fat      204 b- defN 23-Jun-13 00:48 proj00-0.0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:48 proj00-0.0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 00:48 proj00-0.0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      582 b- defN 23-Jun-13 00:48 proj00-0.0.0.7.dist-info/RECORD
+8 files, 5078 bytes uncompressed, 2663 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: proj00/test1.py
 Comment: 
 
 Filename: proj00/test2.py
 Comment: 
 
-Filename: proj00-0.0.0.6.dist-info/METADATA
+Filename: proj00-0.0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: proj00-0.0.0.6.dist-info/WHEEL
+Filename: proj00-0.0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: proj00-0.0.0.6.dist-info/top_level.txt
+Filename: proj00-0.0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: proj00-0.0.0.6.dist-info/RECORD
+Filename: proj00-0.0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proj00/bmi.py

```diff
@@ -11,15 +11,15 @@
     elif bmi <= 24.9:
         string = '과체중'
     else:
         string = '비만'
     return string
 
 def returnMessage(bmi):
-    return f'MY BMI{bmi}\n나의BMI(신체질량지수)는 {bmi:f=.1f}이고, {BMItoString(bmi)}입니다.'
+    return f'MY BMI{bmi:f=.1f}\n나의BMI(신체질량지수)는 {bmi:f=.1f}이고, {BMItoString(bmi)}입니다.'
 
 def printBMIMessage(bmi):
     print(returnMessage(bmi))
 
 
 def printHeightWeightMessage(height, weight):
     bmi = calculateBMI(height, weight)
```

## proj00/test2.py

```diff
@@ -1,15 +1,7 @@
 def print_test2():
     '''테스트 문장을 출력합니다.'''
     print('Hi, This is Test2')
 
-from proj00 import test1, test2
-
-test1.print_test1()
-
-test2.print_test2()
-
 from proj00 import bmi
 
-h, w = 175, 66
-
-bmi.printMessage(h, w)
+bmi.printHeightWeightMessage(175, 66)
```

## Comparing `proj00-0.0.0.6.dist-info/RECORD` & `proj00-0.0.0.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 proj00/baek.py,sha256=ZUIwYt0XXLbo5WnbxT7kTjr_Ypa6uw5RH1qXUnLvEf0,3264
-proj00/bmi.py,sha256=FzMdPhYDbz3gJYdO6zZHnpJMVWwXWd6osJqeBBzpcik,651
+proj00/bmi.py,sha256=fUSSMOy7gPEmucSED_-RdK2gKTmLS2OFg5_lgpVeQxw,657
 proj00/test1.py,sha256=PK1k3CQQ-ANTjNffHaIEG8BK6JJA_hHjoeA6F1hYZCY,98
-proj00/test2.py,sha256=8DczUOzAHZhSJrC5mD1c_vslhb4krpiJDjzBf-u3ehM,249
-proj00-0.0.0.6.dist-info/METADATA,sha256=Fbdgzv8Mef_5bvfD_ejhSdtI0DoHYKzrbLfa9VtuiLI,204
-proj00-0.0.0.6.dist-info/WHEEL,sha256=v8slff5hmCpvciQ3G55d2d1CnOBupjDFJHDE2dUb1Ao,97
-proj00-0.0.0.6.dist-info/top_level.txt,sha256=_auOm2sC2m29hiGFj0ZY2Gt0YDIDxXQ5mOnj32fFSP8,11
-proj00-0.0.0.6.dist-info/RECORD,,
+proj00/test2.py,sha256=r7nfRR1m9UA23pZISAg5b417-PejzdyAcLcFQZxFVag,165
+proj00-0.0.0.7.dist-info/METADATA,sha256=e3rdd7MhKh40hdSo7keyg393FGpSeG7osG-p1ffwEFU,204
+proj00-0.0.0.7.dist-info/WHEEL,sha256=v8slff5hmCpvciQ3G55d2d1CnOBupjDFJHDE2dUb1Ao,97
+proj00-0.0.0.7.dist-info/top_level.txt,sha256=_auOm2sC2m29hiGFj0ZY2Gt0YDIDxXQ5mOnj32fFSP8,11
+proj00-0.0.0.7.dist-info/RECORD,,
```

