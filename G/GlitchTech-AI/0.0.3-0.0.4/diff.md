# Comparing `tmp/GlitchTech-AI-0.0.3.tar.gz` & `tmp/GlitchTech-AI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlitchTech-AI-0.0.3.tar", last modified: Tue Jun 13 17:56:12 2023, max compression
+gzip compressed data, was "GlitchTech-AI-0.0.4.tar", last modified: Tue Jun 13 17:58:15 2023, max compression
```

## Comparing `GlitchTech-AI-0.0.3.tar` & `GlitchTech-AI-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.387309 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      525 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.388306 GlitchTech-AI-0.0.3/glitchtech_ai/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:51:53.000000 GlitchTech-AI-0.0.3/glitchtech_ai/__init__.py
--rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/glitchtech_ai.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/glitchtech_ai/tools/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/tools/adapter.py
--rw-rw-rw-   0        0        0       42 2023-06-13 17:56:12.390300 GlitchTech-AI-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1045 2023-06-13 17:56:09.000000 GlitchTech-AI-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:15.507186 GlitchTech-AI-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:15.505192 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 17:58:15.000000 GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-06-13 17:58:15.506188 GlitchTech-AI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:15.505192 GlitchTech-AI-0.0.4/glitchtech_ai/
+-rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.4/glitchtech_ai/glitchtech_ai.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:58:15.506188 GlitchTech-AI-0.0.4/glitchtech_ai/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.4/glitchtech_ai/tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.4/glitchtech_ai/tools/adapter.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:58:15.507186 GlitchTech-AI-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-06-13 17:58:10.000000 GlitchTech-AI-0.0.4/setup.py
```

### Comparing `GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/PKG-INFO` & `GlitchTech-AI-0.0.4/GlitchTech_AI.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.3/LICENSE` & `GlitchTech-AI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.3/PKG-INFO` & `GlitchTech-AI-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.3
+Version: 0.0.4
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.3/glitchtech_ai/glitchtech_ai.py` & `GlitchTech-AI-0.0.4/glitchtech_ai/glitchtech_ai.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.3/glitchtech_ai/tools/adapter.py` & `GlitchTech-AI-0.0.4/glitchtech_ai/tools/adapter.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.3/setup.py` & `GlitchTech-AI-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='GlitchTech-AI',
-      version='0.0.3',
+      version='0.0.4',
       description='Basic utility to interface with OpenAI via command line or terminal.',
       keywords='openai cli terminal glitchtech',
       author='Clutch_Reboot',
       author_email='clutchshadow26@gmail.com',
       license='GNU General Public License v3.0',
       packages=[
             'glitchtech_ai',
```

