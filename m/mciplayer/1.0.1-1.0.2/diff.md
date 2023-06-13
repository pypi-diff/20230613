# Comparing `tmp/mciplayer-1.0.1.tar.gz` & `tmp/mciplayer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mciplayer-1.0.1.tar", last modified: Tue Jun 13 06:58:19 2023, max compression
+gzip compressed data, was "mciplayer-1.0.2.tar", last modified: Tue Jun 13 07:19:59 2023, max compression
```

## Comparing `mciplayer-1.0.1.tar` & `mciplayer-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.150887 mciplayer-1.0.1/
--rw-rw-rw-   0        0        0      950 2023-06-13 06:58:19.150887 mciplayer-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-06-13 06:57:58.000000 mciplayer-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.146898 mciplayer-1.0.1/mciplayer/
--rw-rw-rw-   0        0        0     5369 2023-06-13 06:55:45.000000 mciplayer-1.0.1/mciplayer/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-13 06:55:14.000000 mciplayer-1.0.1/mciplayer/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:58:19.150887 mciplayer-1.0.1/mciplayer.egg-info/
--rw-rw-rw-   0        0        0      950 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 06:58:19.000000 mciplayer-1.0.1/mciplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5177 2023-06-06 09:39:12.000000 mciplayer-1.0.1/py_mciwnd.cpp
--rw-rw-rw-   0        0        0       42 2023-06-13 06:58:19.150887 mciplayer-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      652 2023-06-12 11:13:03.000000 mciplayer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:19:59.946517 mciplayer-1.0.2/
+-rw-rw-rw-   0        0        0      950 2023-06-13 07:19:59.946517 mciplayer-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-06-13 06:57:58.000000 mciplayer-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:19:59.938737 mciplayer-1.0.2/mciplayer/
+-rw-rw-rw-   0        0        0     6260 2023-06-13 07:19:28.000000 mciplayer-1.0.2/mciplayer/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-13 06:55:14.000000 mciplayer-1.0.2/mciplayer/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:19:59.946517 mciplayer-1.0.2/mciplayer.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-06-13 07:19:59.000000 mciplayer-1.0.2/mciplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-13 07:19:59.000000 mciplayer-1.0.2/mciplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:19:59.000000 mciplayer-1.0.2/mciplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-13 07:19:59.000000 mciplayer-1.0.2/mciplayer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 07:19:59.000000 mciplayer-1.0.2/mciplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5177 2023-06-06 09:39:12.000000 mciplayer-1.0.2/py_mciwnd.cpp
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:19:59.946517 mciplayer-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-13 07:19:50.000000 mciplayer-1.0.2/setup.py
```

### Comparing `mciplayer-1.0.1/PKG-INFO` & `mciplayer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-1.0.1/README.md` & `mciplayer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mciplayer-1.0.1/mciplayer/__init__.py` & `mciplayer-1.0.2/mciplayer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Main module of mciplayer.
 Defines MCIPlayer class which records and plays audio (mp3,wav,wmv,etc. ).
 """
 from ._mciwnd import *
 from .tool import MCIError,SupportError,mciplayermethod
 import os
 from uuid import uuid4
+from argparse import *
 class MCIPlayer():
     @mciplayermethod
     def __init__(self,filename=None):
         """
         Creates a player instance
         If filename is given, it will create a player which has opened the given filename,otherwise it will create a player not opening anything.
         """
@@ -170,9 +171,35 @@
     def wait(self):
         """
         Waits until the player finishes playing current audio.
         """
         while self.position()<self.end():
             pass
     def __del__(self):
+        """
+        Close the player before deletion.
+        """
         self.close()
+def _play_demo():
+    """
+    Demostration for playing.
+    """
+    a=ArgumentParser()
+    a.add_argument('audio_name',help='Input audio file name')
+    p=a.parse_args()
+    player=MCIPlayer(p.audio_name) # Create player instance.
+    player.play() # Play audio.
+    player.wait() # Wait for the audio ends.
+def _record_demo():
+    """
+    Demostration for recording.
+    """
+    a=ArgumentParser()
+    a.add_argument('audio_name',help='Output audio file name.')
+    a.add_argument('record_secs',help='Number of seconds to record.')
+    p=a.parse_args()
+    player=MCIPlayer() # Create player instance.
+    player.enable_record() # Enable recording.
+    player.start_record() # Record.
+    __import__('time').sleep(float(p.record_secs)) # Wait.
+    player.save(p.audio_name)
 __all__=['MCIPlayer','MCIError','SupportError']
```

### Comparing `mciplayer-1.0.1/mciplayer/tool.py` & `mciplayer-1.0.2/mciplayer/tool.py`

 * *Files identical despite different names*

### Comparing `mciplayer-1.0.1/mciplayer.egg-info/PKG-INFO` & `mciplayer-1.0.2/mciplayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-1.0.1/py_mciwnd.cpp` & `mciplayer-1.0.2/py_mciwnd.cpp`

 * *Files identical despite different names*

### Comparing `mciplayer-1.0.1/setup.py` & `mciplayer-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup,Extension
 from pybind11 import get_include
 import platform,sys
 def readme():
     with open('README.md','r') as file:
         return file.read()
-if platform.system()!='Windows':
+if platform.system()!='Windows': # Must be a Windows operating system.
     raise OSError("Please build in Windows!")
 else:
     setup(
         name='mciplayer',
-        version='1.0.1',
+        version='1.0.2',
         description='A simple audio player/recorder using MCI',
         long_description_content_type='text/markdown',
         ext_modules=[
             Extension('mciplayer._mciwnd',sources=['py_mciwnd.cpp'],include_dirs=[get_include()])
         ],
-        packages=['mciplayer'],long_description=readme()
+        packages=['mciplayer'],long_description=readme(),
+        entry_points={
+            'console_scripts':[
+                'play_demo=mciplayer:_play_demo',
+                'record_demo=mciplayer:_record_demo'
+            ]
+        }
     )
```

