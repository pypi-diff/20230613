# Comparing `tmp/FluidPyPLC-0.1.1.tar.gz` & `tmp/FluidPyPLC-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.1.tar", last modified: Tue Jun 13 18:02:29 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.2.tar", last modified: Tue Jun 13 18:41:46 2023, max compression
```

## Comparing `FluidPyPLC-0.1.1.tar` & `FluidPyPLC-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:02:29.121940 FluidPyPLC-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:02:29.109416 FluidPyPLC-0.1.1/FluidPyPLC/
--rw-rw-rw-   0        0        0     6913 2023-06-13 18:02:03.000000 FluidPyPLC-0.1.1/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.1/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-06-13 17:26:48.000000 FluidPyPLC-0.1.1/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3452 2023-06-13 17:47:18.000000 FluidPyPLC-0.1.1/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2287 2023-06-13 17:47:09.000000 FluidPyPLC-0.1.1/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.1/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.1/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.1/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14244 2023-06-13 17:57:42.000000 FluidPyPLC-0.1.1/FluidPyPLC/plc.py
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.1/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.1/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:02:29.120942 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 18:02:29.000000 FluidPyPLC-0.1.1/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-13 18:02:29.120942 FluidPyPLC-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 18:02:29.121940 FluidPyPLC-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-06-13 18:02:09.000000 FluidPyPLC-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.826069 FluidPyPLC-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.784300 FluidPyPLC-0.1.2/FluidPyPLC/
+-rw-rw-rw-   0        0        0     6864 2023-06-13 18:35:22.000000 FluidPyPLC-0.1.2/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:26:38.000000 FluidPyPLC-0.1.2/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2750 2023-06-13 18:34:40.000000 FluidPyPLC-0.1.2/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3452 2023-06-13 18:34:34.000000 FluidPyPLC-0.1.2/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2303 2023-06-13 18:35:30.000000 FluidPyPLC-0.1.2/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.2/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14244 2023-06-13 18:34:24.000000 FluidPyPLC-0.1.2/FluidPyPLC/plc.py
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.2/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.2/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:46.823516 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 18:41:46.000000 FluidPyPLC-0.1.2/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-13 18:41:46.824512 FluidPyPLC-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-06-13 18:17:26.000000 FluidPyPLC-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:41:46.826069 FluidPyPLC-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-06-13 18:36:18.000000 FluidPyPLC-0.1.2/setup.py
```

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.2/FluidPyPLC/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         check = False
 
         while True:
             event, values = window.read()
             if event is None:
                 break
             if event in (sg.WINDOW_CLOSED, 'Exit'):
-                break  # Exit the event loop when the window is closed
+                break
             if event == 'input' + '_Enter':
                 stroke = values['input']
                 check_stroke = stroke_handler(stroke)
                 if stroke == '/':
                     sg.PopupQuickMessage(' Click finish to terminate the sequence. ', background_color='Blue')
                     window['input'].update('')
```

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/data.py` & `FluidPyPLC-0.1.2/FluidPyPLC/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .get_sequence import Sequence
 from .set_groups import Groups
 from .set_switches import Switches
 from copy import deepcopy
 
 # get the number of pistons and their labels
 def pistons(s):
     piston_label = []
```

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.2/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/f.py` & `FluidPyPLC-0.1.2/FluidPyPLC/f.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # class to define the plot rendering and opening window
 class Window(Frame):
     def __init__(self,  master=None):
         Frame.__init__(self, master)
         self.master = master
         self.pack(fill=BOTH, expand=1)
         
-        load = Image.open("../Plots/phases_diagram.png")
+        load = Image.open("./Plots/phases_diagram.png")
         render = ImageTk.PhotoImage(load)
         img = Label(self, image=render)
         img.image = render
         img.place(x=0, y=0)
 
 # function to start the terminal version
 def terminal():
@@ -57,14 +57,15 @@
     parser.add_argument('--plot', action='store_true', help='show plot')
     parser.add_argument('--plc', action='store_true', help='show plc code')
     args = parser.parse_args()
     if args.gui:
         # gui mode
         gui = Gui()
         gui.gui_mode()
+        exit(0)
     elif args.terminal:
         # terminal mode
         terminal()
     elif args.plot:
         # show plot
         show_plot()
     elif args.plc:
```

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.2/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.2/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.2/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.2/FluidPyPLC/plc.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.2/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.2/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.2/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.1
+Version: 0.1.2
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.1.1/LICENSE` & `FluidPyPLC-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/PKG-INFO` & `FluidPyPLC-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.1
+Version: 0.1.2
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `FluidPyPLC-0.1.1/README.md` & `FluidPyPLC-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.1/setup.py` & `FluidPyPLC-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 LONG_DESCRIPTION = "FluidPyPLC solves complex pneumatics/oleodynamics circuits' sequences and generates an ST code to use on any PLC to run those sequences"
 
 # Setting up
 setup(
     name="FluidPyPLC",
     version=VERSION,
```

