# Comparing `tmp/gyoza-0.0.3.tar.gz` & `tmp/gyoza-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyoza-0.0.3.tar", last modified: Fri Jun  2 11:53:52 2023, max compression
+gzip compressed data, was "gyoza-0.0.5.tar", last modified: Tue Jun 13 06:53:11 2023, max compression
```

## Comparing `gyoza-0.0.3.tar` & `gyoza-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.590000 gyoza-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-02 09:45:10.000000 gyoza-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      877 2023-06-02 11:53:54.000000 gyoza-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-06-02 09:48:40.000000 gyoza-0.0.3/README.md
--rw-rw-rw-   0        0        0      762 2023-06-02 11:53:24.000000 gyoza-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 11:53:54.000000 gyoza-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-02 11:51:40.000000 gyoza-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.640000 gyoza-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.660000 gyoza-0.0.3/src/gyoza/
--rw-rw-rw-   0        0        0        0 2023-06-02 09:30:44.000000 gyoza-0.0.3/src/gyoza/__init__.py
--rw-rw-rw-   0        0        0      113 2023-06-02 11:31:44.000000 gyoza-0.0.3/src/gyoza/example.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.750000 gyoza-0.0.3/src/gyoza/sub_package_A/
--rw-rw-rw-   0        0        0        0 2023-06-02 11:33:14.000000 gyoza-0.0.3/src/gyoza/sub_package_A/__init__.py
--rw-rw-rw-   0        0        0       35 2023-06-02 11:52:58.000000 gyoza-0.0.3/src/gyoza/sub_package_A/module_A.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.790000 gyoza-0.0.3/src/gyoza/sub_package_B/
--rw-rw-rw-   0        0        0        0 2023-06-02 11:33:16.000000 gyoza-0.0.3/src/gyoza/sub_package_B/__init__.py
--rw-rw-rw-   0        0        0       99 2023-06-02 11:51:50.000000 gyoza-0.0.3/src/gyoza/sub_package_B/module_B.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.700000 gyoza-0.0.3/src/gyoza.egg-info/
--rw-rw-rw-   0        0        0      877 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/top_level.txt
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.191642 gyoza-0.0.5/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.5/LICENSE
+-rw-r--r--   0 timdick    (501) staff       (20)      767 2023-06-13 06:53:11.191391 gyoza-0.0.5/PKG-INFO
+-rwxr-xr-x   0 timdick    (501) staff       (20)      251 2023-06-11 16:18:38.000000 gyoza-0.0.5/README.md
+-rwxr-xr-x   0 timdick    (501) staff       (20)      854 2023-06-13 06:52:52.000000 gyoza-0.0.5/pyproject.toml
+-rw-r--r--   0 timdick    (501) staff       (20)       38 2023-06-13 06:53:11.191722 gyoza-0.0.5/setup.cfg
+-rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-02 11:51:40.000000 gyoza-0.0.5/setup.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.184231 gyoza-0.0.5/src/
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.186305 gyoza-0.0.5/src/gyoza/
+-rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.5/src/gyoza/__init__.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.189454 gyoza-0.0.5/src/gyoza/modelling/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.5/src/gyoza/modelling/__init__.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    19977 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/flow_layers.py
+-rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/losses.py
+-rw-r--r--   0 timdick    (501) staff       (20)     9717 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/masks.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3396 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/standard_layers.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.189722 gyoza-0.0.5/src/gyoza/scripts/
+-rwxr-xr-x   0 timdick    (501) staff       (20)      160 2023-06-13 06:44:04.000000 gyoza-0.0.5/src/gyoza/scripts/demo.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.190950 gyoza-0.0.5/src/gyoza/utilities/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.5/src/gyoza/utilities/__init__.py
+-rwxrwxrwx   0 timdick    (501) staff       (20)       40 2023-06-02 12:29:06.000000 gyoza-0.0.5/src/gyoza/utilities/file_management.py
+-rwxrwxrwx   0 timdick    (501) staff       (20)     1064 2023-06-02 12:38:46.000000 gyoza-0.0.5/src/gyoza/utilities/math.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3746 2023-06-13 06:39:04.000000 gyoza-0.0.5/src/gyoza/utilities/tensors.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.187980 gyoza-0.0.5/src/gyoza.egg-info/
+-rwxrwxrwx   0 timdick    (501) staff       (20)      767 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/PKG-INFO
+-rwxrwxrwx   0 timdick    (501) staff       (20)      548 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/SOURCES.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/dependency_links.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)      100 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/requires.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/top_level.txt
```

### Comparing `gyoza-0.0.3/LICENSE` & `gyoza-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.3/PKG-INFO` & `gyoza-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: gyoza
-Version: 0.0.3
-Summary: A package to study the latent representations of auditory events processing in the human brain.
-Author-email: Tim Dick <timdi@icloud.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Gyoza 
-## A library for explaining latent representations during auditory event recognition in the human brain.
-### Master thesis project of Tim Dick
-https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
+Metadata-Version: 2.1
+Name: gyoza
+Version: 0.0.5
+Summary: A package for invertible interpretable neural networks.
+Author-email: Tim Dick <timdi@icloud.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Gyoza 
+## A library for building invertible neural networks
+### Master thesis project of Tim Dick
+https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
```

### Comparing `gyoza-0.0.3/src/gyoza.egg-info/PKG-INFO` & `gyoza-0.0.5/src/gyoza.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: gyoza
-Version: 0.0.3
-Summary: A package to study the latent representations of auditory events processing in the human brain.
-Author-email: Tim Dick <timdi@icloud.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Gyoza 
-## A library for explaining latent representations during auditory event recognition in the human brain.
-### Master thesis project of Tim Dick
-https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
+Metadata-Version: 2.1
+Name: gyoza
+Version: 0.0.5
+Summary: A package for invertible interpretable neural networks.
+Author-email: Tim Dick <timdi@icloud.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Gyoza 
+## A library for building invertible neural networks
+### Master thesis project of Tim Dick
+https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
```

