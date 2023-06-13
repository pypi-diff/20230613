# Comparing `tmp/funcStats-0.1.0.tar.gz` & `tmp/funcStats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.1.0.tar", last modified: Tue Jun 13 01:52:05 2023, max compression
+gzip compressed data, was "funcStats-0.1.1.tar", last modified: Tue Jun 13 02:03:36 2023, max compression
```

## Comparing `funcStats-0.1.0.tar` & `funcStats-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.370698 funcStats-0.1.0/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-13 01:44:59.000000 funcStats-0.1.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 01:52:05.370321 funcStats-0.1.0/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.366378 funcStats-0.1.0/config/
--rw-r--r--   0 tom        (501) staff       (20)     6367 2023-06-13 01:50:30.000000 funcStats-0.1.0/config/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.367457 funcStats-0.1.0/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)     4196 2023-06-13 01:44:59.000000 funcStats-0.1.0/funcStats/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-13 01:44:59.000000 funcStats-0.1.0/funcStats/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.369763 funcStats-0.1.0/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 01:52:05.370829 funcStats-0.1.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      968 2023-06-13 01:51:53.000000 funcStats-0.1.0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.965004 funcStats-0.1.1/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-13 01:44:59.000000 funcStats-0.1.1/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 02:03:36.964219 funcStats-0.1.1/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.955305 funcStats-0.1.1/config/
+-rw-r--r--   0 tom        (501) staff       (20)     6367 2023-06-13 01:50:30.000000 funcStats-0.1.1/config/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.957522 funcStats-0.1.1/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     3884 2023-06-13 02:02:45.000000 funcStats-0.1.1/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-13 01:44:59.000000 funcStats-0.1.1/funcStats/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.963034 funcStats-0.1.1/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 02:03:36.965253 funcStats-0.1.1/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      968 2023-06-13 02:03:18.000000 funcStats-0.1.1/setup.py
```

### Comparing `funcStats-0.1.0/LICENSE` & `funcStats-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.0/PKG-INFO` & `funcStats-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.1.0/config/__init__.py` & `funcStats-0.1.1/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.0/funcStats/__init__.py` & `funcStats-0.1.1/funcStats/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,17 +17,14 @@
         self.toFile = toFile
         self.count = 0
 
         # default definitions to overwrite
         self.target = info
         self.loopCount = 1
 
-        # more complex stuff
-        #self.thread = Thread(target=target, args=args)
-
         if self.func is None:
             raise Exception("Monitor needs a method to watch, please use the 'target' argument or the first positional "
                             "argument to set it.")
         else:
             try:
 
                 self.mode = ''
@@ -43,88 +40,88 @@
 
                 self.logStream.add(f"Target Info: {self.targetInfo}")
 
             except TypeError:
                 raise Exception("Impossible to monitor. Not a function or method provided.")
 
     def getInfo(self):
-        # Get the function's name
         self.targetName = self.func.__name__
 
-        # Get the function's arguments
         self.target.signature = inspect.signature(self.func)
         self.targetArgs = list(self.target.signature.parameters.keys())
 
-        # Get the function's docstring
         self.target.as_string = self.func.__doc__
 
-        # Check if the function is a method
         self.target.is_method = inspect.ismethod(self.func)
 
-        # Check if the function is a generator
         self.target.is_generator = inspect.isgeneratorfunction(self.func)
 
-        # Get the function's source code
         self.target.source_code = inspect.getsource(self.func)
 
-        # Get the file name and line number where the function is defined
         self.target.source_location = inspect.getsourcelines(self.func)
 
         self.targetFilename = self.target.source_location[0]
         self.targetLineNumber = self.target.source_location[1]
 
-        # Get the function's module name
         self.targetModule = inspect.getmodule(self.func).__name__
 
-        # Create a dictionary to store the information
         targetInfo = {
             "name": self.targetName,
             "arguments": self.targetArgs,
             "file_name": self.targetFilename,
             "line_number": self.targetLineNumber,
             "module": self.targetModule
         }
 
         return targetInfo
 
-    def meter(self, args: list, loops: int = 1):
+    def meter(self, args: list = None, loops: int = 1):
         self.logStream.skipLine()
 
         self.logStream.add(f'Meter: Loading args... {args}')
 
         self.count = 0
 
-        for argPack in args:
-
-            for i in range(loops):
-
-                self.count += 1
-                self.loopCount += 1
+        if args is not None:
+            for argPack in args:
+                self.run(argPack, loops)
+        else:
+            self.run(None, loops)
 
-                startTime = datetime.now()
 
-                self.logStream.skipLine()
-                self.logStream.add(f'Meter Execution Count: {self.count}')
-                self.logStream.add(f"Meter Execution Starts at: {startTime}")
-                self.logStream.add(f"Meter Execution Args: {argPack}")
+    def run(self, argPack, loops):
+        for i in range(loops):
 
-                try:
-                    if not isinstance(argPack, str):
-                        executionResult = str(self.func(*argPack))
-                    else:
-                        executionResult = str(self.func(argPack))
-                except Exception as e:
-                    executionResult = e
+            self.count += 1
+            self.loopCount += 1
 
-                self.logStream.add(f"Meter Execution Returns: {str(executionResult)}...")
+            startTime = datetime.now()
 
-                endTime = datetime.now()
+            self.logStream.skipLine()
+            self.logStream.add(f'Meter Execution Count: {self.count}')
+            self.logStream.add(f"Meter Execution Starts at: {startTime}")
+            self.logStream.add(f"Meter Execution Args: {argPack}")
 
-                duration = endTime - startTime
+            try:
+                if not isinstance(argPack, str):
+                    executionResult = str(self.func(*argPack))
+                elif isinstance(argPack, str):
+                    executionResult = str(self.func(argPack))
+                elif argPack is None:
+                    executionResult = str(self.func())
+            except Exception as e:
+                executionResult = e
+
+            self.logStream.add(f"Meter Execution Returns: {str(executionResult)}...")
+
+            endTime = datetime.now()
+
+            duration = endTime - startTime
+
+            hours = duration.seconds // 3600
+            minutes = (duration.seconds % 3600) // 60
+            seconds = duration.seconds % 60
+            milliseconds = duration.microseconds // 1000
 
-                hours = duration.seconds // 3600
-                minutes = (duration.seconds % 3600) // 60
-                seconds = duration.seconds % 60
-                milliseconds = duration.microseconds // 1000
+            self.logStream.add(f"Meter Execution Takes: {hours}h {minutes}m {seconds}s {milliseconds}ms")
+            self.logStream.skipLine()
 
-                self.logStream.add(f"Meter Execution Takes: {hours}h {minutes}m {seconds}s {milliseconds}ms")
-                self.logStream.skipLine()
```

### Comparing `funcStats-0.1.0/funcStats/log.py` & `funcStats-0.1.1/funcStats/log.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.0/funcStats.egg-info/PKG-INFO` & `funcStats-0.1.1/funcStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.1.0/setup.py` & `funcStats-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
 from config import LONG_DESCRIPTION
 this_directory = Path(__file__).parent
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
     author_email="<info@elemental.run>",
```

