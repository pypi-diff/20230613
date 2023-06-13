# Comparing `tmp/InfixToPostfix-1.0.2.tar.gz` & `tmp/InfixToPostfix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InfixToPostfix-1.0.2.tar", last modified: Tue Jun 13 15:58:45 2023, max compression
+gzip compressed data, was "InfixToPostfix-1.0.3.tar", last modified: Tue Jun 13 16:04:11 2023, max compression
```

## Comparing `InfixToPostfix-1.0.2.tar` & `InfixToPostfix-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:58:45.159833 InfixToPostfix-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 15:58:45.154730 InfixToPostfix-1.0.2/InfixToPostfix/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.2/InfixToPostfix/__init__.py
--rw-rw-rw-   0        0        0     7421 2023-06-13 15:54:25.000000 InfixToPostfix-1.0.2/InfixToPostfix/infix_to_postfix.py
--rw-rw-rw-   0        0        0     3794 2023-06-13 15:54:06.000000 InfixToPostfix-1.0.2/InfixToPostfix/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:58:45.157825 InfixToPostfix-1.0.2/InfixToPostfix.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-06-13 15:58:45.000000 InfixToPostfix-1.0.2/InfixToPostfix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-13 15:58:45.000000 InfixToPostfix-1.0.2/InfixToPostfix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:58:45.000000 InfixToPostfix-1.0.2/InfixToPostfix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 15:58:45.000000 InfixToPostfix-1.0.2/InfixToPostfix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1130 2023-06-13 15:58:45.158829 InfixToPostfix-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 15:58:45.159833 InfixToPostfix-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-06-13 15:58:34.000000 InfixToPostfix-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.045188 InfixToPostfix-1.0.3/InfixToPostfix/
+-rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.3/InfixToPostfix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.051274 InfixToPostfix-1.0.3/InfixToPostfix/data/
+-rw-rw-rw-   0        0        0       50 2023-06-11 04:58:52.000000 InfixToPostfix-1.0.3/InfixToPostfix/data/conf
+-rw-rw-rw-   0        0        0      832 2023-06-12 02:48:48.000000 InfixToPostfix-1.0.3/InfixToPostfix/data/style.qss
+-rw-rw-rw-   0        0        0     7421 2023-06-13 15:54:25.000000 InfixToPostfix-1.0.3/InfixToPostfix/infix_to_postfix.py
+-rw-rw-rw-   0        0        0     3794 2023-06-13 15:54:06.000000 InfixToPostfix-1.0.3/InfixToPostfix/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.049269 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-13 16:04:11.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       71 2023-06-13 16:03:26.000000 InfixToPostfix-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1130 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-13 16:04:08.000000 InfixToPostfix-1.0.3/setup.py
```

### Comparing `InfixToPostfix-1.0.2/InfixToPostfix/infix_to_postfix.py` & `InfixToPostfix-1.0.3/InfixToPostfix/infix_to_postfix.py`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.2/InfixToPostfix/ui.py` & `InfixToPostfix-1.0.3/InfixToPostfix/ui.py`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.2/InfixToPostfix.egg-info/PKG-INFO` & `InfixToPostfix-1.0.3/InfixToPostfix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `InfixToPostfix-1.0.2/LICENSE` & `InfixToPostfix-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.2/PKG-INFO` & `InfixToPostfix-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `InfixToPostfix-1.0.2/README.md` & `InfixToPostfix-1.0.3/README.md`

 * *Files identical despite different names*

