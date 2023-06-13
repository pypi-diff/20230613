# Comparing `tmp/FluidPyPLC-0.0.1.tar.gz` & `tmp/FluidPyPLC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.0.1.tar", last modified: Tue Jun 13 18:20:25 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.0.2.tar", last modified: Tue Jun 13 16:53:33 2023, max compression
```

## Comparing `FluidPyPLC-0.0.1.tar` & `FluidPyPLC-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:25.466707 FluidPyPLC-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:25.453801 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 18:20:25.000000 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-13 18:20:25.000000 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:20:25.000000 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 18:20:25.000000 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 18:20:25.000000 FluidPyPLC-0.0.1/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 18:20:25.465677 FluidPyPLC-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 18:20:25.466707 FluidPyPLC-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-06-13 18:19:40.000000 FluidPyPLC-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:25.454667 FluidPyPLC-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:25.464686 FluidPyPLC-0.0.1/src/FluidPyPLC/
--rw-rw-rw-   0        0        0     6796 2023-06-08 08:26:41.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 16:14:08.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2783 2023-05-30 21:05:39.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3452 2023-06-13 18:01:07.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2263 2023-06-13 18:11:06.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14296 2023-06-11 21:39:14.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.1/src/FluidPyPLC/set_switches.py
--rw-rw-rw-   0        0        0       27 2023-06-13 18:11:20.000000 FluidPyPLC-0.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:53:33.368838 FluidPyPLC-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:53:33.325301 FluidPyPLC-0.0.2/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6796 2023-06-08 08:26:41.000000 FluidPyPLC-0.0.2/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:14:08.000000 FluidPyPLC-0.0.2/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2783 2023-05-30 21:05:39.000000 FluidPyPLC-0.0.2/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3452 2023-06-13 18:01:07.000000 FluidPyPLC-0.0.2/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2263 2023-06-13 18:11:06.000000 FluidPyPLC-0.0.2/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.2/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.2/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.2/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14296 2023-06-11 21:39:14.000000 FluidPyPLC-0.0.2/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.2/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.2/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:53:33.366908 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-13 16:53:33.000000 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-06-13 16:53:33.000000 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:53:33.000000 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-13 16:53:33.000000 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 16:53:33.000000 FluidPyPLC-0.0.2/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-13 16:53:33.367844 FluidPyPLC-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:53:33.368838 FluidPyPLC-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-06-13 16:52:41.000000 FluidPyPLC-0.0.2/setup.py
```

### Comparing `FluidPyPLC-0.0.1/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.0.2/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.1
+Version: 0.0.2
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.1/LICENSE` & `FluidPyPLC-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/PKG-INFO` & `FluidPyPLC-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.1
+Version: 0.0.2
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.1/README.md` & `FluidPyPLC-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/setup.py` & `FluidPyPLC-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/GUI.py` & `FluidPyPLC-0.0.2/FluidPyPLC/GUI.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/data.py` & `FluidPyPLC-0.0.2/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.0.2/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/f.py` & `FluidPyPLC-0.0.2/FluidPyPLC/f.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.0.2/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.0.2/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.0.2/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/plc.py` & `FluidPyPLC-0.0.2/FluidPyPLC/plc.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.0.2/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.1/src/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.0.2/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

