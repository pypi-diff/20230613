# Comparing `tmp/GlitchTech-AI-0.0.2.tar.gz` & `tmp/GlitchTech-AI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlitchTech-AI-0.0.2.tar", last modified: Tue Jun 13 17:52:43 2023, max compression
+gzip compressed data, was "GlitchTech-AI-0.0.3.tar", last modified: Tue Jun 13 17:56:12 2023, max compression
```

## Comparing `GlitchTech-AI-0.0.2.tar` & `GlitchTech-AI-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:52:43.735176 GlitchTech-AI-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:52:43.731186 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 17:52:43.000000 GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      525 2023-06-13 17:52:43.734180 GlitchTech-AI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 17:52:43.732183 GlitchTech-AI-0.0.2/glitchtech_ai/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:51:53.000000 GlitchTech-AI-0.0.2/glitchtech_ai/__init__.py
--rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.2/glitchtech_ai/glitchtech_ai.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:52:43.734180 GlitchTech-AI-0.0.2/glitchtech_ai/tools/
--rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.2/glitchtech_ai/tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.2/glitchtech_ai/tools/adapter.py
--rw-rw-rw-   0        0        0       42 2023-06-13 17:52:43.735176 GlitchTech-AI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      972 2023-06-13 17:52:41.000000 GlitchTech-AI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.387309 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 17:56:12.000000 GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.388306 GlitchTech-AI-0.0.3/glitchtech_ai/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:51:53.000000 GlitchTech-AI-0.0.3/glitchtech_ai/__init__.py
+-rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/glitchtech_ai.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:56:12.389304 GlitchTech-AI-0.0.3/glitchtech_ai/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.3/glitchtech_ai/tools/adapter.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:56:12.390300 GlitchTech-AI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-06-13 17:56:09.000000 GlitchTech-AI-0.0.3/setup.py
```

### Comparing `GlitchTech-AI-0.0.2/GlitchTech_AI.egg-info/PKG-INFO` & `GlitchTech-AI-0.0.3/GlitchTech_AI.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.2/LICENSE` & `GlitchTech-AI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.2/PKG-INFO` & `GlitchTech-AI-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.2/glitchtech_ai/glitchtech_ai.py` & `GlitchTech-AI-0.0.3/glitchtech_ai/glitchtech_ai.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.2/glitchtech_ai/tools/adapter.py` & `GlitchTech-AI-0.0.3/glitchtech_ai/tools/adapter.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.2/setup.py` & `GlitchTech-AI-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup
 
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='GlitchTech-AI',
-      version='0.0.2',
+      version='0.0.3',
       description='Basic utility to interface with OpenAI via command line or terminal.',
       keywords='openai cli terminal glitchtech',
       author='Clutch_Reboot',
       author_email='clutchshadow26@gmail.com',
       license='GNU General Public License v3.0',
       packages=[
             'glitchtech_ai',
             'glitchtech_ai.tools',
       ],
+      py_modules=[
+            'glitchtech_ai.glitchtech_ai'
+      ],
       entry_points={
             'console_scripts': [
                   'glitchtech-ai = glitchtech_ai:main'
             ]
       },
       zip_safe=False,
       long_description=open('README.md', 'rt').read(),
```

