# Comparing `tmp/shellgenius-0.1.7.tar.gz` & `tmp/shellgenius-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.7.tar", last modified: Tue Jun 13 18:41:07 2023, max compression
+gzip compressed data, was "shellgenius-0.1.8.tar", last modified: Tue Jun 13 20:36:09 2023, max compression
```

## Comparing `shellgenius-0.1.7.tar` & `shellgenius-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.7/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 18:41:07.627063 shellgenius-0.1.7/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3488 2023-06-07 23:47:27.000000 shellgenius-0.1.7/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-13 18:41:07.627063 shellgenius-0.1.7/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-13 18:40:12.000000 shellgenius-0.1.7/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.7/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.7/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5706 2023-06-13 18:26:06.000000 shellgenius-0.1.7/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.957960 shellgenius-0.1.8/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.8/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 20:36:09.947960 shellgenius-0.1.8/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3488 2023-06-07 23:47:27.000000 shellgenius-0.1.8/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-13 20:36:09.957960 shellgenius-0.1.8/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-13 20:36:01.000000 shellgenius-0.1.8/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.947960 shellgenius-0.1.8/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.8/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.8/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5452 2023-06-13 20:35:31.000000 shellgenius-0.1.8/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.947960 shellgenius-0.1.8/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.7/LICENSE` & `shellgenius-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.7/PKG-INFO` & `shellgenius-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.7
+Version: 0.1.8
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
```

### Comparing `shellgenius-0.1.7/README.md` & `shellgenius-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.7/setup.py` & `shellgenius-0.1.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.7/shellgenius/cli.py` & `shellgenius-0.1.8/shellgenius/cli.py`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.7/shellgenius/gpt_integration.py` & `shellgenius-0.1.8/shellgenius/gpt_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,32 +10,37 @@
         {
             "role": "system",
             "content": f"You are an expert in using {os_name} and the shell terminal.",
         },
         {
             "role": "user",
             "content": f"""
-            I will give you a brief description of something I want to achieve in a {os_name} shell.
-            I want you to answer with the command that matches the result I want to produce.
-            The first line of your answer will be the said shell command.
-            Then, I want you to explain it step by step with a bullet list.
-
-            This is very important:
-            * In absolutely no circumstance you are allowed to start your message by anything but the shell command. 
-
-            To be absolutely clear, here is how your answer has to look like:
-            ```{shell_name}
-            command
-            ```
-            ### Explanation:
-            * something
-            * something
-            * something
-            ---
-            {command_description}
+For the given task in a {os_name} shell, I need you to provide the corresponding command along with a step-by-step explanation. Follow these guidelines for your response:
+
+1. Begin your response with the exact shell command.
+2. Follow the command with a step-by-step explanation in bullet point format.
+
+Please note:
+
+* Your response should always start with the shell command. No exceptions.
+
+Here's the required format:
+
+```{shell_name}
+command
+```
+
+### Explanation:
+
+* Step 1: ...
+* Step 2: ...
+* Step 3: ...
+
+---
+{command_description}
             """,
         },
     ]
     return prompt
 
 
 def chatgpt_request(
```

### Comparing `shellgenius-0.1.7/shellgenius.egg-info/PKG-INFO` & `shellgenius-0.1.8/shellgenius.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.7
+Version: 0.1.8
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
```

