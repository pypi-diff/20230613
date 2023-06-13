# Comparing `tmp/InfixToPostfix-1.0.3.tar.gz` & `tmp/InfixToPostfix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InfixToPostfix-1.0.3.tar", last modified: Tue Jun 13 16:04:11 2023, max compression
+gzip compressed data, was "InfixToPostfix-1.0.4.tar", last modified: Tue Jun 13 16:10:17 2023, max compression
```

## Comparing `InfixToPostfix-1.0.3.tar` & `InfixToPostfix-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.045188 InfixToPostfix-1.0.3/InfixToPostfix/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.3/InfixToPostfix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.051274 InfixToPostfix-1.0.3/InfixToPostfix/data/
--rw-rw-rw-   0        0        0       50 2023-06-11 04:58:52.000000 InfixToPostfix-1.0.3/InfixToPostfix/data/conf
--rw-rw-rw-   0        0        0      832 2023-06-12 02:48:48.000000 InfixToPostfix-1.0.3/InfixToPostfix/data/style.qss
--rw-rw-rw-   0        0        0     7421 2023-06-13 15:54:25.000000 InfixToPostfix-1.0.3/InfixToPostfix/infix_to_postfix.py
--rw-rw-rw-   0        0        0     3794 2023-06-13 15:54:06.000000 InfixToPostfix-1.0.3/InfixToPostfix/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:04:11.049269 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-13 16:04:11.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 16:04:10.000000 InfixToPostfix-1.0.3/InfixToPostfix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       71 2023-06-13 16:03:26.000000 InfixToPostfix-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1130 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 16:04:11.052295 InfixToPostfix-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-13 16:04:08.000000 InfixToPostfix-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.274660 InfixToPostfix-1.0.4/InfixToPostfix/
+-rw-rw-rw-   0        0        0        0 2023-06-12 05:01:03.000000 InfixToPostfix-1.0.4/InfixToPostfix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.279676 InfixToPostfix-1.0.4/InfixToPostfix/data/
+-rw-rw-rw-   0        0        0       50 2023-06-11 04:58:52.000000 InfixToPostfix-1.0.4/InfixToPostfix/data/conf
+-rw-rw-rw-   0        0        0      832 2023-06-12 02:48:48.000000 InfixToPostfix-1.0.4/InfixToPostfix/data/style.qss
+-rw-rw-rw-   0        0        0     7462 2023-06-13 16:09:07.000000 InfixToPostfix-1.0.4/InfixToPostfix/infix_to_postfix.py
+-rw-rw-rw-   0        0        0     3835 2023-06-13 16:08:57.000000 InfixToPostfix-1.0.4/InfixToPostfix/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:10:17.277670 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 16:10:17.000000 InfixToPostfix-1.0.4/InfixToPostfix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35148 2023-06-13 15:13:02.000000 InfixToPostfix-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       71 2023-06-13 16:03:26.000000 InfixToPostfix-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1130 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-13 15:37:48.000000 InfixToPostfix-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:10:17.280691 InfixToPostfix-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-13 16:09:22.000000 InfixToPostfix-1.0.4/setup.py
```

### Comparing `InfixToPostfix-1.0.3/InfixToPostfix/data/style.qss` & `InfixToPostfix-1.0.4/InfixToPostfix/data/style.qss`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.3/InfixToPostfix/infix_to_postfix.py` & `InfixToPostfix-1.0.4/InfixToPostfix/infix_to_postfix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 import string
 
 
 class InfixToPostfix:
-    CONFI_PATH = "data/conf"
+    CONFI_PATH = os.path.join(os.path.dirname(__file__), "data/conf")
 
     @staticmethod
     def is_value(value) -> bool:
         for char in value:
             if char not in string.ascii_lowercase:
                 break
         else:
```

### Comparing `InfixToPostfix-1.0.3/InfixToPostfix/ui.py` & `InfixToPostfix-1.0.4/InfixToPostfix/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PyQt6 import QtWidgets, QtCore
 from PyQt6.QtWidgets import QWidget, QGridLayout, QPushButton, QLineEdit, QFileDialog, QLabel, QTableWidget
 
 from InfixToPostfix.infix_to_postfix import InfixToPostfix
 
 
 class MainWindow(QWidget):
-    STYLE_QSS_PATH = "data/style.qss"
+    STYLE_QSS_PATH = os.path.join(os.path.dirname(__file__), "data/style.qss")
 
     def __init__(self):
         super().__init__()
         self.setWindowTitle("后缀表达式生成器")
         self.setStyleSheet(open(MainWindow.STYLE_QSS_PATH).read())
         self.resize(1280, 720)
         self.conf = ""
```

### Comparing `InfixToPostfix-1.0.3/InfixToPostfix.egg-info/PKG-INFO` & `InfixToPostfix-1.0.4/InfixToPostfix.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `InfixToPostfix-1.0.3/LICENSE` & `InfixToPostfix-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.3/PKG-INFO` & `InfixToPostfix-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InfixToPostfix
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python module converts infix expressions to postfix expressions and includes a visual interface.
 Home-page: https://github.com/RoiexLee/InfixToPostfiX
 Author: RoiexLee
 Author-email: luoyixaun1029@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `InfixToPostfix-1.0.3/README.md` & `InfixToPostfix-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `InfixToPostfix-1.0.3/setup.py` & `InfixToPostfix-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="InfixToPostfix",
-    version="1.0.3",
+    version="1.0.4",
     author="RoiexLee",
     author_email="luoyixaun1029@gmail.com",
     description="A python module converts infix expressions to postfix expressions and includes a visual interface.",
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     url="https://github.com/RoiexLee/InfixToPostfiX",
     packages=find_packages(),
```

