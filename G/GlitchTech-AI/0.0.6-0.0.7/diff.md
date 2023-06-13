# Comparing `tmp/GlitchTech-AI-0.0.6.tar.gz` & `tmp/GlitchTech-AI-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlitchTech-AI-0.0.6.tar", last modified: Tue Jun 13 19:15:53 2023, max compression
+gzip compressed data, was "GlitchTech-AI-0.0.7.tar", last modified: Tue Jun 13 19:20:46 2023, max compression
```

## Comparing `GlitchTech-AI-0.0.6.tar` & `GlitchTech-AI-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:15:53.165737 GlitchTech-AI-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-13 19:15:53.163741 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 19:15:53.000000 GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      525 2023-06-13 19:15:53.165737 GlitchTech-AI-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 19:15:53.164739 GlitchTech-AI-0.0.6/glitchtech_ai/
--rw-rw-rw-   0        0        0      513 2023-06-13 19:14:21.000000 GlitchTech-AI-0.0.6/glitchtech_ai/__main__.py
--rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.6/glitchtech_ai/test.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:15:53.165737 GlitchTech-AI-0.0.6/glitchtech_ai/tools/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.6/glitchtech_ai/tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.6/glitchtech_ai/tools/adapter.py
--rw-rw-rw-   0        0        0       42 2023-06-13 19:15:53.166733 GlitchTech-AI-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-06-13 19:15:51.000000 GlitchTech-AI-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:20:46.369094 GlitchTech-AI-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-13 19:20:46.366099 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 19:20:46.000000 GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-06-13 19:20:46.368090 GlitchTech-AI-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 19:20:46.367096 GlitchTech-AI-0.0.7/glitchtech_ai/
+-rw-rw-rw-   0        0        0       33 2023-06-13 19:20:19.000000 GlitchTech-AI-0.0.7/glitchtech_ai/__init__.py
+-rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.7/glitchtech_ai/glitchtech_ai.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:20:46.368090 GlitchTech-AI-0.0.7/glitchtech_ai/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.7/glitchtech_ai/tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.7/glitchtech_ai/tools/adapter.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:20:46.369094 GlitchTech-AI-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-06-13 19:18:09.000000 GlitchTech-AI-0.0.7/setup.py
```

### Comparing `GlitchTech-AI-0.0.6/GlitchTech_AI.egg-info/PKG-INFO` & `GlitchTech-AI-0.0.7/GlitchTech_AI.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.6
+Version: 0.0.7
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.6/LICENSE` & `GlitchTech-AI-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.6/PKG-INFO` & `GlitchTech-AI-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.6
+Version: 0.0.7
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.6/glitchtech_ai/__main__.py` & `GlitchTech-AI-0.0.7/glitchtech_ai/glitchtech_ai.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.6/glitchtech_ai/tools/adapter.py` & `GlitchTech-AI-0.0.7/glitchtech_ai/tools/adapter.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.6/setup.py` & `GlitchTech-AI-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='GlitchTech-AI',
-      version='0.0.6',
+      version='0.0.7',
       description='Basic utility to interface with OpenAI via command line or terminal.',
       keywords='openai cli terminal glitchtech',
       author='Clutch_Reboot',
       author_email='clutchshadow26@gmail.com',
       license='GNU General Public License v3.0',
       packages=[
             'glitchtech_ai',
```

