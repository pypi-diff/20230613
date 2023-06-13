# Comparing `tmp/zzdeeprollover-0.0.2.tar.gz` & `tmp/zzdeeprollover-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zzdeeprollover-0.0.2.tar", last modified: Tue Jun 13 05:53:21 2023, max compression
+gzip compressed data, was "dist\zzdeeprollover-0.0.3.tar", last modified: Tue Jun 13 06:17:41 2023, max compression
```

## Comparing `zzdeeprollover-0.0.2.tar` & `zzdeeprollover-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.207754 zzdeeprollover-0.0.2/
--rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3358 2023-06-13 05:53:21.207754 zzdeeprollover-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-06-13 05:53:21.211753 zzdeeprollover-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-06-13 05:44:55.000000 zzdeeprollover-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.181752 zzdeeprollover-0.0.2/zzdeeprollover/
--rw-rw-rw-   0        0        0        7 2023-06-13 05:52:20.000000 zzdeeprollover-0.0.2/zzdeeprollover/version.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 05:53:21.205753 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/
--rw-rw-rw-   0        0        0     3358 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:53:20.000000 zzdeeprollover-0.0.2/zzdeeprollover.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 06:17:41.781929 zzdeeprollover-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2020-10-14 12:48:01.000000 zzdeeprollover-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3511 2023-06-13 06:17:41.782931 zzdeeprollover-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-06-12 11:29:13.000000 zzdeeprollover-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-13 06:17:41.785918 zzdeeprollover-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-06-13 06:12:14.000000 zzdeeprollover-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:17:41.755918 zzdeeprollover-0.0.3/zzdeeprollover/
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:16:29.000000 zzdeeprollover-0.0.3/zzdeeprollover/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-06-10 11:25:00.000000 zzdeeprollover-0.0.3/zzdeeprollover/cleanFolders.py
+-rw-rw-rw-   0        0        0     5265 2023-06-13 05:17:19.000000 zzdeeprollover-0.0.3/zzdeeprollover/createInitialImages.py
+-rw-rw-rw-   0        0        0     2187 2023-06-13 05:17:08.000000 zzdeeprollover-0.0.3/zzdeeprollover/createTrainOrTestDataset.py
+-rw-rw-rw-   0        0        0     7459 2023-06-13 05:16:58.000000 zzdeeprollover-0.0.3/zzdeeprollover/createValidationVideo.py
+-rw-rw-rw-   0        0        0      920 2023-06-12 10:21:09.000000 zzdeeprollover-0.0.3/zzdeeprollover/dataTransformationAugmentations.py
+-rw-rw-rw-   0        0        0    15694 2023-06-13 05:16:47.000000 zzdeeprollover-0.0.3/zzdeeprollover/detectRolloverFrames.py
+-rw-rw-rw-   0        0        0     1553 2023-06-11 15:05:34.000000 zzdeeprollover-0.0.3/zzdeeprollover/imageTransformFunctions.py
+-rw-rw-rw-   0        0        0     5773 2023-06-13 05:15:44.000000 zzdeeprollover-0.0.3/zzdeeprollover/learnModel.py
+-rw-rw-rw-   0        0        0     3026 2022-07-03 09:38:10.000000 zzdeeprollover-0.0.3/zzdeeprollover/seq_to_avi.py
+-rw-rw-rw-   0        0        0        7 2023-06-13 06:17:23.000000 zzdeeprollover-0.0.3/zzdeeprollover/version.txt
+-rw-rw-rw-   0        0        0     4534 2022-08-11 00:39:47.000000 zzdeeprollover-0.0.3/zzdeeprollover/zzVideoReading.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:17:41.780951 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/
+-rw-rw-rw-   0        0        0     3511 2023-06-13 06:17:41.000000 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-13 06:17:41.000000 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:17:41.000000 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-13 06:17:41.000000 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 06:17:41.000000 zzdeeprollover-0.0.3/zzdeeprollover.egg-info/top_level.txt
```

### Comparing `zzdeeprollover-0.0.2/LICENSE` & `zzdeeprollover-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.2/PKG-INFO` & `zzdeeprollover-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <H1 CLASS="western" style="text-align:center;">ZZDeepRollover</H1>
 
 This code enables the detection of rollovers performed by zebrafish larvae tracked by the open-source software <a href="https://github.com/oliviermirat/ZebraZoom" target="_blank">ZebraZoom</a>. This code is still in "beta mode". For more information visit <a href="https://zebrazoom.org/" target="_blank">zebrazoom.org</a> or email us at info@zebrazoom.org<br/>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.2 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.3 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
-Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
+Learning,Rolling Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
 This code enables the detection of rollovers performed by zebrafish larvae
 tracked by the open-source software ZebraZoom. This code is still in "beta
 mode". For more information visit zebrazoom.org or email us at
 info@zebrazoom.org
 ***** Road Map: *****
```

### Comparing `zzdeeprollover-0.0.2/README.md` & `zzdeeprollover-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zzdeeprollover-0.0.2/setup.py` & `zzdeeprollover-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,10 +37,13 @@
       [
         "zzdeeprollover/version.txt"
       ],
     )
   ],
   include_package_data=True,
   classifiers=[
-    'Programming Language :: Python :: 3'
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8'
   ],
 )
```

### Comparing `zzdeeprollover-0.0.2/zzdeeprollover.egg-info/PKG-INFO` & `zzdeeprollover-0.0.3/zzdeeprollover.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: zzdeeprollover
-Version: 0.0.2
+Version: 0.0.3
 Summary: Detect rollovers in zebrafish larvae
 Home-page: https://github.com/oliviermirat/ZZDeepRollover
 Download-URL: https://github.com/oliviermirat/ZZDeepRollover/releases/latest
 Author: Olivier Mirat
 Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0
 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep Learning,Rolling
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <H1 CLASS="western" style="text-align:center;">ZZDeepRollover</H1>
 
 This code enables the detection of rollovers performed by zebrafish larvae tracked by the open-source software <a href="https://github.com/oliviermirat/ZebraZoom" target="_blank">ZebraZoom</a>. This code is still in "beta mode". For more information visit <a href="https://zebrazoom.org/" target="_blank">zebrazoom.org</a> or email us at info@zebrazoom.org<br/>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.2 Summary: Detect
+Metadata-Version: 2.1 Name: zzdeeprollover Version: 0.0.3 Summary: Detect
 rollovers in zebrafish larvae Home-page: https://github.com/oliviermirat/
 ZZDeepRollover Download-URL: https://github.com/oliviermirat/ZZDeepRollover/
 releases/latest Author: Olivier Mirat Author-email: olivier.mirat.om@gmail.com
 License: AGPL-3.0 Keywords: Animal,Behavior,Tracking,Zebrafish,Deep
-Learning,Rolling Classifier: Programming Language :: Python :: 3 Description-
+Learning,Rolling Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** ZZDeepRollover ******
 This code enables the detection of rollovers performed by zebrafish larvae
 tracked by the open-source software ZebraZoom. This code is still in "beta
 mode". For more information visit zebrazoom.org or email us at
 info@zebrazoom.org
 ***** Road Map: *****
```

