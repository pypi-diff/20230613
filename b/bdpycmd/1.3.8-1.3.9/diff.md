# Comparing `tmp/bdpycmd-1.3.8.tar.gz` & `tmp/bdpycmd-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.8.tar", last modified: Tue Jun 13 16:43:47 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.9.tar", last modified: Tue Jun 13 17:12:34 2023, max compression
```

## Comparing `bdpycmd-1.3.8.tar` & `bdpycmd-1.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.174315 bdpycmd-1.3.8/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2680 2023-06-13 16:43:47.174473 bdpycmd-1.3.8/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     2020 2023-06-13 16:43:14.000000 bdpycmd-1.3.8/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.8/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 16:43:47.175132 bdpycmd-1.3.8/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.171638 bdpycmd-1.3.8/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.172594 bdpycmd-1.3.8/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.8/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.173596 bdpycmd-1.3.8/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.173778 bdpycmd-1.3.8/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.174216 bdpycmd-1.3.8/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     5763 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      975 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/factory/dacmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      956 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/cmd/factory/dafunc.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8133 2023-06-13 16:42:59.000000 bdpycmd-1.3.8/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:43:47.173462 bdpycmd-1.3.8/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2680 2023-06-13 16:43:47.000000 bdpycmd-1.3.8/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-06-13 16:43:47.000000 bdpycmd-1.3.8/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 16:43:47.000000 bdpycmd-1.3.8/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 16:43:47.000000 bdpycmd-1.3.8/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.980728 bdpycmd-1.3.9/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2680 2023-06-13 17:12:34.980795 bdpycmd-1.3.9/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2020 2023-06-13 16:43:14.000000 bdpycmd-1.3.9/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.9/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 17:12:34.981060 bdpycmd-1.3.9/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.978648 bdpycmd-1.3.9/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.979396 bdpycmd-1.3.9/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.9/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.979986 bdpycmd-1.3.9/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.980188 bdpycmd-1.3.9/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.980619 bdpycmd-1.3.9/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     5763 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      975 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/factory/dacmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      946 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/cmd/factory/dafunc.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8133 2023-06-13 17:12:10.000000 bdpycmd-1.3.9/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:34.979879 bdpycmd-1.3.9/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2680 2023-06-13 17:12:34.000000 bdpycmd-1.3.9/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-06-13 17:12:34.000000 bdpycmd-1.3.9/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 17:12:34.000000 bdpycmd-1.3.9/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 17:12:34.000000 bdpycmd-1.3.9/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.8/PKG-INFO` & `bdpycmd-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.8
+Version: 1.3.9
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `bdpycmd-1.3.8/README.md` & `bdpycmd-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.8/setup.cfg` & `bdpycmd-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.8
+version = 1.3.9
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.8/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.9/src/bdpycmd/cmd/camp/assistant.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.8/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.9/src/bdpycmd/cmd/factory/base.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.8/src/bdpycmd/cmd/factory/dacmd.py` & `bdpycmd-1.3.9/src/bdpycmd/cmd/factory/dacmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,21 @@
         Describe information
         """
         return f"""
         ------------------------------
         {self.name}
                 Number: {self.number}
                 {self.alias}
-                {self.desc}
-                    
-        """
+                {self.desc}   
+        """.rstrip()
 
     
     def info(self,) -> str:
         """
         Describe information
         """
         return f"""
         ++++++++++++++++++++++++++++++
         {self.name}
                 {self.alias}
                 {self.desc}
-        """
+        """.rstrip()
```

### Comparing `bdpycmd-1.3.8/src/bdpycmd/cmd/factory/dafunc.py` & `bdpycmd-1.3.9/src/bdpycmd/cmd/factory/dafunc.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,25 +23,23 @@
     
 
     def say(self,) -> str:
         """
         Describe information
         """
         return f"""
-        ******************************
-        {self.cname}
+        *** method run ***************
+        {self.cname} . {self.name}
                 Number: {self.number}
-                {self.name}
                 {self.desc}  
-        """
+        """.rstrip()
 
 
     def info(self,) -> str:
         """
         Describe information
         """
         return f"""
-        ++++++++++++++++++++++++++++++
-        {self.cname} 
-                {self.name}
+        +++ method info +++++++++++++++
+        {self.cname} . {self.name}
                 {self.desc}
-        """
+        """.rstrip()
```

### Comparing `bdpycmd-1.3.8/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.9/src/bdpycmd/pycmd.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.8/src/bdpycmd.egg-info/PKG-INFO` & `bdpycmd-1.3.9/src/bdpycmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.8
+Version: 1.3.9
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

