# Comparing `tmp/correction-helper-2023.5.tar.gz` & `tmp/correction-helper-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "correction-helper-2023.5.tar", last modified: Thu May 25 08:29:13 2023, max compression
+gzip compressed data, was "correction-helper-2023.6.tar", last modified: Tue Jun 13 09:21:38 2023, max compression
```

## Comparing `correction-helper-2023.5.tar` & `correction-helper-2023.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-05-25 08:29:13.334617 correction-helper-2023.5/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2824 2022-04-13 21:56:28.000000 correction-helper-2023.5/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/correction_helper.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      300 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       18 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16964 2023-05-25 08:27:42.000000 correction-helper-2023.5/correction_helper.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)      982 2022-09-02 09:29:40.000000 correction-helper-2023.5/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-05-25 08:29:13.334617 correction-helper-2023.5/setup.cfg
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/tests/
--rw-r--r--   0 mdk       (1000) mdk       (1000)      877 2021-02-09 22:18:51.000000 correction-helper-2023.5/tests/test_compare.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2067 2021-11-07 09:16:28.000000 correction-helper-2023.5/tests/test_contextmanager.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-13 09:21:38.191385 correction-helper-2023.6/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-06-13 09:21:38.191385 correction-helper-2023.6/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2824 2022-04-13 21:56:28.000000 correction-helper-2023.6/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-13 09:21:38.191385 correction-helper-2023.6/correction_helper.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-06-13 09:21:38.000000 correction-helper-2023.6/correction_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      300 2023-06-13 09:21:38.000000 correction-helper-2023.6/correction_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-06-13 09:21:38.000000 correction-helper-2023.6/correction_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2023-06-13 09:21:38.000000 correction-helper-2023.6/correction_helper.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       18 2023-06-13 09:21:38.000000 correction-helper-2023.6/correction_helper.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16969 2023-06-13 09:20:56.000000 correction-helper-2023.6/correction_helper.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      982 2022-09-02 09:29:40.000000 correction-helper-2023.6/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-06-13 09:21:38.191385 correction-helper-2023.6/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-13 09:21:38.191385 correction-helper-2023.6/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      877 2021-02-09 22:18:51.000000 correction-helper-2023.6/tests/test_compare.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2067 2021-11-07 09:16:28.000000 correction-helper-2023.6/tests/test_contextmanager.py
```

### Comparing `correction-helper-2023.5/PKG-INFO` & `correction-helper-2023.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correction-helper
-Version: 2023.5
+Version: 2023.6
 Summary: Some helpers to help writing correction bots, use by hackinscience.org.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://github.com/JulienPalard/correction-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `correction-helper-2023.5/README.md` & `correction-helper-2023.6/README.md`

 * *Files identical despite different names*

### Comparing `correction-helper-2023.5/correction_helper.egg-info/PKG-INFO` & `correction-helper-2023.6/correction_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correction-helper
-Version: 2023.5
+Version: 2023.6
 Summary: Some helpers to help writing correction bots, use by hackinscience.org.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://github.com/JulienPalard/correction-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `correction-helper-2023.5/correction_helper.py` & `correction-helper-2023.6/correction_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pathlib import Path
 from textwrap import indent
 from typing import Optional, Sequence, Tuple, Union
 
 import friendly_traceback
 from friendly_traceback import exclude_file_from_traceback
 
-__version__ = "2023.5"
+__version__ = "2023.6"
 
 friendly_traceback.set_lang(os.environ.get("LANGUAGE", "en"))
 
 exclude_file_from_traceback(__file__)
 
 _ = gettext.translation("check", Path(__file__).parent, fallback=True).gettext
 
@@ -400,15 +400,15 @@
         start_hint = "I started it as:\n\n" + code(
             file + " " + " ".join(shlex.quote(a) for a in args)
         )
         args = ["--"] + list(args)
     try:
         proc = subprocess.run(
             [
-                "python3",
+                sys.executable,
                 "-m",
                 "friendly_traceback",
                 "--formatter",
                 "correction_helper.friendly_traceback_markdown",
                 file,
                 *args,
             ],
```

### Comparing `correction-helper-2023.5/pyproject.toml` & `correction-helper-2023.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `correction-helper-2023.5/tests/test_compare.py` & `correction-helper-2023.6/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `correction-helper-2023.5/tests/test_contextmanager.py` & `correction-helper-2023.6/tests/test_contextmanager.py`

 * *Files identical despite different names*

