# Comparing `tmp/zzdeeprollover-0.0.1.tar.gz` & `tmp/zzdeeprollover-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zzdeeprollover-0.0.1.tar", last modified: Tue Jun 13 05:42:00 2023, max compression
+gzip compressed data, was "dist\zzdeeprollover-0.0.2.tar", last modified: Tue Jun 13 05:53:21 2023, max compression
```

## Comparing `zzdeeprollover-0.0.1.tar` & `zzdeeprollover-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:42:00.943661 zzdeeprollover-0.0.1/
--rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3358 2023-06-13 05:42:00.943661 zzdeeprollover-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-13 05:42:00.946682 zzdeeprollover-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-06-13 05:33:30.000000 zzdeeprollover-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:42:00.925661 zzdeeprollover-0.0.1/zzdeeprollover/
--rw-rw-rw-   0        0        0        7 2023-06-13 05:23:51.000000 zzdeeprollover-0.0.1/zzdeeprollover/version.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 05:42:00.941662 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/
--rw-rw-rw-   0        0        0     3358 2023-06-13 05:42:00.000000 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-13 05:42:00.000000 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:42:00.000000 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-13 05:42:00.000000 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:42:00.000000 zzdeeprollover-0.0.1/zzdeeprollover.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.207754 zzdeeprollover-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3358 2023-06-13 05:53:21.207754 zzdeeprollover-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-13 05:53:21.211753 zzdeeprollover-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-06-13 05:44:55.000000 zzdeeprollover-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.181752 zzdeeprollover-0.0.2/zzdeeprollover/
+-rw-rw-rw-   0        0        0        7 2023-06-13 05:52:20.000000 zzdeeprollover-0.0.2/zzdeeprollover/version.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.205753 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/
+-rw-rw-rw-   0        0        0     3358 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/top_level.txt
```

### Comparing `zzdeeprollover-0.0.1/LICENSE` & `zzdeeprollover-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.1/PKG-INFO` & `zzdeeprollover-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.1 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.2 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
 Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
```

### Comparing `zzdeeprollover-0.0.1/README.md` & `zzdeeprollover-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.1/setup.py` & `zzdeeprollover-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   install_requires=[
     "scikit-learn",
     "torch",
     "numpy",
     "matplotlib",
     "torchvision ",
     "pandas",
-    "PIL",
+    "pillow",
     "opencv-python-headless",
   ],
   packages=setuptools.find_packages(),
   data_files=[
     (
       "zzdeeprollover",
       [
```

### Comparing `zzdeeprollover-0.0.1/zzdeeprollover.egg-info/PKG-INFO` & `zzdeeprollover-0.0.2/zzdeeprollover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.1 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.2 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
 Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
```

