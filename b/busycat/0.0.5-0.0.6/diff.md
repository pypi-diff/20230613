# Comparing `tmp/busycat-0.0.5.tar.gz` & `tmp/busycat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busycat-0.0.5.tar", last modified: Sat Mar 11 04:13:46 2023, max compression
+gzip compressed data, was "busycat-0.0.6.tar", last modified: Tue Jun 13 06:06:27 2023, max compression
```

## Comparing `busycat-0.0.5.tar` & `busycat-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 04:13:46.310614 busycat-0.0.5/
--rw-rw-rw-   0        0        0     1083 2022-08-05 05:03:58.000000 busycat-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      372 2023-03-11 04:13:46.310108 busycat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       34 2022-08-05 05:03:02.000000 busycat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 04:13:46.306564 busycat-0.0.5/busycat/
--rw-rw-rw-   0        0        0       22 2023-03-11 02:46:53.000000 busycat-0.0.5/busycat/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-03-11 02:47:25.000000 busycat-0.0.5/busycat/mysql.py
-drwxrwxrwx   0        0        0        0 2023-03-11 04:13:46.309601 busycat-0.0.5/busycat.egg-info/
--rw-rw-rw-   0        0        0      372 2023-03-11 04:13:46.000000 busycat-0.0.5/busycat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-03-11 04:13:46.000000 busycat-0.0.5/busycat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 04:13:46.000000 busycat-0.0.5/busycat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-11 04:13:46.000000 busycat-0.0.5/busycat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-11 04:13:46.000000 busycat-0.0.5/busycat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 04:13:46.310614 busycat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-03-11 04:13:41.000000 busycat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:06:27.608318 busycat-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2022-08-05 05:03:58.000000 busycat-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      372 2023-06-13 06:06:27.608318 busycat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2022-08-05 05:03:02.000000 busycat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:06:27.603252 busycat-0.0.6/busycat/
+-rw-rw-rw-   0        0        0       22 2023-03-11 02:46:53.000000 busycat-0.0.6/busycat/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-05-19 03:25:19.000000 busycat-0.0.6/busycat/mysql.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:06:27.607305 busycat-0.0.6/busycat.egg-info/
+-rw-rw-rw-   0        0        0      372 2023-06-13 06:06:27.000000 busycat-0.0.6/busycat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-13 06:06:27.000000 busycat-0.0.6/busycat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:06:27.000000 busycat-0.0.6/busycat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 06:06:27.000000 busycat-0.0.6/busycat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 06:06:27.000000 busycat-0.0.6/busycat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:06:27.608824 busycat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-06-13 06:03:53.000000 busycat-0.0.6/setup.py
```

### Comparing `busycat-0.0.5/LICENSE` & `busycat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `busycat-0.0.5/busycat/mysql.py` & `busycat-0.0.6/busycat/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import pymysql
 import json
 
 
 class mysql_connect():
-    def __init__(self,host,user,pwd,db_name,port=None):
-        self.db = pymysql.connect(host=host,user=user,password=pwd,database=db_name,port=port)
+    def __init__(self, host, user, pwd, db_name, port=None):
+        self.db = pymysql.connect(host=host, user=user, password=pwd, database=db_name, port=port)
         self.cursor = self.db.cursor()
-        
-    def trans_to_json(self,description,results):
+
+    def trans_to_json(self, description, results):
         fields = [field[0] for field in description]
-        data = [dict(zip(fields,row)) for row in results]
+        data = [dict(zip(fields, row)) for row in results]
         json_data = json.dumps(data)
         return json_data
-        
 
-    def select(self,sql):
+    def select(self, sql):
         self.cursor.execute(sql)
         results = self.cursor.fetchall()
 
         description = self.cursor.description
-        json_data=self.trans_to_json(description,results)
-
+        json_data = self.trans_to_json(description, results)
+        json_data = json.loads(json_data)
         return json_data
 
-
-    def find(self,sql):
+    def find(self, sql):
         self.cursor.execute(sql)
         results = self.cursor.fetchone()
-        description = self.cursor.description
-        json_data=self.trans_to_json(description,results)
+        description = self.cursor.description[0][0]
+        json_data = {description: results[0]}
         return json_data
 
     def delete(self, sql):
         '''未测试'''
         try:
             self.cursor.execute(sql)
             self.db.commit()
```

### Comparing `busycat-0.0.5/setup.py` & `busycat-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="busycat",
-    version="0.0.5",
+    version="0.0.6",
     author="busycat",
     author_email="",
     description="selfmade pkg",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

