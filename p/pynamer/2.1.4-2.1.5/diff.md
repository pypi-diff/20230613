# Comparing `tmp/pynamer-2.1.4.tar.gz` & `tmp/pynamer-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.4.tar", last modified: Thu Jun  8 20:57:30 2023, max compression
+gzip compressed data, was "pynamer-2.1.5.tar", last modified: Tue Jun 13 14:26:33 2023, max compression
```

## Comparing `pynamer-2.1.4.tar` & `pynamer-2.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.480049 pynamer-2.1.4/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.4/AUTHORS.md
--rw-rw-rw-   0        0        0    10834 2023-06-08 20:57:11.000000 pynamer-2.1.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.4/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0    19579 2023-06-08 20:57:30.480049 pynamer-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    17613 2023-06-06 20:06:46.000000 pynamer-2.1.4/README.md
--rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     2305 2023-06-08 20:57:30.480049 pynamer-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.379697 pynamer-2.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.417562 pynamer-2.1.4/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.4/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-08 20:57:11.000000 pynamer-2.1.4/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.4/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2354 2023-06-04 10:27:28.000000 pynamer-2.1.4/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      823 2023-06-04 16:16:48.000000 pynamer-2.1.4/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.417562 pynamer-2.1.4/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.4/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7701 2023-06-07 10:30:39.000000 pynamer-2.1.4/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.4/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.4/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.4/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    10901 2023-06-07 11:32:19.000000 pynamer-2.1.4/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.417562 pynamer-2.1.4/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    19579 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 20:57:30.000000 pynamer-2.1.4/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 20:57:30.480049 pynamer-2.1.4/tests/
--rw-rw-rw-   0        0        0     2063 2023-06-04 10:27:28.000000 pynamer-2.1.4/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.4/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2822 2023-06-07 13:04:42.000000 pynamer-2.1.4/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.4/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     1927 2023-06-06 13:17:15.000000 pynamer-2.1.4/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.4/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.4/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.4/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.4/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.4/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.4/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:33.111858 pynamer-2.1.5/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.5/AUTHORS.md
+-rw-rw-rw-   0        0        0    11151 2023-06-13 14:26:08.000000 pynamer-2.1.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    19498 2023-06-13 14:26:33.111858 pynamer-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    17533 2023-06-13 14:25:10.000000 pynamer-2.1.5/README.md
+-rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2288 2023-06-13 14:26:33.111858 pynamer-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.721209 pynamer-2.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.830616 pynamer-2.1.5/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-13 14:26:08.000000 pynamer-2.1.5/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.5/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.5/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.5/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.846211 pynamer-2.1.5/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7909 2023-06-12 20:06:37.000000 pynamer-2.1.5/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.5/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.5/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    10288 2023-06-06 13:57:36.000000 pynamer-2.1.5/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    11394 2023-06-12 20:09:06.000000 pynamer-2.1.5/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:32.846211 pynamer-2.1.5/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    19498 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 14:26:32.000000 pynamer-2.1.5/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:26:33.096211 pynamer-2.1.5/tests/
+-rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.5/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.5/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2822 2023-06-07 13:04:42.000000 pynamer-2.1.5/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.5/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.5/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.5/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.5/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.5/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1294 2023-06-06 13:17:15.000000 pynamer-2.1.5/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.5/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.5/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.4/CHANGELOG.md` & `pynamer-2.1.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.5 (2023-06-13)
+### Fix
+* Typeerror for github license ([`bb7bd2a`](https://github.com/Stephen-RA-King/pynamer/commit/bb7bd2aafef6a78db971e6fda7c4e93978088c9e))
+
+### Documentation
+* Minor updates ([`e4e3721`](https://github.com/Stephen-RA-King/pynamer/commit/e4e3721ec3e8e541aa1fc5d746cf048e5c157f28))
+
 ## v2.1.4 (2023-06-08)
 
 
 ## v2.1.3 (2023-06-07)
 ### Fix
 * Regex for package names ([`756c6ff`](https://github.com/Stephen-RA-King/pynamer/commit/756c6ff297ca872ae3805df0ce25064cd4e518a2))
```

### Comparing `pynamer-2.1.4/LICENSE` & `pynamer-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/PKG-INFO` & `pynamer-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.4
+Version: 2.1.5
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -309,24 +309,24 @@
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Display GitHub statistics
+
 You can optionally display some of the most pertinent GitHub statistics if available by using the `-s` argument.
 The statistics will be displayed in the the details section of test 1. e.g.
 
 ```bash
 ~ $ pynamer black -s
-````
+```
 
 ![](assets/usage_stats.png)
 
-
 ## Register the package name with PyPI
 
 You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
@@ -418,15 +418,14 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
--   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
```

### Comparing `pynamer-2.1.4/README.md` & `pynamer-2.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -277,24 +277,24 @@
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Display GitHub statistics
+
 You can optionally display some of the most pertinent GitHub statistics if available by using the `-s` argument.
 The statistics will be displayed in the the details section of test 1. e.g.
 
 ```bash
 ~ $ pynamer black -s
-````
+```
 
 ![](assets/usage_stats.png)
 
-
 ## Register the package name with PyPI
 
 You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
@@ -386,15 +386,14 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
--   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
```

### Comparing `pynamer-2.1.4/pyproject.toml` & `pynamer-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/setup.cfg` & `pynamer-2.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -85,61 +85,59 @@
 00000540: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
 00000550: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
 00000560: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 00000570: 6e20 3a3a 2033 2e31 310d 0a0d 0a5b 6f70  n :: 3.11....[op
 00000580: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
 00000590: 6469 7220 3d20 0d0a 093d 7372 630d 0a70  dir = ...=src..p
 000005a0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000005b0: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-000005c0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-000005d0: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
-000005e0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000005f0: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
-00000600: 7265 7175 6972 6573 203d 200d 0a09 6265  requires = ...be
-00000610: 6175 7469 6675 6c73 6f75 7034 3e3d 342e  autifulsoup4>=4.
-00000620: 3132 2e32 0d0a 0962 7569 6c64 3e3d 302e  12.2...build>=0.
-00000630: 3130 2e30 0d0a 0963 6f6c 6f72 616d 613e  10.0...colorama>
-00000640: 3d30 2e34 2e36 0d0a 096a 696e 6a61 323e  =0.4.6...jinja2>
-00000650: 3d33 2e31 2e32 0d0a 0970 6163 6b61 6769  =3.1.2...packagi
-00000660: 6e67 3e3d 3233 2e31 0d0a 0970 7974 686f  ng>=23.1...pytho
-00000670: 6e2d 6461 7465 7574 696c 3e3d 322e 382e  n-dateutil>=2.8.
-00000680: 320d 0a09 7079 7961 6d6c 3e3d 362e 300d  2...pyyaml>=6.0.
-00000690: 0a09 7265 7175 6573 7473 3e3d 322e 3330  ..requests>=2.30
-000006a0: 2e30 0d0a 0972 6963 683e 3d31 332e 332e  .0...rich>=13.3.
-000006b0: 350d 0a09 7471 646d 3e3d 342e 3635 2e30  5...tqdm>=4.65.0
-000006c0: 0d0a 0974 7769 6e65 3e3d 332e 382e 300d  ...twine>=3.8.0.
-000006d0: 0a09 7768 6565 6c3e 3d30 2e34 302e 300d  ..wheel>=0.40.0.
-000006e0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000006f0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000700: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
-00000710: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000720: 5d0d 0a70 796e 616d 6572 203d 200d 0a09  ]..pynamer = ...
-00000730: 5245 4144 4d45 2e6d 640d 0a09 7072 6f6a  README.md...proj
-00000740: 6563 745f 6e61 6d65 0d0a 0970 726f 6a65  ect_name...proje
-00000750: 6374 5f6e 616d 652f 5f5f 696e 6974 5f5f  ct_name/__init__
-00000760: 2e70 790d 0a09 7365 7475 702e 7478 740d  .py...setup.txt.
-00000770: 0a09 7365 7475 705f 6261 7365 2e74 7874  ..setup_base.txt
-00000780: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000790: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-000007a0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-000007b0: 0970 796e 616d 6572 203d 2070 796e 616d  .pynamer = pynam
-000007c0: 6572 2e70 796e 616d 6572 3a6d 6169 6e0d  er.pynamer:main.
-000007d0: 0a0d 0a5b 666c 616b 6538 5d0d 0a64 6f63  ...[flake8]..doc
-000007e0: 7374 7269 6e67 2d63 6f6e 7665 6e74 696f  string-conventio
-000007f0: 6e20 3d20 6e75 6d70 790d 0a6d 6178 2d63  n = numpy..max-c
-00000800: 6f6d 706c 6578 6974 7920 3d20 3138 0d0a  omplexity = 18..
-00000810: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-00000820: 3d20 3838 0d0a 7365 6c65 6374 203d 2042  = 88..select = B
-00000830: 2c20 4239 2c20 432c 2044 2c20 452c 2046  , B9, C, D, E, F
-00000840: 2c20 4e2c 2057 0d0a 6578 636c 7564 6520  , N, W..exclude 
-00000850: 3d20 7465 7374 732f 2a2c 2e74 6f78 2f2a  = tests/*,.tox/*
-00000860: 2c2e 6e6f 782f 2a2c 646f 6373 2f2a 2c2e  ,.nox/*,docs/*,.
-00000870: 6769 742f 2a2c 2e67 6974 6875 622f 2a0d  git/*,.github/*.
-00000880: 0a69 676e 6f72 6520 3d20 0d0a 0945 3230  .ignore = ...E20
-00000890: 332c 0d0a 0957 3530 332c 0d0a 7065 722d  3,...W503,..per-
-000008a0: 6669 6c65 2d69 676e 6f72 6573 203d 200d  file-ignores = .
-000008b0: 0a09 7079 6e61 6d65 722e 7079 3a43 3930  ..pynamer.py:C90
-000008c0: 310d 0a09 6275 696c 6465 722e 7079 3a43  1...builder.py:C
-000008d0: 3930 310d 0a0d 0a5b 6567 675f 696e 666f  901....[egg_info
-000008e0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000008f0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000900: 0a                                       .
+000005b0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+000005c0: 5f64 6174 6120 3d20 5472 7565 0d0a 7079  _data = True..py
+000005d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000005e0: 3e3d 332e 390d 0a69 6e73 7461 6c6c 5f72  >=3.9..install_r
+000005f0: 6571 7569 7265 7320 3d20 0d0a 0962 6561  equires = ...bea
+00000600: 7574 6966 756c 736f 7570 343e 3d34 2e31  utifulsoup4>=4.1
+00000610: 322e 320d 0a09 6275 696c 643e 3d30 2e31  2.2...build>=0.1
+00000620: 302e 300d 0a09 636f 6c6f 7261 6d61 3e3d  0.0...colorama>=
+00000630: 302e 342e 360d 0a09 6a69 6e6a 6132 3e3d  0.4.6...jinja2>=
+00000640: 332e 312e 320d 0a09 7061 636b 6167 696e  3.1.2...packagin
+00000650: 673e 3d32 332e 310d 0a09 7079 7468 6f6e  g>=23.1...python
+00000660: 2d64 6174 6575 7469 6c3e 3d32 2e38 2e32  -dateutil>=2.8.2
+00000670: 0d0a 0970 7979 616d 6c3e 3d36 2e30 0d0a  ...pyyaml>=6.0..
+00000680: 0972 6571 7565 7374 733e 3d32 2e33 302e  .requests>=2.30.
+00000690: 300d 0a09 7269 6368 3e3d 3133 2e33 2e35  0...rich>=13.3.5
+000006a0: 0d0a 0974 7164 6d3e 3d34 2e36 352e 300d  ...tqdm>=4.65.0.
+000006b0: 0a09 7477 696e 653e 3d33 2e38 2e30 0d0a  ..twine>=3.8.0..
+000006c0: 0977 6865 656c 3e3d 302e 3430 2e30 0d0a  .wheel>=0.40.0..
+000006d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+000006e0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+000006f0: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
+00000700: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000710: 0d0a 7079 6e61 6d65 7220 3d20 0d0a 0952  ..pynamer = ...R
+00000720: 4541 444d 452e 6d64 0d0a 0970 726f 6a65  EADME.md...proje
+00000730: 6374 5f6e 616d 650d 0a09 7072 6f6a 6563  ct_name...projec
+00000740: 745f 6e61 6d65 2f5f 5f69 6e69 745f 5f2e  t_name/__init__.
+00000750: 7079 0d0a 0973 6574 7570 2e74 7874 0d0a  py...setup.txt..
+00000760: 0973 6574 7570 5f62 6173 652e 7478 740d  .setup_base.txt.
+00000770: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
+00000780: 795f 706f 696e 7473 5d0d 0a63 6f6e 736f  y_points]..conso
+00000790: 6c65 5f73 6372 6970 7473 203d 200d 0a09  le_scripts = ...
+000007a0: 7079 6e61 6d65 7220 3d20 7079 6e61 6d65  pynamer = pyname
+000007b0: 722e 7079 6e61 6d65 723a 6d61 696e 0d0a  r.pynamer:main..
+000007c0: 0d0a 5b66 6c61 6b65 385d 0d0a 646f 6373  ..[flake8]..docs
+000007d0: 7472 696e 672d 636f 6e76 656e 7469 6f6e  tring-convention
+000007e0: 203d 206e 756d 7079 0d0a 6d61 782d 636f   = numpy..max-co
+000007f0: 6d70 6c65 7869 7479 203d 2031 380d 0a6d  mplexity = 18..m
+00000800: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
+00000810: 2038 380d 0a73 656c 6563 7420 3d20 422c   88..select = B,
+00000820: 2042 392c 2043 2c20 442c 2045 2c20 462c   B9, C, D, E, F,
+00000830: 204e 2c20 570d 0a65 7863 6c75 6465 203d   N, W..exclude =
+00000840: 2074 6573 7473 2f2a 2c2e 746f 782f 2a2c   tests/*,.tox/*,
+00000850: 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c 2e67  .nox/*,docs/*,.g
+00000860: 6974 2f2a 2c2e 6769 7468 7562 2f2a 0d0a  it/*,.github/*..
+00000870: 6967 6e6f 7265 203d 200d 0a09 4532 3033  ignore = ...E203
+00000880: 2c0d 0a09 5735 3033 2c0d 0a70 6572 2d66  ,...W503,..per-f
+00000890: 696c 652d 6967 6e6f 7265 7320 3d20 0d0a  ile-ignores = ..
+000008a0: 0970 796e 616d 6572 2e70 793a 4339 3031  .pynamer.py:C901
+000008b0: 0d0a 0962 7569 6c64 6572 2e70 793a 4339  ...builder.py:C9
+000008c0: 3031 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  01....[egg_info]
+000008d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000008e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pynamer-2.1.4/src/pynamer/__init__.py` & `pynamer-2.1.5/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.4"
+__version__ = "2.1.5"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.1.4/src/pynamer/builder.py` & `pynamer-2.1.5/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/src/pynamer/config.py` & `pynamer-2.1.5/src/pynamer/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/env python3
-
-# Core Library modules
-import sys
-from pathlib import Path
-from typing import Optional
-
-# Local modules
-from . import project_count
-
-
-class Config:
-    """Configuration class"""
-
-    pypirc: Optional[Path] = None
-    original_project_name: str = "project_name"
-    no_cleanup: bool = False
-    project_count: int = project_count
-    package_version: str = "0.0.0"
-    description: str = "placeholder"
-    pypi_search_url: str = "https://pypi.org/search/"
-    pypi_project_url: str = "https://pypi.org/project/"
-    pypi_json_url: str = "https://pypi.org/pypi/"
-    pypi_simple_index_url: str = "https://pypi.org/simple/"
-    github_api_url = "https://api.github.com/repos/"
-    github_base_url = "https://github.com/"
-    idlemode: int = 1 if "idlelib.run" in sys.modules else 0
-
-
-config = Config()
+#!/usr/bin/env python3
+
+# Core Library modules
+import sys
+from pathlib import Path
+from typing import Optional
+
+# Local modules
+from . import project_count
+
+
+class Config:
+    """Configuration class"""
+
+    pypirc: Optional[Path] = None
+    original_project_name: str = "project_name"
+    no_cleanup: bool = False
+    project_count: int = project_count
+    package_version: str = "0.0.0"
+    description: str = "placeholder"
+    pypi_search_url: str = "https://pypi.org/search/"
+    pypi_project_url: str = "https://pypi.org/project/"
+    pypi_json_url: str = "https://pypi.org/pypi/"
+    pypi_simple_index_url: str = "https://pypi.org/simple/"
+    github_api_url: str = "https://api.github.com/repos/"
+    github_base_url: str = "https://github.com/"
+    idlemode: int = 1 if "idlelib.run" in sys.modules else 0
+
+
+config = Config()
```

### Comparing `pynamer-2.1.4/src/pynamer/utils.py` & `pynamer-2.1.5/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/src/pynamer/validators.py` & `pynamer-2.1.5/src/pynamer/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,297 +1,304 @@
-#!/usr/bin/env python3
-"""Collection of functions to test availability of a package name on PyPI"""
-# Core Library modules
-import json
-import re
-import string
-from datetime import datetime
-from typing import Any, Union
-
-# Third party modules
-import requests
-from bs4 import BeautifulSoup
-from dateutil.parser import isoparse
-from rich.console import Console
-from rich.table import Table
-
-# Local modules
-from . import logger, pypi_index_file_trv
-from .config import config
-from .utils import _generate_pypi_index, _search_json
-
-
-def _is_valid_package_name(project_name: str) -> bool:
-    """Function does a basic check of project name validity.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the name passes the basic check
-        False:          If the name fails the basic check
-    """
-    pattern = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.I)
-    if re.match(pattern, project_name) is not None:
-        return True
-    else:
-        return False
-
-
-def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
-    home_url = project_json["info"]["home_page"]
-
-    if "github.com" in home_url and home_url.endswith(project_name):
-        return "".join(["Homepage: ", home_url]), home_url
-
-    if "github.io" in home_url:
-        for item in (".github.io", "https://"):
-            home_url = home_url.replace(item, "")
-        home_url = home_url.rstrip("/")
-        home_url = "".join([config.github_base_url, home_url])
-        return "".join(["Homepage: ", home_url]), home_url
-
-    homepages = _search_json(project_json, project_name)
-    for home_url in homepages:
-        if "github.com" in home_url and home_url.endswith(project_name):
-            return "".join(["Homepage: ", home_url]), home_url
-
-    if home_url != "":
-        return "".join(["Homepage: ", home_url]), home_url
-
-    return "Homepage: None", ""
-
-
-def _github_meta(url: str) -> str:
-    return_text = "\n\nGitHub Stats\n------------\n"
-    repo_api_url = "".join(
-        [config.github_api_url, url.replace(r"https://github.com/", "")]
-    )
-    try:
-        json_raw = requests.get(repo_api_url, timeout=5)
-    except requests.RequestException:
-        return "".join([return_text, "GitHub can not be contacted"])
-
-    if json_raw.status_code == 200:
-        repo_json = json_raw.json()
-        return "".join(
-            [
-                return_text,
-                f"stars:    {repo_json['stargazers_count']}",
-                "\n",
-                f"forks:    {repo_json['forks']}",
-                "\n",
-                f"license:  {repo_json['license']['name']}",
-                "\n",
-                f"watching: {repo_json['subscribers_count']}",
-                "\n",
-                f"created:  {isoparse(repo_json['created_at']).date()}",
-                "\n",
-                f"updated:  {isoparse(repo_json['updated_at']).date()}",
-            ]
-        )
-    if json_raw.status_code == 404:
-        return "".join([return_text, "repository does not exist"])
-    return ""
-
-
-def _ping_project(project_name: str) -> bool:
-    """Determines if the URL to the project exists in PyPIs project area.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the URLs response code is 200
-        False:          If the URLs response code is not 200
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_project = "".join([config.pypi_project_url, project_name, "/"])
-    logger.debug("attempting to get url %s", url_project)
-    try:
-        project_ping = requests.get(url_project, timeout=5)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_ping.status_code == 200:
-        logger.debug("%s FOUND in the project area of PyPI", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
-    return False
-
-
-def _ping_json(project_name: str, stats: bool = False) -> str:
-    """Collects some details about the project if it exists.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_json = "".join([config.pypi_json_url, project_name, "/json"])
-    logger.debug("attempting to get url %s", url_json)
-    try:
-        project_json_raw = requests.get(url_json, timeout=5)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-
-        homepage_text, homepage_url = _get_homepage(project_json, project_name)
-
-        author = (
-            "".join(["Author:   ", project_json["info"]["author"]])
-            if project_json["info"]["author"]
-            else "Author:   None"
-        )
-        version = (
-            "".join(["Version:  ", project_json["info"]["version"]])
-            if project_json["info"]["version"]
-            else "Version:  None"
-        )
-        email = (
-            "".join(["Email:    ", project_json["info"]["author_email"]])
-            if project_json["info"]["author_email"]
-            else "Email:    None"
-        )
-        summary = (
-            "".join(["Summary:  ", project_json["info"]["summary"]])
-            if project_json["info"]["summary"]
-            else "Summary:  None"
-        )
-        result = "".join(
-            [summary, "\n", author, "\n", email, "\n", version, "\n", homepage_text]
-        )
-
-        if "github" in homepage_url and stats is True:
-            result = "".join([result, _github_meta(homepage_url)])
-        return result
-    logger.debug("No response from JSON URL")
-    return ""
-
-
-def _pypi_search_index(project_name: str) -> bool:
-    """Open the generated index file and search for the project name.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Returns:
-        True:           A match was found.
-        False:          A match was not found.
-    """
-    if not pypi_index_file_trv.is_file():
-        _generate_pypi_index()
-
-    projects = pypi_index_file_trv.read_text(encoding="utf-8")
-    if project_name in projects:
-        logger.debug("%s FOUND in the PyPI simple index", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-    return False
-
-
-def _pypi_search(
-    search_project: str,
-) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
-    """Performs a get request to PyPI's search API for the project name.
-
-    Args:
-        search_project:   The name of the project currently under test.
-
-    Returns:
-        match:          A list of projects matching name comprising:
-                            [project_name, version, released, description]
-        others:         A list of projects not matching but PyPI thinks are relevant.
-                            [project_name, version, released, description]
-        others_total:   A str representation of total projects found (minus matches).
-    """
-    pattern = re.compile(r">([\d,+]*?)<")
-    s = requests.Session()
-    projects_raw: list = []
-    match: list[list[str]] = []
-    others: list[list[str]] = []
-    params = {"q": {search_project}, "page": 1}
-    r = s.get(config.pypi_search_url, params=params)  # type: ignore
-    soup = BeautifulSoup(r.text, "html.parser")
-    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
-    for project_raw in projects_raw:
-        project_name = project_raw.select_one(
-            'span[class*="package-snippet__name"]'
-        ).text.strip()
-        version = project_raw.select_one(
-            'span[class*="package-snippet__version"]'
-        ).text.strip()
-        released_iso_8601 = project_raw.select_one(
-            'span[class*="package-snippet__created"]'
-        ).find("time")["datetime"]
-        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
-            "%Y-%m-%d"
-        )
-        description = project_raw.select_one(
-            'p[class*="package-snippet__description"]'
-        ).text.strip()
-        if project_name.lower() == search_project.lower():
-            match.append([project_name, version, released, description])
-        else:
-            others.append([project_name, version, released, description])
-
-    total_div_raw = soup.select(
-        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
-    )
-    total_raw = re.search(pattern, str(total_div_raw))
-    if total_raw is not None:
-        total_string = total_raw.group(1)
-        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
-        others_total = (
-            "".join([str(total), "+"])
-            if total == 10000
-            else (str(int(total) - len(match)))
-        )
-    else:
-        others_total = "0"
-    return match, others, others_total
-
-
-def _final_analysis(pattern: list[int]) -> None:
-    """Displays a rich console table displaying the conclusion of the test results
-
-    Args:
-        pattern:    A list of the test results:
-                    1 - A 'negative' result, indicating the project has been found.
-                    0 - A 'positive' result, indicating the project was not found.
-    """
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    if pattern == [0, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "It can only be found by searching the simple index which is not available "
-            "through the web interface.\n\n"
-            "The most likely cause is an abandoned or deleted project by the owner.\n\n"
-            "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
-            "to name transfer"
-        )
-    elif pattern == [1, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "However if appears in the simple index and can be displayed by simply"
-            " browsing "
-            "to the projects URL"
-        )
-    elif sum(pattern) >= 1:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row("The package name was found in at least one place")
-    elif sum(pattern) == 0:
-        table.add_row("[green]AVAILABLE![/green]\n")
-        table.add_row("The package name was not found in any part of PyPI")
-
-    console = Console()
-    console.print(table)
+#!/usr/bin/env python3
+"""Collection of functions to test availability of a package name on PyPI"""
+# Core Library modules
+import json
+import re
+import string
+from datetime import datetime
+from typing import Any, Union
+
+# Third party modules
+import requests
+from bs4 import BeautifulSoup
+from dateutil.parser import isoparse
+from rich.console import Console
+from rich.table import Table
+
+# Local modules
+from . import logger, pypi_index_file_trv
+from .config import config
+from .utils import _generate_pypi_index, _search_json
+
+
+def _is_valid_package_name(project_name: str) -> bool:
+    """Function does a basic check of project name validity.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the name passes the basic check
+        False:          If the name fails the basic check
+    """
+    pattern = re.compile("^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.I)
+    if re.match(pattern, project_name) is not None:
+        return True
+    else:
+        return False
+
+
+def _get_homepage(project_json: dict, project_name: str) -> tuple[str, str]:
+    home_url = project_json["info"]["home_page"]
+
+    if "github.com" in home_url and home_url.endswith(project_name):
+        return "".join(["Homepage: ", home_url]), home_url
+
+    if "github.io" in home_url:
+        for item in (".github.io", "https://"):
+            home_url = home_url.replace(item, "")
+        home_url = home_url.rstrip("/")
+        home_url = "".join([config.github_base_url, home_url])
+        return "".join(["Homepage: ", home_url]), home_url
+
+    homepages = _search_json(project_json, project_name)
+    for home_url in homepages:
+        if "github.com" in home_url and home_url.endswith(project_name):
+            return "".join(["Homepage: ", home_url]), home_url
+
+    if home_url != "":
+        return "".join(["Homepage: ", home_url]), home_url
+
+    return "Homepage: None", ""
+
+
+def _github_meta(url: str) -> str:
+    return_text = "\n\nGitHub Stats\n------------\n"
+    repo_api_url = "".join(
+        [config.github_api_url, url.replace(r"https://github.com/", "")]
+    )
+    try:
+        json_raw = requests.get(repo_api_url, timeout=5)
+    except requests.RequestException:
+        return "".join([return_text, "GitHub can not be contacted"])
+
+    if json_raw.status_code == 200:
+        repo_json = json_raw.json()
+
+        license_name = (
+            repo_json["license"]["name"] if repo_json["license"] is not None else "None"
+        )
+
+        return "".join(
+            [
+                return_text,
+                f"stars:    {repo_json['stargazers_count']}",
+                "\n",
+                f"forks:    {repo_json['forks']}",
+                "\n",
+                f"issues:   {repo_json['open_issues']}",
+                "\n",
+                f"license:  {license_name}",
+                "\n",
+                f"watching: {repo_json['subscribers_count']}",
+                "\n",
+                f"created:  {isoparse(repo_json['created_at']).date()}",
+                "\n",
+                f"updated:  {isoparse(repo_json['updated_at']).date()}",
+            ]
+        )
+    if json_raw.status_code == 404:
+        return "".join([return_text, "repository does not exist"])
+    return ""
+
+
+def _ping_project(project_name: str) -> bool:
+    """Determines if the URL to the project exists in PyPIs project area.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the URLs response code is 200
+        False:          If the URLs response code is not 200
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_project = "".join([config.pypi_project_url, project_name, "/"])
+    logger.debug("attempting to get url %s", url_project)
+    try:
+        project_ping = requests.get(url_project, timeout=5)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_ping.status_code == 200:
+        logger.debug("%s FOUND in the project area of PyPI", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
+    return False
+
+
+def _ping_json(project_name: str, stats: bool = False) -> str:
+    """Collects some details about the project if it exists.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_json = "".join([config.pypi_json_url, project_name, "/json"])
+    logger.debug("attempting to get url %s", url_json)
+    try:
+        project_json_raw = requests.get(url_json, timeout=5)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+
+        homepage_text, homepage_url = _get_homepage(project_json, project_name)
+
+        author = (
+            "".join(["Author:   ", project_json["info"]["author"]])
+            if project_json["info"]["author"]
+            else "Author:   None"
+        )
+        version = (
+            "".join(["Version:  ", project_json["info"]["version"]])
+            if project_json["info"]["version"]
+            else "Version:  None"
+        )
+        email = (
+            "".join(["Email:    ", project_json["info"]["author_email"]])
+            if project_json["info"]["author_email"]
+            else "Email:    None"
+        )
+        summary = (
+            "".join(["Summary:  ", project_json["info"]["summary"]])
+            if project_json["info"]["summary"]
+            else "Summary:  None"
+        )
+        result = "".join(
+            [summary, "\n", author, "\n", email, "\n", version, "\n", homepage_text]
+        )
+
+        if "github" in homepage_url and stats is True:
+            result = "".join([result, _github_meta(homepage_url)])
+        return result
+    logger.debug("No response from JSON URL")
+    return ""
+
+
+def _pypi_search_index(project_name: str) -> bool:
+    """Open the generated index file and search for the project name.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Returns:
+        True:           A match was found.
+        False:          A match was not found.
+    """
+    if not pypi_index_file_trv.is_file():
+        _generate_pypi_index()
+
+    projects = pypi_index_file_trv.read_text(encoding="utf-8")
+    if project_name in projects:
+        logger.debug("%s FOUND in the PyPI simple index", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+    return False
+
+
+def _pypi_search(
+    search_project: str,
+) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
+    """Performs a get request to PyPI's search API for the project name.
+
+    Args:
+        search_project:   The name of the project currently under test.
+
+    Returns:
+        match:          A list of projects matching name comprising:
+                            [project_name, version, released, description]
+        others:         A list of projects not matching but PyPI thinks are relevant.
+                            [project_name, version, released, description]
+        others_total:   A str representation of total projects found (minus matches).
+    """
+    pattern = re.compile(r">([\d,+]*?)<")
+    s = requests.Session()
+    projects_raw: list = []
+    match: list[list[str]] = []
+    others: list[list[str]] = []
+    params = {"q": {search_project}, "page": 1}
+    r = s.get(config.pypi_search_url, params=params)  # type: ignore
+    soup = BeautifulSoup(r.text, "html.parser")
+    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
+    for project_raw in projects_raw:
+        project_name = project_raw.select_one(
+            'span[class*="package-snippet__name"]'
+        ).text.strip()
+        version = project_raw.select_one(
+            'span[class*="package-snippet__version"]'
+        ).text.strip()
+        released_iso_8601 = project_raw.select_one(
+            'span[class*="package-snippet__created"]'
+        ).find("time")["datetime"]
+        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
+            "%Y-%m-%d"
+        )
+        description = project_raw.select_one(
+            'p[class*="package-snippet__description"]'
+        ).text.strip()
+        if project_name.lower() == search_project.lower():
+            match.append([project_name, version, released, description])
+        else:
+            others.append([project_name, version, released, description])
+
+    total_div_raw = soup.select(
+        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
+    )
+    total_raw = re.search(pattern, str(total_div_raw))
+    if total_raw is not None:
+        total_string = total_raw.group(1)
+        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
+        others_total = (
+            "".join([str(total), "+"])
+            if total == 10000
+            else (str(int(total) - len(match)))
+        )
+    else:
+        others_total = "0"
+    return match, others, others_total
+
+
+def _final_analysis(pattern: list[int]) -> None:
+    """Displays a rich console table displaying the conclusion of the test results
+
+    Args:
+        pattern:    A list of the test results:
+                    1 - A 'negative' result, indicating the project has been found.
+                    0 - A 'positive' result, indicating the project was not found.
+    """
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the web interface.\n\n"
+            "The most likely cause is an abandoned or deleted project by the owner.\n\n"
+            "Refer to PEP 541 – 'Package Index Name Retention' for details pertaining "
+            "to name transfer"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "However if appears in the simple index and can be displayed by simply"
+            " browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) >= 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
```

### Comparing `pynamer-2.1.4/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.5/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.4
+Version: 2.1.5
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -309,24 +309,24 @@
 pandia          Not Found   Not Found   Found           Not Available
 leda            Not Found   Not Found   Not Found       Available
 ```
 
 Again you can use a combination of names from the command line and input file.
 
 ## Display GitHub statistics
+
 You can optionally display some of the most pertinent GitHub statistics if available by using the `-s` argument.
 The statistics will be displayed in the the details section of test 1. e.g.
 
 ```bash
 ~ $ pynamer black -s
-````
+```
 
 ![](assets/usage_stats.png)
 
-
 ## Register the package name with PyPI
 
 You can optionally 'register' the name on PyPI by using the `-r` argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded
 to PyPI.
 
 The first time you use the 'registration' procedure you will be prompted to enter your name and email address. These are required.
@@ -418,15 +418,14 @@
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
--   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
 ## Planned Future improvements
```

### Comparing `pynamer-2.1.4/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.5/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_build_dist.py` & `pynamer-2.1.5/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_cleanup.py` & `pynamer-2.1.5/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_create_setup_file.py` & `pynamer-2.1.5/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_defaults.py` & `pynamer-2.1.5/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_delete_director.py` & `pynamer-2.1.5/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_feedback.py` & `pynamer-2.1.5/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_final_analysis.py` & `pynamer-2.1.5/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_find_pypirc_file.py` & `pynamer-2.1.5/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_generate_pypi_index.py` & `pynamer-2.1.5/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_get_homepage.py` & `pynamer-2.1.5/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_github_meta.py` & `pynamer-2.1.5/tests/test_github_meta.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,84 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-expected_response_found = """
-
-GitHub Stats
-------------
-stars:    32544
-forks:    2095
-license:  MIT License
-watching: 229
-created:  2018-03-14
-updated:  2023-06-06"""
-
-
-expected_response_http_error = """
-
-GitHub Stats
-------------
-GitHub can not be contacted"""
-
-
-expected_response_404_error = """
-
-GitHub Stats
-------------
-repository does not exist"""
-
-
-@pytest.fixture
-def mock_response_404(monkeypatch):
-    def mock_get(*args, **kwargs):
-        class MockResponse:
-            def __init__(self):
-                self.status_code = 404
-
-            def json(self):
-                return {}
-
-        return MockResponse()
-
-    monkeypatch.setattr(requests, "get", mock_get)
-
-
-def my_custom_get_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_github_json_black.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_github_meta_black(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_found
-
-
-def test_ping_json_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_http_error
-
-
-def test_ping_json_not_exist(mock_response_404):
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_404_error
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+expected_response_found = """
+
+GitHub Stats
+------------
+stars:    32616
+forks:    2102
+issues:   405
+license:  MIT License
+watching: 229
+created:  2018-03-14
+updated:  2023-06-12"""
+
+
+expected_response_http_error = """
+
+GitHub Stats
+------------
+GitHub can not be contacted"""
+
+
+expected_response_404_error = """
+
+GitHub Stats
+------------
+repository does not exist"""
+
+
+@pytest.fixture
+def mock_response_404(monkeypatch):
+    def mock_get(*args, **kwargs):
+        class MockResponse:
+            def __init__(self):
+                self.status_code = 404
+
+            def json(self):
+                return {}
+
+        return MockResponse()
+
+    monkeypatch.setattr(requests, "get", mock_get)
+
+
+def my_custom_get_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_github_json_black.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_github_meta_black(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_found
+
+
+def test_ping_json_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_http_error
+
+
+def test_ping_json_not_exist(mock_response_404):
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_404_error
```

### Comparing `pynamer-2.1.4/tests/test_ping_json.py` & `pynamer-2.1.5/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_ping_project.py` & `pynamer-2.1.5/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_process_input_file.py` & `pynamer-2.1.5/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_pypi_search.py` & `pynamer-2.1.5/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_pypi_search_index.py` & `pynamer-2.1.5/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_rename_project_dir.py` & `pynamer-2.1.5/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_upload_dist.py` & `pynamer-2.1.5/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_utils_search_json.py` & `pynamer-2.1.5/tests/test_utils_search_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_utils_version.py` & `pynamer-2.1.5/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.4/tests/test_write_output_file.py` & `pynamer-2.1.5/tests/test_write_output_file.py`

 * *Files identical despite different names*

