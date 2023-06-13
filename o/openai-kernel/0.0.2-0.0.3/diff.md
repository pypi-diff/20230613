# Comparing `tmp/openai_kernel-0.0.2.tar.gz` & `tmp/openai_kernel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_kernel-0.0.2.tar", last modified: Wed May  3 17:57:10 2023, max compression
+gzip compressed data, was "openai_kernel-0.0.3.tar", last modified: Tue Jun 13 16:19:55 2023, max compression
```

## Comparing `openai_kernel-0.0.2.tar` & `openai_kernel-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/kernel.json
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel/magics/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/clear_history_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/history_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/mode_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/openai_api_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/set_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/mock_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/openai_kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/openai_kernel/magics/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/clear_history_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/history_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/mode_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/openai_api_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/magics/set_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/mock_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/openai_kernel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/openai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-13 16:19:55.000000 openai_kernel-0.0.3/openai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 16:19:55.000000 openai_kernel-0.0.3/openai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:19:55.000000 openai_kernel-0.0.3/openai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 16:19:55.000000 openai_kernel-0.0.3/openai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:19:55.000000 openai_kernel-0.0.3/openai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:19:55.081308 openai_kernel-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-13 16:19:45.000000 openai_kernel-0.0.3/setup.py
```

### Comparing `openai_kernel-0.0.2/PKG-INFO` & `openai_kernel-0.0.3/openai_kernel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: openai_kernel
-Version: 0.0.2
+Name: openai-kernel
+Version: 0.0.3
 Summary: OpenAI jupyter kernel
+Home-page: https://github.com/OakCityLabs/openai_kernel
 Author: Oak City Labs
 Author-email: team@oakcity.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `openai_kernel-0.0.2/openai_kernel/kernel.py` & `openai_kernel-0.0.3/openai_kernel/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.kernel_json = get_kernel_json()
         self._history = []
 
         if self.openai.api_key is None and self.openai.api_key_path is None:
             default_api_key_path = get_default_api_key_path()
             if default_api_key_path:
                 self.openai.api_key_path = default_api_key_path
+                self.api_key_path = default_api_key_path
 
     @property
     def api_key(self):
         return self.openai.api_key
 
     @api_key.setter
     def api_key(self, key):
@@ -77,14 +78,17 @@
 
     @property
     def api_key_path(self):
         return self.openai.api_key_path
 
     @api_key_path.setter
     def api_key_path(self, path):
+        if path.startswith("~/"):
+            home = os.path.expanduser("~")
+            path = os.path.join(home, path[2:])
         self.openai.api_key_path = path
 
     @property
     def organization(self):
         return self.openai.organization
 
     @organization.setter
```

### Comparing `openai_kernel-0.0.2/openai_kernel/magics/history_magic.py` & `openai_kernel-0.0.3/openai_kernel/magics/history_magic.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.retval = self.kernel.history
         self.raw = raw
 
     def post_process(self, retval):
         if not self.raw:
             markdown = ""
             for msg in self.retval:
-                markdown += f"{msg}<br />"
+                markdown += f"{msg}  \n"
             return MarkdownOutput(str(retval), markdown)
         else:
             return self.retval
 
 
 def register_magics(kernel):
     kernel.register_magics(HistoryMagic)
```

### Comparing `openai_kernel-0.0.2/openai_kernel/magics/openai_api_magic.py` & `openai_kernel-0.0.3/openai_kernel/magics/openai_api_magic.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.2/openai_kernel/magics/set_magic.py` & `openai_kernel-0.0.3/openai_kernel/magics/set_magic.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.2/openai_kernel/mock_kernel.py` & `openai_kernel-0.0.3/openai_kernel/mock_kernel.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.2/openai_kernel/utils.py` & `openai_kernel-0.0.3/openai_kernel/utils.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.2/openai_kernel.egg-info/PKG-INFO` & `openai_kernel-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: openai-kernel
-Version: 0.0.2
+Name: openai_kernel
+Version: 0.0.3
 Summary: OpenAI jupyter kernel
+Home-page: https://github.com/OakCityLabs/openai_kernel
 Author: Oak City Labs
 Author-email: team@oakcity.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `openai_kernel-0.0.2/openai_kernel.egg-info/SOURCES.txt` & `openai_kernel-0.0.3/openai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.2/setup.py` & `openai_kernel-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 setuptools.setup(
     name="openai_kernel",
     version=__version__,
     author="Oak City Labs",
     author_email="team@oakcity.io",
     description="OpenAI jupyter kernel",
+    url="https://github.com/OakCityLabs/openai_kernel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={"openai_kernel": ["*.json"]},
     classifiers=[
         "Programming Language :: Python :: 3",
```

