# Comparing `tmp/doy-1.0.5.tar.gz` & `tmp/doy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.0.5.tar", max compression
+gzip compressed data, was "doy-1.0.6.tar", max compression
```

## Comparing `doy-1.0.5.tar` & `doy-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0.5/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0.5/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.0.5/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0.5/doy/data.py
--rw-r--r--   0        0        0     1140 2023-06-06 16:33:01.020114 doy-1.0.5/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0.5/doy/plotting.py
--rw-r--r--   0        0        0     2282 2023-06-06 17:56:22.743114 doy-1.0.5/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0.5/doy/rich_utils.py
--rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0.5/doy/utils.py
--rw-r--r--   0        0        0      344 2023-06-06 17:56:30.743178 doy-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 doy-1.0.5/setup.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 doy-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.0.6/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.0.6/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.0.6/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.0.6/doy/data.py
+-rw-r--r--   0        0        0     1227 2023-06-13 16:12:21.379462 doy-1.0.6/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.0.6/doy/plotting.py
+-rw-r--r--   0        0        0     2282 2023-06-06 17:56:22.743114 doy-1.0.6/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.0.6/doy/rich_utils.py
+-rw-r--r--   0        0        0     1276 2023-06-06 16:01:09.609216 doy-1.0.6/doy/utils.py
+-rw-r--r--   0        0        0      344 2023-06-13 16:12:56.371774 doy-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 doy-1.0.6/setup.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 doy-1.0.6/PKG-INFO
```

### Comparing `doy-1.0.5/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.0.6/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/doy/data.py` & `doy-1.0.6/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/doy/logger.py` & `doy-1.0.6/doy/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 class Logger:
     def __init__(self, use_wandb=True):
         self.data = defaultdict(list)
         self.use_wandb = use_wandb
 
     def __call__(self, step, **kwargs):
         assert kwargs
-        for k, v in kwargs.items():
+        for k, v in list(kwargs.items()):
+            if v is None:
+                del kwargs[k]
+                continue
             try:
                 self.data[k].append(v.item())
             except AttributeError:
                 self.data[k].append(v)
         if self.use_wandb:
             import wandb
             wandb.log(data=kwargs, step=step)
```

### Comparing `doy-1.0.5/doy/plotting.py` & `doy-1.0.6/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/doy/progress.py` & `doy-1.0.6/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/doy/rich_utils.py` & `doy-1.0.6/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/doy/utils.py` & `doy-1.0.6/doy/utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.0.5/setup.py` & `doy-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.0.5/PKG-INFO` & `doy-1.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

