# Comparing `tmp/FluidPyPLC-0.0.7.tar.gz` & `tmp/FluidPyPLC-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.0.7.tar", last modified: Tue Jun 13 17:33:57 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.0.8.tar", last modified: Tue Jun 13 17:45:16 2023, max compression
```

## Comparing `FluidPyPLC-0.0.7.tar` & `FluidPyPLC-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.396731 FluidPyPLC-0.0.7/FluidPyPLC/
--rw-rw-rw-   0        0        0     6800 2023-06-13 17:27:39.000000 FluidPyPLC-0.0.7/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.0.7/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.0.7/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3453 2023-06-13 17:26:54.000000 FluidPyPLC-0.0.7/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2288 2023-06-13 17:33:28.000000 FluidPyPLC-0.0.7/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.7/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14298 2023-06-13 17:27:45.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.7/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.7/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.419796 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-13 17:33:53.000000 FluidPyPLC-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:16.587005 FluidPyPLC-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:16.563525 FluidPyPLC-0.0.8/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6800 2023-06-13 17:27:39.000000 FluidPyPLC-0.0.8/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.0.8/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.0.8/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3453 2023-06-13 17:26:54.000000 FluidPyPLC-0.0.8/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2287 2023-06-13 17:43:46.000000 FluidPyPLC-0.0.8/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.8/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.8/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.8/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14348 2023-06-13 17:43:03.000000 FluidPyPLC-0.0.8/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.8/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.8/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:45:16.586058 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 17:45:16.000000 FluidPyPLC-0.0.8/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:45:16.587005 FluidPyPLC-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:45:16.587994 FluidPyPLC-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-13 17:44:54.000000 FluidPyPLC-0.0.8/setup.py
```

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/GUI.py` & `FluidPyPLC-0.0.8/FluidPyPLC/GUI.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/data.py` & `FluidPyPLC-0.0.8/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.0.8/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/f.py` & `FluidPyPLC-0.0.8/FluidPyPLC/f.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         terminal()
     elif args.plot:
         # show plot
         show_plot()
     elif args.plc:
         try:
             # open plc ST code with notepad
-            subprocess.call(['notepad.exe', '../plc/plc.st'])
+            subprocess.call(['notepad.exe', './plc/plc.st'])
         except:
             print("There is a problem opening the file.")
     else:
         # default argument
         terminal()
 
 main()
```

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.0.8/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.0.8/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.0.8/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/plc.py` & `FluidPyPLC-0.0.8/FluidPyPLC/plc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from .data import Data
 from .set_switches import rotate
 
 class Plc():
     def __init__(self, s):
         self.run(s)
     def run(self, s):
+        print("Test 1")
         d = Data(s)
+        print("Test 2")
         solenoids = []
         g = len(d.groups)
         l = len(d.sequence)
         # change labels to e.g. Apositive, Bnegative, etc ..
         plc_groups = [[] for _ in range(g)]
         solenoids = [stroke.replace('+', 'positive') for stroke in d.sequence]
         solenoids = [stroke.replace('-', 'negative') for stroke in solenoids]
```

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.0.8/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.0.8/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.0.8/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.7
+Version: 0.0.8
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.7/LICENSE` & `FluidPyPLC-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/PKG-INFO` & `FluidPyPLC-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.7
+Version: 0.0.8
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.7/README.md` & `FluidPyPLC-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.7/setup.py` & `FluidPyPLC-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

