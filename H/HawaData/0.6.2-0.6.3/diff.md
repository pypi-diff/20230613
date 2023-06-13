# Comparing `tmp/HawaData-0.6.2.tar.gz` & `tmp/HawaData-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.6.2.tar", last modified: Tue Jun 13 09:16:51 2023, max compression
+gzip compressed data, was "HawaData-0.6.3.tar", last modified: Tue Jun 13 09:39:12 2023, max compression
```

## Comparing `HawaData-0.6.2.tar` & `HawaData-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.979193 HawaData-0.6.2/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.963781 HawaData-0.6.2/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2023-06-13 09:16:51.000000 HawaData-0.6.2/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-13 09:16:51.000000 HawaData-0.6.2/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-13 09:16:51.000000 HawaData-0.6.2/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-13 09:16:51.000000 HawaData-0.6.2/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2023-06-13 09:16:51.978731 HawaData-0.6.2/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.2/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.964284 HawaData-0.6.2/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.2/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.967875 HawaData-0.6.2/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.2/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.6.2/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.2/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.2/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.2/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.970354 HawaData-0.6.2/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.2/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9450 2023-06-13 03:35:19.000000 HawaData-0.6.2/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5630 2023-06-13 03:42:10.000000 HawaData-0.6.2/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.6.2/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.2/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.974566 HawaData-0.6.2/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.2/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.2/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.2/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.2/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.2/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.2/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.976570 HawaData-0.6.2/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.2/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    27826 2023-06-13 08:53:05.000000 HawaData-0.6.2/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.6.2/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-13 09:16:51.979319 HawaData-0.6.2/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.2/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:16:51.977684 HawaData-0.6.2/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.2/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738807 HawaData-0.6.3/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.733116 HawaData-0.6.3/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2870 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2870 2023-06-13 09:39:12.738566 HawaData-0.6.3/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.3/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.733551 HawaData-0.6.3/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.3/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.734772 HawaData-0.6.3/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.3/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.6.3/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.3/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.3/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.3/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.735834 HawaData-0.6.3/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.3/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9450 2023-06-13 03:35:19.000000 HawaData-0.6.3/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5630 2023-06-13 03:42:10.000000 HawaData-0.6.3/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.6.3/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.3/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.737204 HawaData-0.6.3/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.3/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.3/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.3/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.3/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.3/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.3/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738016 HawaData-0.6.3/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.3/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28118 2023-06-13 09:39:06.000000 HawaData-0.6.3/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.6.3/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-13 09:39:12.738875 HawaData-0.6.3/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.3/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738256 HawaData-0.6.3/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.3/test/test_query.py
```

### Comparing `HawaData-0.6.2/HawaData.egg-info/PKG-INFO` & `HawaData-0.6.3/HawaData.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.2
+Version: 0.6.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -98,7 +98,8 @@
 - 0.5.10 add score text
 - 0.5.11 remove text
 - 0.5.12 get grade focus
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
+- 0.6.3 count student grade
```

### Comparing `HawaData-0.6.2/HawaData.egg-info/SOURCES.txt` & `HawaData-0.6.3/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/PKG-INFO` & `HawaData-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.2
+Version: 0.6.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -98,7 +98,8 @@
 - 0.5.10 add score text
 - 0.5.11 remove text
 - 0.5.12 get grade focus
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
+- 0.6.3 count student grade
```

### Comparing `HawaData-0.6.2/README.md` & `HawaData-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/base/db.py` & `HawaData-0.6.3/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/base/init.py` & `HawaData-0.6.3/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/common/data.py` & `HawaData-0.6.3/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/common/query.py` & `HawaData-0.6.3/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/common/utils.py` & `HawaData-0.6.3/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/config.py` & `HawaData-0.6.3/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/data/klass.py` & `HawaData-0.6.3/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/data/school.py` & `HawaData-0.6.3/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/data/student.py` & `HawaData-0.6.3/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/hawa/paper/health.py` & `HawaData-0.6.3/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,21 @@
             gender_box.append(row_data)
 
         return {
             "category": codes,
             "values": gender_box,
         }
 
+    def count_student_grade(self, student_id: int):
+        """计算指定学生的年级"""
+        fa = self.final_answers
+        student_answers = fa.loc[fa['student_id'] == student_id, :]
+        case_ids = student_answers['case_id'].unique().tolist()
+        return case_ids[0] % 100
+
     def get_grade_focus(self, grade: int, gender: str = 'total'):
         """获取年级的优先关注点"""
         dimensions = self.count_dim_or_field_scores_by_answers(
             answers=self.final_answers, item_code='dimension', res_format='dict'
         )
         fields = self.count_dim_or_field_scores_by_answers(
             answers=self.final_answers, item_code='field', res_format='dict'
```

### Comparing `HawaData-0.6.2/hawa/paper/mht.py` & `HawaData-0.6.3/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/setup.py` & `HawaData-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.2/test/test_query.py` & `HawaData-0.6.3/test/test_query.py`

 * *Files identical despite different names*

