# Comparing `tmp/lecore-0.1.6.tar.gz` & `tmp/lecore-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-l1axzm6h\lecore-0.1.6.tar", last modified: Wed Jun  7 10:33:25 2023, max compression
+gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-qierrovb\lecore-0.1.7.tar", last modified: Tue Jun 13 09:28:04 2023, max compression
```

## Comparing `lecore-0.1.6.tar` & `lecore-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1558 2023-06-07 10:33:25.000000 lecore-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.6/README.md
--rw-rw-rw-   0        0        0      704 2023-06-06 10:53:21.000000 lecore-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 10:33:25.000000 lecore-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore/
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore/LeBin/
--rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.6/src/lecore/LeBin/RegisterMap.py
--rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.6/src/lecore/LeBin/SerialCom.py
--rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.6/src/lecore/LeBin/UpgradeFirmware.py
--rw-rw-rw-   0        0        0     5334 2023-06-06 09:06:28.000000 lecore-0.1.6/src/lecore/LeBin/VisualLeBin.py
--rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.6/src/lecore/LeBin/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.6/src/lecore/Looger.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore/VisualModbus/
--rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.6/src/lecore/VisualModbus/AppLogging.py
--rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.6/src/lecore/VisualModbus/Crc32.py
--rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.6/src/lecore/VisualModbus/HelpAbout.py
--rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.6/src/lecore/VisualModbus/MbClient.py
--rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.6/src/lecore/VisualModbus/MbUpgrade.py
--rw-rw-rw-   0        0        0     5083 2020-11-18 16:34:05.000000 lecore-0.1.6/src/lecore/VisualModbus/ReadWrite.py
--rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.6/src/lecore/VisualModbus/RegMap.py
--rw-rw-rw-   0        0        0     8619 2021-08-09 11:26:31.000000 lecore-0.1.6/src/lecore/VisualModbus/VisualMbApp.py
--rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.6/src/lecore/VisualModbus/VmSettings.py
--rw-rw-rw-   0        0        0      170 2023-06-07 10:26:20.000000 lecore-0.1.6/src/lecore/VisualModbus/__init__.py
--rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.6/src/lecore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/
--rw-rw-rw-   0        0        0     1558 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      831 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 10:33:25.000000 lecore-0.1.6/src/lecore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 10:33:25.000000 lecore-0.1.6/tests/
--rw-rw-rw-   0        0        0      852 2023-06-07 10:22:46.000000 lecore-0.1.6/tests/test_lebin.py
--rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.6/tests/test_looger.py
--rw-rw-rw-   0        0        0      733 2023-06-05 15:20:31.000000 lecore-0.1.6/tests/test_modbus.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1558 2023-06-13 09:28:04.000000 lecore-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.7/README.md
+-rw-rw-rw-   0        0        0      704 2023-06-13 09:27:32.000000 lecore-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:28:04.000000 lecore-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore/LeBin/
+-rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.7/src/lecore/LeBin/RegisterMap.py
+-rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.7/src/lecore/LeBin/SerialCom.py
+-rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.7/src/lecore/LeBin/UpgradeFirmware.py
+-rw-rw-rw-   0        0        0     5334 2023-06-06 09:06:28.000000 lecore-0.1.7/src/lecore/LeBin/VisualLeBin.py
+-rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.7/src/lecore/LeBin/__init__.py
+-rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.7/src/lecore/Looger.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore/VisualModbus/
+-rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.7/src/lecore/VisualModbus/AppLogging.py
+-rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.7/src/lecore/VisualModbus/Crc32.py
+-rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.7/src/lecore/VisualModbus/HelpAbout.py
+-rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.7/src/lecore/VisualModbus/MbClient.py
+-rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.7/src/lecore/VisualModbus/MbUpgrade.py
+-rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:17.000000 lecore-0.1.7/src/lecore/VisualModbus/ReadWrite.py
+-rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.7/src/lecore/VisualModbus/RegMap.py
+-rw-rw-rw-   0        0        0     8611 2023-06-13 09:26:48.000000 lecore-0.1.7/src/lecore/VisualModbus/VisualMbApp.py
+-rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.7/src/lecore/VisualModbus/VmSettings.py
+-rw-rw-rw-   0        0        0      170 2023-06-07 10:26:20.000000 lecore-0.1.7/src/lecore/VisualModbus/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.7/src/lecore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/
+-rw-rw-rw-   0        0        0     1558 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      831 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 09:28:04.000000 lecore-0.1.7/src/lecore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 09:28:04.000000 lecore-0.1.7/tests/
+-rw-rw-rw-   0        0        0     1127 2023-06-13 08:49:10.000000 lecore-0.1.7/tests/test_lebin.py
+-rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.7/tests/test_looger.py
+-rw-rw-rw-   0        0        0     1201 2023-06-13 09:27:32.000000 lecore-0.1.7/tests/test_modbus.py
```

### Comparing `lecore-0.1.6/LICENSE` & `lecore-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/PKG-INFO` & `lecore-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.6
+Version: 0.1.7
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.6/README.md` & `lecore-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/pyproject.toml` & `lecore-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lecore"
 description = "Logic Elements core utilities"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Jan Bartovský", email="jan.bartovsky@logicelements.cz" },
 ]
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `lecore-0.1.6/src/lecore/LeBin/RegisterMap.py` & `lecore-0.1.7/src/lecore/LeBin/RegisterMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/LeBin/SerialCom.py` & `lecore-0.1.7/src/lecore/LeBin/SerialCom.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/LeBin/UpgradeFirmware.py` & `lecore-0.1.7/src/lecore/LeBin/UpgradeFirmware.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/LeBin/VisualLeBin.py` & `lecore-0.1.7/src/lecore/LeBin/VisualLeBin.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/Looger.py` & `lecore-0.1.7/src/lecore/Looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/AppLogging.py` & `lecore-0.1.7/src/lecore/VisualModbus/AppLogging.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/Crc32.py` & `lecore-0.1.7/src/lecore/VisualModbus/Crc32.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/HelpAbout.py` & `lecore-0.1.7/src/lecore/VisualModbus/HelpAbout.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/MbClient.py` & `lecore-0.1.7/src/lecore/VisualModbus/MbClient.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/MbUpgrade.py` & `lecore-0.1.7/src/lecore/VisualModbus/MbUpgrade.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/ReadWrite.py` & `lecore-0.1.7/src/lecore/VisualModbus/ReadWrite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from time import sleep
 from sys import stdout
 
 # import own modules
-from VisualModbus.AppLogging import *
-from VisualModbus.RegMap import RegMap as rm
-from VisualModbus.MbClient import MbClient
-import VisualModbus.VmSettings as s
+from .AppLogging import *
+from .RegMap import RegMap as rm
+from .MbClient import MbClient
+import VmSettings as s
 
 # Start logging into log file
 log = AppLogging(logging.WARNING)
 # Load settings from multiple JSONs
 s.read_settings(['VisualSettings.json', 'UpgradeSettings.json', 'ComSettings.json'])
 # Open modbus client connection
 mb = MbClient()
```

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/RegMap.py` & `lecore-0.1.7/src/lecore/VisualModbus/RegMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/VisualMbApp.py` & `lecore-0.1.7/src/lecore/VisualModbus/VisualMbApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import build-in modules
 import PySimpleGUI as SG
 # import own modules
-from VisualModbus.AppLogging import *
-from VisualModbus.RegMap import RegMap
-from VisualModbus.MbClient import MbClient
-import VisualModbus.HelpAbout as Help
-import VisualModbus.VmSettings as Setting
-from VisualModbus.MbUpgrade import *
+from .AppLogging import *
+from .RegMap import RegMap
+from .MbClient import MbClient
+from .HelpAbout import *
+from .VmSettings import *
+from .MbUpgrade import *
 
 
 def _upgrade_callback(progress, size):
     """
     Upgrade firmware callback called after each page is acknowledged by device.
     :param progress: Number of bytes already written
     :param size: Complete size of firmware
@@ -25,51 +25,53 @@
     """
     # Literal constants
     HEX_SUFFIX = "_H"
     INF_SUFFIX = "_INFO_BTN"
     READ_SUFFIX = "_READ_BTN"
     UPG_FILE = '_UPG_FILE'
 
-    def __init__(self, visual='VisualSettings.json', upgrade='UpgradeSettings.json', com='ComSettings.json', slave=None):
+    def __init__(self, visual='VisualSettings.json', upgrade='UpgradeSettings.json', com='ComSettings.json',
+                 slave=None, reg_map=None):
         """
         Initialize VisualModbus application.
 
         This function reads all necessary settings json files, initializes modbus register map and displays
         window layout.
         :param visual: Json containing visual settings
         :param upgrade: Json containing upgrade firmware settings
         :param com: Json containing communication settings
         :param slave: Slave address to override VisualSetting json
+        :param reg_map: Register map override if it differs from the one mentioned in Visual Settings
         """
         self.win_log = None
         self.win_info = None
         self.window = None
         self.upgrade = upgrade
         self.com_settings = com
         # Initialize internal modules
         self.mb = MbClient()
         self.log = AppLogging()
         # Read settings and load jsons
-        Setting.read_settings([visual, upgrade, com])
-        sl = Setting.s['slave_address'] if slave is None else slave
+        read_settings([visual, upgrade, com])
+        sl = s['slave_address'] if slave is None else slave
         self.regs = RegMap(self.mb, sl)
-        self.regs.load(Setting.s['reg_map'])
+        self.regs.load(s['reg_map'] if reg_map is None else reg_map)
         # Create and display window layout
         self._finalize()
 
     def handle(self):
         """
         Handle of GUI features.
 
         This function blocks until window is closed and handles all user logic of GUI.
         :return: None on exit
         """
         periodic = False
         while True:
-            to = max(min(Setting.s['readout_period'] * 1000, 1000), 1000)
+            to = max(min(s['readout_period'] * 1000, 1000), 1000)
             event, values = self.window.Read(timeout=to, timeout_key='_TIMEOUT_')
             if event in (None, 'Close'):
                 self.mb.close()
                 break
             if 'Write' in event:
                 self._write_mb(values)
             if 'Write All' in event:
@@ -81,25 +83,25 @@
                 if periodic:
                     self.window['B_PERIOD'].Update('Stop Periodic')
                 else:
                     self.window['B_PERIOD'].Update('Start Periodic')
             if event in '_TIMEOUT_' and periodic:
                 self._read_mb()
             if event in 'About':
-                Help.show_help()
+                show_help()
             if event in 'B_COMPORT':
                 if self.window['B_COMPORT'].GetText() == 'COM open':
                     if self.mb.open(self.com_settings):
                         self.window['B_COMPORT'].Update('COM close')
                 else:
                     self.window['B_COMPORT'].Update('COM open')
                     self.mb.close()
             if event in 'Edit':
-                Setting.edit(self.window.size)
-                self.regs.slave = Setting.s['slave_address']
+                edit(self.window.size)
+                self.regs.slave = s['slave_address']
             if event in 'Upgrade' and values[self.UPG_FILE] != '':
                 self._upgrade(values[self.UPG_FILE])
             if event in 'Show Log':
                 self.win_log = self._show_log()
             if self.INF_SUFFIX in event:
                 if self.win_info is not None:
                     self.win_info.close()
@@ -146,15 +148,15 @@
     def _upgrade(self, file_name):
         """
         Initialize and run firmware upgrade procedure
         :param file_name: Binary file to upgrade
         :return: None
         """
         # initialize and get first packet obtaining info
-        upg = MbUpgrade(self.upgrade, self.mb, slave=Setting.s['slave_address'])
+        upg = MbUpgrade(self.upgrade, self.mb, slave=s['slave_address'])
         upg.load_file(file_name)
         upg.run_upgrade(_upgrade_callback)
 
     def _show_log(self):
         """
         Show window containing most recent log entries
         :return: Window object
@@ -188,25 +190,25 @@
                     SG.InputText('0', size=(20, 1), key=reg['Name']),
                     SG.InputText('0', size=(12, 1), key=reg['Name'] + self.HEX_SUFFIX)]
             if reg['Min'] != 0 and reg['Max'] != 0:
                 line.append(SG.Text(f"({reg['Min']}, {reg['Max']})"))
             col1.append(line)
 
         layout.append([SG.Column(col1, key='C_REGS', scrollable=True, vertical_scroll_only=True,
-                                 size=(Setting.s['width'] - 10, Setting.s['height']))])
+                                 size=(s['width'] - 10, s['height']))])
         layout.append([SG.FileBrowse('Select file'), SG.Button('Upgrade'), SG.Input(key=self.UPG_FILE)])
         layout.append([SG.Submit('Write'),
                        SG.Button('Write All'),
                        SG.Button('Read'),
                        SG.Button('COM open', key='B_COMPORT'),
                        SG.Button('Show Log'), SG.Cancel('Start Periodic', key='B_PERIOD'), SG.Cancel('Close')])
-        layout.append([SG.Text('Status', key='T_STATUS', size=(Setting.s['width'] // 8, None))])
+        layout.append([SG.Text('Status', key='T_STATUS', size=(s['width'] // 8, None))])
 
-        self.window = SG.Window('VisualModbus. Version: ' + Help.VERSION, layout, resizable=True, finalize=True)
-        Setting.init_size(self.window.size)
+        self.window = SG.Window('VisualModbus. Version: ' + VERSION, layout, resizable=True, finalize=True)
+        init_size(self.window.size)
         self._update_regs()
 
 
 if __name__ == "__main__":
     vm = VisualMbApp()
     vm.handle()
```

### Comparing `lecore-0.1.6/src/lecore/VisualModbus/VmSettings.py` & `lecore-0.1.7/src/lecore/VisualModbus/VmSettings.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/src/lecore.egg-info/PKG-INFO` & `lecore-0.1.7/src/lecore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.6
+Version: 0.1.7
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.6/src/lecore.egg-info/SOURCES.txt` & `lecore-0.1.7/src/lecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lecore-0.1.6/tests/test_looger.py` & `lecore-0.1.7/tests/test_looger.py`

 * *Files identical despite different names*

