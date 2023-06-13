# Comparing `tmp/JBPhD-2.2.7.tar.gz` & `tmp/JBPhD-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.2.7.tar", last modified: Mon Jun 12 11:59:38 2023, max compression
+gzip compressed data, was "JBPhD-2.2.8.tar", last modified: Mon Jun 12 12:06:01 2023, max compression
```

## Comparing `JBPhD-2.2.7.tar` & `JBPhD-2.2.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:59:38.000000 JBPhD-2.2.7/
-drwxrwxrwx   0        0        0        0 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      269 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1597 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      137 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-12 11:59:38.000000 JBPhD-2.2.7/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      269 2023-06-12 11:59:40.000000 JBPhD-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 11:59:38.000000 JBPhD-2.2.7/Task/
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.7/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.7/Task/Api2.json
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.2.7/Task/BL.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.2.7/Task/BR.PNG
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.2.7/Task/Back_Left.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.2.7/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.7/Task/Consent Form.docx
--rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.2.7/Task/Consent.py
--rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.7/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12380 2023-05-24 14:20:54.000000 JBPhD-2.2.7/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.2.7/Task/Email Errors.txt
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.7/Task/Email Output.py
--rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.7/Task/Export.py
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.2.7/Task/FL.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.2.7/Task/FR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.2.7/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.2.7/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.7/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.2.7/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.2.7/Task/Inverse_Back_Right.PNG
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.2.7/Task/Inverse_Front_Left.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.2.7/Task/Inverse_Front_Right.PNG
--rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.2.7/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.7/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.7/Task/N-Back Revision.py
--rw-rw-rw-   0        0        0        2 2023-06-10 22:28:00.000000 JBPhD-2.2.7/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    22361 2023-06-10 22:31:34.000000 JBPhD-2.2.7/Task/N-Back.py
--rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.7/Task/PIS.docx
--rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.7/Task/PIS.txt
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.7/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.7/Task/README.txt.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 16:10:30.000000 JBPhD-2.2.7/Task/RT count.txt
--rw-rw-rw-   0        0        0    20946 2023-06-09 15:09:44.000000 JBPhD-2.2.7/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.7/Task/Suffix.bat
--rw-rw-rw-   0        0        0        3 2023-06-09 14:46:16.000000 JBPhD-2.2.7/Task/Switch count.txt
--rw-rw-rw-   0        0        0    30735 2023-06-10 22:31:22.000000 JBPhD-2.2.7/Task/Switching.py
--rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.7/Task/Task.py
--rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.2.7/Task/Trial.py
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.2.7/Task/UBL.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.2.7/Task/UBR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.2.7/Task/UFL.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.2.7/Task/UFR.PNG
-drwxrwxrwx   0        0        0        0 2023-06-12 11:59:38.000000 JBPhD-2.2.7/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.7/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.7/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.2.7/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.2.7/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.7/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/circle.jpg
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.7/Task/help.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.7/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.7/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.7/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.7/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.7/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 22:47:06.000000 JBPhD-2.2.7/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.7/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.7/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.7/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.7/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-06-12 11:59:40.000000 JBPhD-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-12 11:58:36.000000 JBPhD-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1597 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      269 2023-06-12 12:06:02.000000 JBPhD-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/Task/
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.8/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.8/Task/Api2.json
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.2.8/Task/BL.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.2.8/Task/BR.PNG
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Back_Left.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.8/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.2.8/Task/Consent.py
+-rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.8/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    12380 2023-05-24 14:20:54.000000 JBPhD-2.2.8/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.2.8/Task/Email Errors.txt
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.8/Task/Email Output.py
+-rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.8/Task/Export.py
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.2.8/Task/FL.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.2.8/Task/FR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.8/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.2.8/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.2.8/Task/Inverse_Back_Right.PNG
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.2.8/Task/Inverse_Front_Left.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.2.8/Task/Inverse_Front_Right.PNG
+-rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.2.8/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.8/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.8/Task/N-Back Revision.py
+-rw-rw-rw-   0        0        0        2 2023-06-10 22:28:00.000000 JBPhD-2.2.8/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    22361 2023-06-10 22:31:34.000000 JBPhD-2.2.8/Task/N-Back.py
+-rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.8/Task/PIS.docx
+-rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.8/Task/PIS.txt
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.8/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.8/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 16:10:30.000000 JBPhD-2.2.8/Task/RT count.txt
+-rw-rw-rw-   0        0        0    20946 2023-06-09 15:09:44.000000 JBPhD-2.2.8/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.8/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        3 2023-06-09 14:46:16.000000 JBPhD-2.2.8/Task/Switch count.txt
+-rw-rw-rw-   0        0        0    30735 2023-06-10 22:31:22.000000 JBPhD-2.2.8/Task/Switching.py
+-rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.8/Task/Task.py
+-rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.2.8/Task/Trial.py
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.2.8/Task/UBL.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.2.8/Task/UBR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.2.8/Task/UFL.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.2.8/Task/UFR.PNG
+drwxrwxrwx   0        0        0        0 2023-06-12 12:06:02.000000 JBPhD-2.2.8/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.8/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.8/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.2.8/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.2.8/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.8/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/circle.jpg
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.8/Task/help.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.8/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.8/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.8/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.8/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.8/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-06-10 22:47:06.000000 JBPhD-2.2.8/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.8/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.8/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.8/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:06:02.000000 JBPhD-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-06-12 12:05:22.000000 JBPhD-2.2.8/setup.py
```

### Comparing `JBPhD-2.2.7/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.2.8/JBPhD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Api.json` & `JBPhD-2.2.8/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Api2.json` & `JBPhD-2.2.8/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/BL.PNG` & `JBPhD-2.2.8/Task/BL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/BR.PNG` & `JBPhD-2.2.8/Task/BR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Back_Left.PNG` & `JBPhD-2.2.8/Task/Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Back_Right.PNG` & `JBPhD-2.2.8/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Consent Form.docx` & `JBPhD-2.2.8/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Consent.py` & `JBPhD-2.2.8/Task/Consent.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Dependencies.py` & `JBPhD-2.2.8/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Dependency Installation.py` & `JBPhD-2.2.8/Task/Dependency Installation.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Email Output.py` & `JBPhD-2.2.8/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Export.py` & `JBPhD-2.2.8/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/FL.PNG` & `JBPhD-2.2.8/Task/FL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/FR.PNG` & `JBPhD-2.2.8/Task/FR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Front_Left.PNG` & `JBPhD-2.2.8/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Front_Right.PNG` & `JBPhD-2.2.8/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Graph.py` & `JBPhD-2.2.8/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/ImageSample.PNG` & `JBPhD-2.2.8/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Inverse_Back_Left.PNG` & `JBPhD-2.2.8/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Inverse_Back_Right.PNG` & `JBPhD-2.2.8/Task/Inverse_Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Inverse_Front_Left.PNG` & `JBPhD-2.2.8/Task/Inverse_Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Inverse_Front_Right.PNG` & `JBPhD-2.2.8/Task/Inverse_Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Manikin Back Down Left.png` & `JBPhD-2.2.8/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Manikin Back Up Right.png` & `JBPhD-2.2.8/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Manikin front Down Right.png` & `JBPhD-2.2.8/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Manikin front Up Right.png` & `JBPhD-2.2.8/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/N-Back Revision.py` & `JBPhD-2.2.8/Task/N-Back Revision.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/N-Back.py` & `JBPhD-2.2.8/Task/N-Back.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/PIS.docx` & `JBPhD-2.2.8/Task/PIS.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/PIS.txt` & `JBPhD-2.2.8/Task/PIS.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Python Install.bat` & `JBPhD-2.2.8/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Reaction Time Task - Copy.py` & `JBPhD-2.2.8/Task/Reaction Time Task - Copy.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Switching.py` & `JBPhD-2.2.8/Task/Switching.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Task.py` & `JBPhD-2.2.8/Task/Task.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/Trial.py` & `JBPhD-2.2.8/Task/Trial.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/UBL.PNG` & `JBPhD-2.2.8/Task/UBL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/UBR.PNG` & `JBPhD-2.2.8/Task/UBR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/UFL.PNG` & `JBPhD-2.2.8/Task/UFL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/UFR.PNG` & `JBPhD-2.2.8/Task/UFR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.2.8/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.2.8/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.2.8/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.2.8/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.2.8/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/asterisk.png` & `JBPhD-2.2.8/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/circle.jpg` & `JBPhD-2.2.8/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/redcross.png` & `JBPhD-2.2.8/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/reddot.png` & `JBPhD-2.2.8/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/setup.py` & `JBPhD-2.2.8/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/trial.jpeg` & `JBPhD-2.2.8/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/uop.ico` & `JBPhD-2.2.8/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/uop.jpeg` & `JBPhD-2.2.8/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/Task/uop.png` & `JBPhD-2.2.8/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.7/setup.py` & `JBPhD-2.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_namespace_packages
 
-packagereqs = ['pysqlite3', 'sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
+packagereqs = ['sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.2.7',
+    version='2.2.8',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
```

