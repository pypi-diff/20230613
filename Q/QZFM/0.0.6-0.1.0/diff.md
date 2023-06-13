# Comparing `tmp/QZFM-0.0.6.tar.gz` & `tmp/QZFM-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QZFM-0.0.6.tar", last modified: Tue Jun  6 18:39:28 2023, max compression
+gzip compressed data, was "QZFM-0.1.0.tar", last modified: Tue Jun 13 20:00:02 2023, max compression
```

## Comparing `QZFM-0.0.6.tar` & `QZFM-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.6/LICENSE
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-06 18:39:28.022713 QZFM-0.0.6/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9333 2023-05-31 19:47:23.000000 QZFM-0.0.6/README.md
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-06-06 18:39:18.000000 QZFM-0.0.6/pyproject.toml
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-06-06 18:39:28.022713 QZFM-0.0.6/setup.cfg
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/src/
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-06 18:39:28.022713 QZFM-0.0.6/src/QZFM.egg-info/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/SOURCES.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/dependency_links.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/requires.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-06-06 18:39:28.000000 QZFM-0.0.6/src/QZFM.egg-info/top_level.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33719 2023-06-06 18:39:18.000000 QZFM-0.0.6/src/QZFM.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.6/src/__init__.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-13 20:00:02.774401 QZFM-0.1.0/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.1.0/LICENSE
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-13 20:00:02.774401 QZFM-0.1.0/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9333 2023-05-31 19:47:23.000000 QZFM-0.1.0/README.md
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      814 2023-06-13 19:59:38.000000 QZFM-0.1.0/pyproject.toml
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-06-13 20:00:02.774401 QZFM-0.1.0/setup.cfg
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-13 20:00:02.774401 QZFM-0.1.0/src/
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-13 20:00:02.774401 QZFM-0.1.0/src/QZFM.egg-info/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-13 20:00:02.000000 QZFM-0.1.0/src/QZFM.egg-info/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-06-13 20:00:02.000000 QZFM-0.1.0/src/QZFM.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-06-13 20:00:02.000000 QZFM-0.1.0/src/QZFM.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       55 2023-06-13 20:00:02.000000 QZFM-0.1.0/src/QZFM.egg-info/requires.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-06-13 20:00:02.000000 QZFM-0.1.0/src/QZFM.egg-info/top_level.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    35795 2023-06-13 19:59:21.000000 QZFM-0.1.0/src/QZFM.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.1.0/src/__init__.py
```

### Comparing `QZFM-0.0.6/LICENSE` & `QZFM-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.6/PKG-INFO` & `QZFM-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `QZFM-0.0.6/README.md` & `QZFM-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.6/pyproject.toml` & `QZFM-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QZFM"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
   { name="Derek Fujimoto", email="dfujimoto@triumf.ca" },
 ]
 description = "Python class for serial communication with QuSpin Zero Field Magnetometer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -24,13 +24,14 @@
 ]
 dependencies = [
     "numpy",
     "matplotlib",
     "pyserial",
     "datetime",
     "tqdm",
-    "pandas"
+    "pandas",
+    "plotext"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ucn-triumf/QZFM"
 "Bug Tracker" = "https://github.com/ucn-triumf/QZFM/issues"
```

### Comparing `QZFM-0.0.6/src/QZFM.egg-info/PKG-INFO` & `QZFM-0.1.0/src/QZFM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QZFM
-Version: 0.0.6
+Version: 0.1.0
 Summary: Python class for serial communication with QuSpin Zero Field Magnetometer
 Author-email: Derek Fujimoto <dfujimoto@triumf.ca>
 Project-URL: Homepage, https://github.com/ucn-triumf/QZFM
 Project-URL: Bug Tracker, https://github.com/ucn-triumf/QZFM/issues
 Keywords: QZFM,QuSpin,Magnetometer,Zero Field
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `QZFM-0.0.6/src/QZFM.py` & `QZFM-0.1.0/src/QZFM.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,21 @@
 import matplotlib.pyplot as plt
 import serial
 from tqdm import tqdm
 
 from serial.tools import list_ports
 from time import time
 from datetime import datetime
+import plotext as pltt
+
+try:
+    matplotlib.use('TkAgg')
+except (ModuleNotFoundError, ImportError):
+    print('Failed to use backend "TkAgg"')
 
-matplotlib.use('TkAgg')
 
 class QZFM(object):
     """Low-level control of QuSpin magnetic sensor via QZFM serial commands via USB
 
     Attributes:
 
         axis_mode (str):            readback mode for daq
@@ -265,27 +270,43 @@
 
     def disconnect(self):
         """Disconnect from QuSpin"""
         self._set_data_stream(False)
         self.reboot()
         self.ser.close()
 
-    def draw_data(self):
-        """Draw data to window"""
+    def draw_data(self, ascii=False):
+        """Draw data to window
 
-        # plot
-        plt.figure(figsize=(10,6))
-        plt.plot(self.time-self.time[0], self.field)
+        Args:
+            ascii (bool): if True, draw to stdout
+        """
 
-        # plot elements
-        plt.ylabel(f'$B_{self.read_axis}$ (pT)')
-        plt.xlabel(f'Time Elapsed Since {datetime.fromtimestamp(self.time[0])} (s)',
-                    fontsize='small')
-        plt.tight_layout()
-        plt.show(block=False)
+        # use matplotlib for normal output
+        if not ascii:
+            # plot
+            plt.figure(figsize=(10,6))
+            plt.plot(self.time-self.time[0], self.field)
+
+            # plot elements
+            plt.ylabel(f'$B_{self.read_axis}$ (pT)')
+            plt.xlabel(f'Time Elapsed Since {datetime.fromtimestamp(self.time[0])} (s)',
+                        fontsize='small')
+            plt.tight_layout()
+            plt.show(block=False)
+
+        # use plotext for ascii output
+        else:
+            pltt.plotsize(80, 30)
+            pltt.grid(True, True)
+            pltt.clc()
+            pltt.plot(self.time-self.time[0], self.field)
+            pltt.ylabel(f'$B_{self.read_axis}$ (pT)')
+            pltt.xlabel(f'Time Elapsed Since {datetime.fromtimestamp(self.time[0])} (s)')
+            pltt.show()
 
     def field_reset(self):
         """Sets the internal coil field values to zero"""
         self.ser.write(b'V')
         self._get_next_message()
         self.sensor_par['Bz field (pT)'] = 0
         self.sensor_par['By field (pT)'] = 0
@@ -473,107 +494,147 @@
                 # print n events in buffer
                 print(f'N events remaining in buffer: {self.ser.in_waiting}',
                       flush=True, end='\r')
 
         except KeyboardInterrupt:
             print()
 
-    def monitor_data(self, axis='z', window_s=10, figsize=(10, 6)):
+    def monitor_data(self, axis='z', window_s=10, figsize=None, ascii=False):
         """Continuously stream data to window
 
             See https://matplotlib.org/stable/tutorials/advanced/blitting.html
 
         Args:
             axis (str): x|y|z
             window_s (int): show the last window_s seconds of data on the stream
-            figsize (tuple):  size of display
+            figsize (tuple):  size of display (x, y)
+            ascii (bool): if true, display figure in terminal window
         """
 
+        # get default figsize
+        if figsize is None:
+            if ascii:
+                figsize=(200, 50)
+            else:
+                figsize=(10, 6)
+
         # get npts to show
         npts = self.data_read_rate * window_s
 
         # set data to stream
         if not self.is_data_streaming:
             self._set_data_stream()
 
         # make figure
-        fig, ax = plt.subplots(figsize=figsize)
+        if not ascii:
+            fig, ax = plt.subplots(figsize=figsize)
+        else:
+            pltt.clf()
+            pltt.plotsize(*figsize)
+            pltt.grid(True, True)
+            pltt.clc()
+            pltt.ylabel(f'$B_{self.read_axis}$ (pT)')
+            pltt.xlabel(f'Time (s)')
+
 
         # draw initial window
         x = (-np.arange(npts)/self.data_read_rate)[::-1]
         t, y = self.read_data(window_s, axis=axis, clear_buffer=True)
-        (line,) = plt.plot(x, y, animated=True)
 
-        # plot elements
-        plt.ylabel(f'$B_{self.read_axis}$ (pT)')
-        plt.xlabel(f'Time (s)')
-        plt.tight_layout()
+        if not ascii:
+            (line,) = plt.plot(x, y, animated=True)
 
-        # render
-        plt.show(block=False)
-        plt.pause(0.05)
+            # plot elements
+            plt.ylabel(f'$B_{self.read_axis}$ (pT)')
+            plt.xlabel(f'Time (s)')
+            plt.tight_layout()
 
-        # get bounding box
-        bg = fig.canvas.copy_from_bbox(fig.bbox)
+            # render
+            plt.show(block=False)
+            plt.pause(0.05)
 
-        # draw
-        ax.draw_artist(line)
+            # get bounding box
+            bg = fig.canvas.copy_from_bbox(fig.bbox)
 
-        # show
-        fig.canvas.blit(fig.bbox)
+            # draw
+            ax.draw_artist(line)
 
-        # get bounds
-        ylim = ax.get_ylim()
+            # show
+            fig.canvas.blit(fig.bbox)
+
+            # get bounds
+            ylim = ax.get_ylim()
+
+        else:
+            pltt.plot(x, y)
+            pltt.show()
+            pltt.clear_data()
+            nlines = len(pltt.build().split('\n'))
+            print('\033[F'*nlines)
 
         try:
             # draw forever
             while True:
 
                 # get data
-                tnew, data = self.read_data(0.1, axis=axis, clear_buffer=False)
+                tnew, data = self.read_data(0.1, axis=axis, clear_buffer=ascii)
                 y = np.append(y, data)[-npts:]
                 t = np.append(t, tnew)[-npts:]
 
-                # check bounds: redraw
-                if not (max(data) < ylim[1] and min(data) > ylim[0]):
-                    plt.cla()
-                    (line,) = plt.plot(x, y, animated=True)
+                # matplotlib drawing
+                if not ascii:
 
-                    # plot elements
-                    plt.ylabel(f'$B_{self.read_axis}$ (pT)')
-                    plt.xlabel(f'Time (s)')
-                    plt.tight_layout()
+                    # check bounds: redraw
+                    if not (max(data) < ylim[1] and min(data) > ylim[0]):
+                        plt.cla()
+                        (line,) = plt.plot(x, y, animated=True)
+
+                        # plot elements
+                        plt.ylabel(f'$B_{self.read_axis}$ (pT)')
+                        plt.xlabel(f'Time (s)')
+                        plt.tight_layout()
+
+                        # render
+                        bg = fig.canvas.copy_from_bbox(fig.bbox)
+                        fig.canvas.draw()
+                        bg = fig.canvas.copy_from_bbox(fig.bbox)
+                        ax.draw_artist(line)
+                        fig.canvas.blit(fig.bbox)
+                        ylim = ax.get_ylim()
+
+                    # check for figure
+                    if not plt.fignum_exists(fig.number):
+                        break
 
-                    # render
-                    bg = fig.canvas.copy_from_bbox(fig.bbox)
-                    fig.canvas.draw()
-                    bg = fig.canvas.copy_from_bbox(fig.bbox)
-                    ax.draw_artist(line)
-                    fig.canvas.blit(fig.bbox)
-                    ylim = ax.get_ylim()
+                    # reset background
+                    fig.canvas.restore_region(bg)
 
-                # check for figure
-                if not plt.fignum_exists(fig.number):
-                    break
+                    # set x and y data
+                    line.set_ydata(y)
+                    ax.draw_artist(line)
 
-                # reset background
-                fig.canvas.restore_region(bg)
+                    # update screen
+                    fig.canvas.blit(fig.bbox)
+                    fig.canvas.flush_events()
 
-                # set x and y data
-                line.set_ydata(y)
-                # ~ line.set_xdata(t-t[-1])
-                ax.draw_artist(line)
+                    # print n events in buffer
+                    print(f'N events remaining in buffer: {self.ser.in_waiting}',
+                          flush=True, end='\r')
 
-                # update screen
-                fig.canvas.blit(fig.bbox)
-                fig.canvas.flush_events()
+                # plotext drawing
+                else:
+                    pltt.plot(x, y)
+                    pltt.show()
+                    pltt.clear_data()
+
+                    # print n events in buffer
+                    print(f'N events remaining in buffer: {self.ser.in_waiting}',
+                          flush=True)
 
-                # print n events in buffer
-                print(f'N events remaining in buffer: {self.ser.in_waiting}',
-                      flush=True, end='\r')
+                    print('\033[F'*(nlines+1))
 
         except KeyboardInterrupt:
             # save data
             self.time = t
             self.field = y
             print()
 
@@ -705,15 +766,19 @@
         message = message.replace('!', '')
         message = message.strip().split('\n')[1:-1]
 
         # check for bad byte lengths in message
         good_data = (np.array([len(m) for m in message]) == self.serial_settings['bytesize']-1)
 
         # convert to numeric data
-        data = np.array(message).astype(int)
+        try:
+            data = np.array(message).astype(int)
+        except (ValueError, OverflowError):
+            return (np.nan, np.nan)
+            
         data = (data - 8388608) * 0.01
 
         # check number of points
         if len(data) > npts:
             data = data[:npts]
             good_data = good_data[:npts]
```

