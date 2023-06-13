# Comparing `tmp/adofaipy-0.0.1.tar.gz` & `tmp/adofaipy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adofaipy-0.0.1.tar", last modified: Sun May 28 11:04:34 2023, max compression
+gzip compressed data, was "adofaipy-0.0.2.tar", last modified: Tue Jun 13 16:24:21 2023, max compression
```

## Comparing `adofaipy-0.0.1.tar` & `adofaipy-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 11:04:34.201626 adofaipy-0.0.1/
--rw-rw-rw-   0        0        0       81 2023-05-28 10:20:12.000000 adofaipy-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1825 2023-05-28 11:04:34.200547 adofaipy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-05-28 10:19:06.000000 adofaipy-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 11:04:34.191799 adofaipy-0.0.1/adofaipy/
--rw-rw-rw-   0        0        0    19887 2023-05-28 11:03:21.000000 adofaipy-0.0.1/adofaipy/_init_.py
-drwxrwxrwx   0        0        0        0 2023-05-28 11:04:34.199344 adofaipy-0.0.1/adofaipy.egg-info/
--rw-rw-rw-   0        0        0     1825 2023-05-28 11:04:34.000000 adofaipy-0.0.1/adofaipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-28 11:04:34.000000 adofaipy-0.0.1/adofaipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:04:34.000000 adofaipy-0.0.1/adofaipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-28 11:04:34.000000 adofaipy-0.0.1/adofaipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 11:04:34.000000 adofaipy-0.0.1/adofaipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 11:04:34.201626 adofaipy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-28 11:04:11.000000 adofaipy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.850935 adofaipy-0.0.2/
+-rw-rw-rw-   0        0        0      171 2023-06-13 16:17:13.000000 adofaipy-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-28 10:23:16.000000 adofaipy-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-28 10:21:05.000000 adofaipy-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2145 2023-06-13 16:24:21.849935 adofaipy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-06-13 16:24:06.000000 adofaipy-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.842935 adofaipy-0.0.2/adofaipy/
+-rw-rw-rw-   0        0        0    19887 2023-05-28 11:03:21.000000 adofaipy-0.0.2/adofaipy/_init_.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:24:21.848936 adofaipy-0.0.2/adofaipy.egg-info/
+-rw-rw-rw-   0        0        0     2145 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:24:21.000000 adofaipy-0.0.2/adofaipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:24:21.850935 adofaipy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-06-13 16:22:20.000000 adofaipy-0.0.2/setup.py
```

### Comparing `adofaipy-0.0.1/LICENSE.txt` & `adofaipy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.1/PKG-INFO` & `adofaipy-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
+Description: This is a library that makes automating events in ADOFAI levels more convenient.
+        
+        List of Functions:
+        
+        getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
+        
+        getAngles(filestring : str): takes a file string and returns the list of angles.
+        
+        setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
+        
+        There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
+        The arguments for these functions are the same as the fields that are present in the ingame editor.
+        Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
+        These functions return the event data as a string which can be added with addEvent().
+        
+        Note that addDecoration() works the same as other event functions. 
+        
+        addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
+        
+        writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
+        
+        
+        Change Log
+        ==========
+        
+        0.0.2 (2023/06/13)
+        ------------------
+        - Minor bugfix: 're' is no longer a dependency
+        
+        0.0.1 (2023/05/28)
+        ------------------
+        - First Release
 Keywords: adofai
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE.txt
-
-This is a library that makes automating events in ADOFAI levels more convenient.
-
-List of Functions:
-
-getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
-
-getAngles(filestring : str): takes a file string and returns the list of angles.
-
-setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
-
-There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
-The arguments for these functions are the same as the fields that are present in the ingame editor.
-Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
-These functions return the event data as a string which can be added with addEvent().
-
-Note that addDecoration() works the same as other event functions. 
-
-addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
-
-writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
-
-
-Change Log
-==========
-
-0.0.1 (2023/05/28)
-------------------
-- First Release
-
```

### Comparing `adofaipy-0.0.1/README.txt` & `adofaipy-0.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.1/adofaipy/_init_.py` & `adofaipy-0.0.2/adofaipy/_init_.py`

 * *Files identical despite different names*

### Comparing `adofaipy-0.0.1/adofaipy.egg-info/PKG-INFO` & `adofaipy-0.0.2/adofaipy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: adofaipy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that makes automating events in ADOFAI levels more convenient.
 Home-page: UNKNOWN
 Author: M1n3c4rt
 Author-email: vedicbits@gmail.com
 License: MIT
+Description: This is a library that makes automating events in ADOFAI levels more convenient.
+        
+        List of Functions:
+        
+        getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
+        
+        getAngles(filestring : str): takes a file string and returns the list of angles.
+        
+        setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
+        
+        There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
+        The arguments for these functions are the same as the fields that are present in the ingame editor.
+        Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
+        These functions return the event data as a string which can be added with addEvent().
+        
+        Note that addDecoration() works the same as other event functions. 
+        
+        addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
+        
+        writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
+        
+        
+        Change Log
+        ==========
+        
+        0.0.2 (2023/06/13)
+        ------------------
+        - Minor bugfix: 're' is no longer a dependency
+        
+        0.0.1 (2023/05/28)
+        ------------------
+        - First Release
 Keywords: adofai
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE.txt
-
-This is a library that makes automating events in ADOFAI levels more convenient.
-
-List of Functions:
-
-getFileString(filename : str): returns the ADOFAI file as a string. Many functions in this library depend on this string.
-
-getAngles(filestring : str): takes a file string and returns the list of angles.
-
-setAngles(angles : list, filestring : str): writes the new angles to the file string and returns the file string.
-
-There is also one function for each event. It is recommended to use keyword arguments while calling these functions.
-The arguments for these functions are the same as the fields that are present in the ingame editor.
-Fields with string values (eg. ease="In Out Bounce") must have their spaces removed (ease="InOutBounce").
-These functions return the event data as a string which can be added with addEvent().
-
-Note that addDecoration() works the same as other event functions. 
-
-addEvent(event : str, filestring : str): adds events to the file string and returns the file string. This function is also compatible with addDecoration().
-
-writeToFile(filestring : str, filename : str): writes the modified file string to the file. 
-
-
-Change Log
-==========
-
-0.0.1 (2023/05/28)
-------------------
-- First Release
-
```

