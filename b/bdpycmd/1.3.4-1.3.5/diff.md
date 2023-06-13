# Comparing `tmp/bdpycmd-1.3.4.tar.gz` & `tmp/bdpycmd-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.4.tar", last modified: Tue Jun 13 12:32:08 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.5.tar", last modified: Tue Jun 13 12:39:16 2023, max compression
```

## Comparing `bdpycmd-1.3.4.tar` & `bdpycmd-1.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.117358 bdpycmd-1.3.4/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:32:08.117419 bdpycmd-1.3.4/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.4/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.4/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:32:08.117678 bdpycmd-1.3.4/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.115116 bdpycmd-1.3.4/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116039 bdpycmd-1.3.4/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.4/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116663 bdpycmd-1.3.4/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116861 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.117242 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     4110 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/cmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8321 2023-06-13 12:32:00.000000 bdpycmd-1.3.4/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116556 bdpycmd-1.3.4/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965275 bdpycmd-1.3.5/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.965357 bdpycmd-1.3.5/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.5/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.5/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:39:16.965645 bdpycmd-1.3.5/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.962929 bdpycmd-1.3.5/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.963689 bdpycmd-1.3.5/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.5/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964298 bdpycmd-1.3.5/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964479 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965159 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     4132 2023-06-13 12:39:09.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8331 2023-06-13 12:39:08.000000 bdpycmd-1.3.5/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964191 bdpycmd-1.3.5/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.4/PKG-INFO` & `bdpycmd-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.4
+Version: 1.3.5
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `bdpycmd-1.3.4/README.md` & `bdpycmd-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.4/setup.cfg` & `bdpycmd-1.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.4
+version = 1.3.5
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.4/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.4/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         :param alias: str #alias for the command
         :param description: str #a description of the function of the command
         """
         self.name = name.split('.')[-1] + '.Command'
         self.alias = alias + 'command'
         self.description = description
         self.info = CmdMeta(
+            number=0,
             name=name,
             alias=alias,
             desc=description
         )
         #Methods not shown in the help information
         self.protected_methods = {'__init__','as_cmder'}
```

### Comparing `bdpycmd-1.3.4/src/bdpycmd/cmd/factory/cmd.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.4/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.5/src/bdpycmd/pycmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,27 +120,27 @@
                 break
             
             if keyword == checked:
                 break
             
             if not keyword:
                 for _cmd in cms:
-                    tag_cmd = _cmd
+                    tag_cmd = _cmd.name
                     keyword = input(_cmd.say()).strip()
                     if not keyword:
                         continue
                     else:
                         break
                 else:
                     break
             else:
                 _word = keyword
                 for _cmd in cms:
                     if _cmd.search(_word):
-                        tag_cmd = _cmd
+                        tag_cmd = _cmd.name
                         keyword = input(_cmd.say()).strip()
                         if not keyword or keyword == _word:
                             continue
                         else:
                             break
                 else:
                     break
```

### Comparing `bdpycmd-1.3.4/src/bdpycmd.egg-info/PKG-INFO` & `bdpycmd-1.3.5/src/bdpycmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.4
+Version: 1.3.5
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

