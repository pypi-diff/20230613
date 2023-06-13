# Comparing `tmp/InfixToPostfix-1.0.0.tar.gz` & `tmp/InfixToPostfix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InfixToPostfix-1.0.0.tar", last modified: Tue Jun 13 15:20:18 2023, max compression
+gzip compressed data, was "InfixToPostfix-1.0.1.tar", last modified: Tue Jun 13 15:40:31 2023, max compression
```

## Comparing `InfixToPostfix-1.0.0.tar` & `InfixToPostfix-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:20:18.065864 InfixToPostfix-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-13 15:20:18.060811 InfixToPostfix-1.0.0/InfixToPostfix/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.0/InfixToPostfix/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-06-13 05:23:00.000000 InfixToPostfix-1.0.0/InfixToPostfix/infix_to_postfix.py
--rw-rw-rw-   0        0        0     3835 2023-06-13 15:19:02.000000 InfixToPostfix-1.0.0/InfixToPostfix/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:20:18.064858 InfixToPostfix-1.0.0/InfixToPostfix.egg-info/
--rw-rw-rw-   0        0        0     1134 2023-06-13 15:20:18.000000 InfixToPostfix-1.0.0/InfixToPostfix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-13 15:20:18.000000 InfixToPostfix-1.0.0/InfixToPostfix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:20:18.000000 InfixToPostfix-1.0.0/InfixToPostfix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 15:20:18.000000 InfixToPostfix-1.0.0/InfixToPostfix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1134 2023-06-13 15:20:18.065864 InfixToPostfix-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-06-13 06:10:45.000000 InfixToPostfix-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 15:20:18.065864 InfixToPostfix-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-06-13 15:10:30.000000 InfixToPostfix-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:40:31.417344 InfixToPostfix-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 15:40:31.412343 InfixToPostfix-1.0.1/InfixToPostfix/
+-rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.1/InfixToPostfix/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-06-13 05:23:00.000000 InfixToPostfix-1.0.1/InfixToPostfix/infix_to_postfix.py
+-rw-rw-rw-   0        0        0     3835 2023-06-13 15:19:02.000000 InfixToPostfix-1.0.1/InfixToPostfix/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:40:31.416344 InfixToPostfix-1.0.1/InfixToPostfix.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-06-13 15:40:31.000000 InfixToPostfix-1.0.1/InfixToPostfix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-13 15:40:31.000000 InfixToPostfix-1.0.1/InfixToPostfix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:40:31.000000 InfixToPostfix-1.0.1/InfixToPostfix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 15:40:31.000000 InfixToPostfix-1.0.1/InfixToPostfix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1130 2023-06-13 15:40:31.417344 InfixToPostfix-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:40:31.417344 InfixToPostfix-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      481 2023-06-13 15:39:49.000000 InfixToPostfix-1.0.1/setup.py
```

### Comparing `InfixToPostfix-1.0.0/InfixToPostfix/infix_to_postfix.py` & `InfixToPostfix-1.0.1/InfixToPostfix/infix_to_postfix.py`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.0/InfixToPostfix/ui.py` & `InfixToPostfix-1.0.1/InfixToPostfix/ui.py`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.0/InfixToPostfix.egg-info/PKG-INFO` & `InfixToPostfix-1.0.1/InfixToPostfix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# infix_to_postfix
+# InfixToPostfix
 
 A python module converts infix expressions to postfix expressions and includes a visual interface.
 
 ## Table of Contents
 
 - [Install](#install)
 - [Usage](#usage)
 
 ## Install
 
 ```sh
-pip install infix_to_postfix
+pip install InfixToPostfix
 ```
 
 ## Usage
 
 ### No visual interface
 
 ```python
```

### Comparing `InfixToPostfix-1.0.0/LICENSE` & `InfixToPostfix-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.0/PKG-INFO` & `InfixToPostfix-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# infix_to_postfix
+# InfixToPostfix
 
 A python module converts infix expressions to postfix expressions and includes a visual interface.
 
 ## Table of Contents
 
 - [Install](#install)
 - [Usage](#usage)
 
 ## Install
 
 ```sh
-pip install infix_to_postfix
+pip install InfixToPostfix
 ```
 
 ## Usage
 
 ### No visual interface
 
 ```python
```

### Comparing `InfixToPostfix-1.0.0/README.md` & `InfixToPostfix-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# infix_to_postfix
+# InfixToPostfix
 
 A python module converts infix expressions to postfix expressions and includes a visual interface.
 
 ## Table of Contents
 
 - [Install](#install)
 - [Usage](#usage)
 
 ## Install
 
 ```sh
-pip install infix_to_postfix
+pip install InfixToPostfix
 ```
 
 ## Usage
 
 ### No visual interface
 
 ```python
```

