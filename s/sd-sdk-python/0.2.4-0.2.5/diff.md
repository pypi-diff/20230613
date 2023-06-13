# Comparing `tmp/sd_sdk_python-0.2.4.tar.gz` & `tmp/sd_sdk_python-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_sdk_python-0.2.4.tar", max compression
+gzip compressed data, was "sd_sdk_python-0.2.5.tar", max compression
```

## Comparing `sd_sdk_python-0.2.4.tar` & `sd_sdk_python-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-05-24 15:07:54.903727 sd_sdk_python-0.2.4/LICENSE
--rw-r--r--   0        0        0      636 2023-05-24 15:07:54.903727 sd_sdk_python-0.2.4/README.md
--rw-r--r--   0        0        0     1080 2023-05-24 15:07:54.903727 sd_sdk_python-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2783 2023-05-24 15:07:54.903727 sd_sdk_python-0.2.4/sd_sdk_python/__init__.py
--rw-r--r--   0        0        0    13155 2023-05-24 15:07:54.907727 sd_sdk_python-0.2.4/sd_sdk_python/sd_sdk.py
--rw-r--r--   0        0        0    13130 2023-05-24 15:07:54.907727 sd_sdk_python-0.2.4/sd_sdk_python/sd_sdk_wireless.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/LICENSE
+-rw-r--r--   0        0        0      636 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/README.md
+-rw-r--r--   0        0        0     1080 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2783 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/sd_sdk_python/__init__.py
+-rw-r--r--   0        0        0    12948 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/sd_sdk_python/sd_sdk.py
+-rw-r--r--   0        0        0    13130 2023-06-13 20:55:14.850937 sd_sdk_python-0.2.5/sd_sdk_python/sd_sdk_wireless.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.5/PKG-INFO
```

### Comparing `sd_sdk_python-0.2.4/LICENSE` & `sd_sdk_python-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.4/README.md` & `sd_sdk_python-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.4/pyproject.toml` & `sd_sdk_python-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sd-sdk-python"
 homepage = "https://github.com/markmelvin-onsemi/sd-sdk-python"
-version = "0.2.4"
+version = "0.2.5"
 description = "Python helper module for the Sound Designer SDK"
 authors = ["Mark Melvin <mark.melvin@onsemi.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `sd_sdk_python-0.2.4/sd_sdk_python/__init__.py` & `sd_sdk_python-0.2.5/sd_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.4/sd_sdk_python/sd_sdk.py` & `sd_sdk_python-0.2.5/sd_sdk_python/sd_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,24 +175,18 @@
         if self.product is not None:
             return (len(self.product.SystemMemory.Parameters), 
                     [len(self.product.Memories[w].Parameters) for w in range(len(self.product.Memories))])
         return (0,[0,])
 
     def restore_all_parameters(self,):
         if self.product is not None and self.interface is not None:
-            # Back up current memory
-            current_memory = self.get_current_memory()
-
             self.restore_system_parameters()
             for i in range(len(self.product.Memories)):
                 self.restore_profile_parameters(i)
 
-            # Restore original memory
-            self.set_current_memory(current_memory, read_parameters=False)
-
     def restore_system_parameters(self,):
         if self.product is not None and self.interface is not None:
             self.product.ReadParameters(self.sd.kSystemNvmMemory)
 
     def restore_profile_parameters(self, memory):
         if self.product is not None and self.interface is not None:
             self.product.ReadParameters(memory)
```

### Comparing `sd_sdk_python-0.2.4/sd_sdk_python/sd_sdk_wireless.py` & `sd_sdk_python-0.2.5/sd_sdk_python/sd_sdk_wireless.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.4/PKG-INFO` & `sd_sdk_python-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-sdk-python
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python helper module for the Sound Designer SDK
 Home-page: https://github.com/markmelvin-onsemi/sd-sdk-python
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@onsemi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

