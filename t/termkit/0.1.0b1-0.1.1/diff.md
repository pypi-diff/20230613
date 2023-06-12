# Comparing `tmp/termkit-0.1.0b1.tar.gz` & `tmp/termkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termkit-0.1.0b1.tar", max compression
+gzip compressed data, was "termkit-0.1.1.tar", max compression
```

## Comparing `termkit-0.1.0b1.tar` & `termkit-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1515 2023-06-11 17:43:21.821414 termkit-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     2070 2023-06-11 17:43:21.673433 termkit-0.1.0b1/README.md
--rw-r--r--   0        0        0      676 2023-06-12 07:18:13.079478 termkit-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      199 2023-06-11 17:43:21.897404 termkit-0.1.0b1/termkit/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-11 17:43:21.821414 termkit-0.1.0b1/termkit/arguments.py
--rw-r--r--   0        0        0    10305 2023-06-12 07:16:59.659043 termkit-0.1.0b1/termkit/components.py
--rw-r--r--   0        0        0      698 2023-06-11 17:43:21.825413 termkit-0.1.0b1/termkit/exceptions.py
--rw-r--r--   0        0        0     2575 2023-06-11 17:43:21.825413 termkit-0.1.0b1/termkit/formatters.py
--rw-r--r--   0        0        0      543 2023-06-11 17:43:21.825413 termkit-0.1.0b1/termkit/groups.py
--rw-r--r--   0        0        0      330 2023-06-11 17:43:21.973394 termkit-0.1.0b1/termkit/helpers.py
--rw-r--r--   0        0        0     2052 2023-06-11 17:43:21.825413 termkit-0.1.0b1/termkit/tests.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 termkit-0.1.0b1/setup.py
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 termkit-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2070 2023-06-12 22:04:59.369121 termkit-0.1.1/README.md
+-rw-r--r--   0        0        0      618 2023-06-12 22:12:04.437179 termkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/__init__.py
+-rw-r--r--   0        0        0     3767 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/arguments.py
+-rw-r--r--   0        0        0    10313 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/components.py
+-rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/exceptions.py
+-rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/formatters.py
+-rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/groups.py
+-rw-r--r--   0        0        0      330 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/helpers.py
+-rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/tests.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 termkit-0.1.1/setup.py
+-rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 termkit-0.1.1/PKG-INFO
```

### Comparing `termkit-0.1.0b1/LICENSE` & `termkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/README.md` & `termkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/pyproject.toml` & `termkit-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "termkit"
-version = "0.1.0b1"
+version = "0.1.1"
 description = "Command Line Tools with ease"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.group.devel.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.15"
 tox = "^4.6.0"
-termynal = {version = "^0.3.0", python = ">=3.8"}
 
 [tool.pytest.ini_options]
-pythonpath = "termkit"
+pythonpath = "."
 testpaths = [
     "tests"
 ]
 
 [tool.coverage.run]
 source = [
     "termkit"
```

### Comparing `termkit-0.1.0b1/termkit/arguments.py` & `termkit-0.1.1/termkit/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         if self.type is None and type_hint is None:
             self.type = str
 
         if self.help is None:
             self.help = ""
 
-        self.help = f"(%(type)s) {self.help}".strip()
+        self.help = f"{self.help} (%(type)s) ".strip()
 
         args = self.__dict__.copy()
         del args['group']
 
         parser.positionals.add_argument(argument_name, **args)
```

### Comparing `termkit-0.1.0b1/termkit/components.py` & `termkit-0.1.1/termkit/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import inspect
 import os
 import sys
 import typing
 from abc import ABC
 from typing import Optional, Callable, Union, Dict, Any
 
-from helpers import get_callback_arguments
+from termkit.helpers import get_callback_arguments
 from termkit.groups import ArgumentGroup, MutuallyExclusiveGroup
 
 from termkit.formatters import TermkitDefaultFormatter
 from termkit.arguments import Argument
 from termkit.exceptions import TermkitError, InconsistentTypingError
```

### Comparing `termkit-0.1.0b1/termkit/exceptions.py` & `termkit-0.1.1/termkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/termkit/formatters.py` & `termkit-0.1.1/termkit/formatters.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/termkit/groups.py` & `termkit-0.1.1/termkit/groups.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/termkit/tests.py` & `termkit-0.1.1/termkit/tests.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.0b1/setup.py` & `termkit-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['termkit']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'termkit',
-    'version': '0.1.0b1',
+    'version': '0.1.1',
     'description': 'Command Line Tools with ease',
     'long_description': '<p align="center">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner.png#gh-dark-mode-only" width="450">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner_light.png#gh-light-mode-only" width="450">\n</p>\n<p align="center">\n  <b><i>Command Line Tools with... ease.</i></b>\n\n[![codecov](https://codecov.io/github/thmahe/termkit/branch/master/graph/badge.svg?token=o7UVrOsoq4)](https://codecov.io/github/thmahe/termkit)\n\n</p>\n\n## Table of Contents\n\n- [Introduction](#introduction)\n- [Features](#features)\n- [Requirement](#requirement)\n- [Installation](#installation)\n- [Examples](#examples)\n- [Feedback](#feedback)\n- [Acknowledgments](#acknowledgments)\n\n## Introduction\n\nTermkit is a framework for building command line interface applications using functions \nand type hints [[PEP 484]](https://peps.python.org/pep-0484/). \n**Solely written using [Python Standard Library](https://docs.python.org/3/library/)** and will always be to ensure\nminimal dependency footprint within your project.\n\nIn few words, Termkit is designed to be the foundation of serious CLI tools.\n\n## Features\n\nA few of the things you can do with Termkit:\n\n* Build CLI from functional code\n* Create fast prototypes using implicit arguments\n* Helpers populated from docstrings\n* Named profile for pre-populated arguments\n* Autocompletion through [argcomplete](https://pypi.org/project/argcomplete/) module\n* Cross-platforms\n\n## Requirement\n* Python 3.7 or higher\n\n*Yes... that\'s about it !* \n\n## Installation\n\nTermkit is published as a [Python package](https://pypi.org/project/termkit) and can be installed with pip.\n\nOpen up a terminal and install Termkit with:\n```shell\npip install termkit\n```\n\n## Examples\n\n### Greeting application\n\n```python\n# greet.py\nimport termkit\n\ndef greet(name):\n    print(f\'Hello {name} !\')\n\nif __name__ == \'__main__\':\n    termkit.run(greet)\n```\n\n```\n$ python3 ./greet.py Thomas\nHello Thomas !\n```\n\n## Feedback\n\nFeel free to send me feedback by [raising an issue](https://github.com/thmahe/termkit/issues/new).\nFeature requests are always welcome.\n\n',
     'author': 'Thomas Mahé',
     'author_email': 'contact@tmahe.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `termkit-0.1.0b1/PKG-INFO` & `termkit-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termkit
-Version: 0.1.0b1
+Version: 0.1.1
 Summary: Command Line Tools with ease
 Author: Thomas Mahé
 Author-email: contact@tmahe.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

