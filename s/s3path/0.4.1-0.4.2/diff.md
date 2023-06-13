# Comparing `tmp/s3path-0.4.1.tar.gz` & `tmp/s3path-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3path-0.4.1.tar", last modified: Wed Jan 11 14:07:36 2023, max compression
+gzip compressed data, was "s3path-0.4.2.tar", last modified: Tue Jun 13 07:17:05 2023, max compression
```

## Comparing `s3path-0.4.1.tar` & `s3path-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 14:07:36.641875 s3path-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-11 14:07:26.000000 s3path-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-11 14:07:26.000000 s3path-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-11 14:07:36.641875 s3path-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-01-11 14:07:26.000000 s3path-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 14:07:36.637875 s3path-0.4.1/s3path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-11 14:07:36.000000 s3path-0.4.1/s3path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-11 14:07:36.000000 s3path-0.4.1/s3path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 14:07:36.000000 s3path-0.4.1/s3path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-11 14:07:36.000000 s3path-0.4.1/s3path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-11 14:07:36.000000 s3path-0.4.1/s3path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-01-11 14:07:26.000000 s3path-0.4.1/s3path.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-11 14:07:36.641875 s3path-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-11 14:07:26.000000 s3path-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:17:05.368734 s3path-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 07:16:53.000000 s3path-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 07:16:53.000000 s3path-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-13 07:17:05.368734 s3path-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-13 07:16:53.000000 s3path-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:17:05.368734 s3path-0.4.2/s3path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-13 07:17:05.000000 s3path-0.4.2/s3path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 07:17:05.000000 s3path-0.4.2/s3path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:17:05.000000 s3path-0.4.2/s3path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 07:17:05.000000 s3path-0.4.2/s3path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 07:17:05.000000 s3path-0.4.2/s3path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42832 2023-06-13 07:16:53.000000 s3path-0.4.2/s3path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 07:17:05.368734 s3path-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-13 07:16:53.000000 s3path-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:17:05.368734 s3path-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-13 07:16:53.000000 s3path-0.4.2/tests/test_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27008 2023-06-13 07:16:53.000000 s3path-0.4.2/tests/test_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-13 07:16:53.000000 s3path-0.4.2/tests/test_pure_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-13 07:16:53.000000 s3path-0.4.2/tests/test_s3path_configuration.py
```

### Comparing `s3path-0.4.1/LICENSE` & `s3path-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3path-0.4.1/PKG-INFO` & `s3path-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.4.1 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.4.2 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `s3path-0.4.1/README.rst` & `s3path-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `s3path-0.4.1/s3path.egg-info/PKG-INFO` & `s3path-0.4.2/s3path.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.4.1 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.4.2 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `s3path-0.4.1/s3path.py` & `s3path-0.4.2/s3path.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from boto3.s3.transfer import TransferManager
 from botocore.exceptions import ClientError
 from botocore.docs.docstring import LazyLoadedDocstring
 
 import smart_open
 from packaging.version import Version
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __all__ = (
     'register_configuration_parameter',
     'S3Path',
     'PureS3Path',
     'StatResult',
     'S3DirEntry',
 )
@@ -102,14 +102,15 @@
         self._delayed_setup()
         if arguments is not None:
             self.arguments[path] = arguments
         if resource is not None:
             self.resources[path] = resource
         if glob_new_algorithm is not None:
             self.general_options[path] = {'glob_new_algorithm': glob_new_algorithm}
+        self.get_configuration.cache_clear()
 
     @lru_cache()
     def get_configuration(self, path):
         self._delayed_setup()
         resources = arguments = None
         for path in chain([path], path.parents):
             if resources is None and path in self.resources:
@@ -317,14 +318,16 @@
     def rmdir(self, path):
         bucket_name = path.bucket
         key_name = path.key
         resource, config = self.configuration_map.get_configuration(path)
         bucket = resource.Bucket(bucket_name)
         for object_summary in bucket.objects.filter(Prefix=key_name):
             self._boto3_method_with_parameters(object_summary.delete, config=config)
+        if path.is_bucket:
+            self._boto3_method_with_parameters(bucket.delete, config=config)
 
     def mkdir(self, path, mode):
         resource, config = self.configuration_map.get_configuration(path)
         self._boto3_method_with_parameters(
             resource.create_bucket,
             config=config,
             kwargs={'Bucket': path.bucket},
@@ -631,31 +634,32 @@
     def select(self):
         for target in self._deep_cached_dir_scan():
             target = self._path._flavour.sep.join(('', self._path.bucket, target))
             if self.match(target):
                 yield type(self._path)(target)
 
     def _prefix_splitter(self, pattern):
+        if not _is_wildcard_pattern(pattern):
+            if self._path.key:
+                return f'{self._path.key}{self._path._flavour.sep}{pattern}', ''
+            return pattern, ''
+
         *_, pattern_parts = self._path._flavour.parse_parts((pattern,))
         prefix = ''
-        key_prefix = self._path.key
-        for part in pattern_parts:
+        for index, part in enumerate(pattern_parts):
             if _is_wildcard_pattern(part):
                 break
-            if prefix:
-                prefix += f'{self._path._flavour.sep}{part}'
-            else:
-                prefix = part
-        prefix_folder = f'{prefix}{self._path._flavour.sep}'
-        if prefix_folder == pattern:
-            prefix = prefix_folder
-        if key_prefix:
-            prefix = f'{key_prefix}{self._path._flavour.sep}{prefix}'
+            prefix += f'{part}{self._path._flavour.sep}'
+
         if pattern.startswith(prefix):
             pattern = pattern.replace(prefix, '', 1)
+
+        key_prefix = self._path.key
+        if key_prefix:
+            prefix = self._path._flavour.sep.join((key_prefix, prefix))
         return prefix, pattern
 
     def _calculate_pattern_level(self, pattern):
         if '**' in pattern:
             return None
         if self._prefix:
             pattern = f'{self._prefix}{self._path._flavour.sep}{pattern}'
@@ -673,15 +677,14 @@
 
     def _deep_cached_dir_scan(self):
         cache = _DeepDirCache()
         prefix_sep_count = self._prefix.count(self._path._flavour.sep)
         for key in self._path._accessor.iter_keys(self._path, prefix=self._prefix, full_keys=self._full_keys):
             key_sep_count = key.count(self._path._flavour.sep) + 1
             key_parts = key.rsplit(self._path._flavour.sep, maxsplit=key_sep_count - prefix_sep_count)
-            key_parts_count = sum(1 for _ in key.split(self._path._flavour.sep) if _)
             target_path_parts = key_parts[:self._target_level]
             target_path = (self._path._flavour.sep).join(target_path_parts)
             if cache.in_cache(target_path):
                 continue
             yield target_path
             cache.add(target_path_parts)
 
@@ -771,14 +774,21 @@
         self._absolute_path_validation()
         with suppress(ValueError):
             _, bucket, *_ = self.parts
             return bucket
         return ''
 
     @property
+    def is_bucket(self):
+        """
+        Check if Path is a bucket
+        """
+        return self.is_absolute() and self == PureS3Path(f"/{self.bucket}")
+
+    @property
     def key(self):
         """
         The AWS S3 Key name, or ''
         """
         self._absolute_path_validation()
         key = self._flavour.sep.join(self.parts[2:])
         return key
```

### Comparing `s3path-0.4.1/setup.py` & `s3path-0.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 setup(
     name='s3path',
-    version='0.4.1',
+    version='0.4.2',
     url='https://github.com/liormizr/s3path',
     author='Lior Mizrahi',
     author_email='li.mizr@gmail.com',
     py_modules=['s3path'],
     install_requires=[
         'boto3>=1.16.35',
         'packaging',
```

