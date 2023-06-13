# Comparing `tmp/sphinx_c_autodoc-1.2.0.tar.gz` & `tmp/sphinx_c_autodoc-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_c_autodoc-1.2.0.tar", max compression
+gzip compressed data, was "sphinx_c_autodoc-1.2.1.tar", max compression
```

## Comparing `sphinx_c_autodoc-1.2.0.tar` & `sphinx_c_autodoc-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/LICENSE-MIT
--rw-r--r--   0        0        0     2669 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/README.rst
--rw-r--r--   0        0        0     1187 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    26897 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/__init__.py
--rw-r--r--   0        0        0     7095 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/__init__.py
--rw-r--r--   0        0        0       72 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
--rw-r--r--   0        0        0       57 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
--rw-r--r--   0        0        0      131 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
--rw-r--r--   0        0        0        0 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/__init__.py
--rw-r--r--   0        0        0      514 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/comments.py
--rw-r--r--   0        0        0     5875 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/patches.py
--rw-r--r--   0        0        0        0 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/__init__.py
--rw-r--r--   0        0        0     1393 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/c.py
--rw-r--r--   0        0        0    35622 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/loader.py
--rw-r--r--   0        0        0     6275 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/napoleon/__init__.py
--rw-r--r--   0        0        0    15732 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/viewcode/__init__.py
--rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 sphinx_c_autodoc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/LICENSE-MIT
+-rw-r--r--   0        0        0     2669 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/README.rst
+-rw-r--r--   0        0        0     1187 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    26897 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/__init__.py
+-rw-r--r--   0        0        0     7095 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
+-rw-r--r--   0        0        0       57 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
+-rw-r--r--   0        0        0      131 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
+-rw-r--r--   0        0        0        0 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/__init__.py
+-rw-r--r--   0        0        0      514 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/comments.py
+-rw-r--r--   0        0        0     5875 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/patches.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/__init__.py
+-rw-r--r--   0        0        0     1393 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/c.py
+-rw-r--r--   0        0        0    35949 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/loader.py
+-rw-r--r--   0        0        0     6275 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/napoleon/__init__.py
+-rw-r--r--   0        0        0    15732 2023-06-13 02:30:05.946552 sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/viewcode/__init__.py
+-rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 sphinx_c_autodoc-1.2.1/PKG-INFO
```

### Comparing `sphinx_c_autodoc-1.2.0/LICENSE-MIT` & `sphinx_c_autodoc-1.2.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/README.rst` & `sphinx_c_autodoc-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/pyproject.toml` & `sphinx_c_autodoc-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-c-autodoc"
-version = "1.2.0"
+version = "1.2.1"
 description = "A sphinx autodoc extension for c modules"
 authors = ["Nick <speedyleion@users.noreply.github.com>"]
 license = "MIT License, The Unlicense (Unlicense)"
 readme = "README.rst"
 packages = [{include = "sphinx_c_autodoc", from = "src"}]
 repository = "https://github.com/speedyleion/sphinx-c-autodoc"
 documentation = "https://sphinx-c-autodoc.readthedocs.io/en/latest/"
```

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/__init__.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/__init__.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/apidoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/comments.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/comments.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/patches.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/clang/patches.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/c.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/domains/c.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/loader.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,20 @@
     def format_args(self, **kwargs: Any) -> str:
         """
         Creates the parenthesis version of the function signature.  i.e. this
         will be the `(int hello, int what)` portion of the function header.
         """
         decl = self.declaration
         _, args = decl.split("(", 1)
+
+        # To keep consistency between clang versions we force the "void"
+        # argument. Earlier versions of clang has 'foo()' and newer ones
+        # have 'foo(void)'
+        if args == ")":  # pragma: no cover
+            args = "void)"
         return "(" + args
 
     def format_name(self) -> str:
         """Format the name of *self.object*.
 
         This normally should be something that can be parsed by the generated
         directive, but doesn't need to be (Sphinx will display it unparsed
@@ -733,20 +739,24 @@
     Create an instance from a :class:`cindex.Cursor`
     """
     # Prior to clang 16, anonymous constructs would have an empty `spelling` and
     # `displayname`. Clang 16 began naming anonymous constructs as:
     #   "<construct> (anonymous at # <path_to_c_file>:<lineno>)"
     # So need to look at the type spelling to determine if a construct is anonymous
     name = cursor.spelling
-    if any(anon in cursor.type.spelling for anon in ("anonymous at", "unnamed at")):
+    anonymous_type = any(
+        anon in cursor.type.spelling for anon in ("anonymous at", "unnamed at")
+    )
+
+    if not name or anonymous_type:
         # An anonymous construct which isn't contained in a typedef will have a
         # type spelling of:
         # "<construct> (anonymous at # <path_to_c_file>:<lineno>)"
         # Typedef's should be handled by the get_nested_node() function
-        if cursor.kind in ALLOWED_ANONYMOUS:
+        if cursor.kind in ALLOWED_ANONYMOUS and anonymous_type:
             filename = os.path.basename(cursor.location.file.name)
             # remove the extension from the filename since the '.' is not a
             # valid c identifier. splitext will remove the trailing most
             # extension so if this file is multi dotted it will fail, just use
             # partition and grab the first part.
             filename, _, _ = filename.partition(".")
             name = f"anon_{filename}_{cursor.hash}"
```

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/napoleon/__init__.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/viewcode/__init__.py` & `sphinx_c_autodoc-1.2.1/src/sphinx_c_autodoc/viewcode/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_c_autodoc-1.2.0/PKG-INFO` & `sphinx_c_autodoc-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-c-autodoc
-Version: 1.2.0
+Version: 1.2.1
 Summary: A sphinx autodoc extension for c modules
 Home-page: https://github.com/speedyleion/sphinx-c-autodoc
 License: MIT License, The Unlicense (Unlicense)
 Author: Nick
 Author-email: speedyleion@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

