# Comparing `tmp/bibtex-formatter-1.1.0.tar.gz` & `tmp/bibtex-formatter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtex-formatter-1.1.0.tar", last modified: Mon Nov 14 07:01:42 2022, max compression
+gzip compressed data, was "bibtex-formatter-1.3.0.tar", last modified: Tue Jun 13 12:32:34 2023, max compression
```

## Comparing `bibtex-formatter-1.1.0.tar` & `bibtex-formatter-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/bfm/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/bfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/bfm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13161 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/bfm/format.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-14 07:01:42.000000 bibtex-formatter-1.1.0/bibtex_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/project.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 07:01:42.699465 bibtex-formatter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-14 07:01:27.000000 bibtex-formatter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:34.446480 bibtex-formatter-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:34.438480 bibtex-formatter-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:34.442480 bibtex-formatter-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 12:32:34.446480 bibtex-formatter-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:34.442480 bibtex-formatter-1.3.0/bfm/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/bfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/bfm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25610 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/bfm/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:32:34.446480 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 12:32:34.000000 bibtex-formatter-1.3.0/bibtex_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/project.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:32:34.446480 bibtex-formatter-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-13 12:32:19.000000 bibtex-formatter-1.3.0/setup.py
```

### Comparing `bibtex-formatter-1.1.0/.github/workflows/python-publish.yml` & `bibtex-formatter-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bibtex-formatter-1.1.0/.gitignore` & `bibtex-formatter-1.3.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 tests/
+tmp/
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 .idea/
 **.idea/**
```

### Comparing `bibtex-formatter-1.1.0/LICENSE` & `bibtex-formatter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bibtex-formatter-1.1.0/PKG-INFO` & `bibtex-formatter-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 Metadata-Version: 2.1
 Name: bibtex-formatter
-Version: 1.1.0
+Version: 1.3.0
 Summary: Format
 Home-page: https://github.com/Nickydusk/BibTeX-Formatter.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BibTeX Formatter
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/Nickydusk/bibtex-formatter) ![PyPI](https://img.shields.io/pypi/v/bibtex-formatter) ![PyPI - Downloads](https://img.shields.io/pypi/dm/bibtex-formatter) ![GitHub](https://img.shields.io/github/license/Nickydusk/BibTex-Formatter)
 
 Help generate citations that meet the requirements for conference and journal submissions.
 
 ## Quick Installation
+
 Install from [PyPi](https://pypi.org/project/bibtex-formatter/):
 
 ```bash
-pip install bibtex-formatter
+pip install -U bibtex-formatter
 ```
 
 Alternatively, you can also install the latest version (not stable) from github:
 
 ```bash
-pip install git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
+pip install -U git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
 ```
 
 ## Usage
 
-`$ bfm IN_FILE`
+```bash
+bfm IN_FILE
+```
 
 Positional args:
-- `IN_FILE`: Choose the input .bib file.
+
+- `IN_FILE`: Choose the input .bib file, default to `in.bib`
 
 Options (Please see `bfm --help` for more details):
-- `-no`, `--no_online`: Forbid online check (useful when not have internet)
+
 - `-o OUTPUT`,`--output OUTPUT`: Choose the output .bib file, default to `out.bib`
 - `-l LOG`,`--log LOG`: Choose the output log file, default to `logs.txt`
+- `-d`, `--use_database`: Do online check with NJU database, default to False (The feature may override correct entries, use with caution!)
 
 ## Features
-- [x] Remove duplicate entries, log what is removed
-- [x] Online check contents, make sure they are up to date 
+
+- [x] Remove duplicate citations (keep the first occurrence), log what is removed
 - [x] Simplify keys according to citation type (e.g., `@inproceedings -> [author, title, booktitle, pages, year]`)
-- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems (NeurIPS)`)
+- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems`)
+- [x] Standardize "pages" to `pages = {start-end}`, alert if more or less timestamps.
+- [x] Standardize arXiv citations to **google scholar style**
+  - [x] arXiv export bibtex -> google scholar style
+  - [x] dblp bibtex -> google scholar style
+- [ ] Online check contents, make sure they are up to date
 
 ## Welcome to PR
 
 You can make contribution to the project by filling more standard conference / journal names in `refactor/STANDARD_NAMES`. Please use pull requests to submit your changes.
```

### Comparing `bibtex-formatter-1.1.0/README.md` & `bibtex-formatter-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # BibTeX Formatter
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/Nickydusk/bibtex-formatter) ![PyPI](https://img.shields.io/pypi/v/bibtex-formatter) ![PyPI - Downloads](https://img.shields.io/pypi/dm/bibtex-formatter) ![GitHub](https://img.shields.io/github/license/Nickydusk/BibTex-Formatter)
 
 Help generate citations that meet the requirements for conference and journal submissions.
 
 ## Quick Installation
+
 Install from [PyPi](https://pypi.org/project/bibtex-formatter/):
 
 ```bash
-pip install bibtex-formatter
+pip install -U bibtex-formatter
 ```
 
 Alternatively, you can also install the latest version (not stable) from github:
 
 ```bash
-pip install git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
+pip install -U git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
 ```
 
 ## Usage
 
-`$ bfm IN_FILE`
+```bash
+bfm IN_FILE
+```
 
 Positional args:
-- `IN_FILE`: Choose the input .bib file.
+
+- `IN_FILE`: Choose the input .bib file, default to `in.bib`
 
 Options (Please see `bfm --help` for more details):
-- `-no`, `--no_online`: Forbid online check (useful when not have internet)
+
 - `-o OUTPUT`,`--output OUTPUT`: Choose the output .bib file, default to `out.bib`
 - `-l LOG`,`--log LOG`: Choose the output log file, default to `logs.txt`
+- `-d`, `--use_database`: Do online check with NJU database, default to False (The feature may override correct entries, use with caution!)
 
 ## Features
-- [x] Remove duplicate entries, log what is removed
-- [x] Online check contents, make sure they are up to date 
+
+- [x] Remove duplicate citations (keep the first occurrence), log what is removed
 - [x] Simplify keys according to citation type (e.g., `@inproceedings -> [author, title, booktitle, pages, year]`)
-- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems (NeurIPS)`)
+- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems`)
+- [x] Standardize "pages" to `pages = {start-end}`, alert if more or less timestamps.
+- [x] Standardize arXiv citations to **google scholar style**
+  - [x] arXiv export bibtex -> google scholar style
+  - [x] dblp bibtex -> google scholar style
+- [ ] Online check contents, make sure they are up to date
 
 ## Welcome to PR
 
 You can make contribution to the project by filling more standard conference / journal names in `refactor/STANDARD_NAMES`. Please use pull requests to submit your changes.
```

### Comparing `bibtex-formatter-1.1.0/bibtex_formatter.egg-info/PKG-INFO` & `bibtex-formatter-1.3.0/bibtex_formatter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 Metadata-Version: 2.1
 Name: bibtex-formatter
-Version: 1.1.0
+Version: 1.3.0
 Summary: Format
 Home-page: https://github.com/Nickydusk/BibTeX-Formatter.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BibTeX Formatter
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/Nickydusk/bibtex-formatter) ![PyPI](https://img.shields.io/pypi/v/bibtex-formatter) ![PyPI - Downloads](https://img.shields.io/pypi/dm/bibtex-formatter) ![GitHub](https://img.shields.io/github/license/Nickydusk/BibTex-Formatter)
 
 Help generate citations that meet the requirements for conference and journal submissions.
 
 ## Quick Installation
+
 Install from [PyPi](https://pypi.org/project/bibtex-formatter/):
 
 ```bash
-pip install bibtex-formatter
+pip install -U bibtex-formatter
 ```
 
 Alternatively, you can also install the latest version (not stable) from github:
 
 ```bash
-pip install git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
+pip install -U git+https://github.com/Nickydusk/BibTeX-Formatter.git@main
 ```
 
 ## Usage
 
-`$ bfm IN_FILE`
+```bash
+bfm IN_FILE
+```
 
 Positional args:
-- `IN_FILE`: Choose the input .bib file.
+
+- `IN_FILE`: Choose the input .bib file, default to `in.bib`
 
 Options (Please see `bfm --help` for more details):
-- `-no`, `--no_online`: Forbid online check (useful when not have internet)
+
 - `-o OUTPUT`,`--output OUTPUT`: Choose the output .bib file, default to `out.bib`
 - `-l LOG`,`--log LOG`: Choose the output log file, default to `logs.txt`
+- `-d`, `--use_database`: Do online check with NJU database, default to False (The feature may override correct entries, use with caution!)
 
 ## Features
-- [x] Remove duplicate entries, log what is removed
-- [x] Online check contents, make sure they are up to date 
+
+- [x] Remove duplicate citations (keep the first occurrence), log what is removed
 - [x] Simplify keys according to citation type (e.g., `@inproceedings -> [author, title, booktitle, pages, year]`)
-- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems (NeurIPS)`)
+- [x] Standardize conference / journal names (e.g., `Advances in Neural Information Processing Systems`)
+- [x] Standardize "pages" to `pages = {start-end}`, alert if more or less timestamps.
+- [x] Standardize arXiv citations to **google scholar style**
+  - [x] arXiv export bibtex -> google scholar style
+  - [x] dblp bibtex -> google scholar style
+- [ ] Online check contents, make sure they are up to date
 
 ## Welcome to PR
 
 You can make contribution to the project by filling more standard conference / journal names in `refactor/STANDARD_NAMES`. Please use pull requests to submit your changes.
```

### Comparing `bibtex-formatter-1.1.0/setup.py` & `bibtex-formatter-1.3.0/setup.py`

 * *Files identical despite different names*

