# Comparing `tmp/JBPhD-2.2.8.tar.gz` & `tmp/JBPhD-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.2.8.tar", last modified: Mon Jun 12 12:06:01 2023, max compression
+gzip compressed data, was "JBPhD-2.2.9.tar", last modified: Tue Jun 13 11:17:10 2023, max compression
```

## Comparing `JBPhD-2.2.8.tar` & `JBPhD-2.2.9.tar`

### file list

```diff
@@ -1,83 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/
-drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/
--rw-rw-rw-   0        0        0      269 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1597 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-12 12:06:00.000000 JBPhD-2.2.8/JBPhD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      269 2023-06-12 12:06:02.000000 JBPhD-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 12:06:00.000000 JBPhD-2.2.8/Task/
--rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.8/Task/Api.json
--rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.8/Task/Api2.json
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.2.8/Task/BL.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.2.8/Task/BR.PNG
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Back_Left.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Back_Right.PNG
--rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.8/Task/Consent Form.docx
--rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.2.8/Task/Consent.py
--rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.8/Task/Dependencies.py
--rw-rw-rw-   0        0        0    12380 2023-05-24 14:20:54.000000 JBPhD-2.2.8/Task/Dependency Installation.py
--rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.2.8/Task/Email Errors.txt
--rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.8/Task/Email Output.py
--rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.8/Task/Export.py
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.2.8/Task/FL.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.2.8/Task/FR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Front_Left.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.2.8/Task/Front_Right.PNG
--rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.8/Task/Graph.py
--rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/ImageSample.PNG
--rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.2.8/Task/Inverse_Back_Left.PNG
--rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.2.8/Task/Inverse_Back_Right.PNG
--rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.2.8/Task/Inverse_Front_Left.PNG
--rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.2.8/Task/Inverse_Front_Right.PNG
--rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.2.8/Task/Location.py
--rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.8/Task/MANIFEST.in.txt
--rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin Back Down Left.png
--rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin Back Up Right.png
--rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin front Down Right.png
--rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/Manikin front Up Right.png
--rw-rw-rw-   0        0        0     3101 2023-05-18 16:38:38.000000 JBPhD-2.2.8/Task/N-Back Revision.py
--rw-rw-rw-   0        0        0        2 2023-06-10 22:28:00.000000 JBPhD-2.2.8/Task/N-Back count.txt
--rw-rw-rw-   0        0        0    22361 2023-06-10 22:31:34.000000 JBPhD-2.2.8/Task/N-Back.py
--rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.8/Task/PIS.docx
--rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.8/Task/PIS.txt
--rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.8/Task/Python Install.bat
--rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.8/Task/README.txt.txt
--rw-rw-rw-   0        0        0        2 2023-05-24 16:10:30.000000 JBPhD-2.2.8/Task/RT count.txt
--rw-rw-rw-   0        0        0    20946 2023-06-09 15:09:44.000000 JBPhD-2.2.8/Task/Reaction Time Task - Copy.py
--rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.8/Task/Suffix.bat
--rw-rw-rw-   0        0        0        3 2023-06-09 14:46:16.000000 JBPhD-2.2.8/Task/Switch count.txt
--rw-rw-rw-   0        0        0    30735 2023-06-10 22:31:22.000000 JBPhD-2.2.8/Task/Switching.py
--rw-rw-rw-   0        0        0    13650 2023-05-18 15:49:20.000000 JBPhD-2.2.8/Task/Task.py
--rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.2.8/Task/Trial.py
--rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.2.8/Task/UBL.PNG
--rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.2.8/Task/UBR.PNG
--rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.2.8/Task/UFL.PNG
--rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.2.8/Task/UFR.PNG
-drwxrwxrwx   0        0        0        0 2023-06-12 12:06:02.000000 JBPhD-2.2.8/Task/__pycache__/
--rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.8/Task/__pycache__/Dependencies.cpython-311.pyc
--rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.8/Task/__pycache__/Export.cpython-311.pyc
--rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.2.8/Task/__pycache__/Location.cpython-311.pyc
--rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.2.8/Task/__pycache__/Task.cpython-311.pyc
--rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.8/Task/__pycache__/spwf.cpython-311.pyc
--rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/asterisk.png
--rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/circle.jpg
--rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.8/Task/help.txt
--rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.8/Task/pins.csv
--rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/redcross.png
--rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/reddot.png
--rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.8/Task/setup.py
--rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.8/Task/spwf.py
--rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.8/Task/spwfoutput.txt
--rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.8/Task/spwfvalue.txt
--rw-rw-rw-   0        0        0       14 2023-06-10 22:47:06.000000 JBPhD-2.2.8/Task/suffix.txt
--rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.8/Task/trial.jpeg
--rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.8/Task/uop.ico
--rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.8/Task/uop.jpeg
--rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.8/Task/uop.png
--rw-rw-rw-   0        0        0       42 2023-06-12 12:06:02.000000 JBPhD-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-06-12 12:05:22.000000 JBPhD-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:17:10.000000 JBPhD-2.2.9/
+drwxrwxrwx   0        0        0        0 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1886 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 11:17:10.000000 JBPhD-2.2.9/JBPhD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-06-06 14:46:58.000000 JBPhD-2.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 16:04:18.000000 JBPhD-2.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      269 2023-06-13 11:17:12.000000 JBPhD-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-07 16:42:22.000000 JBPhD-2.2.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 11:17:10.000000 JBPhD-2.2.9/Task/
+-rw-rw-rw-   0        0        0     2336 2023-04-20 18:29:48.000000 JBPhD-2.2.9/Task/Api.json
+-rw-rw-rw-   0        0        0     2332 2023-04-30 20:14:46.000000 JBPhD-2.2.9/Task/Api2.json
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:39:06.000000 JBPhD-2.2.9/Task/BL.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:52.000000 JBPhD-2.2.9/Task/BR.PNG
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:36:30.000000 JBPhD-2.2.9/Task/Back_Left.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:36:30.000000 JBPhD-2.2.9/Task/Back_Right.PNG
+-rw-rw-rw-   0        0        0    60437 2023-02-02 09:16:10.000000 JBPhD-2.2.9/Task/Consent Form.docx
+-rw-rw-rw-   0        0        0     6403 2023-05-25 21:47:58.000000 JBPhD-2.2.9/Task/Consent.py
+-rw-rw-rw-   0        0        0      911 2023-05-18 15:51:28.000000 JBPhD-2.2.9/Task/Dependencies.py
+-rw-rw-rw-   0        0        0    11435 2023-06-13 10:51:44.000000 JBPhD-2.2.9/Task/Dependency Installation.py
+-rw-rw-rw-   0        0        0      156 2023-05-25 21:19:50.000000 JBPhD-2.2.9/Task/Email Errors.txt
+-rw-rw-rw-   0        0        0      552 2023-05-06 17:47:44.000000 JBPhD-2.2.9/Task/Email Output.py
+-rw-rw-rw-   0        0        0     4074 2023-05-18 15:48:40.000000 JBPhD-2.2.9/Task/Export.py
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:42.000000 JBPhD-2.2.9/Task/FL.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:22.000000 JBPhD-2.2.9/Task/FR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:36:30.000000 JBPhD-2.2.9/Task/Front_Left.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:36:30.000000 JBPhD-2.2.9/Task/Front_Right.PNG
+-rw-rw-rw-   0        0        0      883 2023-04-14 22:45:36.000000 JBPhD-2.2.9/Task/Graph.py
+-rw-rw-rw-   0        0        0   281708 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/ImageSample.PNG
+-rw-rw-rw-   0        0        0   256120 2023-06-06 10:38:02.000000 JBPhD-2.2.9/Task/Inverse_Back_Left.PNG
+-rw-rw-rw-   0        0        0   256871 2023-06-06 10:40:46.000000 JBPhD-2.2.9/Task/Inverse_Back_Right.PNG
+-rw-rw-rw-   0        0        0   249966 2023-06-06 10:40:32.000000 JBPhD-2.2.9/Task/Inverse_Front_Left.PNG
+-rw-rw-rw-   0        0        0   249859 2023-06-06 10:41:18.000000 JBPhD-2.2.9/Task/Inverse_Front_Right.PNG
+-rw-rw-rw-   0        0        0      382 2023-05-25 16:51:56.000000 JBPhD-2.2.9/Task/Location.py
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:35:12.000000 JBPhD-2.2.9/Task/MANIFEST.in.txt
+-rw-rw-rw-   0        0        0    14031 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/Manikin Back Down Left.png
+-rw-rw-rw-   0        0        0    13918 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/Manikin Back Up Right.png
+-rw-rw-rw-   0        0        0    16784 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/Manikin front Down Right.png
+-rw-rw-rw-   0        0        0    20357 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/Manikin front Up Right.png
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:53:28.000000 JBPhD-2.2.9/Task/N-Back count.txt
+-rw-rw-rw-   0        0        0    22361 2023-06-10 22:31:34.000000 JBPhD-2.2.9/Task/N-Back.py
+-rw-rw-rw-   0        0        0   765972 2023-05-24 14:10:50.000000 JBPhD-2.2.9/Task/PIS.docx
+-rw-rw-rw-   0        0        0    20182 2023-05-24 14:11:06.000000 JBPhD-2.2.9/Task/PIS.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 11:17:10.000000 JBPhD-2.2.9/Task/Participant 1/
+-rw-rw-rw-   0        0        0      790 2023-06-13 11:10:50.000000 JBPhD-2.2.9/Task/Participant 1/1 - Combined Reaction Times.csv
+-rw-rw-rw-   0        0        0      486 2023-06-13 11:10:50.000000 JBPhD-2.2.9/Task/Participant 1/1 - Combined Scores.csv
+-rw-rw-rw-   0        0        0     8192 2023-06-13 11:10:50.000000 JBPhD-2.2.9/Task/Participant 1/1 - Combined Scores.db
+-rw-rw-rw-   0        0        0     1229 2023-06-13 10:55:24.000000 JBPhD-2.2.9/Task/Participant 1/1 - Consent.txt
+-rw-rw-rw-   0        0        0      746 2023-06-13 11:10:50.000000 JBPhD-2.2.9/Task/Participant 1/1 - Switching Reaction Times.csv
+-rw-rw-rw-   0        0        0      459 2023-06-13 11:10:50.000000 JBPhD-2.2.9/Task/Participant 1/1 - Switching Score.csv
+-rwxrwxrwx   0        0        0      680 2023-04-23 19:01:06.000000 JBPhD-2.2.9/Task/Python Install.bat
+-rw-rw-rw-   0        0        0       20 2023-05-07 14:41:38.000000 JBPhD-2.2.9/Task/README.txt.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:53:12.000000 JBPhD-2.2.9/Task/RT count.txt
+-rw-rw-rw-   0        0        0    20946 2023-06-09 15:09:44.000000 JBPhD-2.2.9/Task/Reaction Time Task - Copy.py
+-rwxrwxrwx   0        0        0      448 2023-05-07 14:17:02.000000 JBPhD-2.2.9/Task/Suffix.bat
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:16:30.000000 JBPhD-2.2.9/Task/Switch count.txt
+-rw-rw-rw-   0        0        0    30983 2023-06-13 11:04:42.000000 JBPhD-2.2.9/Task/Switching.py
+-rw-rw-rw-   0        0        0    13647 2023-06-13 11:03:28.000000 JBPhD-2.2.9/Task/Task.py
+-rw-rw-rw-   0        0        0     6627 2023-05-24 20:53:36.000000 JBPhD-2.2.9/Task/Trial.py
+-rw-rw-rw-   0        0        0   256274 2023-06-06 10:39:36.000000 JBPhD-2.2.9/Task/UBL.PNG
+-rw-rw-rw-   0        0        0   256511 2023-06-06 10:39:32.000000 JBPhD-2.2.9/Task/UBR.PNG
+-rw-rw-rw-   0        0        0   249107 2023-06-06 10:39:26.000000 JBPhD-2.2.9/Task/UFL.PNG
+-rw-rw-rw-   0        0        0   249006 2023-06-06 10:39:18.000000 JBPhD-2.2.9/Task/UFR.PNG
+drwxrwxrwx   0        0        0        0 2023-06-13 11:17:10.000000 JBPhD-2.2.9/Task/__pycache__/
+-rw-rw-rw-   0        0        0     5027 2023-05-07 22:15:14.000000 JBPhD-2.2.9/Task/__pycache__/Dependencies.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6538 2023-05-24 13:46:36.000000 JBPhD-2.2.9/Task/__pycache__/Export.cpython-311.pyc
+-rw-rw-rw-   0        0        0      698 2023-05-25 16:52:10.000000 JBPhD-2.2.9/Task/__pycache__/Location.cpython-311.pyc
+-rw-rw-rw-   0        0        0    19777 2023-06-04 22:02:52.000000 JBPhD-2.2.9/Task/__pycache__/Task.cpython-311.pyc
+-rw-rw-rw-   0        0        0      931 2023-05-05 14:18:56.000000 JBPhD-2.2.9/Task/__pycache__/spwf.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3162 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/asterisk.png
+-rw-rw-rw-   0        0        0    47189 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/circle.jpg
+-rw-rw-rw-   0        0        0    38788 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/greentick.png
+-rw-rw-rw-   0        0        0       54 2023-05-07 14:31:32.000000 JBPhD-2.2.9/Task/help.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:54:50.000000 JBPhD-2.2.9/Task/participant number.txt
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:12:16.000000 JBPhD-2.2.9/Task/pins.csv
+-rw-rw-rw-   0        0        0    24503 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/redcross.png
+-rw-rw-rw-   0        0        0    98588 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/reddot.png
+-rw-rw-rw-   0        0        0      566 2023-05-07 14:26:16.000000 JBPhD-2.2.9/Task/setup.py
+-rw-rw-rw-   0        0        0      472 2023-05-05 14:17:12.000000 JBPhD-2.2.9/Task/spwf.py
+-rw-rw-rw-   0        0        0       44 2023-04-24 16:27:34.000000 JBPhD-2.2.9/Task/spwfoutput.txt
+-rw-rw-rw-   0        0        0      100 2023-04-24 16:27:34.000000 JBPhD-2.2.9/Task/spwfvalue.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 10:57:50.000000 JBPhD-2.2.9/Task/suffix.txt
+-rw-rw-rw-   0        0        0   161693 2023-04-07 13:54:00.000000 JBPhD-2.2.9/Task/trial.jpeg
+-rw-rw-rw-   0        0        0   432254 2023-05-04 10:35:10.000000 JBPhD-2.2.9/Task/uop.ico
+-rw-rw-rw-   0        0        0     3908 2023-05-04 10:32:40.000000 JBPhD-2.2.9/Task/uop.jpeg
+-rw-rw-rw-   0        0        0     7038 2023-04-16 20:40:14.000000 JBPhD-2.2.9/Task/uop.png
+-rw-rw-rw-   0        0        0       42 2023-06-13 11:17:12.000000 JBPhD-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-06-13 11:14:52.000000 JBPhD-2.2.9/setup.py
```

### Comparing `JBPhD-2.2.8/JBPhD.egg-info/SOURCES.txt` & `JBPhD-2.2.9/JBPhD.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 Task/Inverse_Front_Right.PNG
 Task/Location.py
 Task/MANIFEST.in.txt
 Task/Manikin Back Down Left.png
 Task/Manikin Back Up Right.png
 Task/Manikin front Down Right.png
 Task/Manikin front Up Right.png
-Task/N-Back Revision.py
 Task/N-Back count.txt
 Task/N-Back.py
 Task/PIS.docx
 Task/PIS.txt
 Task/Python Install.bat
 Task/README.txt.txt
 Task/RT count.txt
@@ -53,25 +52,33 @@
 Task/Trial.py
 Task/UBL.PNG
 Task/UBR.PNG
 Task/UFL.PNG
 Task/UFR.PNG
 Task/asterisk.png
 Task/circle.jpg
+Task/greentick.png
 Task/help.txt
+Task/participant number.txt
 Task/pins.csv
 Task/redcross.png
 Task/reddot.png
 Task/setup.py
 Task/spwf.py
 Task/spwfoutput.txt
 Task/spwfvalue.txt
 Task/suffix.txt
 Task/trial.jpeg
 Task/uop.ico
 Task/uop.jpeg
 Task/uop.png
+Task/Participant 1/1 - Combined Reaction Times.csv
+Task/Participant 1/1 - Combined Scores.csv
+Task/Participant 1/1 - Combined Scores.db
+Task/Participant 1/1 - Consent.txt
+Task/Participant 1/1 - Switching Reaction Times.csv
+Task/Participant 1/1 - Switching Score.csv
 Task/__pycache__/Dependencies.cpython-311.pyc
 Task/__pycache__/Export.cpython-311.pyc
 Task/__pycache__/Location.cpython-311.pyc
 Task/__pycache__/Task.cpython-311.pyc
 Task/__pycache__/spwf.cpython-311.pyc
```

### Comparing `JBPhD-2.2.8/Task/Api.json` & `JBPhD-2.2.9/Task/Api.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Api2.json` & `JBPhD-2.2.9/Task/Api2.json`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/BL.PNG` & `JBPhD-2.2.9/Task/BL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/BR.PNG` & `JBPhD-2.2.9/Task/BR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Back_Left.PNG` & `JBPhD-2.2.9/Task/Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Back_Right.PNG` & `JBPhD-2.2.9/Task/Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Consent Form.docx` & `JBPhD-2.2.9/Task/Consent Form.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Consent.py` & `JBPhD-2.2.9/Task/Consent.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Dependencies.py` & `JBPhD-2.2.9/Task/Dependencies.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Dependency Installation.py` & `JBPhD-2.2.9/Task/Dependency Installation.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,23 +75,22 @@
             self.date_label.pack(fill='both', expand=False, )
 
             self.submit_button = Button(master, text="Submit", command=self.submit_form)
             self.submit_button.pack(expand=False, pady=10)
 
         def submit_form(self):
             if all(c.get() == 1 for c in self.checkboxes) and self.name_entry.get() != "":
-                # All checkboxes are ticked and name is entered
                 self.export_answers()
                 self.master.destroy()
-                # Call your task function here
             else:
-                # Not all checkboxes are ticked or name is not entered
                 error_message = "Please ensure that all checkboxes are ticked and your name is entered."
                 error_label = Label(self.master, text=error_message)
                 error_label.pack(fill='both', expand=False, )
+            global consent
+            consent = True
 
         def export_answers(self):
             filename = os.path.join(spwf.folder_name, f"{participant_number} - Consent.txt")
             now = datetime.now()
             dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
             with open(filename, "w") as f:
                 f.write(f"Participant name: {self.name_entry.get()}\n \n")
@@ -112,19 +111,17 @@
         first_line = f.readline()
         words = first_line.split()
         participant_number = None
         for word in words:
             if word.isdigit():
                 participant_number = int(word)
 
-    # create a variable to keep track of whether all buttons have been clicked
     global all_buttons_clicked
     all_buttons_clicked = False
 
-    # modify the command for button2 to set all_buttons_clicked to True
     def emailsupport():
                     email_window = tk.Toplevel()
                     email_window.title("Compose Email")
 
                     # Email body input
                     body_label = tk.Label(email_window, text="Please describe your issue/query in as much detail as possible")
                     body_label.pack(fill='both', expand=False, side=tk.TOP, padx=5, pady=5)
@@ -150,42 +147,30 @@
                         except Exception as e:
                             print(e)
                         email_window.destroy()
 
                     submit_button = tk.Button(email_window, text="Send", command=lambda: send_email(body_text.get("1.0", tk.END)))
                     submit_button.pack(expand=False, side=tk.TOP, padx=5, pady=5)
 
-    def pis2():
-        file_path = "PIS.txt"
-        if file_path:
-            with open(file_path, "r") as f:
-                text = f.read()
-                root = tk.Tk()
-                root.title("Participant Information Sheet")
-                text_widget = tk.Text(root, wrap=tk.WORD)
-                text_widget.insert(tk.END, text)
-                text_widget.pack(fill='both', expand=False)
-                close_button = tk.Button(root, text="Close", command=root.destroy)
-                close_button.pack(fill='both', expand=False, side=tk.BOTTOM, pady = 10)
-                global all_buttons_clicked
-                all_buttons_clicked = True
+            
     def pis():
         os.startfile("PIS.docx")
+        global all_buttons_clicked
+        all_buttons_clicked = True
+        global info
+        info = True
 
     def taskstart():
         global all_buttons_clicked
-        if all_buttons_clicked == True:
-            order = random.randint(1, 2)
-            if order == 1:
-                file_path = "Reaction Time Task - Copy.py"
-            else:
-                file_path = "N-Back.py"
-            
-            subprocess.run([python_path, "Trial.py"], check=True)
-            import Export
+        global info
+        global consent
+        print(all_buttons_clicked)
+        if info and consent == True:
+            subprocess.run([python_path, "Trial.py"], check=True)            
+        import Export
         
     root = tk.Tk()
     fontsize = ("Helvetica", 16)
     fontsize1 = ("Helvetica", 18)
     fontsizesmall = ("Helvetica", 12)
 
     root.attributes("-fullscreen", True)
```

### Comparing `JBPhD-2.2.8/Task/Email Output.py` & `JBPhD-2.2.9/Task/Email Output.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Export.py` & `JBPhD-2.2.9/Task/Export.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/FL.PNG` & `JBPhD-2.2.9/Task/FL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/FR.PNG` & `JBPhD-2.2.9/Task/FR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Front_Left.PNG` & `JBPhD-2.2.9/Task/Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Front_Right.PNG` & `JBPhD-2.2.9/Task/Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Graph.py` & `JBPhD-2.2.9/Task/Graph.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/ImageSample.PNG` & `JBPhD-2.2.9/Task/ImageSample.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Inverse_Back_Left.PNG` & `JBPhD-2.2.9/Task/Inverse_Back_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Inverse_Back_Right.PNG` & `JBPhD-2.2.9/Task/Inverse_Back_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Inverse_Front_Left.PNG` & `JBPhD-2.2.9/Task/Inverse_Front_Left.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Inverse_Front_Right.PNG` & `JBPhD-2.2.9/Task/Inverse_Front_Right.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Manikin Back Down Left.png` & `JBPhD-2.2.9/Task/Manikin Back Down Left.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Manikin Back Up Right.png` & `JBPhD-2.2.9/Task/Manikin Back Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Manikin front Down Right.png` & `JBPhD-2.2.9/Task/Manikin front Down Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Manikin front Up Right.png` & `JBPhD-2.2.9/Task/Manikin front Up Right.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/N-Back.py` & `JBPhD-2.2.9/Task/N-Back.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/PIS.docx` & `JBPhD-2.2.9/Task/PIS.docx`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/PIS.txt` & `JBPhD-2.2.9/Task/PIS.txt`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Python Install.bat` & `JBPhD-2.2.9/Task/Python Install.bat`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Reaction Time Task - Copy.py` & `JBPhD-2.2.9/Task/Reaction Time Task - Copy.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/Switching.py` & `JBPhD-2.2.9/Task/Switching.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,23 @@
 filename3 = os.path.join(spwf.folder_name, f"{participant_number} - Combined Reaction Times.csv")
 filename4 = os.path.join(spwf.folder_name, f"{participant_number} - Combined Scores.csv")
 
 sqlfile = os.path.join(spwf.folder_name, f"{participant_number} - Combined Scores.db")
 con = sqlite3.connect(sqlfile)
 cur = con.cursor()
 #cur.execute("CREATE TABLE Participant(id INTEGER PRIMARY KEY, name TEXT, age INTEGER, email TEXT)")
-#cur.execute("CREATE TABLE Data(Date TEXT, Iteration INTEGER, Score TEXT, RT TEXT, Trial TEXT)")
+
+cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='Data'")
+existing_table = cur.fetchone()
+
+if existing_table:
+    print("Table 'Data' already exists. Carrying on...")
+else:
+    cur.execute("CREATE TABLE Data(Date TEXT, Iteration INTEGER, Score TEXT, RT TEXT, Trial TEXT)")
+    print("Table 'Data' created successfully.")
 
 now = datetime.datetime.now()
 
 date_time_string = now.strftime("%d-%m-%y")
 outputtime = now.strftime("%H:%M")
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
@@ -81,15 +89,14 @@
 RED = (255, 0, 0)
 screen = pygame.display.set_mode(size, pygame.FULLSCREEN)
 
 screen.fill(WHITE)
 
 pygame.display.set_caption("Task")
 
-
 def intro():
     os.environ["SDL_VIDEO_CENTERED"] = "1"
 
     score = 0
 
     done = False
     start_time = pygame.time.get_ticks()
@@ -1039,16 +1046,16 @@
             print("\n\n")
 
 
  
 trialcounter = 0
 
 fileremoval()
-'''show_welcome_screen()
+show_welcome_screen()
 intro()
 introR()
 mathsintro()
-intertrial()'''
+intertrial()
 trialorder()
 exitscreen()
 import Export
 pygame.quit()
```

### Comparing `JBPhD-2.2.8/Task/Task.py` & `JBPhD-2.2.9/Task/Task.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Connected = True
 
     if os.path.exists("participant number.txt"):
         pathnum = True
         
     else:
-        
+       
         import tkinter as tk
         import csv
         from tkinter import simpledialog, messagebox
         import os
 
         class PinSystem:
             def __init__(self, master):
@@ -151,15 +151,14 @@
             if word.isdigit():
                 scount = int(word)
                 
     import spwf
     
     def main():
 
-
         import subprocess
         import random
         import platform
         import os
         import sys
         python_path = sys.executable
```

### Comparing `JBPhD-2.2.8/Task/Trial.py` & `JBPhD-2.2.9/Task/Trial.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/UBL.PNG` & `JBPhD-2.2.9/Task/UBL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/UBR.PNG` & `JBPhD-2.2.9/Task/UBR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/UFL.PNG` & `JBPhD-2.2.9/Task/UFL.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/UFR.PNG` & `JBPhD-2.2.9/Task/UFR.PNG`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/__pycache__/Dependencies.cpython-311.pyc` & `JBPhD-2.2.9/Task/__pycache__/Dependencies.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/__pycache__/Export.cpython-311.pyc` & `JBPhD-2.2.9/Task/__pycache__/Export.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/__pycache__/Location.cpython-311.pyc` & `JBPhD-2.2.9/Task/__pycache__/Location.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/__pycache__/Task.cpython-311.pyc` & `JBPhD-2.2.9/Task/__pycache__/Task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/__pycache__/spwf.cpython-311.pyc` & `JBPhD-2.2.9/Task/__pycache__/spwf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/asterisk.png` & `JBPhD-2.2.9/Task/asterisk.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/circle.jpg` & `JBPhD-2.2.9/Task/circle.jpg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/redcross.png` & `JBPhD-2.2.9/Task/redcross.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/reddot.png` & `JBPhD-2.2.9/Task/reddot.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/setup.py` & `JBPhD-2.2.9/Task/setup.py`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/trial.jpeg` & `JBPhD-2.2.9/Task/trial.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/uop.ico` & `JBPhD-2.2.9/Task/uop.ico`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/uop.jpeg` & `JBPhD-2.2.9/Task/uop.jpeg`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/Task/uop.png` & `JBPhD-2.2.9/Task/uop.png`

 * *Files identical despite different names*

### Comparing `JBPhD-2.2.8/setup.py` & `JBPhD-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 packagereqs = ['sendgrid', 'plyer', 'pygame', 'pandas', 'google-auth', 'google-auth-oauthlib', 'google-auth-httplib2', 'google-api-python-client', 'Pillow', 'Scipy', 'Numpy']
 
 with open('README.txt', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='JBPhD',
-    version='2.2.8',
+    version='2.2.9',
     packages=find_namespace_packages(include=['Task']),
     install_requires=packagereqs,
     entry_points={
         'console_scripts': [
             'myproject = myproject.main:main'
         ]
     },
```

