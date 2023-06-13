# Comparing `tmp/project_BMI_Potato-0.0.0.3-py3-none-any.whl.zip` & `tmp/project_BMI_Potato-0.0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1840 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1314 b- defN 23-Jun-13 00:14 project_BMI_Potato/Calculate_BMI_Potato.py
--rw-rw-rw-  2.0 fat      255 b- defN 23-Jun-13 00:15 project_BMI_Potato-0.0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:15 project_BMI_Potato-0.0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       40 b- defN 23-Jun-13 00:15 project_BMI_Potato-0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      448 b- defN 23-Jun-13 00:15 project_BMI_Potato-0.0.0.3.dist-info/RECORD
-5 files, 2154 bytes uncompressed, 994 bytes compressed:  53.9%
+Zip file size: 1868 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1413 b- defN 23-Jun-13 00:32 project_BMI_Potato/Calculate_BMI_Potato.py
+-rw-rw-rw-  2.0 fat      255 b- defN 23-Jun-13 00:36 project_BMI_Potato-0.0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:36 project_BMI_Potato-0.0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jun-13 00:36 project_BMI_Potato-0.0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      448 b- defN 23-Jun-13 00:36 project_BMI_Potato-0.0.0.4.dist-info/RECORD
+5 files, 2253 bytes uncompressed, 1022 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: project_BMI_Potato/Calculate_BMI_Potato.py
 Comment: 
 
-Filename: project_BMI_Potato-0.0.0.3.dist-info/METADATA
+Filename: project_BMI_Potato-0.0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: project_BMI_Potato-0.0.0.3.dist-info/WHEEL
+Filename: project_BMI_Potato-0.0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: project_BMI_Potato-0.0.0.3.dist-info/top_level.txt
+Filename: project_BMI_Potato-0.0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: project_BMI_Potato-0.0.0.3.dist-info/RECORD
+Filename: project_BMI_Potato-0.0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## project_BMI_Potato/Calculate_BMI_Potato.py

```diff
@@ -1,8 +1,12 @@
+def Hello():
+    print('Hello !!!!!!')
+
 def start_Check():
+    Hello()
     print('* ' * 23,
           '\n*                                           *\n'
           '*                                           *\n'
           '*           BMI 계산 프로그램입니다             *\n'
           '*                                           *\n'
           '*                                           *\n',
           '* ' * 23)
@@ -31,8 +35,11 @@
         print('당신은 과체중이니 좀 덜 먹으세요 ㅋㅋ')
     elif bmi > 24.9:
         print()
 
         print('당신의 BMI는 %.2f 입니다.' % bmi)
         print()
 
-        print('비만이니까 그만 드세요 ㅎㅎ')
+        print('비만이니까 그만 드세요 ㅎㅎ')
+
+def Hello():
+    print('Hello !!!!!!')
```

