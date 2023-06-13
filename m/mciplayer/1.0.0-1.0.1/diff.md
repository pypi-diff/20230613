# Comparing `tmp/mciplayer-1.0.0.tar.gz` & `tmp/mciplayer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mciplayer-1.0.0.tar", last modified: Mon Jun 12 11:02:33 2023, max compression
+gzip compressed data, was "mciplayer-1.0.1.tar", last modified: Tue Jun 13 06:58:19 2023, max compression
```

## Comparing `mciplayer-1.0.0.tar` & `mciplayer-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:02:33.191900 mciplayer-1.0.0/
--rw-rw-rw-   0        0        0      897 2023-06-12 11:02:33.191900 mciplayer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-06-12 10:04:35.000000 mciplayer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 11:02:33.184342 mciplayer-1.0.0/mciplayer/
--rw-rw-rw-   0        0        0     5337 2023-06-08 08:32:11.000000 mciplayer-1.0.0/mciplayer/__init__.py
--rw-rw-rw-   0        0        0      638 2023-06-07 11:24:43.000000 mciplayer-1.0.0/mciplayer/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:02:33.187895 mciplayer-1.0.0/mciplayer.egg-info/
--rw-rw-rw-   0        0        0      897 2023-06-12 11:02:33.000000 mciplayer-1.0.0/mciplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-06-12 11:02:33.000000 mciplayer-1.0.0/mciplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:02:33.000000 mciplayer-1.0.0/mciplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-12 11:02:33.000000 mciplayer-1.0.0/mciplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5177 2023-06-06 09:39:12.000000 mciplayer-1.0.0/py_mciwnd.cpp
--rw-rw-rw-   0        0        0       42 2023-06-12 11:02:33.191900 mciplayer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      652 2023-06-12 10:59:14.000000 mciplayer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.150887 mciplayer-1.0.1/
+-rw-rw-rw-   0        0        0      950 2023-06-13 06:58:19.150887 mciplayer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-06-13 06:57:58.000000 mciplayer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.146898 mciplayer-1.0.1/mciplayer/
+-rw-rw-rw-   0        0        0     5369 2023-06-13 06:55:45.000000 mciplayer-1.0.1/mciplayer/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-13 06:55:14.000000 mciplayer-1.0.1/mciplayer/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.150887 mciplayer-1.0.1/mciplayer.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5177 2023-06-06 09:39:12.000000 mciplayer-1.0.1/py_mciwnd.cpp
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:58:19.150887 mciplayer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      652 2023-06-12 11:13:03.000000 mciplayer-1.0.1/setup.py
```

### Comparing `mciplayer-1.0.0/PKG-INFO` & `mciplayer-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
 
@@ -20,7 +20,9 @@
 ```python
 from mciplayer import MCIPlayer
 player=MCIPlayer() # Create a player instance, this will also create a MCI window.
 player.open('test.wav') # Open the audio file
 player.play() # Play the audio
 player.wait() # Wait until the audio ends.
 ```
+
+Python 3.12 wheels will be built in this version.
```

### Comparing `mciplayer-1.0.0/README.md` & `mciplayer-1.0.1/mciplayer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: mciplayer
+Version: 1.0.1
+Summary: A simple audio player/recorder using MCI
+Description-Content-Type: text/markdown
+
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
 
 To build this package, you need:
 
 1. Python>=3.6
@@ -14,7 +20,9 @@
 ```python
 from mciplayer import MCIPlayer
 player=MCIPlayer() # Create a player instance, this will also create a MCI window.
 player.open('test.wav') # Open the audio file
 player.play() # Play the audio
 player.wait() # Wait until the audio ends.
 ```
+
+Python 3.12 wheels will be built in this version.
```

### Comparing `mciplayer-1.0.0/mciplayer/__init__.py` & `mciplayer-1.0.1/mciplayer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Main module of mciplayer.
-Defines MCIPlayer class which records and plays audio (mp3,wav,mid).
+Defines MCIPlayer class which records and plays audio (mp3,wav,wmv,etc. ).
 """
 from ._mciwnd import *
 from .tool import MCIError,SupportError,mciplayermethod
 import os
 from uuid import uuid4
 class MCIPlayer():
     @mciplayermethod
@@ -171,8 +171,8 @@
         """
         Waits until the player finishes playing current audio.
         """
         while self.position()<self.end():
             pass
     def __del__(self):
         self.close()
-__all__=['MCIPlayer']
+__all__=['MCIPlayer','MCIError','SupportError']
```

### Comparing `mciplayer-1.0.0/mciplayer.egg-info/PKG-INFO` & `mciplayer-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: mciplayer
-Version: 1.0.0
-Summary: A simple audio player/recorder using MCI
-Description-Content-Type: text/markdown
-
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
 
 To build this package, you need:
 
 1. Python>=3.6
@@ -20,7 +14,9 @@
 ```python
 from mciplayer import MCIPlayer
 player=MCIPlayer() # Create a player instance, this will also create a MCI window.
 player.open('test.wav') # Open the audio file
 player.play() # Play the audio
 player.wait() # Wait until the audio ends.
 ```
+
+Python 3.12 wheels will be built in this version.
```

### Comparing `mciplayer-1.0.0/py_mciwnd.cpp` & `mciplayer-1.0.1/py_mciwnd.cpp`

 * *Files identical despite different names*

### Comparing `mciplayer-1.0.0/setup.py` & `mciplayer-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md','r') as file:
         return file.read()
 if platform.system()!='Windows':
     raise OSError("Please build in Windows!")
 else:
     setup(
         name='mciplayer',
-        version='1.0.0',
+        version='1.0.1',
         description='A simple audio player/recorder using MCI',
         long_description_content_type='text/markdown',
         ext_modules=[
             Extension('mciplayer._mciwnd',sources=['py_mciwnd.cpp'],include_dirs=[get_include()])
         ],
         packages=['mciplayer'],long_description=readme()
     )
```

