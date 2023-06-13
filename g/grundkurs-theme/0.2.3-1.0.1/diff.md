# Comparing `tmp/grundkurs_theme-0.2.3.tar.gz` & `tmp/grundkurs_theme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grundkurs_theme-0.2.3.tar", last modified: Tue Feb 21 09:11:30 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `grundkurs_theme-0.2.3.tar` & `grundkurs_theme-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,37 @@
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.672052 grundkurs_theme-0.2.3/
--rw-r--r--   0 ten1       (503) staff       (20)       86 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/CHANGELOG.md
--rw-r--r--   0 ten1       (503) staff       (20)     1520 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/LICENSE
--rw-r--r--   0 ten1       (503) staff       (20)      409 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/MANIFEST.in
--rw-r--r--   0 ten1       (503) staff       (20)     3425 2023-02-21 09:11:30.671785 grundkurs_theme-0.2.3/PKG-INFO
--rw-r--r--   0 ten1       (503) staff       (20)     2398 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/README.md
--rw-r--r--   0 ten1       (503) staff       (20)     1897 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/RELEASE.md
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.661543 grundkurs_theme-0.2.3/grundkurs_theme/
--rw-r--r--   0 ten1       (503) staff       (20)      993 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/grundkurs_theme/__init__.py
--rw-r--r--   0 ten1       (503) staff       (20)      625 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/grundkurs_theme/_version.py
--rw-r--r--   0 ten1       (503) staff       (20)     1582 2023-02-21 09:10:48.000000 grundkurs_theme-0.2.3/grundkurs_theme/handlers.py
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.664834 grundkurs_theme-0.2.3/grundkurs_theme/labextension/
--rw-r--r--   0 ten1       (503) staff       (20)    22291 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/build_log.json
--rw-r--r--   0 ten1       (503) staff       (20)     3749 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/package.json
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.655107 grundkurs_theme-0.2.3/grundkurs_theme/labextension/schemas/
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.665350 grundkurs_theme-0.2.3/grundkurs_theme/labextension/schemas/grundkurs_theme/
--rw-r--r--   0 ten1       (503) staff       (20)     3607 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig
--rw-r--r--   0 ten1       (503) staff       (20)      317 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/schemas/grundkurs_theme/plugin.json
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.668085 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/
--rw-r--r--   0 ten1       (503) staff       (20)    14297 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/lib_index_js.e84b150b320b7c747448.js
--rw-r--r--   0 ten1       (503) staff       (20)    11162 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/lib_index_js.e84b150b320b7c747448.js.map
--rw-r--r--   0 ten1       (503) staff       (20)    28865 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/remoteEntry.5e9e98a516686858e742.js
--rw-r--r--   0 ten1       (503) staff       (20)    27636 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/remoteEntry.5e9e98a516686858e742.js.map
--rw-r--r--   0 ten1       (503) staff       (20)      159 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/style.js
--rw-r--r--   0 ten1       (503) staff       (20)    45904 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/style_index_css.47343d2e4b9d6bc5bed9.js
--rw-r--r--   0 ten1       (503) staff       (20)    48592 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/style_index_css.47343d2e4b9d6bc5bed9.js.map
--rw-r--r--   0 ten1       (503) staff       (20)    12060 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.c5dd2030a75045fb191c.js
--rw-r--r--   0 ten1       (503) staff       (20)    13793 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.c5dd2030a75045fb191c.js.map
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.655379 grundkurs_theme-0.2.3/grundkurs_theme/labextension/themes/
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.668521 grundkurs_theme-0.2.3/grundkurs_theme/labextension/themes/grundkurs_theme/
--rw-r--r--   0 ten1       (503) staff       (20)    17214 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/themes/grundkurs_theme/index.css
--rw-r--r--   0 ten1       (503) staff       (20)        0 2023-02-21 07:52:52.000000 grundkurs_theme-0.2.3/grundkurs_theme/labextension/themes/grundkurs_theme/index.js
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.664257 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/
--rw-r--r--   0 ten1       (503) staff       (20)     3425 2023-02-21 09:11:30.000000 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/PKG-INFO
--rw-r--r--   0 ten1       (503) staff       (20)     1750 2023-02-21 09:11:30.000000 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/SOURCES.txt
--rw-r--r--   0 ten1       (503) staff       (20)        1 2023-02-21 09:11:30.000000 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/dependency_links.txt
--rw-r--r--   0 ten1       (503) staff       (20)        1 2022-08-10 12:17:28.000000 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/not-zip-safe
--rw-r--r--   0 ten1       (503) staff       (20)       16 2023-02-21 09:11:30.000000 grundkurs_theme-0.2.3/grundkurs_theme.egg-info/top_level.txt
--rw-r--r--   0 ten1       (503) staff       (20)      191 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/install.json
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.655605 grundkurs_theme-0.2.3/jupyter-config/
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.668646 grundkurs_theme-0.2.3/jupyter-config/nb-config/
--rw-r--r--   0 ten1       (503) staff       (20)      103 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/jupyter-config/nb-config/grundkurs_theme.json
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.669512 grundkurs_theme-0.2.3/jupyter-config/server-config/
--rw-r--r--   0 ten1       (503) staff       (20)      101 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/jupyter-config/server-config/grundkurs_theme.json
--rw-r--r--   0 ten1       (503) staff       (20)     3607 2023-02-21 09:10:56.000000 grundkurs_theme-0.2.3/package.json
--rw-r--r--   0 ten1       (503) staff       (20)      595 2022-08-10 12:11:59.000000 grundkurs_theme-0.2.3/pyproject.toml
--rw-r--r--   0 ten1       (503) staff       (20)       38 2023-02-21 09:11:30.672143 grundkurs_theme-0.2.3/setup.cfg
--rw-r--r--   0 ten1       (503) staff       (20)     3101 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/setup.py
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.670449 grundkurs_theme-0.2.3/src/
--rw-r--r--   0 ten1       (503) staff       (20)      916 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/src/handler.ts
--rw-r--r--   0 ten1       (503) staff       (20)     4787 2023-02-21 07:39:00.000000 grundkurs_theme-0.2.3/src/index.ts
--rw-r--r--   0 ten1       (503) staff       (20)     2961 2023-02-15 16:05:43.000000 grundkurs_theme-0.2.3/src/widget.tsx
-drwxr-xr-x   0 ten1       (503) staff       (20)        0 2023-02-21 09:11:30.670867 grundkurs_theme-0.2.3/style/
--rw-r--r--   0 ten1       (503) staff       (20)     1811 2023-02-15 09:30:24.000000 grundkurs_theme-0.2.3/style/index.css
--rw-r--r--   0 ten1       (503) staff       (20)    15429 2022-08-10 14:05:54.000000 grundkurs_theme-0.2.3/style/variables.css
--rw-r--r--   0 ten1       (503) staff       (20)      554 2023-02-15 16:05:43.000000 grundkurs_theme-0.2.3/tsconfig.json
--rw-r--r--   0 ten1       (503) staff       (20)   259112 2023-02-15 16:05:43.000000 grundkurs_theme-0.2.3/yarn.lock
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.copier-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/babel.config.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/jest.config.js
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/tsconfig.test.json
+-rw-r--r--   0        0        0   406681 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/yarn.lock
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/_version.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/handlers.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/package.json
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/schemas/grundkurs_theme/package.json.orig
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/schemas/grundkurs_theme/plugin.json
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/525.b3511822b6377fa70b30.js
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/remoteEntry.a136c23060f50b65fdb6.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    16411 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/schema/plugin.json
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/handler.ts
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/index.ts
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/widget.tsx
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/src/__tests__/grundkurs_theme.spec.ts
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/style/index.css
+-rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/style/variables.css
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/README.md
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 grundkurs_theme-1.0.1/PKG-INFO
```

### Comparing `grundkurs_theme-0.2.3/LICENSE` & `grundkurs_theme-1.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Noe Thalheim
+Copyright (c) 2023, Noe Thalheim
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `grundkurs_theme-0.2.3/PKG-INFO` & `grundkurs_theme-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,15 @@
-Metadata-Version: 2.1
-Name: grundkurs_theme
-Version: 0.2.3
-Summary: A JupyterLab Theme.
-Home-page: https://github.com/Grundkurs-Programmieren/grundkurs_theme.git
-Author: Noe Thalheim
-Author-email: noe@thalheim.email
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # grundkurs_theme
 
-[![Github Actions Status](https://github.com/Grundkurs-Programmieren/grundkurs_theme.git/workflows/Build/badge.svg)](https://github.com/Grundkurs-Programmieren/grundkurs_theme.git/actions/workflows/build.yml)
-A JupyterLab Theme.
+[![Github Actions Status](https://github.com/grundkurs-programmieren/grundkurs_theme/workflows/Build/badge.svg)](https://github.com/grundkurs-programmieren/grundkurs_theme/actions/workflows/build.yml)
+A JupyterLab extension.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install grundkurs_theme
@@ -61,15 +33,15 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the grundkurs_theme directory
 # Install package in development mode
-pip install -e .
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
@@ -95,10 +67,30 @@
 pip uninstall grundkurs_theme
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `grundkurs_theme` within that folder.
 
+### Testing the extension
+
+#### Frontend tests
+
+This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
+
+To execute them, execute:
+
+```sh
+jlpm
+jlpm test
+```
+
+#### Integration tests
+
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
+More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
+
+More information are provided within the [ui-tests](./ui-tests/README.md) README.
+
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `grundkurs_theme-0.2.3/RELEASE.md` & `grundkurs_theme-1.0.1/RELEASE.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,39 @@
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
 
-This extension can be distributed as Python
-packages. All of the Python
-packaging instructions in the `pyproject.toml` file to wrap your extension in a
-Python package. Before generating a package, we first need to install `build`.
+This extension can be distributed as Python packages. All of the Python
+packaging instructions are in the `pyproject.toml` file to wrap your extension in a
+Python package. Before generating a package, you first need to install some tools:
 
 ```bash
-pip install build twine
+pip install build twine hatch
+```
+
+Bump the version using `hatch`. By default this will create a tag.
+See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
+
+```bash
+hatch version <new-version>
+```
+
+Make sure to clean up all the development files before building the package:
+
+```bash
+jlpm clean:all
+```
+
+You could also clean up the local git repository:
+
+```bash
+git clean -dfX
 ```
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
 python -m build
 ```
@@ -38,24 +56,22 @@
 npm publish --access public
 ```
 
 ## Automated releases with the Jupyter Releaser
 
 The extension repository should already be compatible with the Jupyter Releaser.
 
-Check out the [workflow documentation](https://github.com/jupyter-server/jupyter_releaser#typical-workflow) for more information.
+Check out the [workflow documentation](https://jupyter-releaser.readthedocs.io/en/latest/get_started/making_release_from_repo.html) for more information.
 
 Here is a summary of the steps to cut a new release:
 
-- Fork the [`jupyter-releaser` repo](https://github.com/jupyter-server/jupyter_releaser)
-- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the Github Secrets in the fork
+- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the [Github Secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets) in the repository
 - Go to the Actions panel
-- Run the "Draft Changelog" workflow
-- Merge the Changelog PR
-- Run the "Draft Release" workflow
-- Run the "Publish Release" workflow
+- Run the "Step 1: Prep Release" workflow
+- Check the draft changelog
+- Run the "Step 2: Publish Release" workflow
 
 ## Publishing to `conda-forge`
 
 If the package is not on conda forge yet, check the documentation to learn how to add it: https://conda-forge.org/docs/maintainer/adding_pkgs.html
 
 Otherwise a bot should pick up the new version publish to PyPI, and open a new PR on the feedstock repository automatically.
```

### Comparing `grundkurs_theme-0.2.3/grundkurs_theme/handlers.py` & `grundkurs_theme-1.0.1/grundkurs_theme/handlers.py`

 * *Files identical despite different names*

### Comparing `grundkurs_theme-0.2.3/grundkurs_theme/labextension/package.json` & `grundkurs_theme-1.0.1/grundkurs_theme/labextension/package.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6007166666666667%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/grundkurs-programmieren/grundkurs_theme/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', delete: ['@jupyterlab/notebook', "*

 * *                   "'@lumino/coreutils']}",*

 * * "'description'": "'A JupyterLab extension.'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *                      "'^5.55.0', '@typescrip […]*

```diff
@@ -1,118 +1,190 @@
 {
     "author": {
         "email": "noe@thalheim.email",
         "name": "Noe Thalheim"
     },
     "bugs": {
-        "url": "https://github.com/Grundkurs-Programmieren/grundkurs_theme.git/issues"
+        "url": "https://github.com/grundkurs-programmieren/grundkurs_theme/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/apputils": "^3.1.0",
-        "@jupyterlab/notebook": "^3.5.0",
-        "@jupyterlab/settingregistry": "^3.5.2",
-        "@lumino/coreutils": "^1.12.1"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
-    "description": "A JupyterLab Theme.",
+    "description": "A JupyterLab extension.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/jest": "^29.2.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "^29.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
-    "files": [
-        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "schema/**/*.json",
-        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
-    ],
-    "homepage": "https://github.com/Grundkurs-Programmieren/grundkurs_theme.git",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/naming-convention": [
+                "error",
+                {
+                    "custom": {
+                        "match": true,
+                        "regex": "^I[A-Z]"
+                    },
+                    "format": [
+                        "PascalCase"
+                    ],
+                    "selector": "interface"
+                }
             ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
         }
     },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
+    "files": [
+        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
+        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/*.json"
+    ],
+    "homepage": "https://github.com/grundkurs-programmieren/grundkurs_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5e9e98a516686858e742.js",
-            "style": "./style"
-        },
-        "discovery": {
-            "server": {
-                "base": {
-                    "name": "grundkurs_theme"
-                },
-                "managers": [
-                    "pip"
-                ]
-            }
+            "load": "static/remoteEntry.a136c23060f50b65fdb6.js"
         },
         "extension": true,
         "outputDir": "grundkurs_theme/labextension",
         "schemaDir": "schema",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "grundkurs_theme",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/Grundkurs-Programmieren/grundkurs_theme.git.git"
+        "url": "https://github.com/grundkurs-programmieren/grundkurs_theme.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf grundkurs_theme/labextension",
+        "clean:labextension": "rimraf grundkurs_theme/labextension grundkurs_theme/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
+        "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css"
     ],
-    "style": "style/index.css",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "rules": {
+            "alpha-value-notation": null,
+            "color-function-notation": null,
+            "property-no-vendor-prefix": null,
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "1.0.1",
+    "workspaces": [
+        "ui-tests"
+    ]
 }
```

### Comparing `grundkurs_theme-0.2.3/grundkurs_theme/labextension/themes/grundkurs_theme/index.css` & `grundkurs_theme-1.0.1/grundkurs_theme/labextension/themes/grundkurs_theme/index.css`

 * *Files 5% similar despite different names*

```diff
@@ -87,35 +87,33 @@
    */
 
   --jp-border-width: 1px;
   --jp-border-color0: var(--md-grey-400);
   --jp-border-color1: var(--md-grey-400);
   --jp-border-color2: var(--md-grey-300);
   --jp-border-color3: var(--md-grey-200);
-  --jp-inverse-border-color: var(--md-grey-600);
   --jp-border-radius: 2px;
 
   /* UI Fonts
    *
    * The UI font CSS variables are used for the typography all of the JupyterLab
    * user interface elements that are not directly user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-ui-font-scale-factor: 1.2;
-  --jp-ui-font-size0: 0.83333em;
+  --jp-ui-font-size0: 0.8333em;
   --jp-ui-font-size1: 13px; /* Base font size */
   --jp-ui-font-size2: 1.2em;
   --jp-ui-font-size3: 1.44em;
-  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
-    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
-    'Segoe UI Symbol';
+  --jp-ui-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI', helvetica,
+    arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
 
   /*
    * Use these font colors against the corresponding main layout colors.
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
@@ -141,15 +139,15 @@
    * The font sizing here is done assuming that the body font size of --jp-content-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-content-line-height: 1.6;
   --jp-content-font-scale-factor: 1.2;
-  --jp-content-font-size0: 0.83333em;
+  --jp-content-font-size0: 0.8333em;
   --jp-content-font-size1: 14px; /* Base font size */
   --jp-content-font-size2: 1.2em;
   --jp-content-font-size3: 1.44em;
   --jp-content-font-size4: 1.728em;
   --jp-content-font-size5: 2.0736em;
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
@@ -161,27 +159,27 @@
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: rgba(0, 0, 0, 1);
   --jp-content-font-color1: rgba(0, 0, 0, 0.87);
   --jp-content-font-color2: rgba(0, 0, 0, 0.54);
   --jp-content-font-color3: rgba(0, 0, 0, 0.38);
   --jp-content-link-color: var(--md-blue-700);
-  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
-    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
-    'Segoe UI Emoji', 'Segoe UI Symbol';
+  --jp-content-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI',
+    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+    'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
    * Code font variables are used for typography of code and other monospaces content.
    */
 
   --jp-code-font-size: 13px;
   --jp-code-line-height: 1.3077; /* 17px for 13px base */
-  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
+  --jp-code-padding: 0.385em; /* 5px for 13px base */
   --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
   --jp-code-font-family: var(--jp-code-font-family-default);
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-code-presentation-font-size: 16px;
 
   /* may need to tweak cursor width if you change font size */
@@ -211,40 +209,39 @@
   --jp-inverse-layout-color1: var(--md-grey-900);
   --jp-inverse-layout-color2: var(--md-grey-800);
   --jp-inverse-layout-color3: var(--md-grey-700);
   --jp-inverse-layout-color4: var(--md-grey-600);
 
   /* Brand/accent */
 
-  --jp-brand-color0: var(--md-blue-900);
-  --jp-brand-color1: var(--md-blue-700);
-  --jp-brand-color2: var(--md-blue-300);
-  --jp-brand-color3: var(--md-blue-100);
-  --jp-brand-color4: var(--md-blue-50);
-  --jp-accent-color0: var(--md-green-900);
-  --jp-accent-color1: var(--md-green-700);
+  --jp-brand-color0: #ec0c4b;
+  --jp-brand-color1: #ed225d;
+  --jp-brand-color2: #ee376b;
+  --jp-brand-color3: #ee3b6e;
+  --jp-accent-color0: var(--md-green-700);
+  --jp-accent-color1: var(--md-green-500);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
 
-  --jp-warn-color0: var(--md-orange-900);
-  --jp-warn-color1: var(--md-orange-700);
+  --jp-warn-color0: var(--md-orange-700);
+  --jp-warn-color1: var(--md-orange-500);
   --jp-warn-color2: var(--md-orange-300);
   --jp-warn-color3: var(--md-orange-100);
-  --jp-error-color0: var(--md-red-900);
-  --jp-error-color1: var(--md-red-700);
+  --jp-error-color0: var(--md-red-700);
+  --jp-error-color1: var(--md-red-500);
   --jp-error-color2: var(--md-red-300);
   --jp-error-color3: var(--md-red-100);
-  --jp-success-color0: var(--md-green-900);
-  --jp-success-color1: var(--md-green-700);
+  --jp-success-color0: var(--md-green-700);
+  --jp-success-color1: var(--md-green-500);
   --jp-success-color2: var(--md-green-300);
   --jp-success-color3: var(--md-green-100);
-  --jp-info-color0: var(--md-cyan-900);
-  --jp-info-color1: var(--md-cyan-700);
+  --jp-info-color0: var(--md-cyan-700);
+  --jp-info-color1: var(--md-cyan-500);
   --jp-info-color2: var(--md-cyan-300);
   --jp-info-color3: var(--md-cyan-100);
 
   /* Cell specific styles */
 
   --jp-cell-padding: 5px;
   --jp-cell-collapser-width: 8px;
@@ -252,15 +249,15 @@
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
   --jp-cell-editor-background: var(--md-grey-100);
   --jp-cell-editor-border-color: var(--md-grey-300);
   --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-cell-editor-active-background: var(--jp-layout-color0);
   --jp-cell-editor-active-border-color: var(--jp-brand-color1);
   --jp-cell-prompt-width: 64px;
-  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
+  --jp-cell-prompt-font-family: 'Source Code Pro', monospace;
   --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 0.5;
   --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
 
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
@@ -316,17 +313,16 @@
 
   /* Input field styles */
 
   --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-input-active-background: var(--jp-layout-color1);
   --jp-input-hover-background: var(--jp-layout-color1);
   --jp-input-background: var(--md-grey-100);
-  --jp-input-border-color: var(--jp-inverse-border-color);
+  --jp-input-border-color: var(--jp-border-color1);
   --jp-input-active-border-color: var(--jp-brand-color1);
-  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);
 
   /* General editor styles */
 
   --jp-editor-selected-background: #d9d9d9;
   --jp-editor-selected-focused-background: #d7d4f0;
   --jp-editor-cursor-color: var(--jp-ui-font-color0);
 
@@ -353,163 +349,142 @@
   --jp-mirror-editor-attribute-color: #00c;
   --jp-mirror-editor-header-color: blue;
   --jp-mirror-editor-quote-color: #090;
   --jp-mirror-editor-link-color: #00c;
   --jp-mirror-editor-error-color: #f00;
   --jp-mirror-editor-hr-color: #999;
 
-  /*
-    RTC user specific colors.
-    These colors are used for the cursor, username in the editor,
-    and the icon of the user.
-  */
+  /* User colors */
 
-  --jp-collaborator-color1: #ffad8e;
-  --jp-collaborator-color2: #dac83d;
-  --jp-collaborator-color3: #72dd76;
-  --jp-collaborator-color4: #00e4d0;
-  --jp-collaborator-color5: #45d4ff;
-  --jp-collaborator-color6: #e2b1ff;
-  --jp-collaborator-color7: #ff9de6;
+  --jp-collaborator-color1: #ad4a00;
+  --jp-collaborator-color2: #7b6a00;
+  --jp-collaborator-color3: #007e00;
+  --jp-collaborator-color4: #008772;
+  --jp-collaborator-color5: #0079b9;
+  --jp-collaborator-color6: #8b45c6;
+  --jp-collaborator-color7: #be208b;
+
+  /* File or activity icons and switch semantic variables */
+
+  --jp-jupyter-icon-color: var(--md-orange-900);
+  --jp-notebook-icon-color: var(--md-orange-700);
+  --jp-json-icon-color: var(--md-orange-700);
+  --jp-console-icon-background-color: var(--md-blue-700);
+  --jp-console-icon-color: white;
+  --jp-terminal-icon-background-color: var(--md-grey-200);
+  --jp-terminal-icon-color: var(--md-grey-800);
+  --jp-text-editor-icon-color: var(--md-grey-200);
+  --jp-inspector-icon-color: var(--md-grey-200);
+  --jp-switch-color: var(--md-grey-400);
+  --jp-switch-true-position-color: var(--md-orange-700);
+  --jp-switch-cursor-color: rgba(0, 0, 0, 0.8);
 
   /* Vega extension styles */
 
   --jp-vega-background: white;
 
   /* Sidebar-related styles */
 
-  --jp-sidebar-min-width: 250px;
-
-  /* Search-related styles */
-
-  --jp-search-toggle-off-opacity: 0.5;
-  --jp-search-toggle-hover-opacity: 0.8;
-  --jp-search-toggle-on-opacity: 1;
-  --jp-search-selected-match-background-color: rgb(245, 200, 0);
-  --jp-search-selected-match-color: black;
-  --jp-search-unselected-match-background-color: var(
-    --jp-inverse-layout-color0
-  );
-  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);
-
-  /* Icon colors that work well with light or dark backgrounds */
-  --jp-icon-contrast-color0: var(--md-purple-600);
-  --jp-icon-contrast-color1: var(--md-green-600);
-  --jp-icon-contrast-color2: var(--md-pink-600);
-  --jp-icon-contrast-color3: var(--md-blue-600);
-
-  /* Button colors */
-  --jp-accept-color-normal: var(--md-blue-700);
-  --jp-accept-color-hover: var(--md-blue-800);
-  --jp-accept-color-active: var(--md-blue-900);
-  --jp-warn-color-normal: var(--md-red-700);
-  --jp-warn-color-hover: var(--md-red-800);
-  --jp-warn-color-active: var(--md-red-900);
-  --jp-reject-color-normal: var(--md-grey-600);
-  --jp-reject-color-hover: var(--md-grey-700);
-  --jp-reject-color-active: var(--md-grey-800);
+  --jp-sidebar-min-width: 180px;
 }
+
 /* Set the default typography for monospace elements */
 tt,
 code,
 kbd,
 samp,
 pre {
   font-family: var(--jp-code-font-family);
   font-size: var(--jp-code-font-size);
   line-height: var(--jp-code-line-height);
 }
 
-.html-output {
-  margin-left: 20px;
-  padding: 5px;
-  border-style: solid;
-  border-width: 1px;
-  border-color: black;
-}
-
-.exercise {
+.gk-exercise {
   margin: 0;
   padding: 10px;
   border-style: solid;
   border-width: 2px;
   border-color: green;
 }
 
-.exercise_image {
+.gk-exercise-image {
   float: right;
   width: 75px;
 }
 
-.exercise_label {
+.gk-exercise-label {
   padding: 5px;
   border-radius: 5px;
   background-color: green;
   color: white;
 }
 
-table.keywords tr td code {
-  background-color:transparent;
+table.gk-keywords tr td code {
+  background-color: transparent;
 }
 
-table.keywords tr td code.new {
+table.gk-keywords tr td code.new {
   font-weight: bold;
 }
 
-table.keywords tr td code.known {
-  background-color:lightgreen;
+table.gk-keywords tr td code.known {
+  background-color: lightgreen;
 }
 
-div.gk-cellFeedbackContainer {
+div.gk-cell-feedback-container {
   display: flex;
   justify-content: flex-end;
   flex-direction: column;
   align-items: flex-end;
   margin: 0;
   padding: 10px;
   border-style: solid;
   border-width: 2px;
   border-color: green;
   margin-left: 78px;
   margin-right: 21px;
 }
 
-.star-rating {
+.gk-cell-feedback-container .rating {
   display: flex;
   align-items: center;
   justify-content: flex-end;
 }
 
-.star {
+.gk-cell-feedback-container .star {
   width: 20px;
   height: 20px;
   margin: 5px;
   cursor: pointer;
 }
 
-.submit-button {
+.gk-cell-feedback-container .submit-button {
   background-color: blue;
   color: white;
   border: none;
   border-radius: 10px;
   font-size: 10px;
   cursor: pointer;
   box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
   transition: all 0.3s;
 }
-.submit-button:hover {
+
+.gk-cell-feedback-container .submit-button:hover {
   background-color: deepskyblue;
   transform: translateY(-1px);
   box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
 }
-.submit-button:active {
+
+.gk-cell-feedback-container .submit-button:active {
   transform: translateY(1px);
   box-shadow: none;
 }
-.submitted-message {
+
+.gk-cell-feedback-container .submitted-message {
   margin-left: 10px;
   font-size: 12px;
   font-weight: lighter;
   display: flex;
   gap: 5px;
   justify-content: flex-end;
 }
+
```

### Comparing `grundkurs_theme-0.2.3/src/handler.ts` & `grundkurs_theme-1.0.1/src/handler.ts`

 * *Files 20% similar despite different names*

```diff
@@ -11,28 +11,24 @@
  */
 export async function requestAPI<T>(
   endPoint = '',
   init: RequestInit = {}
 ): Promise<T> {
   // Make request to Jupyter API
   const settings = ServerConnection.makeSettings();
-  const requestUrl = URLExt.join(
-    settings.baseUrl,
-    'grundkurs_theme',
-    endPoint
-  );
+  const requestUrl = URLExt.join(settings.baseUrl, 'grundkurs_theme', endPoint);
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
-  } catch (error) {
+  } catch (error: any) {
     throw new ServerConnection.NetworkError(error);
   }
 
   const data = await response.json();
 
   if (!response.ok) {
     throw new ServerConnection.ResponseError(response, data.message);
   }
 
   return data;
-}
+}
```

### Comparing `grundkurs_theme-0.2.3/src/index.ts` & `grundkurs_theme-1.0.1/src/index.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
-import {
-  ReadonlyPartialJSONObject,
-} from '@lumino/coreutils';
+import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 
 import { CommandRegistry } from '@lumino/commands';
 
 import { ICellFooter, Cell } from '@jupyterlab/cells';
 
-import { CellFooterWithButton } from './widget';
+import { CellFooterWithFeedback } from './widget';
 
-import {
-  INotebookTracker,
-  NotebookPanel,
-} from '@jupyterlab/notebook';
+import { INotebookTracker, NotebookPanel } from '@jupyterlab/notebook';
 
 import { IThemeManager } from '@jupyterlab/apputils';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IEditorServices } from '@jupyterlab/codeeditor';
 
 import { requestAPI } from './handler';
 
@@ -29,15 +24,20 @@
 /**
  * Initialization data for the grundkurs_theme extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
   autoStart: true,
   requires: [INotebookTracker, IThemeManager, ISettingRegistry],
-  activate: (app: JupyterFrontEnd, tracker: INotebookTracker, manager: IThemeManager, settings: ISettingRegistry) => {
+  activate: (
+    app: JupyterFrontEnd,
+    tracker: INotebookTracker,
+    manager: IThemeManager,
+    settings: ISettingRegistry
+  ) => {
     const { commands, shell } = app;
     const command = 'grundkurs:send-feedback';
     let url = '';
 
     /**
      * Load the settings for this extension
      *
@@ -46,49 +46,49 @@
     function loadSetting(setting: ISettingRegistry.ISettings): void {
       // Read the settings and convert to the correct type
       url = setting.get('url').composite as string;
     }
 
     // Wait for the application to be restored and
     // for the settings for this plugin to be loaded
-    Promise.all([app.restored, settings.load(PLUGIN_ID)])
-      .then(([, setting]) => {
+    Promise.all([app.restored, settings.load(PLUGIN_ID)]).then(
+      ([, setting]) => {
         // Read the settings
         loadSetting(setting);
 
         // Listen for your plugin setting changes using Signal
         setting.changed.connect(loadSetting);
 
         commands.addCommand(command, {
           label: 'Send feedback for this assignment',
           execute: async args => {
             const current = getCurrent(tracker, shell, args);
-            if (current) {
-              // Get cellid of current active cell
-              const cellId = current.content.activeCell?.model?.modelDB.basePath
-              const value = args['value']
+            // We need a cellId therefore we need an activeCell
+            if (current && current.content.activeCell) {
+              const cellId = current.content.activeCell.model.id;
+              const value = args['value'];
               // POST request
-              const dataToSend = { 'cellId': cellId, url, value };
+              const dataToSend = { cellId: cellId, url, value };
               try {
-                console.log(JSON.stringify(dataToSend))
+                console.log(JSON.stringify(dataToSend));
                 const reply = await requestAPI<any>('feedback', {
                   body: JSON.stringify(dataToSend),
-                  method: 'POST',
+                  method: 'POST'
                 });
                 console.log(reply);
               } catch (reason) {
                 console.error(
                   `Error on POST /feedback ${dataToSend}.\n${reason}`
                 );
               }
             }
-          },
+          }
         });
-
-      })
+      }
+    );
 
     console.log('JupyterLab extension grundkurs_theme is activated!');
     const style = 'grundkurs_theme/index.css';
 
     manager.register({
       name: 'grundkurs_theme',
       isLight: true,
@@ -113,27 +113,27 @@
 
   return widget;
 }
 
 /**
  * Extend the default implementation of an `IContentFactory`.
  */
-export class ContentFactoryWithFooterButton extends NotebookPanel.ContentFactory {
+export class ContentFactoryWithFooterFeedback extends NotebookPanel.ContentFactory {
   constructor(
     commands: CommandRegistry,
-    options?: Cell.ContentFactory.IOptions | undefined
+    options: Cell.ContentFactory.IOptions
   ) {
     super(options);
     this.commands = commands;
   }
   /**
    * Create a new cell header for the parent widget.
    */
   createCellFooter(): ICellFooter {
-    return new CellFooterWithButton(this.commands);
+    return new CellFooterWithFeedback(this.commands);
   }
 
   private readonly commands: CommandRegistry;
 }
 
 /**
  * The notebook cell factory provider.
@@ -142,26 +142,23 @@
   id: 'jupyterlab-cellcodebtn:factory',
   provides: NotebookPanel.IContentFactory,
   requires: [IEditorServices],
   autoStart: true,
   activate: (app: JupyterFrontEnd, editorServices: IEditorServices) => {
     // tslint:disable-next-line:no-console
     console.log(
-      'JupyterLab extension jupyterlab-cellcodebtn',
+      'JupyterLab extensionn grundkurs_theme',
       'overrides default nootbook content factory'
     );
 
     const { commands } = app;
     const editorFactory = editorServices.factoryService.newInlineEditor;
-    return new ContentFactoryWithFooterButton(commands, { editorFactory });
+    return new ContentFactoryWithFooterFeedback(commands, { editorFactory });
   }
 };
 
 /**
- * Export this plugins as default.
+ * Export these plugins as default.
  */
-const plugins: Array<JupyterFrontEndPlugin<any>> = [
-  plugin,
-  cellFactory
-];
+const plugins: Array<JupyterFrontEndPlugin<any>> = [plugin, cellFactory];
 
-export default plugins;
+export default plugins;
```

### Comparing `grundkurs_theme-0.2.3/src/widget.tsx` & `grundkurs_theme-1.0.1/src/widget.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -2,104 +2,123 @@
 
 import React, { useState, useEffect } from 'react';
 
 import { CommandRegistry } from '@lumino/commands';
 
 import { ICellFooter, Cell, ICellModel } from '@jupyterlab/cells';
 
-const StarRating = ({ submit }: { submit: (value: number) => Promise<void> }): JSX.Element => {
+/**
+ * The CSS classes added to the cell footer.
+ */
+const CELL_FOOTER_DIV_CLASS = 'gk-cell-feedback-container';
+
+const Rating = ({
+  submit
+}: {
+  submit: (value: number) => Promise<void>;
+}): JSX.Element => {
   const [rating, setRating] = useState(0);
   const [clicked, setClicked] = useState(false);
   const [submitted, setSubmitted] = useState(false);
 
   useEffect(() => {
     if (submitted) {
       setTimeout(() => {
         setSubmitted(false);
       }, 5000);
     }
   }, [submitted]);
 
-  // @ts-ignore
   const handleClick = (index: number) => {
     setRating(index + 1);
-    setClicked(true)
-  }
+    setClicked(true);
+  };
 
-  // @ts-ignore
   const handleSubmit = async () => {
     // logic to handle the submit event goes here
     console.log(`Rating submitted: ${rating}`);
-    setClicked(false)
-    submit(rating).then(() => setSubmitted(true)).catch(e => console.log(e))
-  }
+    setClicked(false);
+    submit(rating)
+      .then(() => setSubmitted(true))
+      .catch(e => console.error(e));
+  };
 
-  const ratings = [
-    "too easy",
-    "easy",
-    "good",
-    "hard",
-    "too hard"
-  ]
+  const ratings = ['too easy', 'easy', 'good', 'hard', 'too hard'];
 
   return (
     <div className={CELL_FOOTER_DIV_CLASS}>
-          <span className="exercise_label">Feedback</span>
-      <div className='star-rating'>
-        {['😜', '😛', '🙂', '😕' ,'😖'].map((star, index) => (
-          <span onClick={() => handleClick(index)} style={{margin: '10px'}}>{star}</span>
+      <span className="gk-exercise-label">Feedback</span>
+      <div className="rating">
+        {['😜', '😛', '🙂', '😕', '😖'].map((star, index) => (
+          <span onClick={() => handleClick(index)} style={{ margin: '10px' }}>
+            {star}
+          </span>
         ))}
       </div>
       {clicked && (
-        <div style={{display: 'flex', flexDirection: 'column', width: '280px', justifyContent: 'space-around'}}>
-        <div className="submitted-message">
-          <b>You:</b> <span>The exercise was <b>{ ratings[rating-1] }</b></span> 
-          <button className="submit-button" onClick={() => handleSubmit()}>Submit</button>
-        </div>
+        <div
+          style={{
+            display: 'flex',
+            flexDirection: 'column',
+            width: '280px',
+            justifyContent: 'space-around'
+          }}
+        >
+          <div className="submitted-message">
+            <b>You: </b>
+            <span>
+              The exercise was <b>{ratings[rating - 1]}</b>
+            </span>
+            <button className="submit-button" onClick={() => handleSubmit()}>
+              Submit
+            </button>
+          </div>
         </div>
       )}
       {submitted && (
-          <div className="submitted-message">
-            <b>Us:</b> Thank you for submitting your feedback 🙏
-          </div>
-        )}
+        <div className="submitted-message">
+          <b>Us:</b> Thank you for submitting your feedback 🙏
+        </div>
+      )}
     </div>
   );
 };
 
-export default StarRating;
-
-/**
- * The CSS classes added to the cell footer.
- */
-const CELL_FOOTER_DIV_CLASS = 'gk-cellFeedbackContainer';
-//const CELL_FOOTER_BUTTON_CLASS = 'gk-cellFeedbackBtn';
+export default Rating;
 
 /**
  * Extend default implementation of a cell footer.
  */
-export class CellFooterWithButton extends ReactWidget implements ICellFooter {
+export class CellFooterWithFeedback extends ReactWidget implements ICellFooter {
   /**
    * Construct a new cell footer.
    */
   constructor(commands: CommandRegistry) {
     super();
     this.commands = commands;
   }
 
   private readonly commands: CommandRegistry;
 
-  render() {
-    const metadata = (this.parent as Cell<ICellModel>).model.sharedModel.getMetadata();
+  render(): React.ReactElement<any> {
+    const metadata = (
+      this.parent as Cell<ICellModel>
+    ).model.sharedModel.getMetadata();
 
     return (
       // TOOD: check for specific tag
-      metadata.tags?.includes("exercise") ?
-        <StarRating submit={(i) => {
-          // We return the Promise, so that the component can react on completion 
-          return this.commands.execute('grundkurs:send-feedback', { value: i });
-        }} />
+      metadata.tags?.includes('exercise') ? (
+        <Rating
+          submit={i => {
+            // We return the Promise, so that the component can react on completion
+            return this.commands.execute('grundkurs:send-feedback', {
+              value: i
+            });
+          }}
+        />
+      ) : (
         // Return empty tag
-        : <></>
+        <></>
+      )
     );
   }
-}
+}
```

### Comparing `grundkurs_theme-0.2.3/style/index.css` & `grundkurs_theme-1.0.1/style/index.css`

 * *Files 23% similar despite different names*

```diff
@@ -7,101 +7,96 @@
 samp,
 pre {
   font-family: var(--jp-code-font-family);
   font-size: var(--jp-code-font-size);
   line-height: var(--jp-code-line-height);
 }
 
-.html-output {
-  margin-left: 20px;
-  padding: 5px;
-  border-style: solid;
-  border-width: 1px;
-  border-color: black;
-}
-
-.exercise {
+.gk-exercise {
   margin: 0;
   padding: 10px;
   border-style: solid;
   border-width: 2px;
   border-color: green;
 }
 
-.exercise_image {
+.gk-exercise-image {
   float: right;
   width: 75px;
 }
 
-.exercise_label {
+.gk-exercise-label {
   padding: 5px;
   border-radius: 5px;
   background-color: green;
   color: white;
 }
 
-table.keywords tr td code {
-  background-color:transparent;
+table.gk-keywords tr td code {
+  background-color: transparent;
 }
 
-table.keywords tr td code.new {
+table.gk-keywords tr td code.new {
   font-weight: bold;
 }
 
-table.keywords tr td code.known {
-  background-color:lightgreen;
+table.gk-keywords tr td code.known {
+  background-color: lightgreen;
 }
 
-div.gk-cellFeedbackContainer {
+div.gk-cell-feedback-container {
   display: flex;
   justify-content: flex-end;
   flex-direction: column;
   align-items: flex-end;
   margin: 0;
   padding: 10px;
   border-style: solid;
   border-width: 2px;
   border-color: green;
   margin-left: 78px;
   margin-right: 21px;
 }
 
-.star-rating {
+.gk-cell-feedback-container .rating {
   display: flex;
   align-items: center;
   justify-content: flex-end;
 }
 
-.star {
+.gk-cell-feedback-container .star {
   width: 20px;
   height: 20px;
   margin: 5px;
   cursor: pointer;
 }
 
-.submit-button {
+.gk-cell-feedback-container .submit-button {
   background-color: blue;
   color: white;
   border: none;
   border-radius: 10px;
   font-size: 10px;
   cursor: pointer;
   box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
   transition: all 0.3s;
 }
-.submit-button:hover {
+
+.gk-cell-feedback-container .submit-button:hover {
   background-color: deepskyblue;
   transform: translateY(-1px);
   box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
 }
-.submit-button:active {
+
+.gk-cell-feedback-container .submit-button:active {
   transform: translateY(1px);
   box-shadow: none;
 }
-.submitted-message {
+
+.gk-cell-feedback-container .submitted-message {
   margin-left: 10px;
   font-size: 12px;
   font-weight: lighter;
   display: flex;
   gap: 5px;
   justify-content: flex-end;
-}
+}
```

### Comparing `grundkurs_theme-0.2.3/style/variables.css` & `grundkurs_theme-1.0.1/style/variables.css`

 * *Files 4% similar despite different names*

```diff
@@ -87,35 +87,33 @@
    */
 
   --jp-border-width: 1px;
   --jp-border-color0: var(--md-grey-400);
   --jp-border-color1: var(--md-grey-400);
   --jp-border-color2: var(--md-grey-300);
   --jp-border-color3: var(--md-grey-200);
-  --jp-inverse-border-color: var(--md-grey-600);
   --jp-border-radius: 2px;
 
   /* UI Fonts
    *
    * The UI font CSS variables are used for the typography all of the JupyterLab
    * user interface elements that are not directly user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-ui-font-scale-factor: 1.2;
-  --jp-ui-font-size0: 0.83333em;
+  --jp-ui-font-size0: 0.8333em;
   --jp-ui-font-size1: 13px; /* Base font size */
   --jp-ui-font-size2: 1.2em;
   --jp-ui-font-size3: 1.44em;
-  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
-    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
-    'Segoe UI Symbol';
+  --jp-ui-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI', helvetica,
+    arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
 
   /*
    * Use these font colors against the corresponding main layout colors.
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
@@ -141,15 +139,15 @@
    * The font sizing here is done assuming that the body font size of --jp-content-font-size1
    * is applied to a parent element. When children elements, such as headings, are sized
    * in em all things will be computed relative to that body size.
    */
 
   --jp-content-line-height: 1.6;
   --jp-content-font-scale-factor: 1.2;
-  --jp-content-font-size0: 0.83333em;
+  --jp-content-font-size0: 0.8333em;
   --jp-content-font-size1: 14px; /* Base font size */
   --jp-content-font-size2: 1.2em;
   --jp-content-font-size3: 1.44em;
   --jp-content-font-size4: 1.728em;
   --jp-content-font-size5: 2.0736em;
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
@@ -161,27 +159,27 @@
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: rgba(0, 0, 0, 1);
   --jp-content-font-color1: rgba(0, 0, 0, 0.87);
   --jp-content-font-color2: rgba(0, 0, 0, 0.54);
   --jp-content-font-color3: rgba(0, 0, 0, 0.38);
   --jp-content-link-color: var(--md-blue-700);
-  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
-    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
-    'Segoe UI Emoji', 'Segoe UI Symbol';
+  --jp-content-font-family: -apple-system, blinkmacsystemfont, 'Segoe UI',
+    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+    'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
    * Code font variables are used for typography of code and other monospaces content.
    */
 
   --jp-code-font-size: 13px;
   --jp-code-line-height: 1.3077; /* 17px for 13px base */
-  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
+  --jp-code-padding: 0.385em; /* 5px for 13px base */
   --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
   --jp-code-font-family: var(--jp-code-font-family-default);
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-code-presentation-font-size: 16px;
 
   /* may need to tweak cursor width if you change font size */
@@ -211,40 +209,39 @@
   --jp-inverse-layout-color1: var(--md-grey-900);
   --jp-inverse-layout-color2: var(--md-grey-800);
   --jp-inverse-layout-color3: var(--md-grey-700);
   --jp-inverse-layout-color4: var(--md-grey-600);
 
   /* Brand/accent */
 
-  --jp-brand-color0: var(--md-blue-900);
-  --jp-brand-color1: var(--md-blue-700);
-  --jp-brand-color2: var(--md-blue-300);
-  --jp-brand-color3: var(--md-blue-100);
-  --jp-brand-color4: var(--md-blue-50);
-  --jp-accent-color0: var(--md-green-900);
-  --jp-accent-color1: var(--md-green-700);
+  --jp-brand-color0: #ec0c4b;
+  --jp-brand-color1: #ed225d;
+  --jp-brand-color2: #ee376b;
+  --jp-brand-color3: #ee3b6e;
+  --jp-accent-color0: var(--md-green-700);
+  --jp-accent-color1: var(--md-green-500);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
 
-  --jp-warn-color0: var(--md-orange-900);
-  --jp-warn-color1: var(--md-orange-700);
+  --jp-warn-color0: var(--md-orange-700);
+  --jp-warn-color1: var(--md-orange-500);
   --jp-warn-color2: var(--md-orange-300);
   --jp-warn-color3: var(--md-orange-100);
-  --jp-error-color0: var(--md-red-900);
-  --jp-error-color1: var(--md-red-700);
+  --jp-error-color0: var(--md-red-700);
+  --jp-error-color1: var(--md-red-500);
   --jp-error-color2: var(--md-red-300);
   --jp-error-color3: var(--md-red-100);
-  --jp-success-color0: var(--md-green-900);
-  --jp-success-color1: var(--md-green-700);
+  --jp-success-color0: var(--md-green-700);
+  --jp-success-color1: var(--md-green-500);
   --jp-success-color2: var(--md-green-300);
   --jp-success-color3: var(--md-green-100);
-  --jp-info-color0: var(--md-cyan-900);
-  --jp-info-color1: var(--md-cyan-700);
+  --jp-info-color0: var(--md-cyan-700);
+  --jp-info-color1: var(--md-cyan-500);
   --jp-info-color2: var(--md-cyan-300);
   --jp-info-color3: var(--md-cyan-100);
 
   /* Cell specific styles */
 
   --jp-cell-padding: 5px;
   --jp-cell-collapser-width: 8px;
@@ -252,15 +249,15 @@
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
   --jp-cell-editor-background: var(--md-grey-100);
   --jp-cell-editor-border-color: var(--md-grey-300);
   --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-cell-editor-active-background: var(--jp-layout-color0);
   --jp-cell-editor-active-border-color: var(--jp-brand-color1);
   --jp-cell-prompt-width: 64px;
-  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
+  --jp-cell-prompt-font-family: 'Source Code Pro', monospace;
   --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 0.5;
   --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
 
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
@@ -316,17 +313,16 @@
 
   /* Input field styles */
 
   --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-input-active-background: var(--jp-layout-color1);
   --jp-input-hover-background: var(--jp-layout-color1);
   --jp-input-background: var(--md-grey-100);
-  --jp-input-border-color: var(--jp-inverse-border-color);
+  --jp-input-border-color: var(--jp-border-color1);
   --jp-input-active-border-color: var(--jp-brand-color1);
-  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);
 
   /* General editor styles */
 
   --jp-editor-selected-background: #d9d9d9;
   --jp-editor-selected-focused-background: #d7d4f0;
   --jp-editor-cursor-color: var(--jp-ui-font-color0);
 
@@ -353,58 +349,40 @@
   --jp-mirror-editor-attribute-color: #00c;
   --jp-mirror-editor-header-color: blue;
   --jp-mirror-editor-quote-color: #090;
   --jp-mirror-editor-link-color: #00c;
   --jp-mirror-editor-error-color: #f00;
   --jp-mirror-editor-hr-color: #999;
 
-  /*
-    RTC user specific colors.
-    These colors are used for the cursor, username in the editor,
-    and the icon of the user.
-  */
+  /* User colors */
 
-  --jp-collaborator-color1: #ffad8e;
-  --jp-collaborator-color2: #dac83d;
-  --jp-collaborator-color3: #72dd76;
-  --jp-collaborator-color4: #00e4d0;
-  --jp-collaborator-color5: #45d4ff;
-  --jp-collaborator-color6: #e2b1ff;
-  --jp-collaborator-color7: #ff9de6;
+  --jp-collaborator-color1: #ad4a00;
+  --jp-collaborator-color2: #7b6a00;
+  --jp-collaborator-color3: #007e00;
+  --jp-collaborator-color4: #008772;
+  --jp-collaborator-color5: #0079b9;
+  --jp-collaborator-color6: #8b45c6;
+  --jp-collaborator-color7: #be208b;
+
+  /* File or activity icons and switch semantic variables */
+
+  --jp-jupyter-icon-color: var(--md-orange-900);
+  --jp-notebook-icon-color: var(--md-orange-700);
+  --jp-json-icon-color: var(--md-orange-700);
+  --jp-console-icon-background-color: var(--md-blue-700);
+  --jp-console-icon-color: white;
+  --jp-terminal-icon-background-color: var(--md-grey-200);
+  --jp-terminal-icon-color: var(--md-grey-800);
+  --jp-text-editor-icon-color: var(--md-grey-200);
+  --jp-inspector-icon-color: var(--md-grey-200);
+  --jp-switch-color: var(--md-grey-400);
+  --jp-switch-true-position-color: var(--md-orange-700);
+  --jp-switch-cursor-color: rgba(0, 0, 0, 0.8);
 
   /* Vega extension styles */
 
   --jp-vega-background: white;
 
   /* Sidebar-related styles */
 
-  --jp-sidebar-min-width: 250px;
-
-  /* Search-related styles */
-
-  --jp-search-toggle-off-opacity: 0.5;
-  --jp-search-toggle-hover-opacity: 0.8;
-  --jp-search-toggle-on-opacity: 1;
-  --jp-search-selected-match-background-color: rgb(245, 200, 0);
-  --jp-search-selected-match-color: black;
-  --jp-search-unselected-match-background-color: var(
-    --jp-inverse-layout-color0
-  );
-  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);
-
-  /* Icon colors that work well with light or dark backgrounds */
-  --jp-icon-contrast-color0: var(--md-purple-600);
-  --jp-icon-contrast-color1: var(--md-green-600);
-  --jp-icon-contrast-color2: var(--md-pink-600);
-  --jp-icon-contrast-color3: var(--md-blue-600);
-
-  /* Button colors */
-  --jp-accept-color-normal: var(--md-blue-700);
-  --jp-accept-color-hover: var(--md-blue-800);
-  --jp-accept-color-active: var(--md-blue-900);
-  --jp-warn-color-normal: var(--md-red-700);
-  --jp-warn-color-hover: var(--md-red-800);
-  --jp-warn-color-active: var(--md-red-900);
-  --jp-reject-color-normal: var(--md-grey-600);
-  --jp-reject-color-hover: var(--md-grey-700);
-  --jp-reject-color-active: var(--md-grey-800);
-}
+  --jp-sidebar-min-width: 180px;
+}
```

### Comparing `grundkurs_theme-0.2.3/tsconfig.json` & `grundkurs_theme-1.0.1/tsconfig.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018', 'types': ['jest']}"}*

```diff
@@ -13,14 +13,16 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
-        "types": []
+        "target": "ES2018",
+        "types": [
+            "jest"
+        ]
     },
     "include": [
         "src/*"
     ]
 }
```

