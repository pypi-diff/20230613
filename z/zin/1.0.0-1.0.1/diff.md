# Comparing `tmp/zin-1.0.0.tar.gz` & `tmp/zin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zin-1.0.0.tar", max compression
+gzip compressed data, was "zin-1.0.1.tar", max compression
```

## Comparing `zin-1.0.0.tar` & `zin-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-06-05 09:21:54.804754 zin-1.0.0/LICENSE
--rw-r--r--   0        0        0      908 2023-06-13 14:30:28.881796 zin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2343 2023-06-13 14:24:19.033074 zin-1.0.0/README.md
--rw-r--r--   0        0        0       45 2023-06-13 14:12:54.680094 zin-1.0.0/zin/__init__.py
--rw-r--r--   0        0        0     1762 2023-06-13 14:13:52.712065 zin-1.0.0/zin/__main__.py
--rw-r--r--   0        0        0     2808 2023-06-13 11:21:46.207161 zin-1.0.0/zin/handler.py
--rw-r--r--   0        0        0     1597 2023-06-13 14:16:07.048464 zin-1.0.0/zin/zin.py
--rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 zin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-05 09:21:54.804754 zin-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1085 2023-06-13 17:36:12.783481 zin-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2439 2023-06-13 16:19:37.620830 zin-1.0.1/README.md
+-rw-r--r--   0        0        0       45 2023-06-13 17:38:40.787243 zin-1.0.1/zin/__init__.py
+-rw-r--r--   0        0        0     1762 2023-06-13 14:13:52.712065 zin-1.0.1/zin/__main__.py
+-rw-r--r--   0        0        0     2808 2023-06-13 11:21:46.207161 zin-1.0.1/zin/handler.py
+-rw-r--r--   0        0        0     1597 2023-06-13 14:16:07.048464 zin-1.0.1/zin/zin.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 zin-1.0.1/PKG-INFO
```

### Comparing `zin-1.0.0/LICENSE` & `zin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zin-1.0.0/pyproject.toml` & `zin-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "zin"
-version = "1.0.0"
+version = "1.0.1"
 description = "zin is a lightweight command management tool that simplifies scripting and task automation."
 authors = ["Dishan Sachin <dishansachin99@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dishansa/zin"
 keywords = ["tools", "zin", "automation", "command management", "script"]
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
+    "Development Status :: 5 - Production/Stable",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
-    "Topic :: Utilities"
+    "Topic :: Utilities",
+    "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.7"
 rich = "^13.4.1"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 exclude = ["tests"]
 
 [tool.poetry.scripts]
-zin = 'zin.__main__:main'
+zin = 'zin.__main__:main'
```

### Comparing `zin-1.0.0/README.md` & `zin-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Zin
 
 zin is a lightweight command management tool that simplifies scripting and task automation. It provides an simple interface for defining and executing custom commands, helping you streamline your workflows and boost productivity.
 
-## Features
+## Features ✨
 
 - Command Definition: Easily define custom commands using a YAML configuration file.
 - Command Execution: Use a straightforward command-line interface to carry out the commands you've specified.
 - Modeled after [Rav](https://github.com/jmitchel3/rav): The flexibility and ease-of-use of the command-line program [Rav](https://github.com/jmitchel3/rav) serve as inspiration for zin.
 
 ## Usage
 
 To install `zin`, you can use pip:
 
 ```bash
 pip install zin
 ```
 
-## Configuration
+## Configuration 
 
 Make sure that 'zin.yaml' is present in the root working directory of your project before using 'zin'. But running 'zin' for the first time will automatically create the file if it doesn't already exist.
 
 The `zin.yaml` file follows a simple and easy-to-use format. Start with the `scripts:` section, followed by the command names and their corresponding commands. You can include multiple commands for a single command name using YAML collections.
 
 Example `zin.yaml` configuration:<br>
 (this is just an example for demonstration purposes.)
@@ -45,20 +45,24 @@
 
 **To list all the commands** using `zin`, you can use the following syntax:
 
 ```bash
 zin list
 ``` 
 
-## Contributing
+## Contributing 🤝
 
 Contributions are encouraged! Please start an issue or submit a pull request if you want to share thoughts, ideas, or problem reports. As stated in the [CONTRIBUTING.md](CONTRIBUTING.md) file, be sure that you stick to the guidelines.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ---
 
 **Note:** zin is highly inspired by [Rav](https://github.com/jmitchel3/rav), a command-line tool developed by [Justin Mitchel](https://github.com/jmitchel3).
 
 **Happy coding with zin! 😁**
+
+---
+
+**Project Renamed: pep is now zin. We apologize for any confusion caused.**
```

### Comparing `zin-1.0.0/zin/__main__.py` & `zin-1.0.1/zin/__main__.py`

 * *Files identical despite different names*

### Comparing `zin-1.0.0/zin/handler.py` & `zin-1.0.1/zin/handler.py`

 * *Files identical despite different names*

### Comparing `zin-1.0.0/zin/zin.py` & `zin-1.0.1/zin/zin.py`

 * *Files identical despite different names*

### Comparing `zin-1.0.0/PKG-INFO` & `zin-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: zin
-Version: 1.0.0
+Version: 1.0.1
 Summary: zin is a lightweight command management tool that simplifies scripting and task automation.
 Home-page: https://github.com/dishansa/zin
 Keywords: tools,zin,automation,command management,script
 Author: Dishan Sachin
 Author-email: dishansachin99@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Project-URL: Repository, https://github.com/dishansa/zin
 Description-Content-Type: text/markdown
 
 # Zin
 
 zin is a lightweight command management tool that simplifies scripting and task automation. It provides an simple interface for defining and executing custom commands, helping you streamline your workflows and boost productivity.
 
-## Features
+## Features ✨
 
 - Command Definition: Easily define custom commands using a YAML configuration file.
 - Command Execution: Use a straightforward command-line interface to carry out the commands you've specified.
 - Modeled after [Rav](https://github.com/jmitchel3/rav): The flexibility and ease-of-use of the command-line program [Rav](https://github.com/jmitchel3/rav) serve as inspiration for zin.
 
 ## Usage
 
 To install `zin`, you can use pip:
 
 ```bash
 pip install zin
 ```
 
-## Configuration
+## Configuration 
 
 Make sure that 'zin.yaml' is present in the root working directory of your project before using 'zin'. But running 'zin' for the first time will automatically create the file if it doesn't already exist.
 
 The `zin.yaml` file follows a simple and easy-to-use format. Start with the `scripts:` section, followed by the command names and their corresponding commands. You can include multiple commands for a single command name using YAML collections.
 
 Example `zin.yaml` configuration:<br>
 (this is just an example for demonstration purposes.)
@@ -67,21 +69,25 @@
 
 **To list all the commands** using `zin`, you can use the following syntax:
 
 ```bash
 zin list
 ``` 
 
-## Contributing
+## Contributing 🤝
 
 Contributions are encouraged! Please start an issue or submit a pull request if you want to share thoughts, ideas, or problem reports. As stated in the [CONTRIBUTING.md](CONTRIBUTING.md) file, be sure that you stick to the guidelines.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
 
 ---
 
 **Note:** zin is highly inspired by [Rav](https://github.com/jmitchel3/rav), a command-line tool developed by [Justin Mitchel](https://github.com/jmitchel3).
 
 **Happy coding with zin! 😁**
 
+---
+
+**Project Renamed: pep is now zin. We apologize for any confusion caused.**
+
```

