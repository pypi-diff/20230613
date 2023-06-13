# Comparing `tmp/aichat-cli-0.4.6.tar.gz` & `tmp/aichat-cli-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aichat-cli-0.4.6.tar", last modified: Mon Jun 12 12:16:37 2023, max compression
+gzip compressed data, was "aichat-cli-0.4.7.tar", last modified: Tue Jun 13 18:13:59 2023, max compression
```

## Comparing `aichat-cli-0.4.6.tar` & `aichat-cli-0.4.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:37.063806 aichat-cli-0.4.6/
--rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     5218 2023-06-12 12:16:37.062805 aichat-cli-0.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:37.061806 aichat-cli-0.4.6/aichat_cli.egg-info/
--rw-rw-rw-   0        0        0     5218 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:16:36.000000 aichat-cli-0.4.6/aichat_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 12:16:37.063806 aichat-cli-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-06-12 12:16:06.000000 aichat-cli-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:13:59.526190 aichat-cli-0.4.7/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 15:04:57.000000 aichat-cli-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     5229 2023-06-13 18:13:59.525189 aichat-cli-0.4.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 18:13:59.523172 aichat-cli-0.4.7/aichat_cli.egg-info/
+-rw-rw-rw-   0        0        0     5229 2023-06-13 18:13:59.000000 aichat-cli-0.4.7/aichat_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-13 18:13:59.000000 aichat-cli-0.4.7/aichat_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:13:59.000000 aichat-cli-0.4.7/aichat_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-13 18:13:59.000000 aichat-cli-0.4.7/aichat_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:13:59.000000 aichat-cli-0.4.7/aichat_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:13:59.526190 aichat-cli-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-06-13 18:13:35.000000 aichat-cli-0.4.7/setup.py
```

### Comparing `aichat-cli-0.4.6/LICENSE` & `aichat-cli-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aichat-cli-0.4.6/PKG-INFO` & `aichat-cli-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.6
+Version: 0.4.7
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -46,14 +46,15 @@
 ```
 pip install -r requirements.txt
 ```
 
 4. Run the CLI app:
 
 ```
+cd aichat
 python chatcli.py
 ```
 
 ## OR download it using pip📥📦
 
 ```
 pip install aichat-cli --upgrade
```

### Comparing `aichat-cli-0.4.6/aichat_cli.egg-info/PKG-INFO` & `aichat-cli-0.4.7/aichat_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aichat-cli
-Version: 0.4.6
+Version: 0.4.7
 Summary: A CLI app that allows you to have interactive conversations with different AI bots
 Home-page: https://github.com/TheLime1/aichat-cli
 Author: TheLime1
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -46,14 +46,15 @@
 ```
 pip install -r requirements.txt
 ```
 
 4. Run the CLI app:
 
 ```
+cd aichat
 python chatcli.py
 ```
 
 ## OR download it using pip📥📦
 
 ```
 pip install aichat-cli --upgrade
```

### Comparing `aichat-cli-0.4.6/setup.py` & `aichat-cli-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="aichat-cli",
-    version="0.4.6",
+    version="0.4.7",
     author="TheLime1",
     license="GPLv3",
     description="A CLI app that allows you to have interactive conversations with different AI bots",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

