# Comparing `tmp/pygus-1.0.tar.gz` & `tmp/pygus-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-1.0.tar", max compression
+gzip compressed data, was "pygus-2.0.tar", max compression
```

## Comparing `pygus-1.0.tar` & `pygus-2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-1.0/LICENSE
--rw-r--r--   0        0        0     1541 2023-02-22 17:36:23.738197 pygus-1.0/README-pypi.md
--rw-r--r--   0        0        0      134 2023-04-20 10:39:32.247844 pygus-1.0/pygus/__init__.py
--rw-r--r--   0        0        0      156 2023-04-20 10:39:32.248007 pygus-1.0/pygus/gus/__init__.py
--rw-r--r--   0        0        0    27311 2023-04-20 10:39:32.248384 pygus-1.0/pygus/gus/agents.py
--rw-r--r--   0        0        0     7484 2023-04-20 10:39:32.248656 pygus-1.0/pygus/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2023-04-20 10:39:32.248771 pygus-1.0/pygus/gus/inputs/allometrics.json
--rw-r--r--   0        0        0       95 2023-04-20 10:39:32.248836 pygus-1.0/pygus/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2023-04-20 10:39:32.248895 pygus-1.0/pygus/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2023-04-20 10:39:32.248983 pygus-1.0/pygus/gus/inputs/trees.csv
--rw-r--r--   0        0        0    15469 2023-04-20 10:39:32.249144 pygus-1.0/pygus/gus/models.py
--rw-r--r--   0        0        0  1566870 2023-04-20 10:39:32.257838 pygus-1.0/pygus/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     2241 2023-04-20 12:41:09.601132 pygus-1.0/pygus/gus/utilities.py
--rw-r--r--   0        0        0     1701 2023-04-20 10:39:32.258149 pygus-1.0/pygus/gus/weather.py
--rw-r--r--   0        0        0       58 2023-04-20 10:39:32.258299 pygus-1.0/pygus/impacts/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-20 10:39:32.258425 pygus-1.0/pygus/impacts/carbon.py
--rw-r--r--   0        0        0    32960 2023-04-20 10:39:32.258637 pygus-1.0/pygus/impacts/water.py
--rw-r--r--   0        0        0     1499 2023-04-20 12:46:01.662170 pygus-1.0/pyproject.toml
--rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 pygus-1.0/setup.py
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pygus-1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-31 16:02:43.286749 pygus-2.0/LICENSE
+-rw-r--r--   0        0        0     1541 2023-02-22 17:36:23.738197 pygus-2.0/README-pypi.md
+-rw-r--r--   0        0        0      134 2023-04-20 10:39:32.247844 pygus-2.0/pygus/__init__.py
+-rw-r--r--   0        0        0      156 2023-04-20 10:39:32.248007 pygus-2.0/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27311 2023-04-20 10:39:32.248384 pygus-2.0/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-04-20 10:39:32.248656 pygus-2.0/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-20 10:39:32.248771 pygus-2.0/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0       95 2023-04-20 10:39:32.248836 pygus-2.0/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-20 10:39:32.248895 pygus-2.0/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-20 10:39:32.248983 pygus-2.0/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    15469 2023-04-20 10:39:32.249144 pygus-2.0/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-20 10:39:32.257838 pygus-2.0/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     2241 2023-04-20 12:41:09.601132 pygus-2.0/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-20 10:39:32.258149 pygus-2.0/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-20 10:39:32.258299 pygus-2.0/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-20 10:39:32.258425 pygus-2.0/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-20 10:39:32.258637 pygus-2.0/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1499 2023-06-13 15:12:13.755133 pygus-2.0/pyproject.toml
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 pygus-2.0/setup.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 pygus-2.0/PKG-INFO
```

### Comparing `pygus-1.0/LICENSE` & `pygus-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-1.0/README-pypi.md` & `pygus-2.0/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/agents.py` & `pygus-2.0/pygus/gus/agents.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/allometrics.py` & `pygus-2.0/pygus/gus/allometrics.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/inputs/allometrics.json` & `pygus-2.0/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/inputs/trees.csv` & `pygus-2.0/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/models.py` & `pygus-2.0/pygus/gus/models.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/outputs/trees_yearly.json` & `pygus-2.0/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/utilities.py` & `pygus-2.0/pygus/gus/utilities.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/gus/weather.py` & `pygus-2.0/pygus/gus/weather.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/impacts/carbon.py` & `pygus-2.0/pygus/impacts/carbon.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pygus/impacts/water.py` & `pygus-2.0/pygus/impacts/water.py`

 * *Files identical despite different names*

### Comparing `pygus-1.0/pyproject.toml` & `pygus-2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGUS"
-version = "1.0"
+version = "2.0"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
```

### Comparing `pygus-1.0/setup.py` & `pygus-2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'termcolor>=2.1.1,<3.0.0',
  'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '1.0',
+    'version': '2.0',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-1.0/PKG-INFO` & `pygus-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 1.0
+Version: 2.0
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
```

