# Comparing `tmp/FluidPyPLC-0.0.9.tar.gz` & `tmp/FluidPyPLC-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.0.9.tar", last modified: Tue Jun 13 17:47:58 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.0.tar", last modified: Tue Jun 13 17:58:19 2023, max compression
```

## Comparing `FluidPyPLC-0.0.9.tar` & `FluidPyPLC-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:47:58.387550 FluidPyPLC-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:47:58.375611 FluidPyPLC-0.0.9/FluidPyPLC/
--rw-rw-rw-   0        0        0     6798 2023-06-13 17:46:46.000000 FluidPyPLC-0.0.9/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.0.9/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.0.9/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3452 2023-06-13 17:47:18.000000 FluidPyPLC-0.0.9/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2287 2023-06-13 17:47:09.000000 FluidPyPLC-0.0.9/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.0.9/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.0.9/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.0.9/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14347 2023-06-13 17:47:28.000000 FluidPyPLC-0.0.9/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.0.9/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.0.9/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:47:58.385553 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 17:47:58.000000 FluidPyPLC-0.0.9/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 17:47:58.387550 FluidPyPLC-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 17:47:58.388547 FluidPyPLC-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-13 17:47:53.000000 FluidPyPLC-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:19.763372 FluidPyPLC-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:19.739148 FluidPyPLC-0.1.0/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6790 2023-06-13 17:56:45.000000 FluidPyPLC-0.1.0/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.0/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.1.0/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3452 2023-06-13 17:47:18.000000 FluidPyPLC-0.1.0/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2287 2023-06-13 17:47:09.000000 FluidPyPLC-0.1.0/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.0/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.0/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.0/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14244 2023-06-13 17:57:42.000000 FluidPyPLC-0.1.0/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.0/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.0/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:19.762371 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 17:58:19.000000 FluidPyPLC-0.1.0/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-13 17:58:19.763372 FluidPyPLC-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:58:19.764349 FluidPyPLC-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-13 17:56:59.000000 FluidPyPLC-0.1.0/setup.py
```

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.0/FluidPyPLC/GUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,14 @@
     return data
 
 
 class Gui():
     def __init__(self):
         self.sequence = []
         self.data = []
-    def run(self):
-        self.data = elaborate_data(self.sequence)
-        diagrams(self.sequence)
-        Plc(self.sequence)
     
     def gui_mode(self):
         section = [[sg.Multiline(expand_x = True, horizontal_scroll=True, size = (50, 29), key = 'plc_code', background_color='#BA9D79', text_color='Black')]]
 
         headings = ('N° of Blocks','Groups', 'N° of Memories','Relay Memories Labels', 'Limit Switch Enabled', 'Limit Switch Disabled')
 
         image_viewer_column = [
@@ -108,15 +104,17 @@
                     sg.PopupQuickMessage('No sequence submitted.', background_color='Red')
                 else:
                     check = close_sequence_handler(self.sequence)
                     if check is False:
                         sg.PopupQuickMessage("The sequence isn't completed.", background_color='Red')
                         continue
                     else:
-                        self.run()
+                        self.data = elaborate_data(self.sequence)
+                        diagrams(self.sequence)
+                        Plc(self.sequence)
                         dir1 = './plc/plc.st'
                         with open(dir1, 'r') as p:
                             Text = p.readlines()
                             Text = ''.join(line for line in Text)
                         window['table'].update(self.data, visible = False)
                         window['plc_code'].update(Text)
```

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/data.py` & `FluidPyPLC-0.1.0/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.0/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/f.py` & `FluidPyPLC-0.1.0/FluidPyPLC/f.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.0/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.0/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.0/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.0/FluidPyPLC/plc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from .data import Data
 from .set_switches import rotate
 
 class Plc():
     def __init__(self, s):
         self.run(s)
     def run(self, s):
-        print("Test 1")
         d = Data(s)
-        print("Test 2")
         solenoids = []
         g = len(d.groups)
         l = len(d.sequence)
         # change labels to e.g. Apositive, Bnegative, etc ..
         plc_groups = [[] for _ in range(g)]
         solenoids = [stroke.replace('+', 'positive') for stroke in d.sequence]
         solenoids = [stroke.replace('-', 'negative') for stroke in solenoids]
@@ -119,16 +117,14 @@
                 limit_switches[i] = "EB" + str(plc_range_8bit) + "." + str(plc_index_8bit)
                 plc_seen_IO.append(limit_switches[i])
                 plc_index_8bit += 1
         plc_seen_IO_description = []
         plc_seen_IO = []
         n_of_plcs_8bit = 1 + math.floor(len(set(d.sequence)) / 7)
         d.lswitch = rotate(d.lswitch, 1)
-        print(plc_groups)
-        print(solenoids)
         # open the plc.txt file and write the code, in ST language, on it
         dir = "./plc/plc.st"
         with open(dir,'w') as f:
             #relays variables ----------------------------------------------------
             f.write('PROGRAM PLC_PRG\n')
             f.write('VAR\n')
             for i in range(number_of_memories):
```

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.0/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.0/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.0/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.9
+Version: 0.1.0
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.9/LICENSE` & `FluidPyPLC-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/PKG-INFO` & `FluidPyPLC-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.0.9
+Version: 0.1.0
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.0.9/README.md` & `FluidPyPLC-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.0.9/setup.py` & `FluidPyPLC-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

