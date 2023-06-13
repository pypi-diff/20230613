# Comparing `tmp/project404-0.0.0.1-py3-none-any.whl.zip` & `tmp/project404-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1652 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      122 b- defN 23-Jun-12 08:09 project404/test1.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-12 08:06 project404/test2.py
--rw-rw-rw-  2.0 fat      218 b- defN 23-Jun-12 08:13 project404-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:13 project404-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-12 08:13 project404-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      467 b- defN 23-Jun-12 08:13 project404-0.0.0.1.dist-info/RECORD
-6 files, 1042 bytes uncompressed, 802 bytes compressed:  23.0%
+Zip file size: 2054 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     1055 b- defN 23-Jun-13 00:12 project404/test1.py
+-rw-rw-rw-  2.0 fat      236 b- defN 23-Jun-13 00:14 project404/test2.py
+-rw-rw-rw-  2.0 fat      218 b- defN 23-Jun-13 00:21 project404-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:21 project404-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-13 00:21 project404-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      468 b- defN 23-Jun-13 00:21 project404-0.0.0.2.dist-info/RECORD
+6 files, 2097 bytes uncompressed, 1204 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: project404/test1.py
 Comment: 
 
 Filename: project404/test2.py
 Comment: 
 
-Filename: project404-0.0.0.1.dist-info/METADATA
+Filename: project404-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: project404-0.0.0.1.dist-info/WHEEL
+Filename: project404-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: project404-0.0.0.1.dist-info/top_level.txt
+Filename: project404-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: project404-0.0.0.1.dist-info/RECORD
+Filename: project404-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## project404/test1.py

```diff
@@ -1,6 +1,34 @@
 def print_test1():
     # 테스트 문장출력
     print("Hi, this is test1.py page!")
 
-import os
-print(os.getcwd())
+
+'''BMI 지수를 계산하는 기능'''
+def calculate_bmi(height, weight):
+    var = height * 0.01
+    result = round(weight / (var * var), 1)
+    return result
+
+
+'''BMI 지수에 따라 적절한 멘트를 주는 기능'''
+def get_bmi_comment(result):
+    if result <= 18:
+        return f"당신의 BMI 지수는 {result}이며 저체중입니다."
+    elif 18.5 <= result <= 22.9:
+        return f"당신의 BMI 지수는 {result}이며 정상입니다."
+    elif 23.0 <= result <= 24.9:
+        return f"당신의 BMI 지수는 {result}이며 과체중입니다."
+    elif result > 25.0:
+        return f"당신의 BMI 지수는 {result}이며 비만입니다."
+
+
+'''BMI 지수는 보여주는 기능'''
+def show_bmi():
+    height = int(input("키 입력: "))
+    weight = int(input("몸무게 입력: "))
+    bmi_result = calculate_bmi(height, weight)
+    comment = get_bmi_comment(bmi_result)
+    print(comment)
+
+show_bmi()
+
```

## project404/test2.py

```diff
@@ -1,3 +1,8 @@
 def print_test2():
     # 테스트 문장 출력
-    print("안녕하세요 이것은 test2.py 파일입니다.")
+    print("안녕하세요 이것은 test2.py 파일입니다.")
+
+# 웃음 출력
+def print_test3():
+    # 테스트 문장 출력
+    print("우하하하하ㅏ하하하하하하")
```

