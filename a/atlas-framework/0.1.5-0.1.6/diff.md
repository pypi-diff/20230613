# Comparing `tmp/atlas-framework-0.1.5.tar.gz` & `tmp/atlas-framework-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-framework-0.1.5.tar", last modified: Fri May 19 20:15:42 2023, max compression
+gzip compressed data, was "atlas-framework-0.1.6.tar", last modified: Tue Jun 13 17:35:59 2023, max compression
```

## Comparing `atlas-framework-0.1.5.tar` & `atlas-framework-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/app/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/app/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.247253 atlas-framework-0.1.5/src/atlas/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/src/atlas/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/src/atlas_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 20:15:42.000000 atlas-framework-0.1.5/src/atlas_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:15:42.251253 atlas-framework-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-19 20:15:30.000000 atlas-framework-0.1.5/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.114666 atlas-framework-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/src/atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/src/atlas/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/src/atlas/app/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/thirdparty/maya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/app/thirdparty/unreal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/src/atlas/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/src/atlas/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/src/atlas_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-13 17:35:59.000000 atlas-framework-0.1.6/src/atlas_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-13 17:35:59.000000 atlas-framework-0.1.6/src/atlas_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:35:59.000000 atlas-framework-0.1.6/src/atlas_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 17:35:59.000000 atlas-framework-0.1.6/src/atlas_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:35:59.000000 atlas-framework-0.1.6/src/atlas_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:35:59.118666 atlas-framework-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 17:35:39.000000 atlas-framework-0.1.6/tests/test_context.py
```

### Comparing `atlas-framework-0.1.5/LICENSE` & `atlas-framework-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.5/PKG-INFO` & `atlas-framework-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-framework
-Version: 0.1.5
+Version: 0.1.6
 Summary: Class-based famework for quickly creating robust Python apps.
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/atlas-framework
 Project-URL: Bug Tracker, https://github.com/renderbox/atlas-framework/issues
 Keywords: cli,app,application,framework
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `atlas-framework-0.1.5/README.md` & `atlas-framework-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.5/pyproject.toml` & `atlas-framework-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "atlas-framework"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
 ]
 description = "Class-based famework for quickly creating robust Python apps."
 readme = "README.md"
 requires-python = ">=3.7,<3.12"
 classifiers = [
```

### Comparing `atlas-framework-0.1.5/src/atlas/app/base.py` & `atlas-framework-0.1.6/src/atlas/app/base.py`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.5/src/atlas/app/gui.py` & `atlas-framework-0.1.6/src/atlas/app/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,14 @@
         Load the GUI and run.
 
         Args:
             ctx (Context): Context to execute the tool with
         """
         QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
 
-        self.app = QApplication(sys.argv)
-
         if self.gui_class:
             self.window = self.gui_class()
         else:
             # Get the path to the App Class Instance being evaluated
             gui_path = os.path.join(
                 os.path.dirname(inspect.getfile(self.__class__)), self.gui_file
             )
@@ -94,13 +92,12 @@
         """
         Evaluated when in GUI mode.  By default just loads the GUI.
         Can be overridden to do other things when loading a GUI.
 
         Args:
             ctx (Context): Context to execute the tool with
         """
+        host_app = QApplication(sys.argv)
         self.load_gui()
-
         self.connect_signals_and_slots()
-
         self.window.show()
-        sys.exit(self.app.exec_())
+        sys.exit(host_app.exec_())
```

### Comparing `atlas-framework-0.1.5/src/atlas/context/__init__.py` & `atlas-framework-0.1.6/src/atlas/context/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-framework-0.1.5/src/atlas_framework.egg-info/PKG-INFO` & `atlas-framework-0.1.6/src/atlas_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-framework
-Version: 0.1.5
+Version: 0.1.6
 Summary: Class-based famework for quickly creating robust Python apps.
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/atlas-framework
 Project-URL: Bug Tracker, https://github.com/renderbox/atlas-framework/issues
 Keywords: cli,app,application,framework
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `atlas-framework-0.1.5/tests/test_context.py` & `atlas-framework-0.1.6/tests/test_context.py`

 * *Files identical despite different names*

