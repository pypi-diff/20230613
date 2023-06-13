# Comparing `tmp/flufl.i18n-4.1.1.tar.gz` & `tmp/flufl_i18n-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl.i18n-4.1.1.tar", last modified: Tue Sep  6 01:55:58 2022, max compression
+gzip compressed data, was "flufl_i18n-5.0.1.tar", last modified: Tue Jun 13 20:27:55 2023, max compression
```

## Comparing `flufl.i18n-4.1.1.tar` & `flufl_i18n-5.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-rw-rw-   0 root         (0) root         (0)      558 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      909 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1214 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     5175 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/NEWS.rst
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/apiref.rst
--rw-rw-rw-   0 root         (0) root         (0)     6653 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/expand.rst
--rw-rw-rw-   0 root         (0) root         (0)     2301 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3290 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/strategies.rst
--rw-rw-rw-   0 root         (0) root         (0)    10901 2022-09-06 01:55:19.244842 flufl.i18n-4.1.1/docs/using.rst
--rw-rw-rw-   0 root         (0) root         (0)     3195 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1022 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/src/flufl/i18n/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10549 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/src/flufl/i18n/_application.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/src/flufl/i18n/_expand.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/src/flufl/i18n/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2371 2022-09-06 01:55:19.245843 flufl.i18n-4.1.1/src/flufl/i18n/_strategy.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/src/flufl/i18n/_substitute.py
--rw-rw-rw-   0 root         (0) root         (0)     2983 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/src/flufl/i18n/_translator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/src/flufl/i18n/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     4305 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/src/flufl/i18n/types.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/messages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/messages/xx/LC_MESSAGES/flufl.mo
--rw-rw-rw-   0 root         (0) root         (0)      673 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/messages/xx/LC_MESSAGES/flufl.po
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/messages/yy/LC_MESSAGES/flufl.mo
--rw-rw-rw-   0 root         (0) root         (0)      672 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/data/messages/yy/LC_MESSAGES/flufl.po
--rw-rw-rw-   0 root         (0) root         (0)      370 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/test_application.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/test_expand.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/test_substitute.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/test/test_translator.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2022-09-06 01:55:19.246843 flufl.i18n-4.1.1/tox.ini
--rw-------   0 runner    (1000) runner    (1000)     2156 2022-09-06 01:55:58.619754 flufl.i18n-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/LICENSE
+-rw-r--r--   0        0        0      909 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/README.rst
+-rw-r--r--   0        0        0     1214 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/conftest.py
+-rw-r--r--   0        0        0     5407 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-13 20:27:30.463667 flufl_i18n-5.0.1/docs/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/apiref.rst
+-rw-r--r--   0        0        0     6680 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/conf.py
+-rw-r--r--   0        0        0     1113 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/expand.rst
+-rw-r--r--   0        0        0     2301 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/index.rst
+-rw-r--r--   0        0        0     3290 2023-06-13 20:27:30.440667 flufl_i18n-5.0.1/docs/strategies.rst
+-rw-r--r--   0        0        0    10901 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/docs/using.rst
+-rw-r--r--   0        0        0     3455 2023-06-13 20:27:55.987905 flufl_i18n-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1005 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/__init__.py
+-rw-r--r--   0        0        0    10234 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_application.py
+-rw-r--r--   0        0        0      806 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_expand.py
+-rw-r--r--   0        0        0     1053 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_registry.py
+-rw-r--r--   0        0        0     2371 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_strategy.py
+-rw-r--r--   0        0        0      770 2023-06-13 20:27:30.441666 flufl_i18n-5.0.1/src/flufl/i18n/_substitute.py
+-rw-r--r--   0        0        0     2975 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/src/flufl/i18n/_translator.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/src/flufl/i18n/py.typed
+-rw-r--r--   0        0        0     4442 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/src/flufl/i18n/types.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:27:30.466667 flufl_i18n-5.0.1/test/data/messages/__init__.py
+-rw-r--r--   0        0        0      506 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.mo
+-rw-r--r--   0        0        0      673 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.po
+-rw-r--r--   0        0        0      505 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.mo
+-rw-r--r--   0        0        0      672 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.po
+-rw-r--r--   0        0        0      370 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_application.py
+-rw-r--r--   0        0        0      845 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_expand.py
+-rw-r--r--   0        0        0      520 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_substitute.py
+-rw-r--r--   0        0        0     3617 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/test/test_translator.py
+-rw-r--r--   0        0        0      772 2023-06-13 20:27:30.442666 flufl_i18n-5.0.1/tox.ini
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 flufl_i18n-5.0.1/PKG-INFO
```

### Comparing `flufl.i18n-4.1.1/LICENSE` & `flufl_i18n-5.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2004-2022 Barry Warsaw
+Copyright 2004-2023 Barry Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.i18n-4.1.1/README.rst` & `flufl_i18n-5.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 sophisticated management of multiple-context applications such as Internet
 servers.
 
 
 Author
 ======
 
-``flufl.i18n`` is Copyright (C) 2004-2022 Barry Warsaw <barry@python.org>
+``flufl.i18n`` is Copyright (C) 2004-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
```

### Comparing `flufl.i18n-4.1.1/conftest.py` & `flufl_i18n-5.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/docs/NEWS.rst` & `flufl_i18n-5.0.1/docs/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =====================
 flufl.i18n change log
 =====================
 
+5.0.1 (2023-06-13)
+==================
+* Fix the build backend.
+
+5.0 (unreleased)
+================
+* Drop Python 3.7 support. (GL#15)
+* Switch from ``flake8`` and ``isort`` to ``ruff`` for code quality. (GL#16)
+* Bump dependencies.
+
 4.1.1 (2022-09-05)
 ==================
 * Improvements to the GitLab CI integration.
 * Several minor updates to work better with the latest pdm.
 
 4.1 (2022-08-25)
 ==================
```

### Comparing `flufl.i18n-4.1.1/docs/apiref.rst` & `flufl_i18n-5.0.1/docs/apiref.rst`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/docs/conf.py` & `flufl_i18n-5.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,32 @@
 import sys, os
 from datetime import date
 import importlib.metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
+sys.path.append(os.path.abspath('../src'))
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
-    'sphinx_autodoc_typehints',
     ]
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     }
 
+autodoc_typehints = 'both'
+autoclass_content = 'both'
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['../../_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
```

### Comparing `flufl.i18n-4.1.1/docs/expand.rst` & `flufl_i18n-5.0.1/docs/expand.rst`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/docs/index.rst` & `flufl_i18n-5.0.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 convenient API for multi-context applications, such as servers, which may need
 to switch language contexts for different tasks.
 
 
 Requirements
 ============
 
-``flufl.i18n`` requires Python 3.7 or newer.
+``flufl.i18n`` requires Python 3.8 or newer.
 
 
 Documentation
 =============
 
 A `simple guide`_ to using the library is available, along with a detailed
 `API reference`_.
@@ -44,15 +44,15 @@
 
 You may contact the author via barry@python.org.
 
 
 Copyright
 =========
 
-Copyright (C) 2004-2022 Barry A. Warsaw
+Copyright (C) 2004-2023 Barry A. Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `flufl.i18n-4.1.1/docs/strategies.rst` & `flufl_i18n-5.0.1/docs/strategies.rst`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/docs/using.rst` & `flufl_i18n-5.0.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/pyproject.toml` & `flufl_i18n-5.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "flufl.i18n"
 authors = [
     { name = "Barry Warsaw", email = "barry@python.org" },
 ]
 description = "A high level API for internationalizing Python libraries and applications"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "i18n",
     "internationalization",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Development Status :: 6 - Mature",
@@ -22,33 +22,31 @@
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Internationalization",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Localization",
 ]
 dependencies = [
-    "typing_extensions; python_version<'3.8'",
-    "atpublic>=2.3",
+    "atpublic",
 ]
 dynamic = []
-version = "4.1.1"
+version = "5.0.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://flufli18n.readthedocs.io"
 Documentation = "https://flufli18n.readthedocs.io"
 "Source Code" = "https://gitlab.com/warsaw/flufl.i18n.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/flufl.i18n/issues"
 
-[project.optional-dependencies]
-
 [tool.pdm.version]
-from = "src/flufl/i18n/__init__.py"
+source = "file"
+path = "src/flufl/i18n/__init__.py"
 
 [tool.pdm.build]
 includes = [
     "src/flufl",
 ]
 excludes = [
     "**/.mypy_cache",
@@ -65,22 +63,20 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "flake8",
-    "isort",
-    "mypy",
+    "ruff",
     "blue",
+    "mypy",
 ]
 docs = [
     "sphinx",
-    "sphinx-autodoc-typehints",
     "furo",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=flufl --cov-report=term --cov-report=xml -p no:doctest"
 testpaths = "test docs"
 
@@ -93,24 +89,58 @@
 parallel = true
 
 [tool.coverage.paths]
 source = [
     "flufl/i18n",
 ]
 
-[tool.isort]
-include_trailing_comma = true
-known_first_party = "flufl"
-length_sort_straight = true
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-order_by_type = false
-skip = [
-    "conf.py",
+[tool.ruff]
+line-length = 79
+src = [
+    "src",
+]
+select = [
+    "B",
+    "D",
+    "E",
+    "F",
+    "I",
+    "RUF100",
+    "UP",
+    "W",
+]
+ignore = [
+    "D100",
+    "D104",
+    "D105",
+]
+
+[tool.ruff.pydocstyle]
+convention = "pep257"
+
+[tool.ruff.isort]
+known-first-party = [
+    "flufl.i18n",
+]
+lines-after-imports = 2
+lines-between-types = 1
+order-by-type = true
+
+[tool.ruff.per-file-ignores]
+"src/flufl/i18n/_strategy.py" = [
+    "I001",
+]
+"src/flufl/i18n/_substitute.py" = [
+    "I001",
+]
+"src/flufl/i18n/_translator.py" = [
+    "I001",
+]
+"src/flufl/i18n/_application.py" = [
+    "D412",
 ]
 
 [tool.mypy]
 mypy_path = "src"
 namespace_packages = true
 disallow_any_generics = true
 disallow_subclassing_any = true
@@ -142,10 +172,10 @@
     "sybil.*",
     "psutil",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/__init__.py` & `flufl_i18n-5.0.1/src/flufl/i18n/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from flufl.i18n.types import (
     RuntimeTranslator,
     TranslationContextManager,
     TranslationStrategy,
 )
 
 
-__version__ = '4.1.1'
+__version__ = '5.0.1'
 
 
 _public(
     Application=Application,
     PackageStrategy=PackageStrategy,
     RuntimeTranslator=RuntimeTranslator,
     SimpleStrategy=SimpleStrategy,
@@ -24,15 +24,15 @@
     expand=expand,
     registry=registry,
 )
 
 
 @_public
 def initialize(domain: str) -> RuntimeTranslator:
-    """A convenience function for setting up translation.
+    """Initialize a translation context.
 
     :param domain: The application's name.
     :return: The translation function, typically bound to _()
     """
     strategy = SimpleStrategy(domain)
     application = registry.register(strategy)
     return application._
```

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_application.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 from gettext import NullTranslations
 from types import TracebackType
-from typing import Dict, List, NamedTuple, Optional, Type
+from typing import Dict, List, Literal, NamedTuple, Optional, Type
 
 from public import public
 
 from flufl.i18n._translator import Translator
 from flufl.i18n.types import (
     RuntimeTranslator,
     TranslationContextManager,
     TranslationStrategy,
 )
 
 
-try:
-    from typing import Literal
-except ImportError:                                 # pragma: nocover
-    from typing_extensions import Literal  # type: ignore
-
-
 class _Using(TranslationContextManager):
     """Context manager for _.using()."""
 
-    # 2020-07-06(warsaw): Once Python 3.7 is the minimum supported version, we
-    # can use `from __future__ import annotations` instead of the string type.
     def __init__(self, application: 'Application', language_code: str):
         self._application = application
         self._language_code = language_code
 
     def __enter__(self) -> TranslationContextManager:
         self._application.push(self._language_code)
         return self
```

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_expand.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_expand.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_registry.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_registry.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_strategy.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """
         # gettext.translation() requires None or a sequence.
         languages = None if language_code is None else [language_code]
         try:
             return gettext.translation(
                 self.name, self._messages_dir, languages
             )
-        except IOError:
+        except OSError:
             # Fall back to untranslated source language.
             return gettext.NullTranslations()
 
     @property
     def name(self) -> str:
         """The application's name."""
         return self._name
```

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_substitute.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_substitute.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/_translator.py` & `flufl_i18n-5.0.1/src/flufl/i18n/_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         :param original: The original string to translate.
         :param extras: Extra substitution mapping, elements of which override
             the locals and globals.
         :return: The translated string.
         """
         if original == '':
             return ''
-        assert original, 'Cannot translate: {}'.format(original)
+        assert original, f'Cannot translate: {original}'
         # Because the original string is what the text extractors put into the
         # catalog, we must first look up the original unadulterated string in
         # the catalog.  Use the global translation context for this.
         #
         # Translations must be unicode safe internally.  The translation
         # service is one boundary to the outside world, so to honor this
         # constraint, make sure that all strings to come out of this are
```

### Comparing `flufl.i18n-4.1.1/src/flufl/i18n/types.py` & `flufl_i18n-5.0.1/src/flufl/i18n/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from abc import ABC, abstractmethod
 from gettext import NullTranslations
 from types import TracebackType
-from typing import Dict, Optional, Type
+from typing import Dict, Literal, Optional, Type
 
 from public import public
 
 
-try:
-    from typing import Literal
-except ImportError:                                 # pragma: nocover
-    from typing_extensions import Literal  # type: ignore
-
-
 @public
 class TranslationContextManager(ABC):
     """Context manager for translations in a particular language."""
 
     @abstractmethod
     def __enter__(self) -> 'TranslationContextManager':
         pass                                        # pragma: nocover
@@ -28,14 +22,16 @@
         exc_tb: Optional[TracebackType],
     ) -> Literal[False]:
         pass                                        # pragma nocover
 
 
 @public
 class RuntimeTranslator(ABC):
+    """Abstract class representing the interface for the _() function."""
+
     @abstractmethod
     def __call__(
         self, original: str, extras: Optional[Dict[str, str]] = None
     ) -> str:
         """Translate the string into the language of the current context.
 
         This is the primary method for the runtime behavior or translating a
@@ -85,56 +81,60 @@
         """Pop the current catalog off the translation stack.
 
         No exception is raised for under-runs.  In that case, pop() just
         no-ops and the null translation becomes the current translation
         context.
         """
 
-    @property
+    # 2023-06-08(warsaw): mypy as of 1.3.0 gives us a bogus error:
+    # Overloaded method has both abstract and non-abstract variants  [misc]
+    #
+    # https://github.com/python/mypy/issues/13649
+    # https://github.com/python/mypy/issues/4165
+    @property                                       # type: ignore
+    @abstractmethod
     def default(self) -> Optional[str]:
         """Return the default language code.
 
         :return: The default language code, or None if there is no default
             language.
         """
 
-    # 2020-07-06(warsaw): Despite the recommendations in
-    #
-    # https://docs.python.org/3/library/abc.html#abc.abstractproperty
-    #
-    # says for adding @abstractmethod to @property's, mypy does not support
-    # this.
-    #
-    # https://github.com/python/mypy/issues/1362
-
     @default.setter
+    @abstractmethod
     def default(self, language_code: str) -> None:
         """Set the default language code.
 
         :param language_code: The language code for the default translation
             context.
         """
 
     @default.deleter
+    @abstractmethod
     def default(self) -> None:
         """Reset the default language to the null translator."""
 
     @property
+    @abstractmethod
     def code(self) -> Optional[str]:
         """The language code currently in effect, if there is one."""
 
 
 @public
 class TranslationStrategy(ABC):
+    """Abstract class representing the interface for translation strategies."""
+
+    @abstractmethod
     def __call__(
         self, language_code: Optional[str] = None
     ) -> NullTranslations:
         """Find the catalog for the language.
 
         :param language_code: The language code to find.  If None, then the
             default gettext language code lookup scheme is used.
         :return: A `gettext` catalog.
         """
 
     @property
+    @abstractmethod
     def name(self) -> str:
         """The application's name."""
```

### Comparing `flufl.i18n-4.1.1/test/data/messages/xx/LC_MESSAGES/flufl.po` & `flufl_i18n-5.0.1/test/data/messages/xx/LC_MESSAGES/flufl.po`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/test/data/messages/yy/LC_MESSAGES/flufl.po` & `flufl_i18n-5.0.1/test/data/messages/yy/LC_MESSAGES/flufl.po`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/test/test_expand.py` & `flufl_i18n-5.0.1/test/test_expand.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/test/test_substitute.py` & `flufl_i18n-5.0.1/test/test_substitute.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/test/test_translator.py` & `flufl_i18n-5.0.1/test/test_translator.py`

 * *Files identical despite different names*

### Comparing `flufl.i18n-4.1.1/PKG-INFO` & `flufl_i18n-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
-Name: flufl.i18n
-Version: 4.1.1
+Name: flufl-i18n
+Version: 5.0.1
 Summary: A high level API for internationalizing Python libraries and applications
+Keywords: i18n internationalization
+Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
-Keywords: i18n,internationalization
-Author-email: Barry Warsaw <barry@python.org>
-Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
-Project-URL: Bug Tracker, https://gitlab.com/warsaw/flufl.i18n/issues
+Project-URL: Home page, https://flufli18n.readthedocs.io
 Project-URL: Documentation, https://flufli18n.readthedocs.io
-Project-URL: Home Page, https://flufli18n.readthedocs.io
-Project-URL: Source Code, https://gitlab.com/warsaw/flufl.i18n.git
+Project-URL: Source code, https://gitlab.com/warsaw/flufl.i18n.git
+Project-URL: Bug tracker, https://gitlab.com/warsaw/flufl.i18n/issues
+Requires-Python: >=3.8
+Requires-Dist: atpublic
 Description-Content-Type: text/x-rst
 
 ==========
 flufl.i18n
 ==========
 
 A high level API for internationalizing Python libraries and applications.
@@ -37,22 +38,21 @@
 sophisticated management of multiple-context applications such as Internet
 servers.
 
 
 Author
 ======
 
-``flufl.i18n`` is Copyright (C) 2004-2022 Barry Warsaw <barry@python.org>
+``flufl.i18n`` is Copyright (C) 2004-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
 
  * Project home: https://gitlab.com/warsaw/flufl.i18n
  * Report bugs at: https://gitlab.com/warsaw/flufl.i18n/issues
  * Code hosting: https://gitlab.com/warsaw/flufl.i18n.git
  * Documentation: https://flufli18n.readthedocs.io/
  * PyPI: https://pypi.python.org/pypi/flufl.i18n
-
```

