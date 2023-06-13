# Comparing `tmp/amirispy-1.2.tar.gz` & `tmp/amirispy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amirispy-1.2.tar", last modified: Fri Apr 21 13:24:36 2023, max compression
+gzip compressed data, was "amirispy-1.3.tar", last modified: Tue Jun 13 17:17:58 2023, max compression
```

## Comparing `amirispy-1.2.tar` & `amirispy-1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.735850 amirispy-1.2/
--rw-rw-rw-   0        0        0       42 2022-10-28 14:04:41.000000 amirispy-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7801 2023-04-21 13:24:36.735850 amirispy-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7212 2023-04-21 13:23:31.000000 amirispy-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 13:24:36.735850 amirispy-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1550 2023-04-21 13:23:31.000000 amirispy-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.691769 amirispy-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.698765 amirispy-1.2/src/amirispy/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.709765 amirispy-1.2/src/amirispy/scripts/
--rw-rw-rw-   0        0        0      182 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/scripts/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/amiris.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.713765 amirispy-1.2/src/amirispy/scripts/resources/
--rw-rw-rw-   0        0        0      331 2022-10-28 13:24:56.000000 amirispy-1.2/src/amirispy/scripts/resources/fameSetup.yaml
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.718764 amirispy-1.2/src/amirispy/scripts/subcommands/
--rw-rw-rw-   0        0        0        0 2022-11-04 09:38:53.000000 amirispy-1.2/src/amirispy/scripts/subcommands/__init__.py
--rw-rw-rw-   0        0        0     4659 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/batch.py
--rw-rw-rw-   0        0        0     1711 2022-11-04 09:43:46.000000 amirispy-1.2/src/amirispy/scripts/subcommands/compare.py
--rw-rw-rw-   0        0        0     5797 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/install.py
--rw-rw-rw-   0        0        0     1420 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/scripts/subcommands/run.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.734843 amirispy-1.2/src/amirispy/source/
--rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.2/src/amirispy/source/__init__.py
--rw-rw-rw-   0        0        0     6431 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/cli.py
--rw-rw-rw-   0        0        0     4080 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/fameio_calls.py
--rw-rw-rw-   0        0        0     5671 2022-11-04 09:43:46.000000 amirispy-1.2/src/amirispy/source/file_comparison.py
--rw-rw-rw-   0        0        0     2103 2023-04-21 13:23:31.000000 amirispy-1.2/src/amirispy/source/files.py
--rw-rw-rw-   0        0        0     2641 2023-02-07 15:32:49.000000 amirispy-1.2/src/amirispy/source/logs.py
--rw-rw-rw-   0        0        0      828 2023-02-07 15:47:53.000000 amirispy-1.2/src/amirispy/source/util.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:24:36.706758 amirispy-1.2/src/amirispy.egg-info/
--rw-rw-rw-   0        0        0     7801 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 13:24:36.000000 amirispy-1.2/src/amirispy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.118888 amirispy-1.3/
+-rw-rw-rw-   0        0        0       42 2022-10-28 14:04:41.000000 amirispy-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7801 2023-06-13 17:17:58.118888 amirispy-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7212 2023-04-21 13:23:31.000000 amirispy-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:17:58.118888 amirispy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2023-06-13 17:14:48.000000 amirispy-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.049877 amirispy-1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.056883 amirispy-1.3/src/amirispy/
+-rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.070881 amirispy-1.3/src/amirispy/scripts/
+-rw-rw-rw-   0        0        0      182 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/scripts/amiris.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.071879 amirispy-1.3/src/amirispy/scripts/resources/
+-rw-rw-rw-   0        0        0      331 2022-10-28 13:24:56.000000 amirispy-1.3/src/amirispy/scripts/resources/fameSetup.yaml
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.085877 amirispy-1.3/src/amirispy/scripts/subcommands/
+-rw-rw-rw-   0        0        0        0 2022-11-04 09:38:53.000000 amirispy-1.3/src/amirispy/scripts/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     4659 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/scripts/subcommands/batch.py
+-rw-rw-rw-   0        0        0     1711 2022-11-04 09:43:46.000000 amirispy-1.3/src/amirispy/scripts/subcommands/compare.py
+-rw-rw-rw-   0        0        0     6149 2023-06-13 17:14:48.000000 amirispy-1.3/src/amirispy/scripts/subcommands/install.py
+-rw-rw-rw-   0        0        0     1395 2023-06-13 17:07:39.000000 amirispy-1.3/src/amirispy/scripts/subcommands/run.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.117887 amirispy-1.3/src/amirispy/source/
+-rw-rw-rw-   0        0        0      111 2022-11-04 09:40:34.000000 amirispy-1.3/src/amirispy/source/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-13 17:14:48.000000 amirispy-1.3/src/amirispy/source/cli.py
+-rw-rw-rw-   0        0        0     4080 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/source/fameio_calls.py
+-rw-rw-rw-   0        0        0     5671 2022-11-04 09:43:46.000000 amirispy-1.3/src/amirispy/source/file_comparison.py
+-rw-rw-rw-   0        0        0     2103 2023-04-21 13:23:31.000000 amirispy-1.3/src/amirispy/source/files.py
+-rw-rw-rw-   0        0        0     2641 2023-02-07 15:32:49.000000 amirispy-1.3/src/amirispy/source/logs.py
+-rw-rw-rw-   0        0        0      828 2023-02-07 15:47:53.000000 amirispy-1.3/src/amirispy/source/util.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:17:58.065876 amirispy-1.3/src/amirispy.egg-info/
+-rw-rw-rw-   0        0        0     7801 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2023-06-13 17:17:58.000000 amirispy-1.3/src/amirispy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 13:24:36.000000 amirispy-1.3/src/amirispy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:17:57.000000 amirispy-1.3/src/amirispy.egg-info/top_level.txt
```

### Comparing `amirispy-1.2/PKG-INFO` & `amirispy-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amirispy
-Version: 1.2
+Version: 1.3
 Summary: Python tools for the electricity market model AMIRIS
 Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
 Author: Christoph Schimeczek, Felix Nitsch
 Author-email: amiris@dlr.de
 License: Apache License 2.0
 Keywords: AMIRIS,agent-based modelling
 Platform: UNKNOWN
```

### Comparing `amirispy-1.2/README.md` & `amirispy-1.3/README.md`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/setup.py` & `amirispy-1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="amirispy",  # noqa
-    version="1.2",
+    version="1.3",
     description="Python tools for the electricity market model AMIRIS",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["AMIRIS", "agent-based modelling"],
     url="https://gitlab.com/dlr-ve/esy/amiris/amiris-py",
     author=", ".join(__author__),
     author_email=__email__,
@@ -42,13 +42,13 @@
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pandas", "wget", "fameio>=1.8"],
+    install_requires=["pandas", "wget", "fameio>=1.8.1,<1.9"],
     extras_require={"dev": ["pytest>=7.2"]},
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
 )
```

### Comparing `amirispy-1.2/src/amirispy/scripts/amiris.py` & `amirispy-1.3/src/amirispy/scripts/amiris.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/scripts/subcommands/batch.py` & `amirispy-1.3/src/amirispy/scripts/subcommands/batch.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/scripts/subcommands/compare.py` & `amirispy-1.3/src/amirispy/scripts/subcommands/compare.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/scripts/subcommands/install.py` & `amirispy-1.3/src/amirispy/scripts/subcommands/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 
 import logging as log
 import os
 import shutil
 import zipfile
 from enum import Enum, auto
 from pathlib import Path
+from urllib.error import HTTPError
 
 import pkg_resources
 import wget
 
 from amirispy.source.files import ensure_folder_exists, check_if_write_access
-from amirispy.source.logs import log_and_print
+from amirispy.source.logs import log_and_print, log_and_raise_critical
 from amirispy.source.util import check_java_installation
 
 MSG_SKIPPED_DOWNLOAD = "Skipped download of {} due to option '-m/--mode {}'"
 URL_EXAMPLES = "https://gitlab.com/dlr-ve/esy/amiris/examples/-/archive/main/examples-main.zip"
 
+DEPLOY_URL = "https://gitlab.com/dlr-ve/esy/amiris/amiris/-/artifacts"
+ERROR_URL_INVALID = "Download failed with error: '{}'. Please find latest deploy artifacts here: {}."
+
 
 class InstallMode(Enum):
     """Installation `mode` options"""
 
     ALL = auto()
     MODEL = auto()
     EXAMPLES = auto()
@@ -70,15 +74,18 @@
         force_install: flag to overwrite existing AMIRIS installation of same version
 
     Returns:
         None
     """
     download_file_path = Path(target_folder, "amiris.zip")
     log.info("Starting download of AMIRIS")
-    wget.download(url=url, out=str(download_file_path), bar=progress_bar)
+    try:
+        wget.download(url=url, out=str(download_file_path), bar=progress_bar)
+    except HTTPError as e:
+        log_and_raise_critical(ERROR_URL_INVALID.format(e, DEPLOY_URL))
     log.info(f"Downloaded file to '{download_file_path}'")
 
     if zipfile.is_zipfile(download_file_path):
         with zipfile.ZipFile(download_file_path, "r") as zip_ref:
             zip_ref.extractall(target_folder)
         os.remove(download_file_path)
```

### Comparing `amirispy-1.2/src/amirispy/scripts/subcommands/run.py` & `amirispy-1.3/src/amirispy/scripts/subcommands/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,10 +35,9 @@
     if not path_to_scenario.is_file():
         log_error_and_raise(ValueError(_ERR_NOT_A_FILE.format(path_to_scenario)))
 
     paths = determine_all_paths(path_to_scenario, origin_wd, options, batch=False)
     os.chdir(paths["SCENARIO_DIRECTORY"])
     compile_input(options, paths)
     os.chdir(origin_wd)
-    os.chdir(origin_wd)
     call_amiris(paths)
     compile_output(options, paths)
```

### Comparing `amirispy-1.2/src/amirispy/source/cli.py` & `amirispy-1.3/src/amirispy/source/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 BATCH_RECURSIVE_HELP = "Option to recursively search in provided Path for scenario (default: False)"
 DEFAULT_PATTERN = "*.y*ml"
 BATCH_PATTERN_HELP = f"Optional name pattern that scenario files searched for must match (default: '{DEFAULT_PATTERN}')"
 COMPARE_HELP = "Compare if results of two AMIRIS runs and equivalent"
 COMPARE_EXPECTED_HELP = "Path to folder with expected results"
 COMPARE_TEST_HELP = "Path to folder with results to test"
 COMPARE_IGNORE_HELP = "Optional list of file names to not be compared"
-URL_LATEST_AMIRIS = "https://gitlab.com/dlr-ve/esy/amiris/amiris/-/jobs/artifacts/main/download?job=deploy:jdk8"
+URL_LATEST_AMIRIS = "https://gitlab.com/dlr-ve/esy/amiris/amiris/-/jobs/artifacts/main/download?job=deploy:jdk11"
 
 
 class GeneralOptions(Enum):
     """Specifies general options for workflow"""
 
     LOG = auto()
     LOGFILE = auto()
```

### Comparing `amirispy-1.2/src/amirispy/source/fameio_calls.py` & `amirispy-1.3/src/amirispy/source/fameio_calls.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/source/file_comparison.py` & `amirispy-1.3/src/amirispy/source/file_comparison.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/source/files.py` & `amirispy-1.3/src/amirispy/source/files.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/source/logs.py` & `amirispy-1.3/src/amirispy/source/logs.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy/source/util.py` & `amirispy-1.3/src/amirispy/source/util.py`

 * *Files identical despite different names*

### Comparing `amirispy-1.2/src/amirispy.egg-info/PKG-INFO` & `amirispy-1.3/src/amirispy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amirispy
-Version: 1.2
+Version: 1.3
 Summary: Python tools for the electricity market model AMIRIS
 Home-page: https://gitlab.com/dlr-ve/esy/amiris/amiris-py
 Author: Christoph Schimeczek, Felix Nitsch
 Author-email: amiris@dlr.de
 License: Apache License 2.0
 Keywords: AMIRIS,agent-based modelling
 Platform: UNKNOWN
```

### Comparing `amirispy-1.2/src/amirispy.egg-info/SOURCES.txt` & `amirispy-1.3/src/amirispy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

