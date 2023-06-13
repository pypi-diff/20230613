# Comparing `tmp/resotoappbundler-0.3.0.tar.gz` & `tmp/resotoappbundler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoappbundler-0.3.0.tar", last modified: Fri May 12 14:07:41 2023, max compression
+gzip compressed data, was "resotoappbundler-0.4.0.tar", last modified: Tue Jun 13 13:22:46 2023, max compression
```

## Comparing `resotoappbundler-0.3.0.tar` & `resotoappbundler-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:07:41.452192 resotoappbundler-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-12 14:07:41.452192 resotoappbundler-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:07:41.448192 resotoappbundler-0.3.0/resotoappbundler/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/resotoappbundler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/resotoappbundler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/resotoappbundler/bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/resotoappbundler/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:07:41.448192 resotoappbundler-0.3.0/resotoappbundler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 14:07:41.000000 resotoappbundler-0.3.0/resotoappbundler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 14:07:41.452192 resotoappbundler-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:07:41.452192 resotoappbundler-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 14:06:05.000000 resotoappbundler-0.3.0/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/resotoappbundler/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/resotoappbundler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/resotoappbundler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/resotoappbundler/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/resotoappbundler/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/resotoappbundler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:22:46.000000 resotoappbundler-0.4.0/resotoappbundler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:22:46.346663 resotoappbundler-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 13:20:53.000000 resotoappbundler-0.4.0/test/test_args.py
```

### Comparing `resotoappbundler-0.3.0/LICENSE` & `resotoappbundler-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotoappbundler-0.3.0/PKG-INFO` & `resotoappbundler-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoappbundler
-Version: 0.3.0
+Version: 0.4.0
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto-apps/tree/main/resotoappbundler
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -15,31 +15,34 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `resotoappbundler`
-Resoto Infrastructure Apps Bundler
+# `resotoappbundler` / `resotoapprunner`
+Resoto Infrastructure Apps Bundler and Runner
 
 
 ## Table of contents
 
 * [Overview](#overview)
 * [Usage](#usage)
 * [Contact](#contact)
 * [License](#license)
 
 
 ## Overview
 `resotoappbundler` Bundles Resoto Infrastructure Apps.
+
 `resotoapprunner` Dry runs Resoto Infrastructure Apps.
 
 
+Check [the Resoto Infrastructure Apps repo](https://github.com/someengineering/resoto-apps) for details.
+
 ## Usage of `resotoappbundler`
 
 ```bash
 resotoappbundler --path resoto-apps/ --discover > index.json
 ```
 
 This command discovers all apps in the current directory and writes the index to `index.json`. This file can then be uploaded to a http server like a CDN and used as an app index in Resoto.
@@ -98,15 +101,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoappbundler-0.3.0/README.md` & `resotoappbundler-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-# `resotoappbundler`
-Resoto Infrastructure Apps Bundler
+# `resotoappbundler` / `resotoapprunner`
+Resoto Infrastructure Apps Bundler and Runner
 
 
 ## Table of contents
 
 * [Overview](#overview)
 * [Usage](#usage)
 * [Contact](#contact)
 * [License](#license)
 
 
 ## Overview
 `resotoappbundler` Bundles Resoto Infrastructure Apps.
+
 `resotoapprunner` Dry runs Resoto Infrastructure Apps.
 
 
+Check [the Resoto Infrastructure Apps repo](https://github.com/someengineering/resoto-apps) for details.
+
 ## Usage of `resotoappbundler`
 
 ```bash
 resotoappbundler --path resoto-apps/ --discover > index.json
 ```
 
 This command discovers all apps in the current directory and writes the index to `index.json`. This file can then be uploaded to a http server like a CDN and used as an app index in Resoto.
@@ -77,15 +80,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoappbundler-0.3.0/resotoappbundler/__main__.py` & `resotoappbundler-0.4.0/resotoappbundler/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 
 def run() -> None:
     setup_logger("resotoapprunner")
     arg_parser = ArgumentParser(description="Resoto Infrastructure Apps Runner")
     logging_add_args(arg_parser)
     add_args(arg_parser)
     runner_add_args(arg_parser)
-    arg_parser.parse_args()
+    args, argv = arg_parser.parse_known_args()
 
-    app_path = Path(arg_parser.args.app_path)
+    app_path = Path(args.app_path)
     if not app_path.is_dir():
         log.error(f"Path {app_path} is not a directory")
         sys.exit(1)
 
-    app_dry_run(app_manifest(app_path), arg_parser.args.config_path)
+    app_dry_run(app_manifest(app_path), args.config_path, argv)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `resotoappbundler-0.3.0/resotoappbundler/bundler.py` & `resotoappbundler-0.4.0/resotoappbundler/bundler.py`

 * *Files identical despite different names*

### Comparing `resotoappbundler-0.3.0/resotoappbundler.egg-info/PKG-INFO` & `resotoappbundler-0.4.0/resotoappbundler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoappbundler
-Version: 0.3.0
+Version: 0.4.0
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto-apps/tree/main/resotoappbundler
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
@@ -15,31 +15,34 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `resotoappbundler`
-Resoto Infrastructure Apps Bundler
+# `resotoappbundler` / `resotoapprunner`
+Resoto Infrastructure Apps Bundler and Runner
 
 
 ## Table of contents
 
 * [Overview](#overview)
 * [Usage](#usage)
 * [Contact](#contact)
 * [License](#license)
 
 
 ## Overview
 `resotoappbundler` Bundles Resoto Infrastructure Apps.
+
 `resotoapprunner` Dry runs Resoto Infrastructure Apps.
 
 
+Check [the Resoto Infrastructure Apps repo](https://github.com/someengineering/resoto-apps) for details.
+
 ## Usage of `resotoappbundler`
 
 ```bash
 resotoappbundler --path resoto-apps/ --discover > index.json
 ```
 
 This command discovers all apps in the current directory and writes the index to `index.json`. This file can then be uploaded to a http server like a CDN and used as an app index in Resoto.
@@ -98,15 +101,15 @@
 
 ## Contact
 If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/resoto/issues/new).
 
 
 ## License
 ```
-Copyright 2022 Some Engineering Inc.
+Copyright 2023 Some Engineering Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `resotoappbundler-0.3.0/setup.py` & `resotoappbundler-0.4.0/setup.py`

 * *Files identical despite different names*

