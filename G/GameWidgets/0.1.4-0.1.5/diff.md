# Comparing `tmp/GameWidgets-0.1.4.tar.gz` & `tmp/GameWidgets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.4.tar", last modified: Fri Jun  2 23:59:28 2023, max compression
+gzip compressed data, was "GameWidgets-0.1.5.tar", last modified: Tue Jun 13 21:04:41 2023, max compression
```

## Comparing `GameWidgets-0.1.4.tar` & `GameWidgets-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.051373 GameWidgets-0.1.4/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.043373 GameWidgets-0.1.4/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.043373 GameWidgets-0.1.4/GameWidgets/Examples/
--rw-------   0 runner    (1000) runner    (1000)     1717 2023-06-02 23:55:49.000000 GameWidgets-0.1.4/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Examples/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.047373 GameWidgets-0.1.4/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1422 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.047373 GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)     1497 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/Button.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      148 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/Draw.py
--rw-------   0 runner    (1000) runner    (1000)      652 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/ScreenSlide.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.047373 GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      569 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.047373 GameWidgets-0.1.4/GameWidgets/RuntimeTests/
--rw-------   0 runner    (1000) runner    (1000)      649 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/RuntimeTests/AllTest.py
--rw-------   0 runner    (1000) runner    (1000)      397 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/RuntimeTests/GameWidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)      359 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/RuntimeTests/SetUpTest.py
--rw-------   0 runner    (1000) runner    (1000)      369 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/RuntimeTests/WidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/RuntimeTests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.047373 GameWidgets-0.1.4/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1689 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.051373 GameWidgets-0.1.4/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     2980 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      597 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     3643 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/Colors.py
--rw-------   0 runner    (1000) runner    (1000)     1489 2023-06-02 23:55:18.000000 GameWidgets-0.1.4/GameWidgets/Widgets/Cursor.py
--rw-------   0 runner    (1000) runner    (1000)     2761 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/DialogeBox.py
--rw-------   0 runner    (1000) runner    (1000)     1574 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/ImgDecoder.py
--rw-------   0 runner    (1000) runner    (1000)      246 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)     1914 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/TextInp.py
--rw-------   0 runner    (1000) runner    (1000)      159 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      620 2023-05-31 01:38:09.000000 GameWidgets-0.1.4/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      558 2023-06-02 23:59:04.000000 GameWidgets-0.1.4/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 23:59:28.043373 GameWidgets-0.1.4/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      580 2023-06-02 23:59:27.000000 GameWidgets-0.1.4/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1315 2023-06-02 23:59:27.000000 GameWidgets-0.1.4/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 23:59:27.000000 GameWidgets-0.1.4/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-02 23:59:27.000000 GameWidgets-0.1.4/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-02 23:59:27.000000 GameWidgets-0.1.4/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      580 2023-06-02 23:59:28.051373 GameWidgets-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 23:59:28.051373 GameWidgets-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.457100 GameWidgets-0.1.5/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.445100 GameWidgets-0.1.5/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.445100 GameWidgets-0.1.5/GameWidgets/Engine/
+-rw-------   0 runner    (1000) runner    (1000)     1011 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Engine/Backdrop.py
+-rw-------   0 runner    (1000) runner    (1000)      191 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Engine/Entity.py
+-rw-------   0 runner    (1000) runner    (1000)     1041 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Engine/Group.py
+-rw-------   0 runner    (1000) runner    (1000)       81 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Engine/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.449100 GameWidgets-0.1.5/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1766 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.449100 GameWidgets-0.1.5/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.449100 GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.449100 GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      569 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.453101 GameWidgets-0.1.5/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.453101 GameWidgets-0.1.5/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.457100 GameWidgets-0.1.5/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     2980 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     3643 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/Colors.py
+-rw-------   0 runner    (1000) runner    (1000)     1489 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/DialogeBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1914 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)      159 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      620 2023-06-13 21:00:14.000000 GameWidgets-0.1.5/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      567 2023-06-13 21:03:32.000000 GameWidgets-0.1.5/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-13 21:04:41.445100 GameWidgets-0.1.5/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-13 21:04:41.000000 GameWidgets-0.1.5/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1434 2023-06-13 21:04:41.000000 GameWidgets-0.1.5/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-13 21:04:41.000000 GameWidgets-0.1.5/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-06-13 21:04:41.000000 GameWidgets-0.1.5/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-06-13 21:04:41.000000 GameWidgets-0.1.5/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2023-06-13 21:04:41.457100 GameWidgets-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-13 21:04:41.457100 GameWidgets-0.1.5/setup.cfg
```

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/Animatrix.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/Button.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/Button.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/ScreenSlide.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/Sprite.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/Sprite.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.1.5/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/RuntimeTests/AllTest.py` & `GameWidgets-0.1.5/GameWidgets/RuntimeTests/AllTest.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.1.5/GameWidgets/SetUp/ScreenCommands.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/Btn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/Clock.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/Colors.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/Colors.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/Cursor.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/Cursor.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/DialogeBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/ImgDecoder.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/ImgDecoder.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/Widgets/TextInp.py` & `GameWidgets-0.1.5/GameWidgets/Widgets/TextInp.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/__init__.py` & `GameWidgets-0.1.5/GameWidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.4/GameWidgets/setup.py` & `GameWidgets-0.1.5/GameWidgets/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.4",
+    version="0.1.5",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
-    description="Make Games Easier with GameWidgets ",
+    description="Make Game Easier with pygame and GameWidgets",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
     python_requires='>=3.8',
     install_requires=['pygame'],
     packages=find_packages()
```

### Comparing `GameWidgets-0.1.4/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.1.5/GameWidgets.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 GameWidgets/__init__.py
 GameWidgets/setup.py
 GameWidgets.egg-info/PKG-INFO
 GameWidgets.egg-info/SOURCES.txt
 GameWidgets.egg-info/dependency_links.txt
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
+GameWidgets/Engine/Backdrop.py
+GameWidgets/Engine/Entity.py
+GameWidgets/Engine/Group.py
+GameWidgets/Engine/__init__.py
 GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
 GameWidgets/Examples/__init__.py
 GameWidgets/GameWidgets/Animatrix.py
 GameWidgets/GameWidgets/Draw.py
 GameWidgets/GameWidgets/ScreenSlide.py
 GameWidgets/GameWidgets/__init__.py
 GameWidgets/GameWidgets/Controller/Button.py
```

