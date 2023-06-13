# Comparing `tmp/sudalTest-0.0.0.1-py3-none-any.whl.zip` & `tmp/sudalTest-0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1651 bytes, number of entries: 6
+Zip file size: 1983 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat      105 b- defN 23-Jun-12 08:20 sudalTest/test1.py
--rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-12 08:20 sudalTest/test2.py
--rw-rw-rw-  2.0 fat      243 b- defN 23-Jun-12 08:41 sudalTest-0.0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-12 08:41 sudalTest-0.0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-12 08:41 sudalTest-0.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      461 b- defN 23-Jun-12 08:41 sudalTest-0.0.0.1.dist-info/RECORD
-6 files, 1062 bytes uncompressed, 813 bytes compressed:  23.4%
+-rw-rw-rw-  2.0 fat     1193 b- defN 23-Jun-13 00:09 sudalTest/test2.py
+-rw-rw-rw-  2.0 fat      243 b- defN 23-Jun-13 00:14 sudalTest-0.0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-13 00:14 sudalTest-0.0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-13 00:14 sudalTest-0.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      462 b- defN 23-Jun-13 00:14 sudalTest-0.0.0.2.dist-info/RECORD
+6 files, 2122 bytes uncompressed, 1145 bytes compressed:  46.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sudalTest/test1.py
 Comment: 
 
 Filename: sudalTest/test2.py
 Comment: 
 
-Filename: sudalTest-0.0.0.1.dist-info/METADATA
+Filename: sudalTest-0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: sudalTest-0.0.0.1.dist-info/WHEEL
+Filename: sudalTest-0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sudalTest-0.0.0.1.dist-info/top_level.txt
+Filename: sudalTest-0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sudalTest-0.0.0.1.dist-info/RECORD
+Filename: sudalTest-0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sudalTest/test2.py

```diff
@@ -1,3 +1,48 @@
-def print_test():
-    '''테스트 문장을 출력합니다.'''
-    print("안녕하세요,이것은 test2.py 페이지입니다.")
+def print_test2():
+  import random
+
+  print("주사위전사 게임에 오신걸 환영합니다")
+
+  print("주사위를 굴려보자~")
+
+  knife=2
+  bow=3
+  shield=2
+  armor=3
+  i=0
+
+  user_hp=10
+  for i in range(10):
+    abc=[1,2,3,4,5,6]
+    dice=random.choice(abc)
+
+    if dice==1:
+      print("운이 없네요 함정에 걸렸습니다.")
+      user_hp=user_hp-6
+      print(user_hp)
+    if dice==2:
+      print(f"{dice}가 나왔습니다.칼에 맞았습니다.")
+      user_hp=user_hp-knife
+      print(user_hp)
+    if dice==3:
+      print(f"{dice}가 나왔습니다.활에 맞았습니다.")
+      user_hp=user_hp-bow
+      print(user_hp)
+    if dice==4:
+      print(f"{dice}가 나왔습니다.방패를 얻었습니다!.")
+      user_hp=user_hp+shield
+      print(user_hp)
+    if dice==5:
+      print(f"{dice}가 나왔습니다.갑옷을 얻었습니다!.")
+      user_hp=user_hp+armor
+      print(user_hp)
+    if dice==6:
+      print("운이 좋으시군요! 구급상자를 얻었습니다.")
+      user_hp=user_hp+6
+      print(user_hp)
+    if user_hp<=0:
+      print("당신은 사망했습니다.")
+      break
+
+
+print_test2()
```

