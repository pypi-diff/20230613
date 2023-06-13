# Comparing `tmp/FluidPyPLC-0.0.6.tar.gz` & `tmp/FluidPyPLC-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.0.6.tar", last modified: Tue Jun 13 17:28:26 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.0.7.tar", last modified: Tue Jun 13 17:33:57 2023, max compression
```

## Comparing `FluidPyPLC-0.0.6.tar` & `FluidPyPLC-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:28:26.236029 FluidPyPLC-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:28:26.221972 FluidPyPLC-0.0.6/FluidPyPLC/
--rw-rw-rw-   0        0        0     6800 2023-06-13 17:27:39.000000 FluidPyPLC-0.0.6/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.0.6/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.0.6/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3453 2023-06-13 17:26:54.000000 FluidPyPLC-0.0.6/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2293 2023-06-13 17:27:15.000000 FluidPyPLC-0.0.6/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.6/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.6/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.6/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14298 2023-06-13 17:27:45.000000 FluidPyPLC-0.0.6/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.6/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.6/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:28:26.235017 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 17:28:26.000000 FluidPyPLC-0.0.6/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 17:28:26.236029 FluidPyPLC-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 17:28:26.236029 FluidPyPLC-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-13 17:28:11.000000 FluidPyPLC-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.396731 FluidPyPLC-0.0.7/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6800 2023-06-13 17:27:39.000000 FluidPyPLC-0.0.7/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.0.7/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.0.7/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3453 2023-06-13 17:26:54.000000 FluidPyPLC-0.0.7/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2288 2023-06-13 17:33:28.000000 FluidPyPLC-0.0.7/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.7/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14298 2023-06-13 17:27:45.000000 FluidPyPLC-0.0.7/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.7/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.7/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:33:57.419796 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 17:33:57.000000 FluidPyPLC-0.0.7/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:33:57.420800 FluidPyPLC-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-13 17:33:53.000000 FluidPyPLC-0.0.7/setup.py
```

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/GUI.py` & `FluidPyPLC-0.0.7/FluidPyPLC/GUI.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/data.py` & `FluidPyPLC-0.0.7/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.0.7/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/f.py` & `FluidPyPLC-0.0.7/FluidPyPLC/f.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     root = Tk()
     app = Window(root)
     root.wm_title("Diagram's fases")
     root.geometry("600x500")
     root.mainloop()
 
 # args management
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(
         description='FluidPyPLC',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog=textwrap.dedent('''Example:
         f.py --gui # to use the user interface mode
         f.py -t # to use the terminal version
         f.py --plot # to display the Diagrams's fases
@@ -71,8 +71,10 @@
         try:
             # open plc ST code with notepad
             subprocess.call(['notepad.exe', '../plc/plc.st'])
         except:
             print("There is a problem opening the file.")
     else:
         # default argument
-        terminal()
+        terminal()
+
+main()
```

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.0.7/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.0.7/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.0.7/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/plc.py` & `FluidPyPLC-0.0.7/FluidPyPLC/plc.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.0.7/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.0.7/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.0.7/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.6
+Version: 0.0.7
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.6/LICENSE` & `FluidPyPLC-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/PKG-INFO` & `FluidPyPLC-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.6
+Version: 0.0.7
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.6/README.md` & `FluidPyPLC-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.6/setup.py` & `FluidPyPLC-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

