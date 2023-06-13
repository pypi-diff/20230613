# Comparing `tmp/hnne-0.1.8.tar.gz` & `tmp/hnne-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnne-0.1.8.tar", last modified: Wed Nov  2 17:43:22 2022, max compression
+gzip compressed data, was "dist/hnne-0.1.9.tar", last modified: Tue Jun 13 15:21:25 2023, max compression
```

## Comparing `hnne-0.1.8.tar` & `hnne-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mariosk   (1000) mariosk   (1000)        0 2022-11-02 17:43:22.924993 hnne-0.1.8/
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)    20717 2022-03-02 17:57:11.000000 hnne-0.1.8/LICENSE.txt
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     4816 2022-11-02 17:43:22.924993 hnne-0.1.8/PKG-INFO
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     3086 2022-03-25 08:03:54.000000 hnne-0.1.8/README.rst
-drwxrwxr-x   0 mariosk   (1000) mariosk   (1000)        0 2022-11-02 17:43:22.924993 hnne-0.1.8/hnne/
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)       28 2022-03-03 07:50:28.000000 hnne-0.1.8/hnne/__init__.py
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     4164 2022-03-17 23:41:59.000000 hnne-0.1.8/hnne/cool_functions.py
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     6632 2022-11-02 17:30:06.000000 hnne-0.1.8/hnne/finch_clustering.py
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     6559 2022-03-09 18:23:24.000000 hnne-0.1.8/hnne/hierarchical_projection.py
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     1778 2022-03-08 09:22:12.000000 hnne-0.1.8/hnne/point_spreading.py
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)    12191 2022-03-25 17:12:57.000000 hnne-0.1.8/hnne/projector.py
-drwxrwxr-x   0 mariosk   (1000) mariosk   (1000)        0 2022-11-02 17:43:22.924993 hnne-0.1.8/hnne.egg-info/
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     4816 2022-11-02 17:43:22.000000 hnne-0.1.8/hnne.egg-info/PKG-INFO
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)      319 2022-11-02 17:43:22.000000 hnne-0.1.8/hnne.egg-info/SOURCES.txt
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)        1 2022-11-02 17:43:22.000000 hnne-0.1.8/hnne.egg-info/dependency_links.txt
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)       69 2022-11-02 17:43:22.000000 hnne-0.1.8/hnne.egg-info/requires.txt
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)        5 2022-11-02 17:43:22.000000 hnne-0.1.8/hnne.egg-info/top_level.txt
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)      107 2022-11-02 17:43:22.924993 hnne-0.1.8/setup.cfg
--rw-rw-r--   0 mariosk   (1000) mariosk   (1000)     1389 2022-11-02 17:39:24.000000 hnne-0.1.8/setup.py
+drwxr-xr-x   0 mkoulakis (12249) i14staff (10001)        0 2023-06-13 15:21:25.000000 hnne-0.1.9/
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)    20717 2022-03-03 17:02:59.000000 hnne-0.1.9/LICENSE.txt
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     4816 2023-06-13 15:21:25.000000 hnne-0.1.9/PKG-INFO
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     3086 2022-12-13 20:51:25.000000 hnne-0.1.9/README.rst
+drwxr-xr-x   0 mkoulakis (12249) i14staff (10001)        0 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne/
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)       28 2022-03-03 17:02:59.000000 hnne-0.1.9/hnne/__init__.py
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     4164 2022-12-13 20:51:25.000000 hnne-0.1.9/hnne/cool_functions.py
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     6632 2023-06-13 15:15:20.000000 hnne-0.1.9/hnne/finch_clustering.py
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     6559 2022-03-09 18:24:58.000000 hnne-0.1.9/hnne/hierarchical_projection.py
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     1778 2022-03-08 14:34:31.000000 hnne-0.1.9/hnne/point_spreading.py
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)    12191 2023-06-13 15:15:20.000000 hnne-0.1.9/hnne/projector.py
+drwxr-xr-x   0 mkoulakis (12249) i14staff (10001)        0 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     4816 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/PKG-INFO
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)      319 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)        1 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)       74 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/requires.txt
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)        5 2023-06-13 15:21:25.000000 hnne-0.1.9/hnne.egg-info/top_level.txt
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)      107 2023-06-13 15:21:25.000000 hnne-0.1.9/setup.cfg
+-rw-r--r--   0 mkoulakis (12249) i14staff (10001)     1394 2023-06-13 15:16:15.000000 hnne-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hnne-0.1.8/LICENSE.txt` & `hnne-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/PKG-INFO` & `hnne-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnne
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fast hierarchical dimensionality reduction algorithm.
 Home-page: UNKNOWN
 Author: Marios Koulakis, Saquib Sarfraz
 Author-email: marios.koulakis@gmail.com, saquibsarfraz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hnne.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/koulakis/h-nne
```

### Comparing `hnne-0.1.8/README.rst` & `hnne-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne/cool_functions.py` & `hnne-0.1.9/hnne/cool_functions.py`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne/finch_clustering.py` & `hnne-0.1.9/hnne/finch_clustering.py`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne/hierarchical_projection.py` & `hnne-0.1.9/hnne/hierarchical_projection.py`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne/point_spreading.py` & `hnne-0.1.9/hnne/point_spreading.py`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne/projector.py` & `hnne-0.1.9/hnne/projector.py`

 * *Files identical despite different names*

### Comparing `hnne-0.1.8/hnne.egg-info/PKG-INFO` & `hnne-0.1.9/hnne.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnne
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fast hierarchical dimensionality reduction algorithm.
 Home-page: UNKNOWN
 Author: Marios Koulakis, Saquib Sarfraz
 Author-email: marios.koulakis@gmail.com, saquibsarfraz@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://hnne.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/koulakis/h-nne
```

### Comparing `hnne-0.1.8/setup.py` & `hnne-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 
 setuptools.setup(
     name="hnne",
-    version="0.1.8",
+    version="0.1.9",
     author="Marios Koulakis, Saquib Sarfraz",
     author_email="marios.koulakis@gmail.com, saquibsarfraz@gmail.com",
     description="A fast hierarchical dimensionality reduction algorithm.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=['hnne'],
     classifiers=[
@@ -23,15 +23,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     keywords="dimension dimensionality reduction t-sne umap hierarchical clustering finch",
     install_requires=[
         "scipy",
         "numpy<1.23,>=1.18",
-        "sklearn",
+        "scikit-learn",
         "tqdm",
         "pynndescent",
         "typer",
         "pandas",
         "cython",
     ],
     test_suite="pytest",
```

