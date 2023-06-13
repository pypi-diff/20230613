# Comparing `tmp/litesqlite-2.6.5.tar.gz` & `tmp/litesqlite-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.5.tar", last modified: Tue Jun 13 17:22:35 2023, max compression
+gzip compressed data, was "litesqlite-2.6.7.tar", last modified: Tue Jun 13 17:29:24 2023, max compression
```

## Comparing `litesqlite-2.6.5.tar` & `litesqlite-2.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:22:35.063766 litesqlite-2.6.5/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.5/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:22:35.063766 litesqlite-2.6.5/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.5/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:22:35.059766 litesqlite-2.6.5/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.5/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.5/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7645 2023-06-13 17:18:30.000000 litesqlite-2.6.5/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:22:35.063766 litesqlite-2.6.5/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:22:34.000000 litesqlite-2.6.5/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-13 17:22:34.000000 litesqlite-2.6.5/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-13 17:22:34.000000 litesqlite-2.6.5/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-13 17:22:34.000000 litesqlite-2.6.5/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-13 17:22:34.000000 litesqlite-2.6.5/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-13 17:22:35.063766 litesqlite-2.6.5/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-13 17:22:10.000000 litesqlite-2.6.5/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.802501 litesqlite-2.6.7/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.7/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:29:24.802501 litesqlite-2.6.7/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3242 2023-06-13 17:29:21.000000 litesqlite-2.6.7/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.798501 litesqlite-2.6.7/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.7/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.7/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7645 2023-06-13 17:18:30.000000 litesqlite-2.6.7/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-13 17:29:24.802501 litesqlite-2.6.7/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-13 17:29:24.000000 litesqlite-2.6.7/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-13 17:29:24.802501 litesqlite-2.6.7/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-13 17:24:45.000000 litesqlite-2.6.7/setup.py
```

### Comparing `litesqlite-2.6.5/LICENSE` & `litesqlite-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.5/PKG-INFO` & `litesqlite-2.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.5
+Version: 2.6.7
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.5/README.md` & `litesqlite-2.6.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,79 @@
-<h1 align="center">EasySqlite
+<h1 align="center">LiteSqlite
 
 <h3 align="center">Теперь вам не нужно каждый раз устанавливать соединение, писать sql-запрос и закрывать соединение. Данная библиотека сделает это за вас
 
 Она поддерживает как синхронную, так и асинхронную работу
 
 </h3>
 
 ```python
 
-from easysqlite import Sqlite, AioSqlite, DataTypes
-
-# Создаём объект класса Sqlite, передавая в него имя базы данных
-
-db = Sqlite('database.db')
-
-# Создаём таблицу users с столбцами id, name, age и sex
-
-# В качестве альтернативы DataTypes вы можете просто передать тип текстом
-
-db.create_table('users', {'id': DataTypes.INTEGER(autoincrement=True, primary_key=True), 'name': DataTypes.TEXT(not_null=True), 'age': DataTypes.INTEGER(), 'sex': DataTypes.TEXT(default='М')})
-
-  
-
-# Добавляем людей
-
-db.insert_data('users', {'name': 'Анна', 'age': 20, 'sex': 'Ж'})
-
-db.insert_data('users', {'name': 'Евгений', 'age': 31})
-
-db.insert_data('users', {'name': 'Сергей', 'age': 17})
-
-  
-
-# Выбираем всех людей
-
-# '*' указывается для того, чтоб выбрать все столбцы, а fetchall - для того чтобы получить все записи списком, без него будет первая попавшая запись
-
-people = db.select_data('users', '*', fetchall=True)
-
-print(people)
-
-  
-
-# Выбираем id и имена всех мужчин
-
-# В where передаём уточнение, где ищем. В данном случае везде, где пол - мужской
-
-men = db.select_data('users', ['id', 'name'], where={'sex': 'М'}, fetchall=True)
-
-print(men)
-
-  
-
-# Прибавляем 2 года к текущему возрасту Анны
-
-# Если не передавать аргумент sign, то значение обновится на 2. Но мы передаём знак '+', чтобы к текущему значению прибавить 2
-
-db.update_data('users', {'age': 2} , where={'name': 'Анна'}, sign='+')
+from litesqlite import Sqlite, DataTypes
 
   
-
-# Выбираем возраст Анны
-
-anna = db.select_data('users', ['age'], where={'name': 'Анна'})
-
-print(anna)
-
-  
-
-# Удаляем Сергея
-
-db.delete_data('users', where={'name': 'Сергей'})
+# Используем контекстный менеджер для правильного открытия и закрытия соединения, передаём в класс имя бд
+with Sqlite('database.db'):
+    
+    # Создаём таблицу users с столбцами id, name, age и sex
+    
+    # В качестве альтернативы DataTypes вы можете просто передать тип текстом
+    
+    db.create_table('users', {'id': DataTypes.INTEGER(autoincrement=True, primary_key=True), 'name': DataTypes.TEXT(not_null=True), 'age': DataTypes.INTEGER(), 'sex': DataTypes.TEXT(default='М')})
+    
+    
+    
+    # Добавляем людей
+    
+    db.insert_data('users', {'name': 'Анна', 'age': 20, 'sex': 'Ж'})
+    
+    db.insert_data('users', {'name': 'Евгений', 'age': 31})
+    
+    db.insert_data('users', {'name': 'Сергей', 'age': 17})
+    
+    
+    
+    # Выбираем всех людей
+    
+    # '*' указывается для того, чтоб выбрать все столбцы, а FETCHALL - для того чтобы получить все записи списком, по умолчанию - FETCHONE (Одна запись)
+    
+    people = db.select_data('users', '*', fetch=DataTypes.Fetch.FETCHALL)
+    
+    print(people)
+    
+    
+    
+    # Выбираем id и имена всех мужчин
+    
+    # В where передаём уточнение, где ищем. В данном случае везде, где пол - мужской
+    
+    men = db.select_data('users', ['id', 'name'], where={'sex': 'М'}, fetch=DataTypes.Fetch.FETCHALL)
+    
+    print(men)
+    
+    
+    
+    # Прибавляем 2 года к текущему возрасту Анны
+    
+    # Если не передавать аргумент sign, то значение обновится на 2. Но мы передаём знак '+', чтобы к текущему значению прибавить 2
+    
+    db.update_data('users', {'age': 2} , where={'name': 'Анна'}, sign='+')
+    
+    
+    
+    # Выбираем возраст Анны
+    
+    anna = db.select_data('users', ['age'], where={'name': 'Анна'})
+    
+    print(anna)
+    
+    
+    
+    # Удаляем Сергея
+    
+    db.delete_data('users', where={'name': 'Сергей'})
 
 ```
 
   
 
-## Ну а для асинхронной работы всё то же самое, только использовать вместо Sqlite - Aiosqlite и во всех методах использовать ключевое слово 'await'. Ну, надеюсь, знаете, что такое асинхронность и как с ней работать:)
-
-  
-
-[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=Удачи😉)](https://git.io/typing-svg)
+### Ну а для асинхронной работы всё то же самое, только использовать вместо Sqlite - Aiosqlite, вместо with - async with и во всех методах добавлять ключевое слово 'await'. Надеюсь, знаете, что такое асинхронность и как с ней работать:)
```

### Comparing `litesqlite-2.6.5/litesqlite/datatypes.py` & `litesqlite-2.6.7/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.5/litesqlite/lite_sqlite.py` & `litesqlite-2.6.7/litesqlite/lite_sqlite.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.5/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.7/litesqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.5
+Version: 2.6.7
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.5/setup.py` & `litesqlite-2.6.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.5',
+    version='2.6.7',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

