# Comparing `tmp/bdpycmd-1.3.3.tar.gz` & `tmp/bdpycmd-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.3.tar", last modified: Tue Jun 13 12:27:18 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.4.tar", last modified: Tue Jun 13 12:32:08 2023, max compression
```

## Comparing `bdpycmd-1.3.3.tar` & `bdpycmd-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.167132 bdpycmd-1.3.3/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:27:18.167203 bdpycmd-1.3.3/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.3/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.3/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:27:18.167477 bdpycmd-1.3.3/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.164726 bdpycmd-1.3.3/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.165523 bdpycmd-1.3.3/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.3/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166400 bdpycmd-1.3.3/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166641 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.167033 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     4110 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/cmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8247 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166121 bdpycmd-1.3.3/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.117358 bdpycmd-1.3.4/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:32:08.117419 bdpycmd-1.3.4/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.4/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.4/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:32:08.117678 bdpycmd-1.3.4/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.115116 bdpycmd-1.3.4/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116039 bdpycmd-1.3.4/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.4/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116663 bdpycmd-1.3.4/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116861 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.117242 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     4110 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.4/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8321 2023-06-13 12:32:00.000000 bdpycmd-1.3.4/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:32:08.116556 bdpycmd-1.3.4/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:32:08.000000 bdpycmd-1.3.4/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.3/PKG-INFO` & `bdpycmd-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.3
+Version: 1.3.4
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `bdpycmd-1.3.3/README.md` & `bdpycmd-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.3/setup.cfg` & `bdpycmd-1.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.3
+version = 1.3.4
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.3/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.4/src/bdpycmd/cmd/camp/assistant.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.3/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.4/src/bdpycmd/cmd/factory/base.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.3/src/bdpycmd/cmd/factory/cmd.py` & `bdpycmd-1.3.4/src/bdpycmd/cmd/factory/cmd.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.3/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.4/src/bdpycmd/pycmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,25 +120,27 @@
                 break
             
             if keyword == checked:
                 break
             
             if not keyword:
                 for _cmd in cms:
+                    tag_cmd = _cmd
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
+                        tag_cmd = _cmd
                         keyword = input(_cmd.say()).strip()
                         if not keyword or keyword == _word:
                             continue
                         else:
                             break
                 else:
                     break
```

### Comparing `bdpycmd-1.3.3/src/bdpycmd.egg-info/PKG-INFO` & `bdpycmd-1.3.4/src/bdpycmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.3
+Version: 1.3.4
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

