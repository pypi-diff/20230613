# Comparing `tmp/ranktier-1.4.4.tar.gz` & `tmp/ranktier-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ranktier-1.4.4.tar", last modified: Tue Nov  9 14:01:30 2021, max compression
+gzip compressed data, was "ranktier-1.4.5.tar", last modified: Tue Jun 13 12:49:56 2023, max compression
```

## Comparing `ranktier-1.4.4.tar` & `ranktier-1.4.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-11-09 14:01:30.594905 ranktier-1.4.4/
--rw-rw-rw-   0        0        0       17 2021-11-09 13:30:38.000000 ranktier-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2592 2021-11-09 14:01:30.594905 ranktier-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2021-11-09 13:30:38.000000 ranktier-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2021-11-09 14:01:30.570413 ranktier-1.4.4/ranktier/
--rw-rw-rw-   0        0        0     2518 2021-11-09 13:52:52.000000 ranktier-1.4.4/ranktier/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 14:01:30.579239 ranktier-1.4.4/ranktier.egg-info/
--rw-rw-rw-   0        0        0     2592 2021-11-09 14:01:30.000000 ranktier-1.4.4/ranktier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2021-11-09 14:01:30.000000 ranktier-1.4.4/ranktier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-09 14:01:30.000000 ranktier-1.4.4/ranktier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-11-09 14:01:30.000000 ranktier-1.4.4/ranktier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-11-09 14:01:30.594905 ranktier-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1167 2021-11-09 13:52:52.000000 ranktier-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-09 14:01:30.594905 ranktier-1.4.4/test/
--rw-rw-rw-   0        0        0      190 2021-11-09 13:30:38.000000 ranktier-1.4.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:49:56.407150 ranktier-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-13 12:49:46.000000 ranktier-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 12:49:46.000000 ranktier-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-13 12:49:56.407150 ranktier-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-13 12:49:46.000000 ranktier-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:49:56.407150 ranktier-1.4.5/ranktier/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-13 12:49:46.000000 ranktier-1.4.5/ranktier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:49:56.407150 ranktier-1.4.5/ranktier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-13 12:49:56.000000 ranktier-1.4.5/ranktier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 12:49:56.000000 ranktier-1.4.5/ranktier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:49:56.000000 ranktier-1.4.5/ranktier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 12:49:56.000000 ranktier-1.4.5/ranktier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 12:49:56.407150 ranktier-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 12:49:46.000000 ranktier-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:49:56.407150 ranktier-1.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-13 12:49:46.000000 ranktier-1.4.5/test/test.py
```

### Comparing `ranktier-1.4.4/PKG-INFO` & `ranktier-1.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-Metadata-Version: 2.1
-Name: ranktier
-Version: 1.4.4
-Summary: A Dota rank tier converter
-Home-page: https://github.com/marcusmunch/ranktier
-Author: Marcus Grünewald
-Author-email: marcus@marcusmunch.dk
-License: GPLv3
-Description: ranktier
-        ========
-        [![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
-        [![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        [![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        [![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        
-        ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
-        
-        Setup
-        -----
-        `ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
-        `pip install ranktier`
-        
-        It can also be installed by downloading the repo and running `pip install .`
-        
-        Usage
-        -----
-        ```python
-        >>> import ranktier
-        >>> r = ranktier.Rank(42)
-        >>> print(r)
-        Archon [2]
-        >>> p = ranktier.Player(86745912)
-        >>> print(p.rank)
-        Immortal rank 3
-        ```
-        `Rank.name` can also be used, but returns the same as above.
-        
-        `rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
-        `int`-type variable.
-        
-        As of 1.4, Player objects also have names:
-        ```python
-        >>> p.personaname
-        å¤©é¸½
-        >>> p.name
-        Arteezy
-        ```
-        
-        `personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: ranktier
+Version: 1.4.5
+Summary: A Dota rank tier converter
+Home-page: https://github.com/marcusmunch/ranktier
+Author: Marcus Grünewald
+Author-email: marcus@marcusmunch.dk
+License: GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ranktier
+========
+[![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
+[![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+
+ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
+
+Setup
+-----
+`ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
+`pip install ranktier`
+
+It can also be installed by downloading the repo and running `pip install .`
+
+Usage
+-----
+```python
+>>> import ranktier
+>>> r = ranktier.Rank(42)
+>>> print(r)
+Archon [2]
+>>> p = ranktier.Player(86745912)
+>>> print(p.rank)
+Immortal rank 3
+```
+`Rank.name` can also be used, but returns the same as above.
+
+`rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
+`int`-type variable.
+
+As of 1.4, Player objects also have names:
+```python
+>>> p.personaname
+天鸽
+>>> p.name
+Arteezy
+```
+
+`personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
```

### Comparing `ranktier-1.4.4/README.md` & `ranktier-1.4.5/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-ranktier
-========
-[![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
-[![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-[![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-[![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-
-ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
-
-Setup
------
-`ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
-`pip install ranktier`
-
-It can also be installed by downloading the repo and running `pip install .`
-
-Usage
------
-```python
->>> import ranktier
->>> r = ranktier.Rank(42)
->>> print(r)
-Archon [2]
->>> p = ranktier.Player(86745912)
->>> print(p.rank)
-Immortal rank 3
-```
-`Rank.name` can also be used, but returns the same as above.
-
-`rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
-`int`-type variable.
-
-As of 1.4, Player objects also have names:
-```python
->>> p.personaname
-天鸽
->>> p.name
-Arteezy
-```
-
-`personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
+ranktier
+========
+[![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
+[![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+
+ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
+
+Setup
+-----
+`ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
+`pip install ranktier`
+
+It can also be installed by downloading the repo and running `pip install .`
+
+Usage
+-----
+```python
+>>> import ranktier
+>>> r = ranktier.Rank(42)
+>>> print(r)
+Archon [2]
+>>> p = ranktier.Player(86745912)
+>>> print(p.rank)
+Immortal rank 3
+```
+`Rank.name` can also be used, but returns the same as above.
+
+`rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
+`int`-type variable.
+
+As of 1.4, Player objects also have names:
+```python
+>>> p.personaname
+天鸽
+>>> p.name
+Arteezy
+```
+
+`personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
```

### Comparing `ranktier-1.4.4/ranktier.egg-info/PKG-INFO` & `ranktier-1.4.5/ranktier.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-Metadata-Version: 2.1
-Name: ranktier
-Version: 1.4.4
-Summary: A Dota rank tier converter
-Home-page: https://github.com/marcusmunch/ranktier
-Author: Marcus Grünewald
-Author-email: marcus@marcusmunch.dk
-License: GPLv3
-Description: ranktier
-        ========
-        [![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
-        [![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        [![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        [![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
-        
-        ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
-        
-        Setup
-        -----
-        `ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
-        `pip install ranktier`
-        
-        It can also be installed by downloading the repo and running `pip install .`
-        
-        Usage
-        -----
-        ```python
-        >>> import ranktier
-        >>> r = ranktier.Rank(42)
-        >>> print(r)
-        Archon [2]
-        >>> p = ranktier.Player(86745912)
-        >>> print(p.rank)
-        Immortal rank 3
-        ```
-        `Rank.name` can also be used, but returns the same as above.
-        
-        `rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
-        `int`-type variable.
-        
-        As of 1.4, Player objects also have names:
-        ```python
-        >>> p.personaname
-        å¤©é¸½
-        >>> p.name
-        Arteezy
-        ```
-        
-        `personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: ranktier
+Version: 1.4.5
+Summary: A Dota rank tier converter
+Home-page: https://github.com/marcusmunch/ranktier
+Author: Marcus Grünewald
+Author-email: marcus@marcusmunch.dk
+License: GPLv3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ranktier
+========
+[![Build Status](https://travis-ci.org/marcusmunch/ranktier.svg?branch=master)](https://travis-ci.org/marcusmunch/ranktier)
+[![PyPI](https://img.shields.io/pypi/v/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/pyversions/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+[![PyPI](https://img.shields.io/pypi/l/ranktier.svg)](https://pypi.python.org/pypi/ranktier)
+
+ranktier converts `rank_tier` numbers from APIs like [OpenDota](https://OpenDota.com) to human-readable ranks
+
+Setup
+-----
+`ranktier` can be installed from [PyPi](https://pypi.python.org/pypi):
+`pip install ranktier`
+
+It can also be installed by downloading the repo and running `pip install .`
+
+Usage
+-----
+```python
+>>> import ranktier
+>>> r = ranktier.Rank(42)
+>>> print(r)
+Archon [2]
+>>> p = ranktier.Player(86745912)
+>>> print(p.rank)
+Immortal rank 3
+```
+`Rank.name` can also be used, but returns the same as above.
+
+`rank` has to be a two-digit number for ranktier to work. Ranktier works regardless of `rank` being a `str`-type or
+`int`-type variable.
+
+As of 1.4, Player objects also have names:
+```python
+>>> p.personaname
+天鸽
+>>> p.name
+Arteezy
+```
+
+`personaname` refers to a profile's most recent alias, while `name` is the tag used by pros in-game.
```

### Comparing `ranktier-1.4.4/setup.py` & `ranktier-1.4.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
-
-import ranktier
-from setuptools import setup
-
-with open("README.md", "r") as f:
-    readme = f.read()
-
-setup(name="ranktier",
-    version=ranktier.__version__,
-    description="A Dota rank tier converter",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    url="https://github.com/marcusmunch/ranktier",
-    license="GPLv3",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        ],
-    author="Marcus Grünewald",
-    author_email="marcus@marcusmunch.dk",
-    packages=["ranktier"])
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+
+import ranktier
+from setuptools import setup
+
+with open("README.md", "r") as f:
+    readme = f.read()
+
+setup(name="ranktier",
+    version=ranktier.__version__,
+    description="A Dota rank tier converter",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    url="https://github.com/marcusmunch/ranktier",
+    license="GPLv3",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
+        ],
+    author="Marcus Grünewald",
+    author_email="marcus@marcusmunch.dk",
+    packages=["ranktier"])
```

