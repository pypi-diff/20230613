# Comparing `tmp/dissect.ole-3.5.dev1.tar.gz` & `tmp/dissect.ole-3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ole-3.5.dev1.tar", last modified: Tue May 16 13:26:30 2023, max compression
+gzip compressed data, was "dissect.ole-3.6.dev1.tar", last modified: Tue Jun 13 13:42:45 2023, max compression
```

## Comparing `dissect.ole-3.5.dev1.tar` & `dissect.ole-3.6.dev1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect/ole/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/c_ole.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/dissect/ole/ole.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/dissect.ole.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:30.000000 dissect.ole-3.5.dev1/dissect.ole.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-16 13:26:20.000000 dissect.ole-3.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:30.698049 dissect.ole-3.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 13:26:16.000000 dissect.ole-3.5.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.415758 dissect.ole-3.6.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/dissect/ole/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/dissect/ole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/dissect/ole/c_ole.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/dissect/ole/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/dissect/ole/ole.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/dissect.ole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-13 13:42:45.000000 dissect.ole-3.6.dev1/dissect.ole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 13:42:45.000000 dissect.ole-3.6.dev1/dissect.ole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:42:45.000000 dissect.ole-3.6.dev1/dissect.ole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 13:42:45.000000 dissect.ole-3.6.dev1/dissect.ole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 13:42:45.000000 dissect.ole-3.6.dev1/dissect.ole.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-13 13:42:35.000000 dissect.ole-3.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.415758 dissect.ole-3.6.dev1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:42:45.423759 dissect.ole-3.6.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 13:42:31.000000 dissect.ole-3.6.dev1/tox.ini
```

### Comparing `dissect.ole-3.5.dev1/LICENSE` & `dissect.ole-3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.5.dev1/PKG-INFO` & `dissect.ole-3.6.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.5.dev1
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ole-3.5.dev1/README.md` & `dissect.ole-3.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.5.dev1/dissect/ole/c_ole.py` & `dissect.ole-3.6.dev1/dissect/ole/c_ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.5.dev1/dissect/ole/ole.py` & `dissect.ole-3.6.dev1/dissect/ole/ole.py`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.5.dev1/dissect.ole.egg-info/PKG-INFO` & `dissect.ole-3.6.dev1/dissect.ole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ole
-Version: 3.5.dev1
+Version: 3.6.dev1
 Summary: A Dissect module implementing a parser for the Object Linking & Embedding (OLE) format, commonly used by document editors on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ole
 Project-URL: repository, https://github.com/fox-it/dissect.ole
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.ole-3.5.dev1/pyproject.toml` & `dissect.ole-3.6.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ole-3.5.dev1/tox.ini` & `dissect.ole-3.6.dev1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -51,7 +51,28 @@
 
 [flake8]
 max-line-length = 120
 extend-ignore =
     # See https://github.com/PyCQA/pycodestyle/issues/373
     E203,
 statistics = True
+
+[testenv:docs-build]
+allowlist_externals = make
+deps =
+    sphinx
+    sphinx-autoapi
+    sphinx_argparse_cli
+    sphinx-copybutton
+    sphinx-design
+    furo
+
+commands =
+    make -C tests/docs clean
+    make -C tests/docs html
+
+[testenv:docs-linkcheck]
+allowlist_externals = make
+deps = {[testenv:docs-build]deps}
+commands =
+    make -C tests/docs clean
+    make -C tests/docs linkcheck
```

