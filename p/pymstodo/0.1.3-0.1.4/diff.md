# Comparing `tmp/pymstodo-0.1.3.tar.gz` & `tmp/pymstodo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymstodo-0.1.3.tar", last modified: Thu May 11 13:56:57 2023, max compression
+gzip compressed data, was "pymstodo-0.1.4.tar", last modified: Tue Jun 13 05:46:44 2023, max compression
```

## Comparing `pymstodo-0.1.3.tar` & `pymstodo-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 13:56:48.000000 pymstodo-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 13:56:57.640868 pymstodo-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 13:56:48.000000 pymstodo-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/pymstodo/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 13:56:48.000000 pymstodo-0.1.3/pymstodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-05-11 13:56:48.000000 pymstodo-0.1.3/pymstodo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:56:57.640868 pymstodo-0.1.3/pymstodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 13:56:57.000000 pymstodo-0.1.3/pymstodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:56:57.640868 pymstodo-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-11 13:56:48.000000 pymstodo-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 05:46:35.000000 pymstodo-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 05:46:44.078767 pymstodo-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-13 05:46:35.000000 pymstodo-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 05:46:35.000000 pymstodo-0.1.4/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-06-13 05:46:35.000000 pymstodo-0.1.4/pymstodo/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:46:44.078767 pymstodo-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 05:46:35.000000 pymstodo-0.1.4/setup.py
```

### Comparing `pymstodo-0.1.3/LICENSE` & `pymstodo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.3/PKG-INFO` & `pymstodo-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -48,9 +48,10 @@
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
 print(*tasks, sep='\n')
 ```
-3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
-API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
+3. Full documentation: https://inbalboa.github.io/pymstodo/
+
+4. API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.1.3/README.md` & `pymstodo-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
 print(*tasks, sep='\n')
 ```
-3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
-API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
+3. Full documentation: https://inbalboa.github.io/pymstodo/
+
+4. API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.1.3/pymstodo/client.py` & `pymstodo-0.1.4/pymstodo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
     Args:
         client_id: API client ID
         client_secret: API client secret
         token: Token obtained by method `get_token`        
     '''
     _redirect: str = 'https://localhost/login/authorized'
-    _scope: str = 'openid offline_access tasks.readwrite'
+    _scope: str = 'openid Tasks.ReadWrite'
     _authority: str = 'https://login.microsoftonline.com/common'
     _authorize_endpoint: str = '/oauth2/v2.0/authorize'
     _token_endpoint: str = '/oauth2/v2.0/token'
     _base_api_url: str = 'https://graph.microsoft.com/v1.0/me/todo/'
 
     def __init__(self, client_id: str, client_secret: str, token: Token) -> None:
         self.client_id: str = client_id
```

### Comparing `pymstodo-0.1.3/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.4/pymstodo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -48,9 +48,10 @@
 lists = todo_client.get_lists()
 task_list = lists[0]
 tasks = todo_client.get_tasks(task_list.list_id)
 
 print(task_list)
 print(*tasks, sep='\n')
 ```
-3. Full description of library objects and methods: https://raw.githubusercontent.com/inbalboa/pymstodo/master/docs/index.html
-API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
+3. Full documentation: https://inbalboa.github.io/pymstodo/
+
+4. API description by Microsoft see at https://docs.microsoft.com/en-us/graph/api/resources/todo-overview
```

### Comparing `pymstodo-0.1.3/setup.py` & `pymstodo-0.1.4/setup.py`

 * *Files identical despite different names*

