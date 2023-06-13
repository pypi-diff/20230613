# Comparing `tmp/myl-0.8.2.tar.gz` & `tmp/myl-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.2.tar", last modified: Tue Jun 13 20:35:30 2023, max compression
+gzip compressed data, was "myl-0.8.3.tar", last modified: Tue Jun 13 20:47:53 2023, max compression
```

## Comparing `myl-0.8.2.tar` & `myl-0.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.917270 myl-0.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:35:19.000000 myl-0.8.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:35:19.000000 myl-0.8.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 20:35:19.000000 myl-0.8.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:35:19.000000 myl-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:35:19.000000 myl-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:35:30.921270 myl-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 20:35:19.000000 myl-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-13 20:35:19.000000 myl-0.8.2/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 20:35:19.000000 myl-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:35:30.921270 myl-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:47:41.000000 myl-0.8.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:47:41.000000 myl-0.8.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 20:47:41.000000 myl-0.8.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:47:41.000000 myl-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:47:41.000000 myl-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:47:53.636262 myl-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 20:47:41.000000 myl-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:47:53.636262 myl-0.8.3/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 20:47:53.000000 myl-0.8.3/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-13 20:47:41.000000 myl-0.8.3/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 20:47:41.000000 myl-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:47:53.636262 myl-0.8.3/setup.cfg
```

### Comparing `myl-0.8.2/.github/workflows/release.yaml` & `myl-0.8.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.2/LICENSE` & `myl-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.2/PKG-INFO` & `myl-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.2
+Version: 0.8.3
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.2/myl.egg-info/PKG-INFO` & `myl-0.8.3/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.2
+Version: 0.8.3
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.2/myl.py` & `myl-0.8.3/myl.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if args.sent or args.folder == "Sent":
             args.folder = GMAIL_SENT_FOLDER
         # elif args.folder == "INBOX":
         #     args.folder = GMAIL_ALL_FOLDER
     else:
         if args.auto:
             try:
-                settings = autodiscover(args.username)
+                settings = autodiscover(args.username).get("imap")
             except Exception:
                 error_msg("Failed to autodiscover IMAP settings")
                 if args.debug:
                     console.print_exception(show_locals=True)
                 return 1
             LOGGER.debug(f"Discovered settings: {settings})")
             args.server = settings.get("server")
```

### Comparing `myl-0.8.2/pyproject.toml` & `myl-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap_tools",
   "myl-discovery",
   "rich",
 ]
-version = "0.8.2"
+version = "0.8.3"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

