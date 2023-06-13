# Comparing `tmp/robotframework-testsuitesmanagement-0.7.1.tar.gz` & `tmp/robotframework-testsuitesmanagement-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-testsuitesmanagement-0.7.1.tar", last modified: Thu Jun  8 14:02:05 2023, max compression
+gzip compressed data, was "robotframework-testsuitesmanagement-0.7.2.tar", last modified: Tue Jun 13 14:59:43 2023, max compression
```

## Comparing `robotframework-testsuitesmanagement-0.7.1.tar` & `robotframework-testsuitesmanagement-0.7.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/CConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/CStruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/LibListener.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.274739 robotframework-testsuitesmanagement-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-13 14:59:43.274739 robotframework-testsuitesmanagement-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.270739 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.270739 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Config/CConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.270739 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.270739 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/CStruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.270739 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/LibListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:59:43.274739 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 14:59:43.000000 robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:59:43.274739 robotframework-testsuitesmanagement-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-13 14:57:23.000000 robotframework-testsuitesmanagement-0.7.2/setup.py
```

### Comparing `robotframework-testsuitesmanagement-0.7.1/LICENSE` & `robotframework-testsuitesmanagement-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.1
+Version: 0.7.2
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.1/README.rst` & `robotframework-testsuitesmanagement-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/CConfig.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Config/CConfig.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/__init__.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/CSetup.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/CSetup.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/__init__.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/CStruct.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/CStruct.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/Event.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/Event.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/LibListener.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/LibListener.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/__init__.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/__init__.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/version.py` & `robotframework-testsuitesmanagement-0.7.2/RobotFramework_TestsuitesManagement/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of package RobotFramework_TestsuitesManagement
 #
-VERSION      = "0.7.1"
-VERSION_DATE = "26.05.2023"
+VERSION      = "0.7.2"
+VERSION_DATE = "13.06.2023"
```

### Comparing `robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.1
+Version: 0.7.2
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt` & `robotframework-testsuitesmanagement-0.7.2/robotframework_testsuitesmanagement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.1/setup.py` & `robotframework-testsuitesmanagement-0.7.2/setup.py`

 * *Files identical despite different names*

