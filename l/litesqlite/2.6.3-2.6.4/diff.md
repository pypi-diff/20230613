# Comparing `tmp/litesqlite-2.6.3.tar.gz` & `tmp/litesqlite-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.3.tar", last modified: Mon Jun 12 11:23:38 2023, max compression
+gzip compressed data, was "litesqlite-2.6.4.tar", last modified: Tue Jun 13 07:33:59 2023, max compression
```

## Comparing `litesqlite-2.6.3.tar` & `litesqlite-2.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.612458 litesqlite-2.6.3/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.3/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:23:38.612458 litesqlite-2.6.3/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.3/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.608458 litesqlite-2.6.3/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.3/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.3/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8324 2023-06-12 11:23:15.000000 litesqlite-2.6.3/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.612458 litesqlite-2.6.3/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 11:23:38.612458 litesqlite-2.6.3/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 11:23:22.000000 litesqlite-2.6.3/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 07:33:59.318880 litesqlite-2.6.4/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.4/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 07:33:59.318880 litesqlite-2.6.4/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.4/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 07:33:59.318880 litesqlite-2.6.4/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.4/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.4/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8354 2023-06-13 07:33:19.000000 litesqlite-2.6.4/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 07:33:59.318880 litesqlite-2.6.4/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 07:33:58.000000 litesqlite-2.6.4/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-13 07:33:59.000000 litesqlite-2.6.4/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-13 07:33:58.000000 litesqlite-2.6.4/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-13 07:33:58.000000 litesqlite-2.6.4/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-13 07:33:58.000000 litesqlite-2.6.4/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-13 07:33:59.318880 litesqlite-2.6.4/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-13 07:33:19.000000 litesqlite-2.6.4/setup.py
```

### Comparing `litesqlite-2.6.3/LICENSE` & `litesqlite-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.3/PKG-INFO` & `litesqlite-2.6.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.3
+Version: 2.6.4
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.3/README.md` & `litesqlite-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.3/litesqlite/datatypes.py` & `litesqlite-2.6.4/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.3/litesqlite/lite_sqlite.py` & `litesqlite-2.6.4/litesqlite/lite_sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,26 +120,26 @@
         return self
 
     async def create_table(self,
                            table_name: str,
                            columns: Dict[str, Union[DataTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
         if not self.__conn:
-            self.__aenter__()
+            await self.__aenter__()
         await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
         await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
                           data: Dict[str, Union[str, int, float]]) -> None:
         columns = ', '.join(data.keys())
         placeholders = ', '.join(['?' for _ in range(len(data))])
         values = tuple(data.values())
         if not self.__conn:
-            self.__aenter__()
+            await self.__aenter__()
         await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
         await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], str, None] = None,
                           where: Union[str, Dict[str, Union[str, int, float]], None] = None,
@@ -161,15 +161,15 @@
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
         if not self.__conn:
-            self.__aenter__()
+            await self.__aenter__()
         await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
                                     values)
 
         if fetch == DataTypes.Fetch.FETCHONE:
             result = await self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
@@ -183,25 +183,25 @@
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
         values = tuple(set_data.values()) + tuple(where.values())
         if not self.__conn:
-            self.__aenter__()
+            await self.__aenter__()
         await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
         await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Dict[str, Union[str, int, float]]) -> None:
         where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
         values = tuple(where.values())
         if not self.__conn:
-            self.__aenter__()
+            await self.__aenter__()
         await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
         await self.__conn.commit()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if not self.__conn:
             await self.__conn.close()
```

### Comparing `litesqlite-2.6.3/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.4/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.3
+Version: 2.6.4
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.3/setup.py` & `litesqlite-2.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.3',
+    version='2.6.4',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

