# Comparing `tmp/gentoo-update-0.1.3.tar.gz` & `tmp/gentoo-update-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.3.tar", last modified: Sun Jun 11 19:07:15 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.4.tar", last modified: Tue Jun 13 21:28:34 2023, max compression
```

## Comparing `gentoo-update-0.1.3.tar` & `gentoo-update-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/gentoo_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/shell_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/gentoo_update/updater.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 19:07:15.000000 gentoo-update-0.1.3/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:15.576996 gentoo-update-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-11 19:07:04.000000 gentoo-update-0.1.3/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/gentoo_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.3/LICENSE` & `gentoo-update-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.3/PKG-INFO` & `gentoo-update-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.3
+Version: 0.1.4
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Gentoo Updater
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
-but it can also be used to update `@world`.  
+but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
```

### Comparing `gentoo-update-0.1.3/README.md` & `gentoo-update-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Gentoo Updater
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
-but it can also be used to update `@world`.  
+but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
```

### Comparing `gentoo-update-0.1.3/gentoo_update/gentoo_update.py` & `gentoo-update-0.1.4/gentoo_update/gentoo_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import argparse
 from .shell_runner import ShellRunner
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def create_cli():
     """
     Define CLI command flags using argparse.
 
@@ -58,30 +58,30 @@
         "Default: n\n",
     )
     parser.add_argument(
         "-e",
         "--clean",
         default="n",
         choices=["y", "n"],
-        help="Set wether to clean orphaned packaged after an update.\n"
+        help="Set whether to clean orphaned packaged after an update.\n"
         "Default: n\n",
     )
     parser.add_argument(
         "-l",
         "--read-logs",
         default="n",
         choices=["y", "n"],
-        help="Set wether to read elogs after an update.\n" "Default: n\n",
+        help="Set whether to read elogs after an update.\n" "Default: n\n",
     )
     parser.add_argument(
         "-n",
         "--read-news",
         default="n",
         choices=["y", "n"],
-        help="Set wether to read news after an update.\n" "Default: n\n",
+        help="Set whether to read news after an update.\n" "Default: n\n",
     )
     parser.add_argument(
         "-q",
         "--quiet",
         default="n",
         choices=["y", "n"],
         help="Do not show logs on the terminal screen.\n" "Default: n\n",
```

### Comparing `gentoo-update-0.1.3/gentoo_update/shell_runner.py` & `gentoo-update-0.1.4/gentoo_update/shell_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
         self.quiet = True if quiet == "y" else False
 
         self.timestamp = datetime.now().strftime("%Y-%m-%d-%H-%M")
         self.log_dir = "/var/log/gentoo_update"
         self.log_filename = f"{self.log_dir}/log_{self.timestamp}"
         self.logger = self.initiate_logger()
 
+        self.script_dir = os.path.join(os.path.dirname(__file__), "scripts")
+        self.script_path = os.path.join(self.script_dir, "updater.sh")
+
     def initiate_logger(self):
         """
         Create a logger with two handlers:
             1. terminal output
             2. file output
         Both handlers have the same logging level (INFO)
         and share the same formatter.
@@ -105,15 +108,15 @@
         and standard error to terminal and a log file.
 
         Args:
             script_path (str): Shell script path.
             *args (str): Arguments for the shell script.
                          They need to be handled by the script.
         """
-        command = shlex.split(f"updater.sh {' '.join(args)}")
+        command = shlex.split(f"{self.script_path} {' '.join(args)}")
         with subprocess.Popen(
             command, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ) as script_stream:
             self.stdout_output = self._log_stream_output(
                 script_stream, "stdout"
             )
             self.stderr_output = self._log_stream_output(
```

### Comparing `gentoo-update-0.1.3/gentoo_update/updater.sh` & `gentoo-update-0.1.4/gentoo_update/scripts/updater.sh`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.3/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.4/gentoo_update.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.3
+Version: 0.1.4
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Gentoo Updater
 
 `gentoo-update` is a tool that automates updates on Gentoo Linux. 
 By default it only installs security updates from [GLSA](https://security.gentoo.org/glsa/), 
-but it can also be used to update `@world`.  
+but it can also be used to update all packages on the system. i.e. `@world`.  
 
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
```

### Comparing `gentoo-update-0.1.3/setup.cfg` & `gentoo-update-0.1.4/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: POSIX :: Linux
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.10
+packages = gentoo_update
 include_package_data = True
-scripts = gentoo_update/updater.sh
 
 [options.entry_points]
 console_scripts = 
 	gentoo-update = gentoo_update.gentoo_update:main
 
 [egg_info]
 tag_build =
```

### Comparing `gentoo-update-0.1.3/tests/test_updater.py` & `gentoo-update-0.1.4/tests/test_updater.py`

 * *Files identical despite different names*

