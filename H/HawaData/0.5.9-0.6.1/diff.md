# Comparing `tmp/HawaData-0.5.9.tar.gz` & `tmp/HawaData-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.9.tar", last modified: Thu Jun  1 01:32:32 2023, max compression
+gzip compressed data, was "HawaData-0.6.1.tar", last modified: Tue Jun 13 08:39:26 2023, max compression
```

## Comparing `HawaData-0.5.9.tar` & `HawaData-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.128128 HawaData-0.5.9/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.118232 HawaData-0.5.9/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2638 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2638 2023-06-01 01:32:32.127901 HawaData-0.5.9/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.9/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.118746 HawaData-0.5.9/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.9/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.121218 HawaData-0.5.9/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.9/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.9/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.9/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.9/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.9/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.123071 HawaData-0.5.9/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.9/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.9/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.9/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.5.9/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.9/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.125006 HawaData-0.5.9/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.9/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.9/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.9/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.9/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.9/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.126881 HawaData-0.5.9/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.9/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    26659 2023-05-31 12:59:00.000000 HawaData-0.5.9/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.9/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-01 01:32:32.128195 HawaData-0.5.9/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.9/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.127370 HawaData-0.5.9/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.9/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.877719 HawaData-0.6.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.866294 HawaData-0.6.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2809 2023-06-13 08:39:26.000000 HawaData-0.6.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-13 08:39:26.000000 HawaData-0.6.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-13 08:39:26.000000 HawaData-0.6.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-13 08:39:26.000000 HawaData-0.6.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2809 2023-06-13 08:39:26.877396 HawaData-0.6.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.866825 HawaData-0.6.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.869957 HawaData-0.6.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.6.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.1/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.872032 HawaData-0.6.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9450 2023-06-13 03:35:19.000000 HawaData-0.6.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5630 2023-06-13 03:42:10.000000 HawaData-0.6.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.6.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.875028 HawaData-0.6.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.1/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.1/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.1/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.1/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.876101 HawaData-0.6.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28013 2023-06-13 08:01:42.000000 HawaData-0.6.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.6.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-13 08:39:26.877841 HawaData-0.6.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 08:39:26.876673 HawaData-0.6.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.1/test/test_query.py
```

### Comparing `HawaData-0.5.9/HawaData.egg-info/PKG-INFO` & `HawaData-0.6.1/HawaData.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.9
+Version: 0.6.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -91,7 +91,13 @@
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
 - 0.5.7 update describe_grade_text
 - 0.5.8 update other report text
 - 0.5.9 add grade periods
+- 0.5.10 add score text
+- 0.5.11 remove text
+- 0.5.12 get grade focus
+- 0.5.13 count grade class scores
+- 0.6.0 add student health api data
+- 0.6.1 count dim field scores
```

### Comparing `HawaData-0.5.9/HawaData.egg-info/SOURCES.txt` & `HawaData-0.6.1/HawaData.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 hawa/common/query.py
 hawa/common/utils.py
 hawa/data/__init__.py
 hawa/data/city.py
 hawa/data/district.py
 hawa/data/klass.py
 hawa/data/school.py
+hawa/data/student.py
 hawa/paper/__init__.py
 hawa/paper/health.py
 hawa/paper/mht.py
 test/test_query.py
```

### Comparing `HawaData-0.5.9/PKG-INFO` & `HawaData-0.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.9
+Version: 0.6.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -91,7 +91,13 @@
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
 - 0.5.7 update describe_grade_text
 - 0.5.8 update other report text
 - 0.5.9 add grade periods
+- 0.5.10 add score text
+- 0.5.11 remove text
+- 0.5.12 get grade focus
+- 0.5.13 count grade class scores
+- 0.6.0 add student health api data
+- 0.6.1 count dim field scores
```

### Comparing `HawaData-0.5.9/README.md` & `HawaData-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/base/db.py` & `HawaData-0.6.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/base/init.py` & `HawaData-0.6.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/common/data.py` & `HawaData-0.6.1/hawa/common/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,18 @@
             match self.meta_unit_type:
                 case 'country':
                     self.schools = self.query.query_schools_all()
                 case 'province':
                     self.schools = self.query.query_schools_by_startwith(self.meta_unit_id // 10000)
                 case 'city':
                     self.schools = self.query.query_schools_by_startwith(self.meta_unit_id // 100)
-                case 'district' | 'school' | 'class':
+                case 'district' | 'school' | 'class' | 'student':
                     self.schools = self.query.query_schools_by_startwith(self.meta_unit_id)
+                case _:
+                    raise ValueError(f'unknown meta_unit_type: {self.meta_unit_type}')
             self.school_ids = self.schools['id'].tolist()
         project.logger.debug(f'schools: {len(self.schools)}')
 
     def _to_init_d_cases(self):
         start_stamp = pendulum.datetime(self.target_year, 1, 1)
         end_stamp = pendulum.datetime(self.target_year + 1, 1, 1)
         start_stamp_str = start_stamp.format(project.format)
```

### Comparing `HawaData-0.5.9/hawa/common/query.py` & `HawaData-0.6.1/hawa/common/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 @singleton
 class DataQuery:
     db = DbUtil()
 
     def query_unit(self, meta_unit_type: str, meta_unit_id: str):
         match meta_unit_type:
+            case 'student':
+                sql = f"select id,nickname from users where id={meta_unit_id};"
+                data = self.db.query_by_sql(sql=sql, mode='one')
+                meta_unit = MetaUnit(id=data['id'], name=data['nickname'], short_name=data['nickname'])
             case 'school' | 'class':
                 sql = f"select id,name,short_name from schools where id={meta_unit_id};"
                 data = self.db.query_by_sql(sql=sql, mode='one')
                 meta_unit = MetaUnit(**data)
             case 'district' | 'city' | 'province':
                 sql = f"select id,name from locations where id={meta_unit_id};"
                 data = self.db.query_by_sql(sql=sql, mode='one')
@@ -94,14 +98,15 @@
         answers = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(
             subset=['case_id', 'student_id', 'item_id'])
         return answers
 
     def query_students(self, student_ids: list[int]):
         user_cols = "id, username, first_name, last_name, nickname, gender, role, source, created, " \
                     "unit_id, client_id, extra"
+        student_ids.append(0)
         sql = f"select {user_cols} from users where id in {tuple(student_ids)} and length(id)>=18;"
         students = pd.read_sql(text(sql), self.db.engine_conn).drop_duplicates(subset=['id'])
         return students
 
     def query_items(self, item_ids: list[int]):
         item_cols = "id, item_text, choices, item_key, item_type, grade, test_type, pattern, " \
                     "`source`, created"
```

### Comparing `HawaData-0.5.9/hawa/common/utils.py` & `HawaData-0.6.1/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/config.py` & `HawaData-0.6.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/data/klass.py` & `HawaData-0.6.1/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/hawa/paper/health.py` & `HawaData-0.6.1/hawa/paper/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 @dataclass
 class HealthApiData(HealthData):
     """为 yingde api 项目提供基类"""
     grade: Optional[int] = None  # 必填
     grade_final_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     def _to_init_d_cases(self):
-        """如果有年级参数，则筛选年级暑假"""
+        """如果有年级参数，则筛选年级数据"""
         super()._to_init_d_cases()
         if self.grade:
             self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
             self.case_ids = self.cases['id'].tolist()
             self.case_project_ids = Counter(self.cases['project_id'].tolist())
             project.logger.debug(f'cases: {len(self.cases)}')
         if len(self.cases) == 0:
@@ -75,18 +75,17 @@
         raw_data = {
             'total': answers,
             'M': answers.loc[answers.gender == 'M', :],
             'F': answers.loc[answers.gender == 'F', :]
         }
         res = {}
         for gender_k, gender_v in raw_data.items():
-            res[gender_k] = {}
-            for this_item_code, code_group in gender_v.groupby(item_code):
-                score = round(code_group.score.mean() * 100, 2)
-                res[gender_k][this_item_code] = score
+            res[gender_k] = self.count_dim_or_field_scores_by_answers(
+                answers=gender_v, item_code=item_code, res_format='dict'
+            )
         codes = answers[item_code].unique().tolist()
         gender_box = []
         for gender_k, gender_data in res.items():
             row_data = {
                 "name": gender_k,
                 "value": []
             }
@@ -95,20 +94,54 @@
             gender_box.append(row_data)
 
         return {
             "category": codes,
             "values": gender_box,
         }
 
+    def get_grade_focus(self, grade: int, gender: str = 'total'):
+        """获取年级的优先关注点"""
+        dimensions = self.dim_field_gender_compare(grade=grade, item_code='dimension')
+        fields = self.dim_field_gender_compare(grade=grade, item_code='field')
+        res = []
+        for data in (dimensions, fields):
+            code_names = data.get('category', [])
+            try:
+                code_scores = [row['value'] for row in data['values'] if row['name'] == gender][0]
+            except IndexError:
+                code_scores = []
+            for n, s in zip(code_names, code_scores):
+                res.append(n) if s < 60 else None
+        return res
+
     def __get_grade_final_answers(self, grade: int):
         return self.final_answers[self.final_answers['grade'] == grade]
 
     def __get_grade_final_scores(self, grade: int):
         return self.final_scores[self.final_scores['grade'] == grade]
 
+    def count_dim_or_field_scores_by_answers(self, answers, item_code, res_format: str = 'dict'):
+        """
+        计算维度或领域得分
+        :param answers: 由 final answers 中取出的部分数据，属于某一主体
+        :param item_code: dimension/field
+        :return:
+        """
+        keys, values, mapping = [], [], {}
+        for code, code_group in answers.groupby(item_code):
+            score = round(code_group.score.mean() * 100, 2)
+            keys.append(code)
+            values.append(score)
+            mapping[code] = score
+        match res_format:
+            case 'dict':
+                return mapping
+            case 'list':
+                return keys, values
+
 
 @dataclass
 class HealthReportData(HealthData):
     # 计算数据
     code_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
     summary_scores: dict = field(default_factory=dict)
     grade_good_bad = None  # 优势 优先关注点
@@ -513,15 +546,15 @@
         return res
 
     def _build_codes(self, codes: list[str]):
         if len(codes) == 1:
             return f'“{codes[0]}”'
         elif len(codes) > 1:
             code_text = '、'.join([f'“{i}”' for i in codes[:-1]]) + f'和“{codes[-1]}”'
-            return f"在{code_text}等维度和领域，"
+            return f"在{code_text}维度和领域，"
         else:
             return ''
 
     def compare_grade_gen_text(self):
         """生成整体分析标题及一句分析文本。"""
         data = {}
         for grade in self.grade.grades:
@@ -568,28 +601,28 @@
             elif first - second <= -5:
                 smaller.append(f"{project.grade_simple[grade]}年级")
             else:
                 others.append(f"{project.grade_simple[grade]}年级")
         res = ''
         if bigger:
             local_codes = self._build_codes(bigger)
-            res += f"{self.meta_unit.short_name}{local_codes}分数"
+            res += f"{self.meta_unit.short_name}{local_codes}"
             match category:
                 case 'total':
-                    res += '明显高于全国平均分数，'
+                    res += '分数明显高于全国平均分数，'
                 case 'gender':
-                    res += '男生明显高于女生，'
+                    res += '男生分数明显高于女生分数，'
 
         if smaller:
             local_codes = self._build_codes(smaller)
-            res += f"{self.meta_unit.short_name}{local_codes}分数"
+            res += f"{self.meta_unit.short_name}{local_codes}"
             match category:
                 case 'total':
-                    res += "明显低于全国平均分数，"
+                    res += "分数明显低于全国平均分数，"
                 case 'gender':
-                    res += "男生明显低于女生，"
+                    res += "男生分数明显低于女生分数，"
         if (bigger or smaller) and ((len(bigger) + len(smaller)) < len(self.grade.grades)):
             local_codes = self._build_codes(others)
             res += f'{local_codes}没有明显差异。'
         if not bigger and not smaller:
             res = f'{self.meta_unit.short_name}分数对比无明显差异。'
         return res
```

### Comparing `HawaData-0.5.9/hawa/paper/mht.py` & `HawaData-0.6.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/setup.py` & `HawaData-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.9/test/test_query.py` & `HawaData-0.6.1/test/test_query.py`

 * *Files identical despite different names*

