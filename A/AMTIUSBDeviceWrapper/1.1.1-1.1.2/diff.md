# Comparing `tmp/amtiusbdevicewrapper-1.1.1.tar.gz` & `tmp/amtiusbdevicewrapper-1.1.2.tar.gz`

## Comparing `amtiusbdevicewrapper-1.1.1.tar` & `amtiusbdevicewrapper-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    39459 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/src/AMTIUSBDeviceWrapper/AMTIUSBDevice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/src/AMTIUSBDeviceWrapper/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/tests/Blink_Test.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/tests/Live_Plot_Example.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/tests/Rate_Change_Test_Script.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/tests/USB_Device_Test_Suite.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/LICENSE
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    39459 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/src/AMTIUSBDeviceWrapper/AMTIUSBDevice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/src/AMTIUSBDeviceWrapper/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/tests/Blink_Test.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/tests/Live_Plot_Example.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/tests/Rate_Change_Test_Script.py
+-rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/tests/USB_Device_Test_Suite.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/README.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 amtiusbdevicewrapper-1.1.2/PKG-INFO
```

### Comparing `amtiusbdevicewrapper-1.1.1/src/AMTIUSBDeviceWrapper/AMTIUSBDevice.py` & `amtiusbdevicewrapper-1.1.2/src/AMTIUSBDeviceWrapper/AMTIUSBDevice.py`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/tests/Live_Plot_Example.py` & `amtiusbdevicewrapper-1.1.2/tests/Live_Plot_Example.py`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/tests/Rate_Change_Test_Script.py` & `amtiusbdevicewrapper-1.1.2/tests/Rate_Change_Test_Script.py`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/tests/USB_Device_Test_Suite.py` & `amtiusbdevicewrapper-1.1.2/tests/USB_Device_Test_Suite.py`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/.gitignore` & `amtiusbdevicewrapper-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/LICENSE` & `amtiusbdevicewrapper-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amtiusbdevicewrapper-1.1.1/pyproject.toml` & `amtiusbdevicewrapper-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AMTIUSBDeviceWrapper"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
-  { name="Jordy Larrea Rodriguez", email="Jordy.larrearodriguez@example.com" },
+  { name="Jordy Larrea Rodriguez", email="Jordy.larrearodriguez@gmail.com" },
 ]
 description = "Wrapper for AMTI USB Device library. Currently only supported on Windows Systems for 32 and 64 bit versions of the SDK. Use 64 bit dll if running 64 bit python interpreter and vice versa with 32 bit dll."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
```

### Comparing `amtiusbdevicewrapper-1.1.1/PKG-INFO` & `amtiusbdevicewrapper-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AMTIUSBDeviceWrapper
-Version: 1.1.1
+Version: 1.1.2
 Summary: Wrapper for AMTI USB Device library. Currently only supported on Windows Systems for 32 and 64 bit versions of the SDK. Use 64 bit dll if running 64 bit python interpreter and vice versa with 32 bit dll.
 Project-URL: Homepage, https://github.com/Lenz-Lab/AMTIUSBDeviceWrapper
-Author-email: Jordy Larrea Rodriguez <Jordy.larrearodriguez@example.com>
+Author-email: Jordy Larrea Rodriguez <Jordy.larrearodriguez@gmail.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # AMTIUSBDeviceWrapper
 
 ## Description
 
-Python wrapper for AMTI USB Device dynamically linked shared library via ctypes module.
+A digestable wrapper API for communication with AMTI GEN 5 and Optima USB Devices in python that simplifies AMTI's API.
 
 ## Getting Started
 
 ### Dependencies
 * Windows 7 64/32-bit and later
 * Python V 3.9.13 and later
 * AMTI USB Device SDK V 1.3
@@ -29,46 +29,63 @@
 * Recommended install
 ```
 python3 -m pip install amtiusbdevicewrapper
 ```
 
 ### Execution
 
-* Build the package
+Ignore build step if installing from pypi.
+* Build and install the package
 ```
+git clone https://github.com/Lenz-Lab/AMTIUSBDeviceWrapper
 py -m build # Windows
+# or...
 python -m build # Unix
-```
-* Install the package
-```
+
+# Install the package
 pip install C:/some-dir/AMTIUSBDeviceWrapper/amtiusbdevicewrapper-<>.whl
 ```
-* Import package
-```
+* Simple Initialization and Data Acquisition at 500 Hz Example
+```python
+# Import and load library
 from AMTIUSBDeviceWrapper import AMTIUSBDevice as amti
+amti.AMTIUSBDevice.InitializeLibrary(dll_path=<path_to_dll>)
+
+# Initialize and setup amti device for data acquisition
+amti_device = amti.AMTIUSBDevice("gen5")
+amti_device.init() # Default settings
+amti_device.broadcastAcquisitionRate(rate=500)
+
+amti_device.broadcastStart()
+sleep(0.01) # wait 10 ms for signal conditioners to acquire data
+
+# Get data matrix
+data, sample_num = amti_device.getData(opt=1) # opt 1->caller allocates memory
+
+amti_device.broadcastStop()
 ```
 
 ## Help
 
-Ensure that you are using a version of python compatible with this package.
+Ensure that you are using a version of python compatible with this package. IO specific exceptions are likely a result of an incorrect path.
 
 ## Authors
 
-Jordy Larrea Rodriguez ([CasuallyAlive](https://github.com/CasuallyAlive), jordy.larrearodriguez@gmail.com)
+Jordy Larrea Rodriguez ([CasuallyAlive](https://github.com/CasuallyAlive))
 
 ## Version History
 * 1.1
     * Supports all basic functionality for interfacing Gen5 signal conditioners
     * Passes all tests
 * 1.0
     * Data acquisition is functional
     * Broadcast functions nonspecific to AMTI parameter configuration are functional
     * MISC bug fixes
 * 0.2
-    * C++ API is closed without issue
+    * C++ API handle is closed without issues
     * initialization functions pass tests
     * Various bug fixes and optimizations
     * See [commit change]() or See [release history]()
 * 0.1
     * Initial Release
 
 ## License
```

