# Comparing `tmp/xklb-1.30.7.tar.gz` & `tmp/xklb-1.31.2.tar.gz`

## Comparing `xklb-1.30.7.tar` & `xklb-1.31.2.tar`

### file list

```diff
@@ -1,63 +1,66 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.7/.gitattributes
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.30.7/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.7/Windows.md
--rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.7/pdm.lock
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.7/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.30.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.7/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/books.py
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/consts.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/dl_config.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/dl_extract.py
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/hn_extract.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/lb.py
--rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/play_actions.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/playback.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/player.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/praw_extract.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tabs_extract.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tube_backend.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/tube_extract.py
--rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/usage.py
--rw-r--r--   0        0        0    36215 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.7/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.7/LICENSE
--rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.7/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.7/pyproject.toml
--rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.7/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.31.2/.gitattributes
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 xklb-1.31.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.31.2/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-1.31.2/pdm.lock
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 xklb-1.31.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.31.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/books.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/consts.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    12453 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/lb.py
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/media.py
+-rw-r--r--   0        0        0    25135 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/play_actions.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/playback.py
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/player.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/playlists.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    75374 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/usage.py
+-rw-r--r--   0        0        0    36702 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.31.2/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.31.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.31.2/LICENSE
+-rw-r--r--   0        0        0    97830 2020-02-02 00:00:00.000000 xklb-1.31.2/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-1.31.2/pyproject.toml
+-rw-r--r--   0        0        0   101457 2020-02-02 00:00:00.000000 xklb-1.31.2/PKG-INFO
```

### Comparing `xklb-1.30.7/Windows.md` & `xklb-1.31.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/pdm.lock` & `xklb-1.31.2/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -485,16 +485,16 @@
 summary = "Python implementation of John Gruber's Markdown."
 dependencies = [
     "importlib-metadata>=4.4; python_version < \"3.10\"",
 ]
 
 [[package]]
 name = "markdown-it-py"
-version = "2.2.0"
-requires_python = ">=3.7"
+version = "3.0.0"
+requires_python = ">=3.8"
 summary = "Python port of markdown-it. Markdown parsing, done right!"
 dependencies = [
     "mdurl~=0.1",
 ]
 
 [[package]]
 name = "markupsafe"
@@ -557,15 +557,15 @@
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python package to parse, read and write Microsoft OLE2 files (Structured Storage or Compound Document, Microsoft Office)"
 
 [[package]]
 name = "orjson"
-version = "3.9.0"
+version = "3.9.1"
 requires_python = ">=3.7"
 summary = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
@@ -641,15 +641,15 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.5.1"
+version = "3.5.3"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
@@ -798,15 +798,15 @@
 name = "pysubs2"
 version = "1.6.1"
 requires_python = ">=3.7"
 summary = "A library for editing subtitle files"
 
 [[package]]
 name = "pytest"
-version = "7.3.1"
+version = "7.3.2"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
@@ -870,19 +870,19 @@
     "chardet<4,>=3.0.2",
     "idna<3,>=2.5",
     "urllib3!=1.25.0,!=1.25.1,<1.26,>=1.21.1",
 ]
 
 [[package]]
 name = "rich"
-version = "13.4.1"
+version = "13.4.2"
 requires_python = ">=3.7.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 dependencies = [
-    "markdown-it-py<3.0.0,>=2.2.0",
+    "markdown-it-py>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
 version = "0.0.272"
@@ -1194,15 +1194,15 @@
 [[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
 
 [[package]]
 name = "websocket-client"
-version = "1.5.2"
+version = "1.5.3"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
 version = "11.0.3"
 requires_python = ">=3.7"
@@ -1257,15 +1257,15 @@
     "mutagen",
     "pycryptodomex",
     "websockets",
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.64.1"
+version = "0.66.0"
 requires_python = ">=3.7,<4.0"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 
@@ -1275,15 +1275,15 @@
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
 lock_version = "4.2"
 cross_platform = true
 groups = ["default", "all", "deluxe", "dev", "test"]
-content_hash = "sha256:838a39f6efcdf7890f45ea1f5c4bde5c496a26b207eb1344404bdaf9e0d230b0"
+content_hash = "sha256:def5380a32e603b2ddeeeea22583e403c33051d6f6e517afab5e71d22e69bda9"
 
 [metadata.files]
 "aiohttp 3.8.4" = [
     {url = "https://files.pythonhosted.org/packages/03/e7/84b65e341b1f45753fea51158d8a9522e57a5ae804acbc6dc34edf07cea0/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bca5f24726e2919de94f047739d0a4fc01372801a3672708260546aa2601bf57"},
     {url = "https://files.pythonhosted.org/packages/04/03/3ce412b191aba5961b4ada3ee7a93498623e218fb4d50ac6d357da61dc26/aiohttp-3.8.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8189c56eb0ddbb95bfadb8f60ea1b22fcfa659396ea36f6adcc521213cd7b44d"},
     {url = "https://files.pythonhosted.org/packages/05/ee/77b3dc08f41a1bce842e30134233c58b3bbe8c0fa7be121295aa2fad885d/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17b79c2963db82086229012cff93ea55196ed31f6493bb1ccd2c62f1724324e4"},
     {url = "https://files.pythonhosted.org/packages/07/3c/04c65b5873524a415509cbcf21787be32c31f4e729840fab9866dd197030/aiohttp-3.8.4-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:7c7837fe8037e96b6dd5cfcf47263c1620a9d332a87ec06a6ca4564e56bd0f36"},
@@ -2129,17 +2129,17 @@
     {url = "https://files.pythonhosted.org/packages/f6/45/232a3be71587fc534c009147b36081eb9bebd3bf6e608aec84598325aa41/lxml-4.9.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:df0623dcf9668ad0445e0558a21211d4e9a149ea8f5666917c8eeec515f0a6d1"},
     {url = "https://files.pythonhosted.org/packages/ff/d9/e821232295ec540a9c62bbfd6121c2e2969996ee8bc3b0c5325cc88272d0/lxml-4.9.2-cp310-cp310-win32.whl", hash = "sha256:d02a5399126a53492415d4906ab0ad0375a5456cc05c3fc0fc4ca11771745cda"},
 ]
 "markdown 3.4.3" = [
     {url = "https://files.pythonhosted.org/packages/9a/a1/1352b0e5a3c71a79fa9265726e2217f69df9fd4de0bcb5725cc61f62a5df/Markdown-3.4.3-py3-none-any.whl", hash = "sha256:065fd4df22da73a625f14890dd77eb8040edcbd68794bcd35943be14490608b2"},
     {url = "https://files.pythonhosted.org/packages/9d/80/cc67bfb7deb973d5ae662ee6454d2dafaa8f7c106feafd0d1572666ebde5/Markdown-3.4.3.tar.gz", hash = "sha256:8bf101198e004dc93e84a12a7395e31aac6a9c9942848ae1d99b9d72cf9b3520"},
 ]
-"markdown-it-py 2.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/bf/25/2d88e8feee8e055d015343f9b86e370a1ccbec546f2865c98397aaef24af/markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
-    {url = "https://files.pythonhosted.org/packages/e4/c0/59bd6d0571986f72899288a95d9d6178d0eebd70b6650f1bb3f0da90f8f7/markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
+"markdown-it-py 3.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/38/71/3b932df36c1a044d397a1f92d1cf91ee0a503d91e470cbd670aa66b07ed0/markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
+    {url = "https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
 ]
 "markupsafe 2.1.3" = [
     {url = "https://files.pythonhosted.org/packages/03/06/e72e88f81f8c91d4f488d21712d2d403fd644e3172eaadc302094377bc22/MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
     {url = "https://files.pythonhosted.org/packages/03/65/3473d2cb84bb2cda08be95b97fc4f53e6bcd701a2d50ba7b7c905e1e9273/MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
     {url = "https://files.pythonhosted.org/packages/10/b3/c2b0a61cc0e1d50dd8a1b663ba4866c667cb58fb35f12475001705001680/MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
     {url = "https://files.pythonhosted.org/packages/12/b3/d9ed2c0971e1435b8a62354b18d3060b66c8cb1d368399ec0b9baa7c0ee5/MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
     {url = "https://files.pythonhosted.org/packages/20/1d/713d443799d935f4d26a4f1510c9e61b1d288592fb869845e5cc92a1e055/MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
@@ -2344,61 +2344,61 @@
     {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
     {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
     {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
-"orjson 3.9.0" = [
-    {url = "https://files.pythonhosted.org/packages/00/a3/f645f6bdf235e217114250f8354705d6307ad2b083f4e3ae7c22b763f0be/orjson-3.9.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:bd89d63707ac616462832bfc5d16fa0c12483f86add2432ce55c8710c9531c03"},
-    {url = "https://files.pythonhosted.org/packages/02/6c/c29d9f8d0bd85d105d9b8508008831cd5ec4895a48e1283134f8ed8699de/orjson-3.9.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:748c1e8df0b0880c63d323e167ad17ab4db2e1178a40902c2fcb68cbe402d7c8"},
-    {url = "https://files.pythonhosted.org/packages/06/52/2e60bda73f04f66859c6b0ab2468275d0cf4519804d85d4daecc5935c142/orjson-3.9.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e44ebe2129d43c5a48f3affa3fa59c6484ed16faf5b00486add1061a95384ab0"},
-    {url = "https://files.pythonhosted.org/packages/0c/75/e41f01986e5ee56362c93ac5c92149f8fb6b6c8123c5aa5afe8a8b96746e/orjson-3.9.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:88626d898c408450c57664899831cf072787898af4847fa4466607ad2a83f454"},
-    {url = "https://files.pythonhosted.org/packages/10/1f/2915887049c72a195a7991ec8e5cf0344fcd6a940a2e50abee860752b7bf/orjson-3.9.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:9ee5f1ba82146a50d61fb58d310a37c0f406eda898172f9c98673b5d6f9461c3"},
-    {url = "https://files.pythonhosted.org/packages/15/a3/7520991c2e46ad7d9c2a9076aac4c3ca2bbe6820fc166b184f49ccbcea81/orjson-3.9.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:09522937479bd39d5bb32d11a5ecdf6926fda43ac2cbde21cc1a9508b4e4ea29"},
-    {url = "https://files.pythonhosted.org/packages/1b/4a/bb3412d18379e708311166699a4eccee9f6c1eadc756c7227246939da8a3/orjson-3.9.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:c68af71b1110820c914f9df75842895b5528ff524d3286fde57097b2b5ed8f22"},
-    {url = "https://files.pythonhosted.org/packages/2a/38/f0026e0413e3de18cbd03ad5120ed9651ed5675b5d8b3e8732a14aae765b/orjson-3.9.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f6ab80b60195f166a9d666b2eaf6d2c74202b6da2a1fb4b4d66b9cc0ce5c9957"},
-    {url = "https://files.pythonhosted.org/packages/2a/9f/e6e15918c7ef6fc38e3c009aa704937dfb31ba3916a7783eaf365b7a257f/orjson-3.9.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:2af7dff1c7ddb0c83eb5773acf6566b153f8cd32e4ba782ae9ccd6d0f324efd3"},
-    {url = "https://files.pythonhosted.org/packages/2e/ee/2b2ca51b317e975ef8fbc67b7909269c97591bc921bb5946174905b71d16/orjson-3.9.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1e3bde77c1e0061eb34bae6fea44818b2198e043ee10a16ad7b160921fee26ea"},
-    {url = "https://files.pythonhosted.org/packages/3a/d5/835fa231ae3e6811b9333522d4dbd09d02927d1e1c387820b1890c673b6e/orjson-3.9.0-cp38-cp38-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d4c2d31178e3027affd98eead033f1c406890df83a0ca2016604cc21f722a1d1"},
-    {url = "https://files.pythonhosted.org/packages/3e/b0/75635bd68fcf9dc3139e7c0f9d84dec8e0db1fcaa9d06a289c4e657edac7/orjson-3.9.0-cp38-none-win_amd64.whl", hash = "sha256:3a208d0bca609de3152eb8320d5093ad9c52979332f626c13500d1645c66bf8d"},
-    {url = "https://files.pythonhosted.org/packages/40/51/9d5dcc6c72996d6cc9192cc31aac2326d5ca388bbf6342963e7489a2897b/orjson-3.9.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:04e61db09ff155846b69d07cf5aa21001f2010ea669ec3169c1fbad9c9e40cd5"},
-    {url = "https://files.pythonhosted.org/packages/44/1e/cc7c47dcf5ce59a4b9b1fd873d3813a4bf8e3f18fbda3c402e70e07fdd87/orjson-3.9.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:45df5bf6531ffda518331cc93cdcd4c84f4a4a0507d72af8fb698c7131a440a0"},
-    {url = "https://files.pythonhosted.org/packages/45/46/baedf92b3d24ae05325441e8d04c835ebf96e154d270530c48e7cd4ca4a2/orjson-3.9.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8a1fcddcabe121e393f3c4a31ed6d3535214d42a4ece0f9dde2e250006d6a58d"},
-    {url = "https://files.pythonhosted.org/packages/46/ed/5b360740dae0de25303789d2447a4a5827a162314a376ace7112b22d83b5/orjson-3.9.0-cp37-none-win_amd64.whl", hash = "sha256:5afd22847b07b63f2b8fcfddd5b7a6f47c5aaa25e19b97a3d6d39508b8fd465a"},
-    {url = "https://files.pythonhosted.org/packages/49/a1/de519d9901d92ef086d8ddfc80d63a2ee51871887af5397ed4896cf06202/orjson-3.9.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:2536a7f30fd4d77532769ea9285cd20c69bd2b40acf980de94bbc79b1c6fad5a"},
-    {url = "https://files.pythonhosted.org/packages/56/f4/571b77ad51b91641aabef03e135792daa741939855d6e1ed4e830786f26d/orjson-3.9.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c50654e4870805e4b1a587c2c3c5ef2f36f3e67fc463a738339ff40d65f7db1"},
-    {url = "https://files.pythonhosted.org/packages/5c/ca/4d7a76381df4119c9ccfdaae1ab62004ed909f24519673118c3ad651a857/orjson-3.9.0-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:a901c432828c191332d75f358142736c433d4a192f7794123e1d30d68193de86"},
-    {url = "https://files.pythonhosted.org/packages/61/ac/1923bf83c0e36a9ac35d4c7347f715ce87b807c8692403b66047c7ac11e1/orjson-3.9.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:0e7fe5d603ee9177ff2e45858b4fc47fea2da0688f23d9773654889d56dfbc82"},
-    {url = "https://files.pythonhosted.org/packages/69/63/a0a20c4d858e23be5d7cb544d28bd513771d71bab04f20b293a06eb9ecb1/orjson-3.9.0-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:f6476e2487c0b7387187de15e5b8f6635c29b75934f2e689ca8cad6550439f3d"},
-    {url = "https://files.pythonhosted.org/packages/6f/1b/7aa9c75c7f6647c0c4b41c8a77d84d409fead13a23dc63f407ef964222fa/orjson-3.9.0-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:d414fd0678e949779104f5b307f0f9fac861728e19d3cdde66759af77f892da0"},
-    {url = "https://files.pythonhosted.org/packages/73/59/cb014160188df36c74aac8c1fcab3b4a59a0f0d070c69f65423cf1ddfca6/orjson-3.9.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c7b241c3229084035b38cac9b5c96b43644da829da41d9d5be0fefb96fb116e1"},
-    {url = "https://files.pythonhosted.org/packages/73/dc/377f4ab9875b25f79e3c46d025922045c66e2057592f473a0675091a6f6a/orjson-3.9.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:721d47dffedb7795ffea8a06f2de7d192de7b58e085cf357a99abf0eb931f2c3"},
-    {url = "https://files.pythonhosted.org/packages/87/15/f643ee5e696ab43a690c4745310553d2c3e8180c8cac59bab4e50dccd22a/orjson-3.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2fbf34667a8be48ec89d5ef479a00d4e7b3acda62d722c97377702da0c30ffd"},
-    {url = "https://files.pythonhosted.org/packages/8b/8a/59611e84d2d76f5eb23ffaa9c7c8aaa728174b5e1cb86c6a29b8418ec349/orjson-3.9.0-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:949698bdddb1daff986d73e6bbe6cd68833cd80c4adc6b69fafbd46634d4672c"},
-    {url = "https://files.pythonhosted.org/packages/8e/87/61885b10fa30cb2ed4ddf0f9149cdd295d8cf409cf78370b55a200e4db2b/orjson-3.9.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebe372e9f4e4f0335b7b4ebfab991b3734371e3d5b7f989ca3baa5da25185f4a"},
-    {url = "https://files.pythonhosted.org/packages/95/1c/be392b9e88f568a67fe546008a1d46cb955798c5bb02f11f9d0485dfa8ed/orjson-3.9.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7a3693fde44b2eeb80074ecbe8c504b25baf71e66c080af2a574193a5ba81960"},
-    {url = "https://files.pythonhosted.org/packages/a9/d0/c3341cc7d1818dc80df738e3879275a8236da26cd17823ba4a66d12d577b/orjson-3.9.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:edd77183c154cbedaa6dac32fee9cb770b04e2a7f367a5864f444578554cc946"},
-    {url = "https://files.pythonhosted.org/packages/ad/c3/bdc121a246921d0699c695eb73cf56417ab487767c4f761f9425dd1bf59c/orjson-3.9.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:108c58d2c7648c991f82f9b2217c50981ad7cf6aaee3efbfaa9d807e49cd69b8"},
-    {url = "https://files.pythonhosted.org/packages/b1/e6/6389d8ea0a3d9981f13c61be638715c8f616d1231574131081d35195b9fe/orjson-3.9.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d4fcf598bd5a99a94caa7ec92ce657939f12491e4753ea7e4d6c03faf5f7912e"},
-    {url = "https://files.pythonhosted.org/packages/b2/95/707184b9b991a58bc8f290aed0c3942f642e85c089f0228168af41e54cf3/orjson-3.9.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:271b6f1018757fc6bca40ae72e6cdb6cf84584dde2d1e5eaac30e387a13d9e72"},
-    {url = "https://files.pythonhosted.org/packages/c3/cb/683a60de5c1820412979aeca04e43cdb6c01a282edf1583bf84054d22458/orjson-3.9.0-cp311-none-win_amd64.whl", hash = "sha256:44fa74b497e608a8cdca1ee37fe3533a30f17163c7e2872ab1b854900cf0dfcf"},
-    {url = "https://files.pythonhosted.org/packages/c9/35/31348485dd1e303c5f87c2e2d3be6ae4bdfdb51c2677227190543b5a3f0b/orjson-3.9.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9de2129d40674007cb24164939e075b5b39fee768bf20801e08c0e3283bfb18e"},
-    {url = "https://files.pythonhosted.org/packages/c9/d9/0382e682322a996476ece62f92cc90cb067da3266a6a9ed71da9b49cc442/orjson-3.9.0-cp39-none-win_amd64.whl", hash = "sha256:3235c31d0fe674f6e3433e9ddfed212aa840c83a9b6ef5ae128950e2c808c303"},
-    {url = "https://files.pythonhosted.org/packages/ce/19/ae05dd3d72f8036ad4f7ab6ff5e41d4dd44e81fb62aa6a04d6c1f53d051f/orjson-3.9.0-cp310-cp310-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:128b1cd0f00a37ba64a12cceeba4e8070655d4400edd55a737513ee663c1ed5a"},
-    {url = "https://files.pythonhosted.org/packages/d5/64/9e81da69bb5dfc0a30d7ce2682f1a0aa4637a82fde9fd56e2e188f040898/orjson-3.9.0-cp311-cp311-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:47d7e4a3effc0e9314bd5b06e7431f2490a5e64dcdcbbc4d60e713786fec327d"},
-    {url = "https://files.pythonhosted.org/packages/d7/c8/a604ad0c7f0ffb5897328e0ca4a81697c2ffe1fac3f72bbaee59b12629cb/orjson-3.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:09ee828572fadcd58bf356d2c1bad99a95c7c9c1f182b407abbc7dec1810f542"},
-    {url = "https://files.pythonhosted.org/packages/df/8c/1184f03df5233823f88a1d3c5c1878f985a9958d06512d875fc9f8f5340b/orjson-3.9.0-cp310-none-win_amd64.whl", hash = "sha256:46c9733330b75c116438f555c0b971a2388b5f502e2dd4ec3bf6bacb96f82741"},
-    {url = "https://files.pythonhosted.org/packages/e3/96/fa927d1c19866b11dcfaf56d4de9d29b4ec4c14786b4a8c816cb58bb7e95/orjson-3.9.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:21f6a6fdfbc13cd715c61e9fa9daeff732df6401ab7d6a2ebad0042313a40bd1"},
-    {url = "https://files.pythonhosted.org/packages/e5/e4/b48906b617a14e8e9b4d99d5b5f470002674ba434bc10770f17511255f1f/orjson-3.9.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c41d1ef6ec308e9e3701764b3de889ed8c1c126eceaea881dd1027bffbed89fe"},
-    {url = "https://files.pythonhosted.org/packages/e8/7a/fffa0e31dde392a9116718e371e9deb27ac35b6f089644a1fd9ffdb6b3fe/orjson-3.9.0-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3f1193417b5a93deb41bcb8db27b61179b9b3e299b337b578c31f19159664da3"},
-    {url = "https://files.pythonhosted.org/packages/ea/d0/59c5a2e35724d2af65f42b05030783d356035f91ca81c3bf2dee454070fa/orjson-3.9.0-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:c4949fc1304b702197c0840882e84b86d8d5ca33c3d945cc60727bc1786c2b20"},
-    {url = "https://files.pythonhosted.org/packages/ec/2b/a2530675913d060f7ee760efcb88dd94b4d2b4bb1dedf3b09c401a0b82f9/orjson-3.9.0-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:86da00836029b2a071229c8aecab998a2f316c1bc7de10ae020d7311de3a6d0d"},
-    {url = "https://files.pythonhosted.org/packages/ee/45/47bcbad2c90b2846428bcd3a0a4623e37bb74ae3583bb96929b2e625d095/orjson-3.9.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:08cb43569198c1f5c89ecafcbfc62414f6115d894ff908d8cf8e5e24801364e6"},
-    {url = "https://files.pythonhosted.org/packages/ef/00/f3beb032641547b01c5850a4ff02bf6dbc318207c10b116d405f071321a0/orjson-3.9.0.tar.gz", hash = "sha256:f6dd27c71cd6e146795f876449a8eae74f67ae1e4e244dfc1203489103eb2d94"},
+"orjson 3.9.1" = [
+    {url = "https://files.pythonhosted.org/packages/0a/9d/19dd0d6cedcfec3355f2808dc3927b04c629e9d2eca5914a0360f1b2ada5/orjson-3.9.1-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d4b68d01a506242316a07f1d2f29fb0a8b36cee30a7c35076f1ef59dce0890c1"},
+    {url = "https://files.pythonhosted.org/packages/15/c4/3a97924d8768fa982042f1b5b7a1c8dbb161815b8545a4af9faa73b0a4d7/orjson-3.9.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:06f6ab4697fab090517f295915318763a97a12ee8186054adf21c1e6f6abbd3d"},
+    {url = "https://files.pythonhosted.org/packages/17/04/7ea9f49162e13749646d9ef296de6e20d486e68d8b487a2735115b00a356/orjson-3.9.1-cp310-none-win_amd64.whl", hash = "sha256:a4cc5d21e68af982d9a2528ac61e604f092c60eed27aef3324969c68f182ec7e"},
+    {url = "https://files.pythonhosted.org/packages/1d/0f/ad6a2ed3d5ae3d0dac2b33e4d5ab716b8edbbf63874b59ad7aced6570824/orjson-3.9.1-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:0b7ab18d55ecb1de543d452f0a5f8094b52282b916aa4097ac11a4c79f317b86"},
+    {url = "https://files.pythonhosted.org/packages/20/dc/1999b9039bd7effe26c141895068a886e7e69aebd9e55153517f9231e309/orjson-3.9.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:393d0697d1dfa18d27d193e980c04fdfb672c87f7765b87952f550521e21b627"},
+    {url = "https://files.pythonhosted.org/packages/2a/48/6ff75751042bf7fb716752d3705e02d7d012ab8f6af14faff841cba6aa3e/orjson-3.9.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:31229f9d0b8dc2ef7ee7e4393f2e4433a28e16582d4b25afbfccc9d68dc768f8"},
+    {url = "https://files.pythonhosted.org/packages/2e/0a/20e91274d3f07206e94431b5b1c095606131c81c566b1f55045f89ac1798/orjson-3.9.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:103952c21575b9805803c98add2eaecd005580a1e746292ed2ec0d76dd3b9746"},
+    {url = "https://files.pythonhosted.org/packages/2e/12/094e0bd8d80ae47c464832126086b5fba8ef276259102e6847db330047ee/orjson-3.9.1-cp39-none-win_amd64.whl", hash = "sha256:48a27da6c7306965846565cc385611d03382bbd84120008653aa2f6741e2105d"},
+    {url = "https://files.pythonhosted.org/packages/2f/b9/b0f154c70f4bec80efb6b9f4e056764c81300df7996ffbb280125b389f52/orjson-3.9.1-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:375d65f002e686212aac42680aed044872c45ee4bc656cf63d4a215137a6124a"},
+    {url = "https://files.pythonhosted.org/packages/35/05/9b95801d68159ec924d415144e38bf26d9eb9dafa4ae5a2c0bf0800fdfc4/orjson-3.9.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:e186ae76b0d97c505500664193ddf508c13c1e675d9b25f1f4414a7606100da6"},
+    {url = "https://files.pythonhosted.org/packages/3c/1c/4d00e6645a9e11cd3368418cb8d1c4e44004a83c7a5f9e2601a108fdd8bf/orjson-3.9.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:20f2804b5a1dbd3609c086041bd243519224d47716efd7429db6c03ed28b7cc3"},
+    {url = "https://files.pythonhosted.org/packages/43/e6/21a8e4701aa5cb00ca70c9b2e10080ca7d52c83ee918ad8f2476ae092cbb/orjson-3.9.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8515867713301fa065c58ec4c9053ba1a22c35113ab4acad555317b8fd802e50"},
+    {url = "https://files.pythonhosted.org/packages/48/6d/6c34e7fdaab79baee85ccd102ef3b11a11d7391b2171fba5586b84d39dde/orjson-3.9.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5d1dbf36db7240c61eec98c8d21545d671bce70be0730deb2c0d772e06b71af3"},
+    {url = "https://files.pythonhosted.org/packages/48/87/f2ba953e8f0c2a0067e811d36773a4595d452a3c0e62d855f77b672d17ae/orjson-3.9.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:46b4facc32643b2689dfc292c0c463985dac4b6ab504799cf51fc3c6959ed668"},
+    {url = "https://files.pythonhosted.org/packages/4c/8d/feb2b29389ec30cf4c694dfd77867e4e5455f5a928f6f5aba2df13df7ed8/orjson-3.9.1-cp38-none-win_amd64.whl", hash = "sha256:402f9d3edfec4560a98880224ec10eba4c5f7b4791e4bc0d4f4d8df5faf2a006"},
+    {url = "https://files.pythonhosted.org/packages/53/6c/760381c99d4a6d43bb18b804fe7e269cc79d5d1cbc1633c6957ff8428e1e/orjson-3.9.1-cp38-cp38-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d1c2b0b4246c992ce2529fc610a446b945f1429445ece1c1f826a234c829a918"},
+    {url = "https://files.pythonhosted.org/packages/54/82/cff82768761a17b169232ae5e783facb0fc52eadb7edda4d287eeba46c19/orjson-3.9.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:24d4ddaa2876e657c0fd32902b5c451fd2afc35159d66a58da7837357044b8c2"},
+    {url = "https://files.pythonhosted.org/packages/55/75/bde3d235e979ac7f91e65ab9566ea8655844a9ee90f145ba2eaeb3dcfc92/orjson-3.9.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:d3a40b0fbe06ccd4d6a99e523d20b47985655bcada8d1eba485b1b32a43e4904"},
+    {url = "https://files.pythonhosted.org/packages/55/d1/03769e06ac4b76cdf2caf33cb6097f690f621c9903d772b5c11abcdc2bbf/orjson-3.9.1-cp310-cp310-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:c4434b7b786fdc394b95d029fb99949d7c2b05bbd4bf5cb5e3906be96ffeee3b"},
+    {url = "https://files.pythonhosted.org/packages/56/fc/947a5ea8d5d53dba23e935429b26fcd93be4d0c43b6b6af4e8fcc27b99ed/orjson-3.9.1-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d8ae0467d01eb1e4bcffef4486d964bfd1c2e608103e75f7074ed34be5df48cc"},
+    {url = "https://files.pythonhosted.org/packages/5c/e2/f3e3139a6bd056d4f8047a2ad56aba2cd21b7affe2b99a18b5e5ca5476b6/orjson-3.9.1-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f9a744e212d4780ecd67f4b6b128b2e727bee1df03e7059cddb2dfe1083e7dc4"},
+    {url = "https://files.pythonhosted.org/packages/68/56/ac71a3dea1b31cc9aa1256399288b82c3b4e0defffa257a745cb7a34a5ba/orjson-3.9.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:78d9a2a4b2302d5ebc3695498ebc305c3568e5ad4f3501eb30a6405a32d8af22"},
+    {url = "https://files.pythonhosted.org/packages/69/c4/f586ace6b08a0ddc0d6a79d1f7ee3deb5c3d72271167a0bc24747b619089/orjson-3.9.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ec7c8a0f1bf35da0d5fd14f8956f3b82a9a6918a3c6963d718dfd414d6d3b604"},
+    {url = "https://files.pythonhosted.org/packages/70/38/d7c2520e4046f129bebfda2d27cfa7c98125ca99938401f3ff6172c61204/orjson-3.9.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:15d28872fb055bf17ffca913826e618af61b2f689d2b170f72ecae1a86f80d52"},
+    {url = "https://files.pythonhosted.org/packages/7b/5f/cd8154d6d91a5ea94404ac07b7e536f2f72556a97aed1c6264d565826989/orjson-3.9.1-cp37-none-win_amd64.whl", hash = "sha256:6d173d3921dd58a068c88ec22baea7dbc87a137411501618b1292a9d6252318e"},
+    {url = "https://files.pythonhosted.org/packages/7d/ab/9a3c48034cefe21682b7b45b6e651ce1364d5109382477a89b54099074cf/orjson-3.9.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:125f63e56d38393daa0a1a6dc6fedefca16c538614b66ea5997c3bd3af35ef26"},
+    {url = "https://files.pythonhosted.org/packages/8d/3c/2cca0f380a55a2025c4fab460e4e6662a490301866f85967567aa0a4c631/orjson-3.9.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ae47ef8c0fe89c4677db7e9e1fb2093ca6e66c3acbee5442d84d74e727edad5e"},
+    {url = "https://files.pythonhosted.org/packages/8d/65/2b4a7580a92ca57fcb698112c26c4c59861c110b61767646fa326dd6a4b7/orjson-3.9.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:09faf14f74ed47e773fa56833be118e04aa534956f661eb491522970b7478e3b"},
+    {url = "https://files.pythonhosted.org/packages/8e/58/2f181db661502ba1d49b2ffda58e9fd0520d83795975859bc548f1242caf/orjson-3.9.1.tar.gz", hash = "sha256:db373a25ec4a4fccf8186f9a72a1b3442837e40807a736a815ab42481e83b7d0"},
+    {url = "https://files.pythonhosted.org/packages/95/a0/9c0eeba11b179e0b66cc6b0262c2959c286d2cecbefe96ef1850d73f4148/orjson-3.9.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:2cb0121e6f2c9da3eddf049b99b95fef0adf8480ea7cb544ce858706cdf916eb"},
+    {url = "https://files.pythonhosted.org/packages/9d/5d/428f202649e92574d542df23991ddefbfe333e37742cab49208e6737a153/orjson-3.9.1-cp39-cp39-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:49c0d78dcd34626e2e934f1192d7c052b94e0ecadc5f386fd2bda6d2e03dadf5"},
+    {url = "https://files.pythonhosted.org/packages/a5/a2/66d0f3573c94cb7ff373d2d319feeb2f1214a583430ba955c26cc8da0c3d/orjson-3.9.1-cp311-none-win_amd64.whl", hash = "sha256:0b53b5f72cf536dd8aa4fc4c95e7e09a7adb119f8ff8ee6cc60f735d7740ad6a"},
+    {url = "https://files.pythonhosted.org/packages/a9/b0/c32fee7aa0c7b24b344a7a9a8301fd6a4196a62d34ada133232124941204/orjson-3.9.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:db774344c39041f4801c7dfe03483df9203cbd6c84e601a65908e5552228dd25"},
+    {url = "https://files.pythonhosted.org/packages/ac/a3/59a94065eb40abf5295dc74ba5c64b7803b82fcd930a8f820c4c582e03f6/orjson-3.9.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d96747662d3666f79119e5d28c124e7d356c7dc195cd4b09faea4031c9079dc9"},
+    {url = "https://files.pythonhosted.org/packages/b9/f7/c9f4a585eb89ab971285b221fc27fe1a14b962ca140bda78687df92cdc09/orjson-3.9.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:80a1e384626f76b66df615f7bb622a79a25c166d08c5d2151ffd41f24c4cc104"},
+    {url = "https://files.pythonhosted.org/packages/bb/03/adade19312afe58fcda4242d1288d891cbd37979a73bc9f4df304fa42b65/orjson-3.9.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0fd828e0656615a711c4cc4da70f3cac142e66a6703ba876c20156a14e28e3fa"},
+    {url = "https://files.pythonhosted.org/packages/c1/0b/c72305cf80577f20ab2a6ecc7801e7479f4a4bde9ef8b10b314fdaa796d9/orjson-3.9.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:19f70ba1f441e1c4bb1a581f0baa092e8b3e3ce5b2aac2e1e090f0ac097966da"},
+    {url = "https://files.pythonhosted.org/packages/c5/09/836f32cc0a3c13e18ec3487957989387b60f9e7cfbe920773ad4b329db55/orjson-3.9.1-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:503eb86a8d53a187fe66aa80c69295a3ca35475804da89a9547e4fce5f803822"},
+    {url = "https://files.pythonhosted.org/packages/d5/b8/abf74e95f7fd5b868fcc1e7e1c77720ddd9c5b18e8d0edb9250579356942/orjson-3.9.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ec53d648176f873203b9c700a0abacab33ca1ab595066e9d616f98cdc56f4434"},
+    {url = "https://files.pythonhosted.org/packages/e3/1f/66215d4a849722a15ae17def93d66af0e4081297454915bf6097fc8e017b/orjson-3.9.1-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:4751cee4a7b1daeacb90a7f5adf2170ccab893c3ab7c5cea58b45a13f89b30b3"},
+    {url = "https://files.pythonhosted.org/packages/e3/fb/e86b9fecd26ca0aedcb9d1baa66bf7563cc6b4b2b8511f3d27c57073386d/orjson-3.9.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:1e4d905338f9ef32c67566929dfbfbb23cc80287af8a2c38930fb0eda3d40b76"},
+    {url = "https://files.pythonhosted.org/packages/e8/32/b4fef2c0561dc163df7dc389ba667f56758d7f3140fc6d1dea9d6962c348/orjson-3.9.1-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:9e20bca5e13041e31ceba7a09bf142e6d63c8a7467f5a9c974f8c13377c75af2"},
+    {url = "https://files.pythonhosted.org/packages/ec/08/95c96389c6b7f09bb033c5f37671a7dabae5d890a50e6167cfd6bb0d390b/orjson-3.9.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d4edee78503016f4df30aeede0d999b3cb11fb56f47e9db0e487bce0aaca9285"},
+    {url = "https://files.pythonhosted.org/packages/fa/1b/7847871e1cc8497a89691251dff6d79e890e79104b2231d4ca7d75f0f25e/orjson-3.9.1-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:08927970365d2e1f3ce4894f9ff928a7b865d53f26768f1bbdd85dd4fee3e966"},
+    {url = "https://files.pythonhosted.org/packages/fa/60/46d78e622a238ce13f1055b9ec85eb82951b02098f28d94eb7d87f76f3f1/orjson-3.9.1-cp311-cp311-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:761b6efd33c49de20dd73ce64cc59da62c0dab10aa6015f582680e0663cc792c"},
+    {url = "https://files.pythonhosted.org/packages/ff/0c/48c3e15025e044f732699b2e732025734ec5e38806b7d73f690db348fa93/orjson-3.9.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d9dd4abe6c6fd352f00f4246d85228f6a9847d0cc14f4d54ee553718c225388f"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandas 2.0.2" = [
     {url = "https://files.pythonhosted.org/packages/07/66/a1c77bc7af5358f4404e47a28a0f16d624fffa20ed35ba189d03872023b8/pandas-2.0.2-cp38-cp38-win32.whl", hash = "sha256:6d6d10c2142d11d40d6e6c0a190b1f89f525bcf85564707e31b0a39e3b398e08"},
@@ -2519,17 +2519,17 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.5.1" = [
-    {url = "https://files.pythonhosted.org/packages/89/7e/c6ff9ddcf93b9b36c90d88111c4db354afab7f9a58c7ac3257fa717f1268/platformdirs-3.5.1-py3-none-any.whl", hash = "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"},
-    {url = "https://files.pythonhosted.org/packages/9c/0e/ae9ef1049d4b5697e79250c4b2e72796e4152228e67733389868229c92bb/platformdirs-3.5.1.tar.gz", hash = "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f"},
+"platformdirs 3.5.3" = [
+    {url = "https://files.pythonhosted.org/packages/6d/1a/96efea7b36835ce89911d7813fe68f5b1db7ecae4023bf209a7aeba93017/platformdirs-3.5.3-py3-none-any.whl", hash = "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed"},
+    {url = "https://files.pythonhosted.org/packages/d2/5d/29eed8861e07378ef46e956650615a9677f8f48df7911674f923236ced2b/platformdirs-3.5.3.tar.gz", hash = "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
@@ -2775,17 +2775,17 @@
 "pysrt 1.1.2" = [
     {url = "https://files.pythonhosted.org/packages/31/1a/0d858da1c6622dcf16011235a2639b0a01a49cecf812f8ab03308ab4de37/pysrt-1.1.2.tar.gz", hash = "sha256:b4f844ba33e4e7743e9db746492f3a193dc0bc112b153914698e7c1cdeb9b0b9"},
 ]
 "pysubs2 1.6.1" = [
     {url = "https://files.pythonhosted.org/packages/22/3e/fb1b08a06144ba63f19cc4758dd72e2eb8c7fc95c6c8364faccfc570c7bf/pysubs2-1.6.1.tar.gz", hash = "sha256:0261611e71735ff7763972c519c72593c8063efcb9039c54af65f31b81cec116"},
     {url = "https://files.pythonhosted.org/packages/4f/dc/dc1763a3abab92af2253b1abb3dd48e07b2a3613d7ae64a3ab5c27da3019/pysubs2-1.6.1-py3-none-any.whl", hash = "sha256:1f96d9dfb5f859a54a00e04621beb20ff21ea1d788821b2f4935c5c0ef8dc68e"},
 ]
-"pytest 7.3.1" = [
-    {url = "https://files.pythonhosted.org/packages/1b/d1/72df649a705af1e3a09ffe14b0c7d3be1fd730da6b98beb4a2ed26b8a023/pytest-7.3.1-py3-none-any.whl", hash = "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362"},
-    {url = "https://files.pythonhosted.org/packages/ec/d9/36b65598f3d19d0a14d13dc87ad5fa42869ae53bb7471f619a30eaabc4bf/pytest-7.3.1.tar.gz", hash = "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"},
+"pytest 7.3.2" = [
+    {url = "https://files.pythonhosted.org/packages/58/2a/07c65fdc40846ecb8a9dcda2c38fcb5a06a3e39d08d4a4960916431951cb/pytest-7.3.2.tar.gz", hash = "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"},
+    {url = "https://files.pythonhosted.org/packages/7a/d0/de969198293cdea22b3a6fb99a99aeeddb7b3827f0823b33c5dc0734bbe5/pytest-7.3.2-py3-none-any.whl", hash = "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295"},
 ]
 "python-dateutil 2.8.2" = [
     {url = "https://files.pythonhosted.org/packages/36/7a/87837f39d0296e723bb9b62bbb257d0355c7f6128853c78955f57342a56d/python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
     {url = "https://files.pythonhosted.org/packages/4c/c4/13b4776ea2d76c115c1d1b84579f3764ee6d57204f6be27119f13a61d0a9/python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
 ]
 "python-mpv-jsonipc 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/6f/65/232563752a049831fdd6ae7b4caf8a557529d2f3c72ecbc40fb8b69e372c/python-mpv-jsonipc-1.2.0.tar.gz", hash = "sha256:2199beefa6643d16483dda17c976bf2bbbf5dfedb1a5ca8d7d4611527ae6ad7a"},
@@ -2896,17 +2896,17 @@
     {url = "https://files.pythonhosted.org/packages/f8/bc/01e6a5597904147d13c1a6dc16ec334b73cddb190b6b8f05fca2c0bfbe89/regex-2023.6.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:9edcbad1f8a407e450fbac88d89e04e0b99a08473f666a3f3de0fd292badb6aa"},
     {url = "https://files.pythonhosted.org/packages/f9/a5/703d590158a252b3e96332d7a420669b0395b7b98a2b34395af1f4f8f95f/regex-2023.6.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0b49c764f88a79160fa64f9a7b425620e87c9f46095ef9c9920542ab2495c8bc"},
 ]
 "requests 2.24.0" = [
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
-"rich 13.4.1" = [
-    {url = "https://files.pythonhosted.org/packages/02/97/0046b5e3c6a5057b5817e5e6c51a776d410b953e6a9c67ae249dafdd2999/rich-13.4.1.tar.gz", hash = "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1"},
-    {url = "https://files.pythonhosted.org/packages/ea/93/c68645c689d10a035010e3ae314b6b2855d040ce0d11fdfdfbb8be416581/rich-13.4.1-py3-none-any.whl", hash = "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"},
+"rich 13.4.2" = [
+    {url = "https://files.pythonhosted.org/packages/e3/12/67d0098eb77005f5e068de639e6f4cfb8f24e6fcb0fd2037df0e1d538fee/rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
+    {url = "https://files.pythonhosted.org/packages/fc/1e/482e5eec0b89b593e81d78f819a9412849814e22225842b598908e7ac560/rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
 ]
 "ruff 0.0.272" = [
     {url = "https://files.pythonhosted.org/packages/1f/12/1b0b513ccf7a0ea19430843bf3a82b51704a1c8001900ca99066b69270ec/ruff-0.0.272-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:691d72a00a99707a4e0b2846690961157aef7b17b6b884f6b4420a9f25cd39b5"},
     {url = "https://files.pythonhosted.org/packages/2e/96/1a4b3b9c658bf2a04ba7820aefa24d8561f73379bf0d79c2f01321c4dd84/ruff-0.0.272-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:d5a208f8ef0e51d4746930589f54f9f92f84bb69a7d15b1de34ce80a7681bc00"},
     {url = "https://files.pythonhosted.org/packages/48/cb/2e8b7d690eec62a16971f15ca018248bc9058fb2d6abf0588f1fcc9fafb4/ruff-0.0.272-py3-none-win_arm64.whl", hash = "sha256:06b8ee4eb8711ab119db51028dd9f5384b44728c23586424fd6e241a5b9c4a3b"},
     {url = "https://files.pythonhosted.org/packages/4a/8f/66590b978ceeb3d62eee4f46eeabff4a4967cde81c05e9d4e8a28ca18f7d/ruff-0.0.272-py3-none-win_amd64.whl", hash = "sha256:a37ec80e238ead2969b746d7d1b6b0d31aa799498e9ba4281ab505b93e1f4b28"},
     {url = "https://files.pythonhosted.org/packages/4b/f8/50874f1992355a8c565bc6322659abf7cc86ce2e929ea4930d14768a022b/ruff-0.0.272-py3-none-musllinux_1_2_i686.whl", hash = "sha256:19643d448f76b1eb8a764719072e9c885968971bfba872e14e7257e08bc2f2b7"},
@@ -3143,17 +3143,17 @@
     {url = "https://files.pythonhosted.org/packages/3e/09/bbd7e880b56e825d5859a58adb1bd1feb45b604218706057ca1e3278fa62/wasabi-1.1.2.tar.gz", hash = "sha256:1aaef3aceaa32edb9c91330d29d3936c0c39fdb965743549c173cb54b16c30b5"},
     {url = "https://files.pythonhosted.org/packages/8f/69/26cbf0bad11703241cb84d5324d868097f7a8faf2f1888354dac8883f3fc/wasabi-1.1.2-py3-none-any.whl", hash = "sha256:0a3f933c4bf0ed3f93071132c1b87549733256d6c8de6473c5f7ed2e171b5cf9"},
 ]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
-"websocket-client 1.5.2" = [
-    {url = "https://files.pythonhosted.org/packages/3f/f2/2624e12ef854ee667d92ac5dc7815932095e0852e5ff2b2bf57feda8a11b/websocket-client-1.5.2.tar.gz", hash = "sha256:c7d67c13b928645f259d9b847ab5b57fd2d127213ca41ebd880de1f553b7c23b"},
-    {url = "https://files.pythonhosted.org/packages/86/5c/2ebfbb7d4dbb7f35a1f70c40d003f7844d78945ac7c69757067ebaea9c78/websocket_client-1.5.2-py3-none-any.whl", hash = "sha256:f8c64e28cd700e7ba1f04350d66422b6833b82a796b525a51e740b8cc8dab4b1"},
+"websocket-client 1.5.3" = [
+    {url = "https://files.pythonhosted.org/packages/98/be/1aa255e5b937e62ca81b6d990e372bc013e355bd8048b8579eefe24ad57d/websocket-client-1.5.3.tar.gz", hash = "sha256:b96f3bce3e54e3486ebe6504bc22bd4c140392bd2eb71764db29be8f2639aa65"},
+    {url = "https://files.pythonhosted.org/packages/c6/12/76e939a8b7757eb7675d5b8996e07733a180161397ed0904c16128721e40/websocket_client-1.5.3-py3-none-any.whl", hash = "sha256:3566f8467cd350874c4913816355642a4942f6c1ed1e9406e3d42fae6d6c072a"},
 ]
 "websockets 11.0.3" = [
     {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
     {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
     {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
     {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
     {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
@@ -3315,62 +3315,62 @@
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
 "yt-dlp 2023.3.4" = [
     {url = "https://files.pythonhosted.org/packages/a7/df/498c57f641e9993376cf52489047158e6d660e8bab06b72c470ad5cce2bd/yt_dlp-2023.3.4-py2.py3-none-any.whl", hash = "sha256:40ca421407ce07c8fd700854fd978d58526ec6fff3468caa34ff1c7333b8dc34"},
     {url = "https://files.pythonhosted.org/packages/e8/4a/1e01f24fcb49191626e2b17d00e13a093315d03a9da09fccb1c75913e420/yt-dlp-2023.3.4.tar.gz", hash = "sha256:265d5da97a76c15d7d9a4088a67b78acd5dcf6f8cfd8257c52f581ff996ff515"},
 ]
-"zeroconf 0.64.1" = [
-    {url = "https://files.pythonhosted.org/packages/00/d8/f458e724741859bbd95b28c37bf3f35ad3c1400fc33795a330922eb4bb2d/zeroconf-0.64.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5f6f15be681889bbdcd2ef98ddd9753f5d158bf45a3d29708cefd84a5b704f7e"},
-    {url = "https://files.pythonhosted.org/packages/1d/a9/68534a61caea8345ff7358e24f99732d44fbefba9bb01af731dc375a4c03/zeroconf-0.64.1-cp311-cp311-win_amd64.whl", hash = "sha256:f13d20fccda4a8e0d1f654336f0163b3a64e6ce111573245d88e15e4598fddc1"},
-    {url = "https://files.pythonhosted.org/packages/21/06/3d9381e80714da1ba2f6887708c0dfe8c6903ee4b3509249704d78478d0a/zeroconf-0.64.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:1698e085ea350772dd0cf828888bf83d3f25ae94f213fff31a01c77f498511b0"},
-    {url = "https://files.pythonhosted.org/packages/31/8f/ce3402ec68b11429880a1dc840ea5f3c0792268350db248996be4d8e92bb/zeroconf-0.64.1-cp38-cp38-win32.whl", hash = "sha256:23c37b785a5141bf392f809fd7f21267f57458042081c76b3fcf5a1305890dff"},
-    {url = "https://files.pythonhosted.org/packages/37/88/fac09749a3d98016237c914d1d002d33c04e7788f087e3992e94e4c86d28/zeroconf-0.64.1-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:3e3da076095a575bdecd2e0fa03294d0ae243d20de8aa40d352ce98fa403b866"},
-    {url = "https://files.pythonhosted.org/packages/3d/53/26b929bed81f50597bb3b8abedad6bef2b98d7b59107c2276bee66ab0099/zeroconf-0.64.1-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:4cf58733440a17d92190c0b70b71f4a8920559d1c83fcf340415689eb2eec510"},
-    {url = "https://files.pythonhosted.org/packages/44/54/2c725573d61839ec17646ff62931a2f10249dc02bf52236d7c4f1784b7e7/zeroconf-0.64.1-cp310-cp310-win_amd64.whl", hash = "sha256:8daa679bdb0ccc2747127dbfc38b74988229236bab12dc3ee8d8a4d2411070d6"},
-    {url = "https://files.pythonhosted.org/packages/47/be/a15556a8b80a34b92f386cf36f388cd9ca30489a7466a5c658d3813aba0f/zeroconf-0.64.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8619e5d0873a27a86bb3739a6b2d30dc4ede35b04814aee7896fe3006f8dbceb"},
-    {url = "https://files.pythonhosted.org/packages/4a/2e/fafb26b35c0c51173ee28ce448db77553df064447895e7858b105fcebac8/zeroconf-0.64.1-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:c6eebc50f8428b16739ac410352c9b80e87587bdd741937055f7ef0860e57623"},
-    {url = "https://files.pythonhosted.org/packages/4b/c8/64f2f42b95ff8cdc020ed2fd8326d60100bd45b21746b3909eac213ce957/zeroconf-0.64.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:718d5c5cbdecffad3ad4c8aee0f0982752bbfd070e0a3f001780840340551d2f"},
-    {url = "https://files.pythonhosted.org/packages/4e/95/e0af3ec7f96265b580199925a10e148c08e5200fea1e1857eaa6257c393e/zeroconf-0.64.1-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:10f6ec14b6c48faf770dc9ebf081659595ed333a9c539acf520c3d898feaeae5"},
-    {url = "https://files.pythonhosted.org/packages/51/31/02a544c2ecf466a992ae620f297eb958b2404f6aaa365a37fe8c796fc80d/zeroconf-0.64.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b076156e6ea1e4888b019690c60fce96cba967c8fcb28c8bf6d0cc3dc66b600f"},
-    {url = "https://files.pythonhosted.org/packages/53/4e/c16299bc06adca837091538d424303fe3b37ce7322fa61e5d3f102adc66e/zeroconf-0.64.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d58730a1a3ea97e9bd84cda310637eb8eebec76d218e69b13226abb73fe71dbb"},
-    {url = "https://files.pythonhosted.org/packages/59/06/08d2f0139c8993262086babf63367bf721a1f217f90c9229ca98b21e9b1a/zeroconf-0.64.1-cp39-cp39-win_amd64.whl", hash = "sha256:b0b837a2a44d074a859255bf090acd6de2d381994d6b69b873356bdfc1e07f49"},
-    {url = "https://files.pythonhosted.org/packages/6b/1e/75047ca027e5b04ea15f39a573d577fe972f5e639a951f4708a076d34ba9/zeroconf-0.64.1-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:4dc87631691c2c3c0b812c25dfabc78dec903029875216d567e86f08fa7d2c5b"},
-    {url = "https://files.pythonhosted.org/packages/6c/77/b43efbfaa87afa5d72dc6c37c99d309e57015fd8af19e36a527d7cdbd7ed/zeroconf-0.64.1-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:8b7118535d151e604f980c1836a78d6229f10c0c672baeda6e686c512baed8b0"},
-    {url = "https://files.pythonhosted.org/packages/70/b1/304b7bf1db4d8a7cd9a551e3e71091a20300970bd641cfab4e87f0a91a61/zeroconf-0.64.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e8044365e0158d5d0d86c0bcec7e36aa1d8bae0ac639714816352175710230e1"},
-    {url = "https://files.pythonhosted.org/packages/72/36/66a0d78f683e33359802c7ade25fe1623c24a6aaf1ae6d528bf3f2e50d36/zeroconf-0.64.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:5844ae653dc8a96250a91bb6b067ede254ff54af26d9a829ce7c49926679bea0"},
-    {url = "https://files.pythonhosted.org/packages/77/30/c1d765594c551675fa777481727b2b5efb221df97e2a91500541849aabdb/zeroconf-0.64.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:96e4f9fa87ab46c392143aa64cd318ac200c709c66f04556ed3af5783543d415"},
-    {url = "https://files.pythonhosted.org/packages/77/81/dba620d9381a18c2d63c948534f8a45450a09514a83744b7e54afbc9a8e2/zeroconf-0.64.1-cp37-cp37m-win32.whl", hash = "sha256:0c67d13fa459b4e1a660456a3db5fcf43501be5743392f20c75e950dbb036aeb"},
-    {url = "https://files.pythonhosted.org/packages/7a/42/135f53a02178424313168a07d5a520215a78ed13673b11314b5c17fb2a7f/zeroconf-0.64.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4e492f4104879a80fb4320f0577d18982b9deb9333360ff056f823551e1a951d"},
-    {url = "https://files.pythonhosted.org/packages/7a/8e/79223c855c4abf13a5aa7b7ecbf53bf3e504d77abae202488e52b12fcceb/zeroconf-0.64.1.tar.gz", hash = "sha256:e90b2d5d247474b6ccf49bc7e02de516cc459efca6e3ac052b48eeb4a11985af"},
-    {url = "https://files.pythonhosted.org/packages/7e/f0/a09a29b336e9270eff923a457ad87891929503c4b70e5977c5845faba83e/zeroconf-0.64.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:13d18b7a583fe3b1c7825eba4a0c540bc1bcbd9b07763e14b5b684fa4c7bd911"},
-    {url = "https://files.pythonhosted.org/packages/85/02/ad7ed46298e39152dc9b0ddc31a22397db6f5f3b6997224122f8ce87778d/zeroconf-0.64.1-cp38-cp38-win_amd64.whl", hash = "sha256:4eea37ef58a914e0e16f3048011faf137b103ed5f97afa990a166ca91d3c3285"},
-    {url = "https://files.pythonhosted.org/packages/87/85/84b30557b9d62e59ff6e26f6729a686f48882e81fca537b7d2ed53cc727d/zeroconf-0.64.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:c7142fc4a77c58edbd772a73dcd4ce6ac9c5545ea93cf8fb303714e32070544e"},
-    {url = "https://files.pythonhosted.org/packages/8f/e3/e1792a57482e337b2515a9dcba94a44741e4624edf97aa3a79e62cbb1718/zeroconf-0.64.1-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:8eff98ff2f83aaa01d8ada4bf0efa3286b15739f8308cf85fbffbb9f177f10a4"},
-    {url = "https://files.pythonhosted.org/packages/94/41/fedf65eb4802c98ab75644344f2b8b722b04d237754667a391a2909e0d73/zeroconf-0.64.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7a31eba6720e0b58188c66e4b70879bb45b11c41092acbbfd265fe192b428c0c"},
-    {url = "https://files.pythonhosted.org/packages/99/7b/385ec5a78f1c6f6baa23114c09790049be7fce5abcfce5df88af9b2d26ef/zeroconf-0.64.1-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:573d1fe384be94dabe58610bdca3200f9c3505a513d379cf802367d4196a386b"},
-    {url = "https://files.pythonhosted.org/packages/9b/94/bc42ba7bfbe3b83b64b64abe863e2e48948bb5c1f42c29675d7e1d6802a5/zeroconf-0.64.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:0a7732a7a6b0b32c8132b7ab2216d492bcb5291bbc6dc3a5afdefe0bc6dbfef5"},
-    {url = "https://files.pythonhosted.org/packages/9f/37/63a17631cbc3cd20ccc563b72c245260e178aa77b47aacce48ba65cafbc5/zeroconf-0.64.1-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:d6bbfb5c297d29e0a3c0ee5a64018001c5e66ea058435197a58edbe73455f4af"},
-    {url = "https://files.pythonhosted.org/packages/a0/7e/07eb46301a8860dde7db6a7be13ebf56e9b3a533e442862d85f6c5013cd6/zeroconf-0.64.1-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:9f8ebbff504bad200275167bfd496a1e1348138f8e92d5d2bd67b650b9677336"},
-    {url = "https://files.pythonhosted.org/packages/a5/54/3ae0de65d5fdb0fa97625c19667d5f02412d3a009b05bc8c4b732a5fc364/zeroconf-0.64.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8dd1f353da75c3a5aef03654826caa3cfed244d1a13675ac6d52816f69d62427"},
-    {url = "https://files.pythonhosted.org/packages/a5/7d/719e02d5b0fd1f8b512685904b12d252c2b05f320e5509b8e5603d6ac0ae/zeroconf-0.64.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:88314f29df7bf568a085decc15c7b60b1b228f646b8e1ffa0ae3c418f8cd28d0"},
-    {url = "https://files.pythonhosted.org/packages/a6/ec/73462bce7b7e8d4c20b0a571bdcc762a32810c696084e87af64775ff5566/zeroconf-0.64.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a74ccda6490bf44ee776850d16df8680a908884c41d800095ca7e716a0e75502"},
-    {url = "https://files.pythonhosted.org/packages/b3/c6/22ee7eeff35e06151162f77c7fe4b506cda1c530742dbdb573e7b331b942/zeroconf-0.64.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:e722131b9fe9e74d5682bc146d5271677154c1af3b45638bf9880d04d9edb869"},
-    {url = "https://files.pythonhosted.org/packages/b5/e4/077c0d84cb7afc28cc70299a74208a698010a1d358bca0661736bb2ad631/zeroconf-0.64.1-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:f5a9766743eac52f91e6dc2d4ac5e7f8f25466f58c0ef51f01f3461920911fdf"},
-    {url = "https://files.pythonhosted.org/packages/b6/cf/1f82d2a6ae12f3d1518318438e74e2973db40a32979c68d440c3e810d774/zeroconf-0.64.1-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:f4551b21aaa42061ffc69af1c32e79775665ac32f662f20f6ee2a7c4db83af6b"},
-    {url = "https://files.pythonhosted.org/packages/c0/86/d49cb22e79a8077dd363f1a3871dc0e14365910fc856f614d887c189a5fd/zeroconf-0.64.1-cp37-cp37m-win_amd64.whl", hash = "sha256:0de5eeeeda68056ba6cab252a1946f67d0aaa950215aa59e5840171561b41f7d"},
-    {url = "https://files.pythonhosted.org/packages/c2/06/7046b7408a6df0f38f7402a34cdd90542a726463a630c7743f7866ad617d/zeroconf-0.64.1-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:06c07e578963fb4448bd1759f241b3ce2cd6062974a1ed8c438bc86f01aed61e"},
-    {url = "https://files.pythonhosted.org/packages/cb/4a/6bc84fdb60aebc9fba701b2c2fe2938fe99682c715001c6b7833b7ec38bf/zeroconf-0.64.1-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:60bdb7a2baa54907854b7d64f71e4da3bedae4a630de576a71a740acaba29957"},
-    {url = "https://files.pythonhosted.org/packages/ce/03/55744d3954d6b7da2b5ae628db1384090f3a27fccfb15fbdfd4b957500f6/zeroconf-0.64.1-cp310-cp310-win32.whl", hash = "sha256:97fbe8c6846b3bc4f4d24c0794fcda05c7e916e91acddae0075500857d5809f5"},
-    {url = "https://files.pythonhosted.org/packages/d3/d2/05f8232bff9d26bdd72ef7f24947e96019d65d909bf7c43c1a61c81f43c0/zeroconf-0.64.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:e9abee5ef2cdd56c866646540c1b75113bb88db16e4860f8abc85aade136fd24"},
-    {url = "https://files.pythonhosted.org/packages/d8/19/e9d5c03cc14a2cc70bb0aa98f2cdc7baa4c496f274e0091eb4d80de52fb1/zeroconf-0.64.1-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:76ef331202523598d6b197a6459551e1d7aaef9f5d60fc1014dc2e23a1a4dde5"},
-    {url = "https://files.pythonhosted.org/packages/dc/3b/e7dbc3ca10f05d0f60d4879282eafd651f252f9ba3ed4a8ed2d921a6c198/zeroconf-0.64.1-cp39-cp39-win32.whl", hash = "sha256:7b5b56df376a74c56d5f3cbaf0f988cfdd86828ac049c81d29aadf4e563eb2f8"},
-    {url = "https://files.pythonhosted.org/packages/e2/73/576a008aed4db514e22709eab6ada3b27ba2092af40d64b13d3d61a40289/zeroconf-0.64.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:66275596a39bb55b0a3d10ee0213080d8087b4dabe500e4fdb851f4eb3c5a597"},
-    {url = "https://files.pythonhosted.org/packages/ed/87/58648e72a28f196a3790520555a8b0ad9fac352f9b0acbf200bc9786ef77/zeroconf-0.64.1-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:1a09997044cf3dd5f24d11b8f17b41a59ee8d04d5cec5b040bd8a3e7b8c86f35"},
-    {url = "https://files.pythonhosted.org/packages/f5/16/94ce16f23aafdab975b9d90f56c9b614800dddc5bf42a0ca7ff0526f3a5a/zeroconf-0.64.1-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:10d3ba25a0d43b4daadc3089fc0446db332e5db6bf1fc41cd6b8a8808082b14e"},
-    {url = "https://files.pythonhosted.org/packages/f7/07/3394fbe745bd7e673569395829b33f40739a65f3329dfed14d4e67f69131/zeroconf-0.64.1-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d7ac86caa31a613d306a35ffd521c83f9420a55e3f6aa279c0edf24f932a2044"},
-    {url = "https://files.pythonhosted.org/packages/fa/0c/31f03decd88171224291c70c8d77c92b927ab751e8378976be38201d69f3/zeroconf-0.64.1-cp311-cp311-win32.whl", hash = "sha256:958465c5229788b685ad4f2b503c4a80aa4376452bbb486fa798655afb2e293e"},
+"zeroconf 0.66.0" = [
+    {url = "https://files.pythonhosted.org/packages/01/8d/21b7888f9ff1ba9636b20b04047ad0ed3adc50412c23583955dd17022533/zeroconf-0.66.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9a24696415df8fab6c588ab42cde5d90ede8e5b2f491f1bf430f345993697648"},
+    {url = "https://files.pythonhosted.org/packages/05/8b/4e33d4cd95f3ce0305d033eebc5dfbc5355c54a3fa9a010749a18756858f/zeroconf-0.66.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:7d525441081ece62a08caf39d5fbfcd63d0f4207534c48847339a467abcb3ebf"},
+    {url = "https://files.pythonhosted.org/packages/06/06/3fb05d32ab98779fa749164eae148a652ded2ff567afe88d86e3bcc19044/zeroconf-0.66.0-pp37-pypy37_pp73-macosx_11_0_x86_64.whl", hash = "sha256:414581e7cd3074132c9ce55cde9dcd8b1dfb95c69d4d7a9d61f206915f5b3be6"},
+    {url = "https://files.pythonhosted.org/packages/07/22/c38d8501f829fe3287cac4765b63a1876180e9848562ecf2c81fb5ff3b38/zeroconf-0.66.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0844743c5bc5ca57310a5939d388f72b3973f32d75bc2c5d9b475104e09c66ef"},
+    {url = "https://files.pythonhosted.org/packages/09/ba/1176554e377100f1f1d963397dc33fd27e33166774423846732e2f8aa497/zeroconf-0.66.0-cp38-cp38-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:19b70f63950a60d3729de9f7a45cd01704d796dab01e8246a79f3420c527878e"},
+    {url = "https://files.pythonhosted.org/packages/09/c1/cae76f0b9580ff1d116f2f61659e7c74f950d6e4ea433ceba697711fd76e/zeroconf-0.66.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:a6a857dcb71ed5c6a5a3b8668effbdfe09a2383bf33fe659c6bcd034f1263467"},
+    {url = "https://files.pythonhosted.org/packages/0c/1f/28b1099f31751f9cfa4d4071082022509d55726f92b097d398b3db587af6/zeroconf-0.66.0-cp37-cp37m-win32.whl", hash = "sha256:c632a04b2d314b52a2e29dcc453d3fa3d1133b0da94e6025410a21b8323be08b"},
+    {url = "https://files.pythonhosted.org/packages/21/18/fcd54add5cea152355fe99ddfde28f74a4d359cda7bf6e90c4a9ef90f529/zeroconf-0.66.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:20887b20f26453c41660184895dff387a8155e61f89206ae223b8262b44ae2c8"},
+    {url = "https://files.pythonhosted.org/packages/2a/9c/c1a4bb6f8a073f422b7d264b857ee19f42ba97192e57ef5afe1927a5bf97/zeroconf-0.66.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:0356fcbe7073fab997c1e8a475255de64a1f5d891f550c008b68017409373d77"},
+    {url = "https://files.pythonhosted.org/packages/3f/1b/4bcc4b9cd61516ff80fdabdd3344f37081b32cd799fb1a8cd9cd1611417a/zeroconf-0.66.0-cp310-cp310-win32.whl", hash = "sha256:1214f2291f2ee96efeaebc604137cba1408b0054f433af3502321603e218a4b7"},
+    {url = "https://files.pythonhosted.org/packages/42/53/65bc5f9239f52701b1b9cd155a3184bd635a39e10fad8caf3d50c492ea1e/zeroconf-0.66.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:9dca4aafee95c92bea2e68791bad7db1d34cb1b792c3f5d348c5f3dbc26ab58e"},
+    {url = "https://files.pythonhosted.org/packages/42/5d/28572cca42b3dab479f705f38684a618b00d8bbd6495ff0dfdd446b6a212/zeroconf-0.66.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:45d98c460a9bb51e85e15be95b7d33c01f73ce8302489d67fe961da5d7662139"},
+    {url = "https://files.pythonhosted.org/packages/53/9c/abeefab0652d2ebe78fe8f4bcd6a8c38fbd212c066a2b85a48022327de84/zeroconf-0.66.0-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:1545d10f20152c28e9e73b1f9918bac0174a421ab4d86c1badb1078d89fb0574"},
+    {url = "https://files.pythonhosted.org/packages/56/04/5433a0465e828b2c0fdb844c882a20cb50d6d3abafd7ae44737a23da38cd/zeroconf-0.66.0-cp39-cp39-win32.whl", hash = "sha256:5edc86847ce23c86db6fcef91a162f5a9974928115f158d9e347042fae27663d"},
+    {url = "https://files.pythonhosted.org/packages/5f/15/effb9ac7fabfa95b963bec892da85012014774099928548d47bf096a8ea1/zeroconf-0.66.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:886c665b42df65b35d092e502180f475495d919db0c8b51b462afb8a8c7763c4"},
+    {url = "https://files.pythonhosted.org/packages/5f/45/940e523d7576db80660589c9d7207ce0b38d19332e116eb7bd46404eddcd/zeroconf-0.66.0-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:455daec7b7e9095fc81a2973a0be92187c26d60bdc0009230662e233acc02289"},
+    {url = "https://files.pythonhosted.org/packages/5f/a4/7ce118203229f63bd3c7f29a21568d03c5c6a76db35d07d814cd000118fa/zeroconf-0.66.0-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:bbced1ba8013fb9c8e8384e77bded79d8d4ed87195935ccfc9254ffab9f5372f"},
+    {url = "https://files.pythonhosted.org/packages/61/e6/c82b1c39df5b8ff7979272e641b7561b62994845a4d805f9ecdd1447ced6/zeroconf-0.66.0-cp37-cp37m-macosx_11_0_x86_64.whl", hash = "sha256:d560798fd9cffebfc1b22c28e385cb3068cb3511b53fe93334813bb7fa100759"},
+    {url = "https://files.pythonhosted.org/packages/6d/97/e273c09740f12688ed1d00bcb65424e42c6489e3182c00d9e74b44f8fa22/zeroconf-0.66.0.tar.gz", hash = "sha256:1af7dc50d6c26d174e4cd79bc9b390cf42d5ed2dd1ee91c1b113201888143c0d"},
+    {url = "https://files.pythonhosted.org/packages/75/d3/e1118c8f4870f891ca00d098d13826f5d63363dbac307116d8e920dd4596/zeroconf-0.66.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:44c4990e9e766b23cab86dc7fa0c2191604290b09c07b8cd9326d2ef3abe9415"},
+    {url = "https://files.pythonhosted.org/packages/80/54/59812395d7caa08235b1a47673f4e504b90d3e465be2ebf4a100a7671363/zeroconf-0.66.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54a6aeec0c0ca680ddc7b3367cd6b070de3c87082f052f16a5cae91be3ecaab1"},
+    {url = "https://files.pythonhosted.org/packages/80/f6/0538e24d8eceb80c53bb8cbe9fa046afca2924e6b9bc9696ac4b35941d48/zeroconf-0.66.0-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:776be3098fc1e361288905a4ea05379c51dad166f049327b524d5cb98bace0c0"},
+    {url = "https://files.pythonhosted.org/packages/90/48/582ae01ea5ab8ece075d1c01acc2bcff06ff9d5fd8274f1b95ca489c1ec3/zeroconf-0.66.0-cp311-cp311-win_amd64.whl", hash = "sha256:1fec47c1d8dd84aa61196d081b32752a42d19bd78ed3b3cced5478305fa5bcb6"},
+    {url = "https://files.pythonhosted.org/packages/90/a6/fd0d52ac6fed8434157659d6c61db508e8f0c2bd1054c61434166f535a2b/zeroconf-0.66.0-cp311-cp311-win32.whl", hash = "sha256:04d12703423aea6546511bce9747cad2e3eaec7a47a4f7188ce6c67f204098ce"},
+    {url = "https://files.pythonhosted.org/packages/97/27/d0362dba626c6abe9f767a6c7e68722b383b5dc6ac04f08202fac7ef8290/zeroconf-0.66.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:4b211886b0a5cbef7c7f9d15d1492e9f323de0fb7e8c750cd86224002a2efc55"},
+    {url = "https://files.pythonhosted.org/packages/a6/08/59a7af0c3527d070b060c71624089c4bb0f2b6c0def24aed912be572d584/zeroconf-0.66.0-cp38-cp38-win_amd64.whl", hash = "sha256:5fe741398486564b5c457c77d9167591e59034cdee85dd7a40531e80b97cb7ee"},
+    {url = "https://files.pythonhosted.org/packages/a6/8c/fcbbb3558425d84e240ea79bdde28d0fd5cc755cd6820654691082d728ef/zeroconf-0.66.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:2c55b7acd4a23133484eeb9814de1e281981b0389f7268ba6fcdedf199362820"},
+    {url = "https://files.pythonhosted.org/packages/ae/8e/af12216a116049091b4348d3a60980be498af81d31e59bb9d9eb872b5794/zeroconf-0.66.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:b15ff89c605da12c245cd89fe8b0b7db7b054566b97c58eceaa13bafcc18ad96"},
+    {url = "https://files.pythonhosted.org/packages/af/7d/50704d3a4558b70c101382e776627d77bee4e8c62d49574b600137563795/zeroconf-0.66.0-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:ca6520bd128f7fdb043f909b50fcdc2666ac8968ef22ef9f5f77d326ebeab3ad"},
+    {url = "https://files.pythonhosted.org/packages/b0/bf/c8a0b0f970bd704a764874a644f12d75923e2433b2f4abbff2e020cdae1a/zeroconf-0.66.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:ce399141063a517ffef3c6504d36ae203828e26c35e39a3bc2948c9230fd1b71"},
+    {url = "https://files.pythonhosted.org/packages/b3/dd/34e5a4271e7ce5ab03b77e97ecbaf7c7aa184f40471340b19cc4557b37b6/zeroconf-0.66.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:2d42cd53da6cfa5a4c89ed89621c0faa6b28718db6f290464ac83ee9f33a49ea"},
+    {url = "https://files.pythonhosted.org/packages/b6/62/e66769e70ab3f46e8a803632bdffe613bc9cd0e2a645b5f98dfbf5d81e1c/zeroconf-0.66.0-cp39-cp39-win_amd64.whl", hash = "sha256:eaddcd38486b47137257ee80bd943d66f2ce6c36a431ff229e3d3bcc12dd2d62"},
+    {url = "https://files.pythonhosted.org/packages/be/b5/cb7238b69aed8b40d0963d767adce50c1c0d053b947dd174246aae69ce37/zeroconf-0.66.0-cp310-cp310-win_amd64.whl", hash = "sha256:64cdce0750a6d18b8dde9ee1401724e3165f31a3a58d898e06dea8e618edd67f"},
+    {url = "https://files.pythonhosted.org/packages/c1/4c/a2cd16cc98456df8684f00e8780640bd923bcc35e37a27123716704431be/zeroconf-0.66.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:91e3e0264b040578e4895fe090fed3782f2a7f67857548b82ad9fdf2c8e59fed"},
+    {url = "https://files.pythonhosted.org/packages/c6/17/e2e852ad98eb69f1477e6795b003994b4cccd99fafcf349119716545ab8e/zeroconf-0.66.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8eaea03f9ee65a69035716070644d40548f66dfc333403f92c4e4fd43b5704c6"},
+    {url = "https://files.pythonhosted.org/packages/cb/a7/f0fcb5112326846649e6a64a39799a6ab238f180989996674889a069d41e/zeroconf-0.66.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:1396389b9fd2cc7da570eae1068dfbbeb93508c1e913b6b09096eccbc4dafa44"},
+    {url = "https://files.pythonhosted.org/packages/cc/04/fd4ee7486bffb82ea0797845658ed88b5631d94456c9dd914deabc386369/zeroconf-0.66.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:2c27c45486de5094925d9a8a48e647854396995e74e9819513b0e2159f71de1b"},
+    {url = "https://files.pythonhosted.org/packages/cd/d7/49f2bd9326a14c0c63675753674c88578f2a68b3bb9d5ac40632f3b79e29/zeroconf-0.66.0-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:cfe90abdd093b859ee344a94866f1b3c2c9dc054f7473745fb190b14083a70b1"},
+    {url = "https://files.pythonhosted.org/packages/ce/8a/bc01e9856ba197453c54c26e4dae851cfbccd4e574b1395118af25bc3552/zeroconf-0.66.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:56962db72a9439645c956979e9fcf00fd391ee8b769180284a87be3e906fef20"},
+    {url = "https://files.pythonhosted.org/packages/d2/49/e5158404daf23899e99d72c4a1ec88879b3af467a9f616c946443778c91d/zeroconf-0.66.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f4d43cdbf4a108e1e0727f12bf7a2222dec0ab0566197bbeb504d0f1e53447f"},
+    {url = "https://files.pythonhosted.org/packages/db/d6/6a17c10fd09de8a45747cb0dd85ef04d76e948d9454c0ddb58e7fb72fddb/zeroconf-0.66.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be5687c8a4834b8b343676793ba269831d34f69cbaae0adcacc881559d940e5a"},
+    {url = "https://files.pythonhosted.org/packages/e2/77/1bde47d1d9dd0dddc64cc5a7ec7e299f0e203d6ec478c058735a98b635c1/zeroconf-0.66.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c182cac6633d517a11c06ab3b04b5d3d2bea356de81d5f57273d78cfa1aa04b9"},
+    {url = "https://files.pythonhosted.org/packages/e3/01/0f04de804ae2469b1a165cdf01e40fe099158869d6defd8a699d1bb4d81e/zeroconf-0.66.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:829478a8dee2fea754e2c8fd54b28462d61b016945aba94c3b51b984d18209dc"},
+    {url = "https://files.pythonhosted.org/packages/e5/ac/7f6fb7143b04014f0f6ca5a99b35a4bdc189e5514e5221f2a904acdd3431/zeroconf-0.66.0-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:c12e38b2ccfaaebfe4a1516a1e97647872e7b5193d3711be014c982da5768121"},
+    {url = "https://files.pythonhosted.org/packages/e9/95/4593816ab58f8a90dee06f96c32c2cd7d1b5d71d9511d3a86cac6e77de94/zeroconf-0.66.0-cp37-cp37m-win_amd64.whl", hash = "sha256:b65dceae6fcaeb95f1fd7b3e348a6b795a85fc2d15a16b72104e366915b062e1"},
+    {url = "https://files.pythonhosted.org/packages/e9/e1/b278980b921f98cdb7072c522e9f030b6801ca279fbf16089c69fe9d894b/zeroconf-0.66.0-cp38-cp38-macosx_11_0_x86_64.whl", hash = "sha256:555660a7dc720ae92c0f409447200cb751e90353bfe7717aedf8114ec19b053e"},
+    {url = "https://files.pythonhosted.org/packages/ee/ed/b2e08281b95e008e288216bb4a13d5a9c4321dd1d5d7a13cadb7d9a3ea61/zeroconf-0.66.0-cp38-cp38-win32.whl", hash = "sha256:57a1c0c2681bb86e2be3200480149429545df5d477c5b702ecc0b140cdc01a8e"},
+    {url = "https://files.pythonhosted.org/packages/ef/a9/d952f9805084d504f8ada522bdb6535a17b06e667cb3923623686ed4f59a/zeroconf-0.66.0-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:10ad59230f826cc37500dffb54aba82a70d22afa6f25b2ff7a44e9e020517eca"},
+    {url = "https://files.pythonhosted.org/packages/f5/24/7b37c243ad7b6bd83f74c6e9efe8db915a80abcc50926792337d0c3c6960/zeroconf-0.66.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9939600589a9fbfb00e5a90bdf8b3ece45029147e2e99eafe641d5f1d83fb0d9"},
 ]
 "zipp 3.15.0" = [
     {url = "https://files.pythonhosted.org/packages/00/27/f0ac6b846684cecce1ee93d32450c45ab607f65c2e0255f0092032d91f07/zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
     {url = "https://files.pythonhosted.org/packages/5b/fa/c9e82bbe1af6266adf08afb563905eb87cab83fde00a0a08963510621047/zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
 ]
```

### Comparing `xklb-1.30.7/readme.py` & `xklb-1.31.2/readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 And you can always add more later--even from different websites.
 
     library tubeadd maker.db https://vimeo.com/terburg
 
 To prevent mistakes the default configuration is to download metadata for only
 the most recent 20,000 videos per playlist/channel.
 
-    library tubeadd maker.db --dl-config playlistend=1000
+    library tubeadd maker.db --extractor-config playlistend=1000
 
 Be aware that there are some YouTube Channels which have many items--for example
 the TEDx channel has about 180,000 videos. Some channels even have upwards of
 two million videos. More than you could likely watch in one sitting--maybe even one lifetime.
 On a high-speed connection (>500 Mbps), it can take up to five hours to download
 the metadata for 180,000 videos.
```

### Comparing `xklb-1.30.7/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.31.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.31.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/.github/workflows/push.yaml` & `xklb-1.31.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/av.py` & `xklb-1.31.2/xklb/av.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,16 @@
             mu.get("TDOR"),
             mu.get("TORY"),
             mu.get("date"),
             mu.get("TDRC"),
             mu.get("TDRL"),
             ti.get("year"),
         ),
-        "bpm": safe_unpack(mu.get("fBPM"), mu.get("bpm"), mu.get("bpm_start")),
+        "bpm": utils.safe_int(safe_unpack(mu.get("fBPM"), mu.get("bpm"), mu.get("bpm_start"))),
         "key": safe_unpack(mu.get("TIT1"), mu.get("key"), mu.get("TKEY"), mu.get("key_start")),
-        "time": combine(mu.get("time_signature")),
         "decade": safe_unpack(mu.get("Songs-DB_Custom1")),
         "categories": safe_unpack(mu.get("Songs-DB_Custom2")),
         "city": safe_unpack(mu.get("Songs-DB_Custom3")),
         "country": combine(
             mu.get("Songs-DB_Custom4"),
             mu.get("MusicBrainz Album Release Country"),
             mu.get("musicbrainz album release country"),
@@ -239,7 +238,24 @@
         video_tags = get_subtitle_tags(args, path, streams, codec_types)
         media = {**media, **video_tags}
 
     if args.profile == DBType.audio:
         stream_tags = get_audio_tags(path)
         media = {**media, **stream_tags}
     return media
+
+
+def decode_full_scan(path):
+    output = ffmpeg.input(path).output("/dev/null", f="null")
+    ffmpeg.run(output, quiet=True)
+
+
+def decode_quick_scan(path, scans, scan_duration=3):
+    fail_count = 0
+    for scan in scans:
+        try:
+            output = ffmpeg.input(path, ss=scan).output("/dev/null", t=scan_duration, f="null")
+            ffmpeg.run(output, quiet=True)
+        except ffmpeg.Error:
+            fail_count += 1
+
+    return (fail_count / len(scans)) * 100
```

### Comparing `xklb-1.30.7/xklb/books.py` & `xklb-1.31.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/consts.py` & `xklb-1.31.2/xklb/consts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import os, re, secrets, shutil, string, sys
+import re, secrets, shutil, string, sys
 from datetime import datetime, timezone
 from pathlib import Path
 from tempfile import gettempdir
-from types import SimpleNamespace
 from typing import List
 
 
 def now():
     return int(datetime.now(tz=timezone.utc).timestamp())
 
 
@@ -50,15 +49,14 @@
         ],
     ),
 )
 REGEX_V_REDD_IT = re.compile("https?://v.redd.it/(?:[^/?#&]+)")
 APPLICATION_START = now()
 TERMINAL_SIZE = shutil.get_terminal_size(fallback=(80, 60))
 
-
 TIME_COLUMNS = (
     "time_scanned",
     "time_downloaded",
     "time_deleted",
     "time_modified",
     "time_created",
     "time_played",
@@ -81,14 +79,16 @@
     fsadd = "fsadd"
     fsupdate = "fsupdate"
     watch = "watch"
     listen = "listen"
     filesystem = "filesystem"
     tubeadd = "tubeadd"
     tubeupdate = "tubeupdate"
+    galleryadd = "galleryadd"
+    galleryupdate = "galleryupdate"
     tabs = "tabs"
     read = "read"
     view = "view"
     download = "download"
     block = "block"
     stats = "stats"
     search = "search"
@@ -181,16 +181,105 @@
     "created",
     "modified",
     "downloaded",
 ]
 
 frequency = ["daily", "weekly", "monthly", "quarterly", "yearly"]
 
+PLAYLIST_KNOWN_KEYS = (
+    "url",
+    "duration",
+    "view_count",
+    "webpage_url",
+    "original_url",
+)
 
-TUBE_IGNORE_KEYS = (
+MEDIA_KNOWN_KEYS = (
+    "photoset_layout",
+    "asks_allow_media",
+    "submission_page_title",
+    "post_author_is_adult",
+    "is_submission",
+    "fragment",
+    "is_anonymous",
+    "ask",
+    "ask_anon",
+    "ask_page_title",
+    "avatar",
+    "theme",
+    "count",
+    "can_chat",
+    "can_subscribe",
+    "share_likes",
+    "subscribed",
+    "total_posts",
+    "is_blocks_post_format",
+    "blog_name",
+    "id_string",
+    "is_blazed",
+    "is_blaze_pending",
+    "can_blaze",
+    "slug",
+    "state",
+    "reblog_key",
+    "short_url",
+    "summary",
+    "should_open_in_legacy",
+    "note_count",
+    "caption",
+    "reblog",
+    "can_like",
+    "interactability_reblog",
+    "interactability_blaze",
+    "can_reblog",
+    "can_send_in_message",
+    "can_reply",
+    "display_avatar",
+    "reblogged",
+    "hash",
+    "link_url",
+    "query",
+    "domain",
+    "etag",
+    "pages",
+    "posts",
+    "locale",
+    "num",
+    "kind",
+    "ie_key",
+    "extractor_key",
+    "extractor",
+    "upvote_count",
+    "downvote_count",
+    "filename",
+    "extension",
+    "category",
+    "subcategory",
+    "virality",
+    "in_most_viral",
+    "is_album",
+    "is_mature",
+    "cover_id",
+    "image_count",
+    "privacy",
+    "vote",
+    "favorite",
+    "is_ad",
+    "include_album_ads",
+    "shared_with_community",
+    "is_pending",
+    "display",
+    "mime_type",
+    "type",
+    "name",
+    "basename",
+    "is_animated",
+    "is_looping",
+    "has_sound",
+    "platform",
     "track_id",
     "track_number",
     "repost_count",
     "fragments",
     "thumbnail",
     "thumbnails",
     "availability",
```

### Comparing `xklb-1.30.7/xklb/db.py` & `xklb-1.31.2/xklb/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,31 +57,39 @@
         return db
 
     if not Path(args.database).exists() and ":memory:" not in args.database:
         log.error(f"Database file '{args.database}' does not exist. Create one with lb fsadd, tubeadd, or tabsadd.")
         raise SystemExit(1)
 
     db = DB(conn or args.database, tracer=tracer if args.verbose >= consts.LOG_DEBUG_SQL else None, **kwargs)  # type: ignore
-    with db.conn:
-        db.conn.execute("PRAGMA main.cache_size = 8000")
+    with db.conn:  # type: ignore
+        db.conn.execute("PRAGMA main.cache_size = 8000")  # type: ignore
 
     db.enable_wal()
     return db
 
 
+def columns(args, table_name):
+    return args.db[table_name].columns_dict
+
+
 config = {
+    "playlists": {
+        "column_order": ["path", "extractor_key"],
+        "ignore_columns": ["id", "extractor_playlist_id"],
+    },
     "media": {
         "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
-        "column_order": ["path", "webpath", "tube_id", "ie_key", "playlist_path"],
-        "ignore_columns": ["id", "tube_id"],
+        "column_order": ["path", "webpath", "extractor_id"],
+        "ignore_columns": ["id", "extractor_id"],
     },
     "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
-        "column_order": ["playlist_path", "path"],
+        "column_order": ["path"],
     },
     "reddit_comments": {
         "search_columns": ["body"],
     },
     "hn_comment": {
         "search_columns": ["text", "author"],
     },
@@ -93,17 +101,14 @@
     },
     "hn_job": {
         "search_columns": ["title", "text", "author", "path"],
     },
     "hn_story": {
         "search_columns": ["title", "text", "author", "path"],
     },
-    "playlists": {
-        "column_order": ["path", "ie_key"],
-    },
 }
 
 
 def optimize(args) -> None:
     if not hasattr(args, "force"):
         args.force = False
 
@@ -157,15 +162,15 @@
                 create_triggers=True,
                 replace=True,
                 tokenize="trigram"
                 if sqlite3.sqlite_version_info >= (3, 34, 0)
                 else 'unicode61 "tokenchars=_."',  # https://www.sqlite.org/releaselog/3_34_0.html
             )
         else:
-            with db.conn:
+            with db.conn:  # type: ignore
                 log.info("Optimizing fts index: %s", table)
                 db[table].optimize()  # type: ignore
 
     log.info("Running VACUUM")
     db.vacuum()
     log.info("Running ANALYZE")
     db.analyze()
@@ -206,15 +211,14 @@
         "categories",
         "city",
         "country",
         "description",
         "album",
         "artist",
         "tags",
-        "playlist_path",
     ]
 
     valid_cols = [f"m.{c}" for c in searchable_columns if c in cols_available]
 
     incl = ":include{0}"
     excl = ":exclude{0}"
     include_string = "AND (" + " OR ".join([f"{col} LIKE {incl}" for col in valid_cols]) + ")"
@@ -228,25 +232,7 @@
 
     for idx, inc in enumerate(args.include):
         args.filter_sql.append(includes.format(idx))
         args.filter_bindings[f"include{idx}"] = "%" + inc.replace(" ", "%").replace("%%", " ") + "%"
     for idx, exc in enumerate(args.exclude):
         args.filter_sql.append(excludes.format(idx))
         args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
-
-
-def get_playlists(args, cols="path, dl_config", constrain=False, sql_filters=None) -> List[dict]:
-    columns = args.db["playlists"].columns_dict
-    if sql_filters is None:
-        sql_filters = []
-    if "time_deleted" in columns:
-        sql_filters.append("AND COALESCE(time_deleted,0) = 0")
-    if constrain and args.category:
-        sql_filters.append(f"AND category='{args.category}'")
-
-    try:
-        known_playlists = list(
-            args.db.query(f"select {cols} from playlists where 1=1 {' '.join(sql_filters)} order by random()"),
-        )
-    except sqlite3.OperationalError:
-        known_playlists = []
-    return known_playlists
```

### Comparing `xklb-1.30.7/xklb/dl_config.py` & `xklb-1.31.2/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/fs_extract.py` & `xklb-1.31.2/xklb/fs_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import argparse, math, os, sys
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
-from copy import deepcopy
 from functools import partial
 from multiprocessing import TimeoutError as mp_TimeoutError
 from pathlib import Path
 from shutil import which
 from timeit import default_timer as timer
 from typing import Dict, List, Optional
 
-from xklb import av, books, consts, db, player, usage, utils
+from xklb import av, books, consts, db, player, playlists, usage, utils
 from xklb.consts import SC, DBType
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
 
@@ -55,27 +54,26 @@
         action="store_const",
         dest="profile",
         const=DBType.image,
         help="Create image database",
     )
     parser.set_defaults(profile=DBType.video)
     parser.add_argument("--scan-all-files", "-a", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
 
     parser.add_argument(
         "--io-multiplier",
         type=float,
         default=1.0,
         help="Especially useful for text, image, filesystem db types",
     )
     parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--extra-media-data", default={})
-    parser.add_argument("--extra-playlist-data", default={})
+    parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
+    parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
 
     parser.add_argument("--delete-unplayable", action="store_true")
     parser.add_argument(
         "--check-corrupt",
         type=float,
         default=0.0,
         help="check that 0 to 100 percent of media decodes correctly",
@@ -152,15 +150,14 @@
         "time_played": 0,
         "playhead": 0,
         "size": stat.st_size,
         "time_created": int(stat.st_ctime),
         "time_modified": int(stat.st_mtime) or consts.now(),
         "time_downloaded": consts.APPLICATION_START,
         "time_deleted": 0,
-        "ie_key": "Local",
     }
 
     if hasattr(stat, "st_blocks"):
         media = {**media, "sparseness": calculate_sparseness(stat)}
 
     if mp_args.profile == DBType.filesystem:
         media = {**media, "is_dir": Path(path).is_dir()}
@@ -210,14 +207,15 @@
         if description:
             tags += "\n" + description
         if tags:
             caption["captions_t0"] = {"time": 0, "text": tags}
 
         captions.append(caption)
 
+    media = [{"playlist_id": args.playlist_id, **d} for d in media]
     media = utils.list_dict_filter_bool(media)
     args.db["media"].insert_all(utils.list_dict_filter_bool(media), pk="id", alter=True, replace=True)
 
     for d in captions:
         media_id = args.db.pop("select id from media where path = ?", [d["path"]])
         if len(d["chapters"]) > 0:
             args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["chapters"]], alter=True)
@@ -252,26 +250,26 @@
             else:
                 msg = f"fs_extract for profile {args.profile}"
                 raise NotImplementedError(msg)
         except FileNotFoundError:
             print(f"[{path}] Not found")
             return []
 
-    columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     scanned_set = set(scanned_files)
 
     try:
         deleted_set = {
             d["path"]
             for d in args.db.query(
                 f"""select path from media
                 where 1=1
                     and time_deleted > 0
                     and path like '{path}%'
-                    {'AND time_downloaded > 0' if 'time_downloaded' in columns else ''}
+                    {'AND time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
                 """,
             )
         }
     except Exception as e:
         log.debug(e)
     else:
         undeleted_files = list(deleted_set.intersection(scanned_set))
@@ -281,18 +279,19 @@
 
     try:
         existing_set = {
             d["path"]
             for d in args.db.query(
                 f"""select path from media
                 where 1=1
-                    and time_deleted = 0
-                    and path like '{path}%'
-                    {'AND time_downloaded > 0' if 'time_downloaded' in columns else ''}
+                    and path like ?
+                    and coalesce(time_deleted, 0) = 0
+                    {'AND coalesce(time_downloaded, 0) > 0' if 'time_downloaded' in m_columns else ''}
                 """,
+                [str(path) + "%"],
             )
         }
     except Exception as e:
         log.debug(e)
         new_files = list(scanned_set)
     else:
         new_files = list(scanned_set - existing_set)
@@ -304,29 +303,14 @@
         deleted_count = player.mark_media_deleted(args, deleted_files)
         if deleted_count > 0:
             print(f"[{path}] Marking", deleted_count, "orphaned metadata records as deleted")
 
     return new_files
 
 
-def _add_folder(args, folder_path: Path) -> None:
-    category = args.category or folder_path.parts[-1]
-
-    playlist = {
-        "ie_key": "Local",
-        "path": str(folder_path),
-        "config": utils.filter_namespace(args, ["ocr", "speech_recognition", "scan_subtitles"]),
-        "time_deleted": 0,
-        "profile": args.profile,
-        "category": category,
-        **args.extra_playlist_data,
-    }
-    args.db["playlists"].upsert(utils.dict_filter_bool(playlist), pk="path", alter=True)
-
-
 def scan_path(args, path_str: str) -> int:
     path = Path(path_str).expanduser().resolve()
     if not path.exists():
         print(f"[{path}] Path does not exist")
         if args.force:
             player.delete_playlists(args, [str(path)])
         return 0
@@ -337,14 +321,21 @@
     if args.io_multiplier > 1:
         n_jobs = int(max(os.cpu_count() or 4, 4) * args.io_multiplier)
     if args.verbose >= consts.LOG_DEBUG:
         n_jobs = 1
 
     threadsafe = [DBType.audio, DBType.video, DBType.filesystem]
 
+    info = {
+        "extractor_key": "Local",
+        "extractor_config": utils.filter_namespace(args, ["ocr", "speech_recognition", "scan_subtitles"]),
+        "time_deleted": 0,
+    }
+    args.playlist_id = playlists.add(args, str(path), info)
+
     print(f"[{path}] Building file list...")
     new_files = find_new_files(args, path)
     if new_files:
         print(f"[{path}] Adding {len(new_files)} new media")
         log.debug(new_files)
 
         if args.profile in (DBType.text):
@@ -367,16 +358,14 @@
                 print(f"[{path}] Extracting metadata {percent:3.1f}% (chunk {idx + 1} of {chunks_count})")
 
                 mp_args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
                 metadata = parallel.map(partial(extract_metadata, mp_args), chunk_paths)
                 metadata = list(filter(None, metadata))
                 extract_chunk(args, metadata)
 
-    _add_folder(args, path)
-
     return len(new_files)
 
 
 def extractor(args, paths) -> None:
     new_files = 0
     for path in paths:
         new_files += scan_path(args, path)
@@ -400,26 +389,26 @@
 
 def fs_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args = parse_args(SC.fsupdate, usage.fsupdate)
 
-    playlists = list(
+    fs_playlists = list(
         args.db.query(
             """
             SELECT *
             FROM playlists
-            WHERE ie_key = 'Local'
+            WHERE extractor_key = 'Local'
             ORDER BY
                 length(path)-length(REPLACE(path, '/', '')) desc
                 , path
             """,
         ),
     )
 
-    for playlist in playlists:
+    for playlist in fs_playlists:
         args_env = argparse.Namespace(
-            **{**(playlist.get("config") or {}), **args.__dict__, "profile": playlist["profile"]},
+            **{**(playlist.get("extractor_config") or {}), **args.__dict__, "profile": playlist["profile"]},
         )
 
         extractor(args_env, [playlist["path"]])
```

### Comparing `xklb-1.30.7/xklb/gui.py` & `xklb-1.31.2/xklb/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from pathlib import Path
 from typing import NoReturn, Tuple
 
-from xklb.utils import log
-
 base_folder = Path(__file__).resolve().parent
 
 
 class UserQuit(BaseException):
     pass
```

### Comparing `xklb-1.30.7/xklb/hn_extract.py` & `xklb-1.31.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/lb.py` & `xklb-1.31.2/xklb/lb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse, sys
 
 from xklb import __version__, utils
 from xklb.consts import SC
 from xklb.dl_extract import dl_download
 from xklb.fs_extract import fs_add, fs_update
+from xklb.gdl_extract import gallery_add, gallery_update
 from xklb.hn_extract import hacker_news_add
 from xklb.play_actions import filesystem, listen, read, view, watch
 from xklb.playback import playback_next, playback_now, playback_pause, playback_stop
 from xklb.praw_extract import reddit_add, reddit_update
 from xklb.scripts.bigdirs import bigdirs
 from xklb.scripts.block import block
 from xklb.scripts.christen import christen
@@ -61,14 +62,17 @@
       lb merge-dbs             Merge multiple SQLITE files
       lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
+      lb galleryadd            Create a gallery database; Add albums
+      lb galleryupdate         Fetch new images from saved playlists
+
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
@@ -174,24 +178,29 @@
     subp_dedupe = add_parser(subparsers, "dedupe")
     subp_dedupe.set_defaults(func=dedupe)
     subp_dedupe_local = add_parser(subparsers, "merge-online-local")
     subp_dedupe_local.set_defaults(func=merge_online_local)
     subp_optimize = add_parser(subparsers, "optimize", ["optimize-db"])
     subp_optimize.set_defaults(func=optimize_db)
 
-    subp_tubeadd = add_parser(subparsers, "tubeadd", ["dladd", "ta", "da", "xt"])
+    subp_tubeadd = add_parser(subparsers, "tubeadd", ["ta", "dladd", "da"])
     subp_tubeadd.set_defaults(func=tube_add)
     subp_tubeupdate = add_parser(subparsers, "tubeupdate", ["dlupdate", "tu"])
     subp_tubeupdate.set_defaults(func=tube_update)
 
-    subp_redditadd = add_parser(subparsers, "redditadd", ["ra", "xr"])
+    subp_galleryadd = add_parser(subparsers, "galleryadd", ["gdladd", "ga"])
+    subp_galleryadd.set_defaults(func=gallery_add)
+    subp_galleryupdate = add_parser(subparsers, "galleryupdate", ["gdlupdate", "gu"])
+    subp_galleryupdate.set_defaults(func=gallery_update)
+
+    subp_redditadd = add_parser(subparsers, "redditadd", ["ra"])
     subp_redditadd.set_defaults(func=reddit_add)
-    subp_redditupdate = add_parser(subparsers, "redditupdate", ["ru", "xru"])
+    subp_redditupdate = add_parser(subparsers, "redditupdate", ["ru"])
     subp_redditupdate.set_defaults(func=reddit_update)
-    subp_pushshift = add_parser(subparsers, "pushshift", ["ps"])
+    subp_pushshift = add_parser(subparsers, "pushshift")
     subp_pushshift.set_defaults(func=pushshift_extract)
 
     subp_hnadd = add_parser(subparsers, "hnadd")
     subp_hnadd.set_defaults(func=hacker_news_add)
 
     subp_download = add_parser(subparsers, "download", ["dl"])
     subp_download.set_defaults(func=dl_download)
@@ -218,23 +227,23 @@
     subp_playback_pause = add_parser(subparsers, "pause")
     subp_playback_pause.set_defaults(func=playback_pause)
 
     subp_tabsadd = add_parser(subparsers, "tabsadd")
     subp_tabsadd.set_defaults(func=tabs_add)
     subp_tabs = add_parser(subparsers, "tabs", ["tb"])
     subp_tabs.set_defaults(func=tabs)
-    subp_surf = add_parser(subparsers, "surf", ["browse", "load"])
+    subp_surf = add_parser(subparsers, "surf")
     subp_surf.set_defaults(func=streaming_tab_loader)
 
     subp_nouns = add_parser(subparsers, "nouns")
     subp_nouns.set_defaults(func=nouns)
     subp_cluster_sort = add_parser(subparsers, "cluster-sort", ["cs", "clustersort", "cluster_sort"])
     subp_cluster_sort.set_defaults(func=cluster_sort)
 
-    subp_reddit_selftext = add_parser(subparsers, "reddit-selftext", ["rst"])
+    subp_reddit_selftext = add_parser(subparsers, "reddit-selftext")
     subp_reddit_selftext.set_defaults(func=reddit_selftext)
     subp_nfb_directors = add_parser(subparsers, "extract-links", ["links"])
     subp_nfb_directors.set_defaults(func=extract_links)
 
     parser.add_argument("--version", "-V", action="store_true")
     return parser
```

### Comparing `xklb-1.30.7/xklb/play_actions.py` & `xklb-1.31.2/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,27 @@
 
 def parse_args_sort(args) -> None:
     if args.sort:
         args.sort = " ".join(args.sort)
     elif not args.sort and hasattr(args, "defaults"):
         args.defaults.append("sort")
 
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
 
     # switching between videos with and without subs is annoying
     subtitle_count = "=0"
     if random() < getattr(args, "subtitle_mix", consts.DEFAULT_SUBTITLE_MIX):
         # bias slightly toward videos without subtitles
         subtitle_count = ">0"
 
     sorts = [
         "random" if getattr(args, "random", False) else None,
         "rank" if args.sort and "rank" in args.sort else None,
         "video_count > 0 desc" if "video_count" in m_columns and args.action == SC.watch else None,
         "audio_count > 0 desc" if "audio_count" in m_columns else None,
-        "time_downloaded > 0 desc"
-        if "time_downloaded" in m_columns and "time_downloaded" not in " ".join(sys.argv)
-        else None,
         'm.path like "http%"',
         "width < height desc" if "width" in m_columns and hasattr(args, "portrait") and args.portrait else None,
         f"subtitle_count {subtitle_count} desc"
         if "subtitle_count" in m_columns
         and args.action == SC.watch
         and not any(
             [
@@ -46,14 +43,17 @@
                 consts.PYTEST_RUNNING,
                 "subtitle_count" in args.where,
                 args.limit != consts.DEFAULT_PLAY_QUEUE,
             ],
         )
         else None,
         args.sort,
+        "time_downloaded > 0 desc"
+        if "time_downloaded" in m_columns and "time_downloaded" not in " ".join(sys.argv)
+        else None,
         "duration desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "size desc" if args.action in (SC.listen, SC.watch) and args.include else None,
         "play_count" if args.action in (SC.listen, SC.watch) and "play_count" in m_columns else None,
         "size desc, duration"
         if args.action in (SC.listen, SC.watch) and "size" in m_columns and "duration" in m_columns
         else None,
         "sparseness" if args.action == SC.filesystem else None,
@@ -262,15 +262,15 @@
     utils.timeout(args.timeout)
 
     args.sock = None
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
@@ -485,15 +485,15 @@
 
     m["now_playing"] = now_playing(m["path"])
 
     return m
 
 
 def save_playhead(args, m, start_time):
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     if "playhead" in m_columns:
         playhead = utils.get_playhead(
             args,
             m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
@@ -593,19 +593,19 @@
     if args.safe:
         media = [d for d in media if tube_backend.is_supported(d["path"]) or Path(d["path"]).exists()]
         log.debug("tube_backend.is_supported: %s", t.elapsed())
 
     if args.big_dirs:
         media_keyed = {d["path"]: d for d in media}
         dirs = process_bigdirs(args, media)
-        dirs = list(reversed(list(d["path"] for d in dirs)))
+        dirs = list(reversed([d["path"] for d in dirs]))
         if "limit" in args.defaults:
             media = player.get_dir_media(args, dirs)
         else:
-            media = [media_keyed[key] for dir in dirs for key in media_keyed.keys() if key.startswith(dir)]
+            media = [media_keyed[key] for dir in dirs for key in media_keyed if key.startswith(dir)]
         log.debug("big_dirs: %s", t.elapsed())
 
     if args.related >= consts.RELATED:
         media = player.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
 
     if args.cluster:
```

### Comparing `xklb-1.30.7/xklb/playback.py` & `xklb-1.31.2/xklb/playback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, os, platform, textwrap
+import argparse, platform, textwrap
 from pathlib import Path
 
 from xklb import consts, utils
 from xklb.utils import cmd, log
 
 
 def parse_args(action) -> argparse.Namespace:
```

### Comparing `xklb-1.30.7/xklb/player.py` & `xklb-1.31.2/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from shlex import join, quote, split
 from shutil import which
 from time import sleep
 from typing import Dict, List, Optional, Tuple, Union
 
 from tabulate import tabulate
 
-from xklb import consts, db, utils
+from xklb import consts, db, media, utils
 from xklb.consts import SC
 from xklb.utils import cmd, cmd_interactive, human_time, log
 
 try:
     import tkinter  # noqa
 
     from xklb import gui
@@ -280,15 +280,20 @@
             playlist_paths,
         )
 
     online_media = [p for p in playlists if p.startswith("http")]
     if online_media:
         with args.db.conn:
             args.db.conn.execute(
-                "delete from media where playlist_path in (" + ",".join(["?"] * len(online_media)) + ")",
+                """DELETE from media where
+                playlist_id in (
+                    SELECT id from playlists
+                    WHERE path IN ("""
+                + ",".join(["?"] * len(online_media))
+                + "))",
                 (*online_media,),
             )
 
     local_media = [p.rstrip(os.sep) for p in playlists if not p.startswith("http")]
     for folder in local_media:
         with args.db.conn:
             args.db.conn.execute("delete from media where path like ?", (folder + "%",))
@@ -398,15 +403,15 @@
 
 
 def get_ordinal_media(args, m: Dict, ignore_paths=None) -> Dict:
     # TODO: maybe try https://dba.stackexchange.com/questions/43415/algorithm-for-finding-the-longest-prefix
     if ignore_paths is None:
         ignore_paths = []
 
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
 
     cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir"]
     args.select_sql = "\n        , ".join([c for c in cols if c in m_columns or c in ["*"]])
 
     total_media = args.db.execute("select count(*) val from media").fetchone()[0]
     candidate = deepcopy(m["path"])
     if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS_PARENT:
@@ -461,18 +466,18 @@
                 log.debug("Using commonprefix")
                 return m
 
     return similar_videos[0]
 
 
 def get_related_media(args, m: Dict) -> List[Dict]:
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     m_columns.update(rank=int)
 
-    m = args.db["media"].get(m["path"])
+    m = media.get(args, m["path"])
     words = set(
         utils.conform(utils.extract_words(m.get(k)) for k in m if k in db.config["media"]["search_columns"]),
     )
     args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
     query = f"""
@@ -501,15 +506,15 @@
     return [m, *related_videos]
 
 
 def get_dir_media(args, dirs: List, include_subdirs=False) -> List[Dict]:
     if len(dirs) == 0:
         return utils.no_media_found()
 
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
 
     if include_subdirs:
         filter_paths = "AND (" + " OR ".join([f"path LIKE :subpath{i}" for i in range(len(dirs))]) + ")"
     else:
         filter_paths = (
             "AND ("
             + " OR ".join([f"(path LIKE :subpath{i} and path not like :subpath{i} || '/%')" for i in range(len(dirs))])
@@ -860,15 +865,16 @@
     elif freq == "monthly":
         time_period = f"strftime('%Y-%m', datetime({time_column}, 'unixepoch'))"
     elif freq == "quarterly":
         time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch', '-3 months')) || '-Q' || ((strftime('%m', datetime({time_column}, 'unixepoch', '-3 months')) - 1) / 3 + 1)"
     elif freq == "yearly":
         time_period = f"strftime('%Y', datetime({time_column}, 'unixepoch'))"
     else:
-        raise ValueError(f"Invalid value for 'freq': {freq}")
+        msg = f"Invalid value for 'freq': {freq}"
+        raise ValueError(msg)
 
     query = f"""
     SELECT
         {time_period} AS time_period
         , SUM(duration) AS duration_sum
         , AVG(duration) AS duration_avg
         , SUM(size) AS size_sum
```

### Comparing `xklb-1.30.7/xklb/praw_extract.py` & `xklb-1.31.2/xklb/praw_extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import sys
 from functools import partial
 from itertools import takewhile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
-from xklb import consts, db, usage, utils
+from xklb import consts, db, media, playlists, usage, utils
 from xklb.utils import log
 
 PRAW_SETUP_INSTRUCTIONS = r"""
 You will need your Reddit user login info, client id, and secret.
 See https://www.reddit.com/wiki/api for client id / secret.
 
 Then create a praw.ini file:
@@ -47,16 +47,14 @@
     parser.add_argument("--limit", default=1000, type=int)
     parser.add_argument("--lookback", default=4, type=int, help="Number of days to look back")
     parser.add_argument("--praw-site", default="bot1")
 
     parser.add_argument("--subreddits", action="store_true")
     parser.add_argument("--redditors", action="store_true")
 
-    parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
-
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == "redditadd":
         parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
@@ -144,15 +142,15 @@
 
 
 def saveable(item) -> Dict[str, Any]:
     result = {k: legalize(v) for k, v in item.__dict__.items() if not k.startswith("_")}
     return _parent_ids_interpreted(result)
 
 
-def slim_post_data(d: dict, playlist_path=None) -> dict:
+def slim_post_data(d: dict, subreddit=None) -> dict:
     skip_domains = ["linktr.ee", "twitter.com", "t.me", "patreon", "onlyfans", "fans.ly", "file-upload", "file-link"]
     url = d.get("url")
     if url:
         url = url.lower()
     if not url or any(domain in url for domain in skip_domains):
         d["url"] = d.get("url_overridden_by_dest")
 
@@ -179,15 +177,15 @@
         "num_comments": d.get("num_comments"),
         "num_crossposts": d.get("num_crossposts"),
         "score": d.get("score"),
         "upvote_ratio": d.get("upvote_ratio"),
         "selftext": selftext,
         "title": d.get("title"),
         "total_awards_received": d.get("total_awards_received"),
-        "playlist_path": playlist_path,
+        "subreddit": subreddit,
     }
 
 
 def save_post(args, post_dict, subreddit_path) -> None:
     slim_dict = utils.dict_filter_bool(slim_post_data(post_dict, subreddit_path))
 
     if slim_dict:
@@ -213,29 +211,29 @@
             "time_deleted": 0,
             **(existing_meta or {}),
         }
 
         if post_dict.get("author_is_blocked") == 1:
             pass
         elif "selftext" in slim_dict:
-            args.db["reddit_posts"].upsert(slim_dict, pk=["path", "playlist_path"], alter=True)
+            args.db["reddit_posts"].upsert(slim_dict, pk=["path", "subreddit"], alter=True)
         else:
-            args.db["media"].upsert(slim_dict, pk=["path", "playlist_path"], alter=True)
+            media._add(args, slim_dict)
 
 
 def since_last_created(args, playlist_path):
     latest_post_utc = args.db.pop(
         """
         select max(time_created)
         from (
-            select time_created, playlist_path from reddit_posts
+            select time_created, playlist_id from reddit_posts
             UNION ALL
-            select time_created, playlist_path from media
+            select time_created, playlist_id from media
         )
-        where playlist_path = ?
+        where playlist_id = (select id from playlists where path = ?)
     """,
         [playlist_path],
         ignore_errors=["no such column", "no such table"],
     )
     if latest_post_utc:
         get_since = dt.datetime.fromtimestamp(latest_post_utc, tz=dt.timezone.utc) - dt.timedelta(days=args.lookback)
         get_since = int(get_since.timestamp())
@@ -266,24 +264,23 @@
 
     _takewhile = since_last_created(args, subreddit_path)
     log.info("Getting new posts")
     for idx, post in enumerate(takewhile(_takewhile, subreddit.new(limit=args.limit))):
         post_dict = saveable(post)
 
         if idx == 0:
-            args.db["playlists"].upsert(
+            playlists._add(
+                args,
                 utils.dict_filter_bool(
                     {
                         "path": subreddit_path,
                         "subscribers": post_dict.pop("subreddit_subscribers", None),
                         "visibility": post_dict.pop("subreddit_type", None),
                     },
                 ),
-                pk="path",
-                alter=True,
             )
 
         save_post(args, post_dict, subreddit_path)
 
 
 def subreddit_top(args, subreddit_dict) -> None:
     subreddit_path, subreddit_name = subreddit_dict.values()
@@ -345,72 +342,69 @@
     args = parse_args("redditadd", usage=usage.redditadd)
 
     subreddits = []
     redditors = []
     for path in args.paths:
         subreddit_matches = consts.REGEX_SUBREDDIT.match(path)
         redditor_matches = consts.REGEX_REDDITOR.match(path)
-        ie_key = "reddit_praw"
+        extractor_key = "reddit_praw"
         name = path
         if subreddit_matches:
-            ie_key = "reddit_praw_subreddit"
+            extractor_key = "reddit_praw_subreddit"
             name = utils.conform(subreddit_matches.groups()).pop()
             subreddits.append({"path": path, "name": name})
         elif redditor_matches:
-            ie_key = "reddit_praw_redditor"
+            extractor_key = "reddit_praw_redditor"
             name = utils.conform(redditor_matches.groups()).pop()
             redditors.append({"path": path, "name": name})
         else:
             if args.subreddits:
-                ie_key = "reddit_praw_subreddit"
+                extractor_key = "reddit_praw_subreddit"
                 path = f"https://old.reddit.com/r/{name}/"
                 subreddits.append({"path": path, "name": name})
             elif args.redditors:
-                ie_key = "reddit_praw_redditor"
+                extractor_key = "reddit_praw_redditor"
                 path = f"https://old.reddit.com/user/{name}/"
                 redditors.append({"path": path, "name": name})
             else:
                 log.error(f"[{path}]: Skipping unknown URL")
                 continue
 
-        args.db["playlists"].upsert(
+        playlists._add(
+            args,
             utils.dict_filter_bool(
                 {
                     "path": path,
-                    "playlist_id": name,
-                    "config": utils.filter_namespace(args, ["limit", "lookback", "praw_site"]),
-                    "category": args.category or ie_key,
-                    "ie_key": ie_key,
+                    "extractor_playlist_id": name,
+                    "extractor_config": utils.filter_namespace(args, ["limit", "lookback", "praw_site"]),
+                    "extractor_key": extractor_key,
                     "time_deleted": 0,
                 },
             ),
-            pk="path",
-            alter=True,
         )
 
     process_subreddits(args, subreddits)
     process_redditors(args, redditors)
     LARGE_NUMBER = 75
     if not args.db["media"].detect_fts() or len(subreddits + redditors) > LARGE_NUMBER:
         db.optimize(args)
 
 
 def reddit_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args = parse_args("redditupdate", usage=usage.redditupdate)
-    playlists = db.get_playlists(
+    reddit_playlists = playlists.get_all(
         args,
-        "ie_key, path, id, config",
-        sql_filters=['AND ie_key in ("reddit_praw_subreddit","reddit_praw_redditor")'],
-        constrain=True,
+        "extractor_key, path, id, extractor_config",
+        sql_filters=['AND extractor_key in ("reddit_praw_subreddit","reddit_praw_redditor")'],
     )
 
-    for playlist in playlists:
-        config = json.loads(playlist["config"])
-        args_env = args if not config else argparse.Namespace(**{**config, **args.__dict__})
-
-        if playlist["ie_key"] == "reddit_praw_subreddit":
-            process_subreddits(args_env, [{"path": playlist["path"], "name": playlist["playlist_id"]}])
-        elif playlist["ie_key"] == "reddit_praw_subreddit":
-            process_redditors(args_env, [{"path": playlist["path"], "name": playlist["playlist_id"]}])
+    for playlist in reddit_playlists:
+        extractor_config = json.loads(playlist["extractor_config"])
+        args_env = args if not extractor_config else argparse.Namespace(**{**extractor_config, **args.__dict__})
+
+        if playlist["extractor_key"] == "reddit_praw_subreddit":
+            process_subreddits(args_env, [{"path": playlist["path"], "name": playlist["extractor_playlist_id"]}])
+        elif playlist["extractor_key"] == "reddit_praw_redditor":
+            process_redditors(args_env, [{"path": playlist["path"], "name": playlist["extractor_playlist_id"]}])
```

### Comparing `xklb-1.30.7/xklb/search.py` & `xklb-1.31.2/xklb/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             for caption in path_group:
                 for line in textwrap.wrap(caption["text"], subsequent_indent=" " * 9, initial_indent=f"{caption['time']} ", width=consts.TERMINAL_SIZE.columns - 2):  # type: ignore
                     print(line)
             print()
 
 
 def construct_query(args) -> Tuple[str, dict]:
-    m_columns = args.db["media"].columns_dict
-    c_columns = args.db["captions"].columns_dict
+    m_columns = db.columns(args, "media")
+    c_columns = db.columns(args, "captions")
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     table = "captions"
     if args.db["captions"].detect_fts():
```

### Comparing `xklb-1.30.7/xklb/subtitle.py` & `xklb-1.31.2/xklb/subtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 import ffmpeg
 
 from xklb import db, utils
 from xklb.consts import SUB_TEMP_DIR
-from xklb.utils import flatten, log, remove_consecutive_whitespace, remove_text_inside_brackets
+from xklb.utils import log, remove_consecutive_whitespace, remove_text_inside_brackets
 
 SUBTITLE_FORMATS = "vtt|srt|ssa|ass|jss|aqt|mpl2|mpsub|pjs|rt|sami|smi|stl|xml|txt|psb|ssf|usf"
 IMAGE_SUBTITLE_CODECS = ["dvbsub", "dvdsub", "pgssub", "xsub", "dvb_subtitle", "dvd_subtitle", "hdmv_pgs_subtitle"]
 SUBSTATION_OVERRIDE_TAG = re.compile(r"{[^}]*}")
 
 
 def extract_from_video(path, stream_index) -> Optional[str]:
```

### Comparing `xklb-1.30.7/xklb/tabs_actions.py` & `xklb-1.31.2/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/tabs_extract.py` & `xklb-1.31.2/xklb/tabs_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, sys
 from pathlib import Path
 from typing import List
 
-from xklb import consts, db, player, usage, utils
+from xklb import consts, db, media, player, usage, utils
 from xklb.utils import log, sanitize_url
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tabsadd", usage=usage.tabsadd)
     parser.add_argument(
         "--frequency",
@@ -87,9 +87,10 @@
 
 
 def tabs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
     args = parse_args()
 
-    tabs = [extract_url_metadata(args, path) for path in get_new_paths(args)]
-    args.db["media"].insert_all(utils.list_dict_filter_bool(tabs), pk="path", alter=True, replace=True)
+    tabs = utils.list_dict_filter_bool([extract_url_metadata(args, path) for path in get_new_paths(args)])
+    for tab in tabs:
+        media._add(args, tab)
```

### Comparing `xklb-1.30.7/xklb/tube_extract.py` & `xklb-1.31.2/xklb/tube_extract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db, tube_backend, usage, utils
+from xklb import consts, db, playlists, tube_backend, usage, utils
 from xklb.consts import SC
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library " + action,
         usage=usage,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
-        "--dl-config",
-        "-dl-config",
+        "--extractor-config",
+        "-extractor-config",
         nargs=1,
         action=utils.ArgparseDict,
         default={},
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
     parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
     parser.add_argument(
-        "--force", action="store_true", help="Fetch metadata for paths even if they are already in the media table"
+        "--force",
+        "-f",
+        action="store_true",
+        help="Fetch metadata for paths even if they are already in the media table",
     )
     parser.add_argument("--subs", action="store_true")
     parser.add_argument("--auto-subs", "--autosubs", action="store_true")
     parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
-    parser.add_argument("--extra-media-data", default={})
-    parser.add_argument("--extra-playlist-data", default={})
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", "-f", action="store_true", help=argparse.SUPPRESS)
-
-    if action in (SC.tubeadd, SC.tubeupdate):
-        parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
+    parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
+    parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
+    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.tubeadd:
@@ -61,14 +61,15 @@
         args.playlists = list(set(s.strip() for s in args.playlists))
         if not args.no_sanitize:
             args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
         args.playlists = utils.conform(args.playlists)
 
     utils.timeout(args.timeout)
 
+    args.profile = consts.DBType.video
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
@@ -76,15 +77,15 @@
     args = parse_args(SC.tubeadd, usage=usage.tubeadd)
     if args.playlist_files:
         args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
     tables = args.db.table_names()
     known_playlists = []
     if "media" in tables and not args.force:
-        m_columns = args.db["media"].columns_dict
+        m_columns = db.columns(args, "media")
         known_playlists = list(
             set(
                 d["path"]
                 for d in args.db.query(
                     (
                         "SELECT path from media"
                         + " WHERE path in ("
@@ -93,27 +94,27 @@
                         + ",".join(["?"] * len(args.playlists))
                         + ")"
                         + " UNION ALL"
                         + " SELECT path from playlists"
                     ),
                     [*args.playlists, *args.playlists],
                 )
-            )
+            ),
         )
 
     for path in args.playlists:
         if args.safe and not tube_backend.is_supported(path):
             log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
             continue
 
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
 
-        tube_backend.process_playlist(args, path, tube_backend.tube_opts(args))
+        tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
 
         if args.extra:
             log.warning("[%s]: Getting extra metadata", path)
             tube_backend.get_extra_metadata(args, path)
 
     LARGE_NUMBER = 100_000
     if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
@@ -121,9 +122,22 @@
 
 
 def tube_update(args=None) -> None:
     if args:
         sys.argv = ["tubeupdate", *args]
 
     args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
-    playlists = db.get_playlists(args, constrain=True)
-    tube_backend.update_playlists(args, playlists)
+    tube_playlists = playlists.get_all(args)
+    for d in tube_playlists:
+        tube_backend.get_playlist_metadata(
+            args,
+            d["path"],
+            tube_backend.tube_opts(
+                args,
+                playlist_opts=d.get("extractor_config", "{}"),
+                func_opts={"ignoreerrors": "only_download"},
+            ),
+        )
+
+        if args.extra:
+            log.warning("[%s]: Getting extra metadata", d["path"])
+            tube_backend.get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("extractor_config", "{}"))
```

### Comparing `xklb-1.30.7/xklb/usage.py` & `xklb-1.31.2/xklb/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
         library download dl.db --prefix ~/output/path/root/
 
     Download stuff in a random order, limited to the specified playlist URLs.
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
-    Files will be saved to <lb download prefix>/<lb download category>/
+    Files will be saved to <lb download prefix>/<extractor>/
 
         For example:
         library dladd Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Print list of queued up downloads
@@ -22,24 +22,24 @@
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
         library download-status audio.db
-        ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
-        │                     │            │ and 20 minutes   │                    │          │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
-        ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key     │ duration         │   never_downloaded │   errors │
+        ╞════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Soundcloud │                  │                 10 │        0 │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
+        │            │ and 20 minutes   │                    │          │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 7.68 minutes     │                 99 │        1 │
+        ╘════════════╧══════════════════╧════════════════════╧══════════╛
 """
 
 block = r"""library block DATABASE URLS ...
 
     Blocklist specific URLs (eg. YouTube channels, etc). With YT URLs this will block
     videos from the playlist uploader
 
@@ -407,15 +407,15 @@
 
     Note that reddit's API is limited to 1000 posts and it usually doesn't go back very far historically.
     Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
     my suggestion is to use pushshift data.
     You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 """
 
-redditupdate = """library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+redditupdate = """library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 """
 
 search = """library search DATABASE QUERY
@@ -544,24 +544,24 @@
 
 playlists = """library playlists DATABASE [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
-        │ ie_key   │ title              │ path                                                                     │
+        │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╛
 
     Aggregate Report of Videos in each Playlist
 
         library playlists -p a
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╤═══════════════╤═════════╕
-        │ ie_key   │ title              │ path                                                                     │ duration      │   count │
+        │ extractor_key   │ title              │ path                                                                     │ duration      │   count │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╪═══════════════╪═════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │ 53.28 minutes │      15 │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╧═══════════════╧═════════╛
         1 playlist
         Total duration: 53.28 minutes
 
     Print only playlist urls:
@@ -575,48 +575,44 @@
 """
 
 download_status = """library download-status DATABASE
 
     Print download queue groups
 
         library download-status video.db
-        ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
-        │                     │             │ and 6 minutes    │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Dailymotion         │ Dailymotion │                  │                186 │      198 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Uncategorized       │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Vimeo               │ Vimeo       │                  │                253 │       49 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Youtube             │ Youtube     │ 2 years, 4       │              51676 │      197 │
-        │                     │             │ months, 15 days  │                    │          │
-        │                     │             │ and 6 hours      │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
-        │                     │             │ days, 19 hours   │                    │          │
-        │                     │             │ and 33 minutes   │                    │          │
-        ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒═════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key      │ duration         │   never_downloaded │   errors │
+        ╞═════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                 53 │        0 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
+        │             │ and 6 minutes    │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                186 │      198 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Vimeo       │                  │                253 │       49 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 2 years, 4       │              51676 │      197 │
+        │             │ months, 15 days  │                    │          │
+        │             │ and 6 hours      │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 4 months, 23     │               2686 │        7 │
+        │             │ days, 19 hours   │                    │          │
+        │             │ and 33 minutes   │                    │          │
+        ╘═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
         library download-status video.db --safe
-
-    Show only download attempts with errors
-
-        library download-status video.db --errors
 """
 
 tabs = """library tabs DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
         45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
@@ -678,15 +674,15 @@
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
         │ p/?sort=top&t=year                    │             │              │
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
 """
 
-tabsadd = r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
+tabsadd = r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -698,33 +694,29 @@
 
     Importing from a line-delimitated file:
 
         library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 """
 
-tubeadd = r"""library tubeadd [-c CATEGORY] [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+tubeadd = r"""library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
-    You can also include a category for file organization
-
-        library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
-
-    Files will be saved to <download prefix>/<tubeadd category>/
+    Files will be saved to <download prefix>/<extractor>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -732,36 +724,35 @@
         By default tubeadd will quickly add media at the expense of less metadata.
         If you plan on using `library download` then it doesn't make sense to use `--extra`.
         Downloading will add the extra metadata automatically to the database.
         You can always fetch more metadata later via tubeupdate:
         library tubeupdate tw.db --extra
 """
 
-tubeupdate = """library tubeupdate [--audio | --video] [-c CATEGORY] DATABASE
+tubeupdate = """library tubeupdate [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
-    Or limit to specific categories...
-
-        library tubeupdate -c "Bob Ross" educational.db
-
     Run with --optimize to add indexes (might speed up searching but the size will increase):
 
         library tubeupdate --optimize examples/music.tl.db
 
     Fetch extra metadata:
 
         By default tubeupdate will quickly add media.
         You can run with --extra to fetch more details: (best resolution width, height, subtitle tags, etc)
 
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 """
 
+galleryadd = None
+galleryupdate = None
+
 bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
@@ -817,15 +808,15 @@
 
     Merge database data and tables
 
         library merge-dbs --upsert --pk path video.db tv.db movies.db
         library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path audio-fts.db audio.db
 
         library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
-        library merge-dbs --only-new-rows --pk playlist_path,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 """
 
 merge_online_local = """library merge-online-local DATABASE
 
     If you have previously downloaded YouTube or other online media, you can dedupe
     your database and combine the online and local media records as long as your
     files have the youtube-dl / yt-dlp id in the filename.
```

### Comparing `xklb-1.30.7/xklb/utils.py` & `xklb-1.31.2/xklb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import wraps
 from pathlib import Path
 from random import shuffle
 from shutil import which
 from timeit import default_timer
 from typing import Any, Dict, Generator, List, NoReturn, Optional, Union
 
-import ffmpeg, humanize
+import humanize
 from IPython.core import ultratb
 from IPython.terminal.debugger import TerminalPdb
 from rich import prompt
 from rich.logging import RichHandler
 
 from xklb import consts
 from xklb.scripts.mining import data
@@ -127,14 +127,16 @@
         elif isinstance(x, bytes):
             yield x.decode("utf-8")
         else:
             yield x
 
 
 def conform(list_: Union[str, Iterable]) -> List:
+    if not list_:
+        return []
     if not isinstance(list_, list):
         list_ = [list_]
     list_ = flatten(list_)
     list_ = list(filter(bool, list_))
     return list_
 
 
@@ -364,14 +366,16 @@
         .replace("}", " ")
         .replace("_", " ")
         .replace("-", " "),
     )
 
 
 def safe_int(s) -> Optional[int]:
+    if not s:
+        return None
     try:
         return int(float(s))
     except Exception:
         return None
 
 
 def concat(*args):
@@ -523,15 +527,15 @@
 
     def mpv_progress(m):
         playhead = m.get("playhead")
         duration = m.get("duration")
         if not playhead:
             return float("-inf")
         if not duration:
-            return float("-max")
+            return float("-inf")
 
         if "p" in args.partial and "t" in args.partial:
             return (duration / playhead) * -(duration - playhead)  # weighted remaining
         elif "t" in args.partial:
             return -(duration - playhead)  # time remaining
         else:
             return playhead / duration  # percent remaining
@@ -635,25 +639,34 @@
     no_double_space = [_RE_COMBINE_WHITESPACE.sub(" ", s).strip() for s in no_semicolon]
     no_unknown = [x for x in no_double_space if x.lower() not in ("unknown", "none", "und", "")]
 
     no_duplicates = list(dict.fromkeys(no_unknown))
     return ";".join(no_duplicates)
 
 
-def safe_unpack(*list_, idx=0) -> Optional[Any]:
+def safe_unpack(*list_, idx=0, keep_0=True) -> Optional[Any]:
     list_ = conform(list_)
     if not list_:
         return None
 
     try:
-        return list_[idx]
+        value = list_[idx]
+        return value if keep_0 or value != 0 else None
     except IndexError:
         return None
 
 
+def safe_sum(*list_, keep_0=False) -> Optional[Any]:
+    list_ = conform(list_)
+    if not list_:
+        return None
+    value = sum(list_)
+    return value if keep_0 or value != 0 else None
+
+
 def path_fill(text, size):
     width = max(10, int(size * (consts.TERMINAL_SIZE.columns / 80)))
     lines = []
     current_line = ""
     for char in text:
         if char == "\r":
             continue  # Ignore carriage return character
@@ -682,14 +695,22 @@
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             tbl[idx][col] = humanize.naturaldate(datetime.fromtimestamp(int(tbl[idx][col]), timezone.utc))
 
     return tbl
 
 
+def col_naturaltime(tbl: List[Dict], col: str) -> List[Dict]:
+    for idx, _d in enumerate(tbl):
+        if tbl[idx].get(col) is not None:
+            tbl[idx][col] = humanize.naturaltime(datetime.fromtimestamp(int(tbl[idx][col])))
+
+    return tbl
+
+
 def col_naturalsize(tbl: List[Dict], col: str) -> List[Dict]:
     for idx, _d in enumerate(tbl):
         if tbl[idx].get(col) is not None:
             if tbl[idx][col] == 0:
                 tbl[idx][col] = None
             else:
                 tbl[idx][col] = humanize.naturalsize(tbl[idx][col])
@@ -770,20 +791,14 @@
         setattr(args, self.dest, d)
 
 
 def filter_namespace(args, config_opts) -> Optional[Dict]:
     return dict_filter_bool({k: v for k, v in args.__dict__.items() if k in config_opts})
 
 
-def ensure_playlists_exists(args) -> None:
-    if "playlists" not in args.db.table_names():
-        with args.db.conn:
-            args.db.conn.execute("create table playlists (path text, category text, ie_key text, time_deleted int)")
-
-
 def clear_input() -> None:
     if platform.system() == "Linux":
         from termios import TCIFLUSH, tcflush
 
         tcflush(sys.stdin, TCIFLUSH)
     elif platform.system() == "Windows":
         if getattr(clear_input, "kbhit", None) is None:
@@ -1048,31 +1063,14 @@
     scans = sorted(set(int(scan * scan_interval) for scan in range(num_scans)))
     if scans[-1] < media_duration - (scan_duration * 2):
         scans.append(math.floor(media_duration - scan_duration))
 
     return scans, scan_duration
 
 
-def decode_full_scan(path):
-    output = ffmpeg.input(path).output("/dev/null", f="null")
-    ffmpeg.run(output, quiet=True)
-
-
-def decode_quick_scan(path, scans, scan_duration=3):
-    fail_count = 0
-    for scan in scans:
-        try:
-            output = ffmpeg.input(path, ss=scan).output("/dev/null", t=scan_duration, f="null")
-            ffmpeg.run(output, quiet=True)
-        except ffmpeg.Error:
-            fail_count += 1
-
-    return (fail_count / len(scans)) * 100
-
-
 def fast_glob(path_dir, limit=100):
     files = []
     with os.scandir(path_dir) as entries:
         for entry in entries:
             if entry.is_file():
                 files.append(entry.path)
                 if len(files) == limit:
@@ -1223,7 +1221,26 @@
                     break
             if is_blocked:
                 break
         if is_blocked:
             allowed_media.append(m)
 
     return allowed_media
+
+
+def trim_path_segments(path, desired_length):
+    path = Path(path)
+    segments = [*list(path.parent.parts), path.stem]
+    extension = path.suffix
+
+    desired_length -= len(extension)
+
+    while len("".join(segments)) > desired_length:
+        longest_segment_index = max(range(len(segments)), key=lambda i: len(segments[i]))
+        segments[longest_segment_index] = segments[longest_segment_index][:-1]
+
+        if all(len(segment) % 2 == 0 for segment in segments):
+            for i in range(len(segments)):
+                segments[i] = segments[i][:-1]
+
+    segments[-1] += extension
+    return str(Path(*segments))
```

### Comparing `xklb-1.30.7/xklb/scripts/bigdirs.py` & `xklb-1.31.2/xklb/scripts/bigdirs.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         elif args.upper is not None and pdict["count"] > args.upper:
             d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> List[dict]:
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     args.filter_sql = []
     args.filter_bindings = {}
 
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
     db.construct_search_bindings(args, m_columns)
```

### Comparing `xklb-1.30.7/xklb/scripts/block.py` & `xklb-1.31.2/xklb/scripts/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse, sys
-from token import NEWLINE
 
 import humanize
 from tabulate import tabulate
 
 from xklb import consts, db, player, tube_backend, usage, utils
 from xklb.consts import SC
 from xklb.utils import log
@@ -47,25 +46,25 @@
 
 
 def block(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args = parse_args()
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     if args.match_column not in m_columns:
         raise ValueError(
-            "Match column does not exist in the media table. You may need to run tubeadd first or check your spelling"
+            "Match column does not exist in the media table. You may need to run tubeadd first or check your spelling",
         )
 
     columns = set(["path", "webpath", args.match_column, "size", "playlist_path", "time_deleted"])
     select_sql = ", ".join(s for s in columns if s in m_columns)
 
     if args.match_column == "playlist_path":
-        playlist_paths = list(s for s in args.playlists)
+        playlist_paths = list(args.playlists)
         for p in playlist_paths:
             add_to_blocklist(args, [p])
 
         with args.db.conn:
             args.db.conn.execute(
                 f"""UPDATE playlists
                 SET time_deleted={consts.APPLICATION_START}
@@ -75,56 +74,58 @@
                 (*playlist_paths,),
             )
         with args.db.conn:
             args.db.conn.execute(
                 f"""UPDATE media
                 SET time_deleted={consts.APPLICATION_START}
                 WHERE path LIKE 'http%'
-                AND playlist_path IN ("""
+                AND playlist_id in (
+                    SELECT id from playlists
+                    WHERE path IN ("""
                 + ",".join(["?"] * len(playlist_paths))
-                + ")",
+                + "))",
                 (*playlist_paths,),
             )
 
         playlist_media = list(
             args.db.query(
                 """SELECT path, size FROM media
                 WHERE time_deleted = 0
                 AND time_downloaded > 0
-                AND playlist_path IN ("""
+                AND playlist_id in (
+                    SELECT id from playlists
+                    WHERE path IN ("""
                 + ",".join(["?"] * len(playlist_paths))
-                + ")",
+                + "))",
                 (*playlist_paths,),
-            )
+            ),
         )
         total_size = sum(d["size"] for d in playlist_media)
         paths_to_delete = [d["path"] for d in playlist_media]
         if paths_to_delete:
             print(paths_to_delete)
             if utils.confirm(
-                f"Would you like to delete these {len(paths_to_delete)} local files ({humanize.naturalsize(total_size)})?"
+                f"Would you like to delete these {len(paths_to_delete)} local files ({humanize.naturalsize(total_size)})?",
             ):
                 player.delete_media(args, paths_to_delete)
         return
 
     unmatched_playlists = []
     for p in args.playlists:
         p = [p]
         if consts.PYTEST_RUNNING or args.force:
             add_to_blocklist(args, p)
             continue
 
         matching_media = list(
-            args.db.query(f"select {select_sql} from media where {args.match_column} LIKE ?", (p[0],))
+            args.db.query(f"select {select_sql} from media where {args.match_column} LIKE ?", (p[0],)),
         )
 
         if not matching_media:
-            matching_media = list(
-                args.db.query(f"select {select_sql} from media where path = ? or playlist_path = ?", (p[0], p[0]))
-            )
+            matching_media = list(args.db.query(f"select {select_sql} from media where path = ?", (p[0])))
             if matching_media:
                 log.debug("tube: found local %s", matching_media)
 
         if args.match_column in ("playlist_path", "path") and not args.offline and not matching_media:
             data = tube_backend.get_video_metadata(args, p[0])
             if data:
                 if args.match_column not in data:
@@ -136,37 +137,35 @@
                             preview = preview[:77] + "..."
                         msg += f"  {key}: {preview}\n"
                     log.warning(msg)
                 else:
                     p[1] = data[args.match_column]
                     if p[1]:
                         matching_media = list(
-                            args.db.query(f"select {select_sql} from media where {args.match_column} = ?", (p[1],))
+                            args.db.query(f"select {select_sql} from media where {args.match_column} = ?", (p[1],)),
                         )
 
         if not matching_media:
             unmatched_playlists.append(p)
             continue
 
         try:
             matching_media = list(reversed(utils.cluster_dicts(matching_media)))
         except ModuleNotFoundError:
             pass
 
         tbl = utils.list_dict_filter_bool(matching_media)
         tbl = [
             {
-                "title_path": "\n".join(
-                    utils.concat(d.get("title"), d.get("webpath"), d["path"], d.get("playlist_path"))
-                ),
+                "title_path": "\n".join(utils.concat(d.get("title"), d.get("webpath"), d["path"])),
                 **d,
             }
             for d in tbl
         ]
-        tbl = [{k: v for k, v in d.items() if k not in ("title", "path", "webpath", "playlist_path")} for d in tbl]
+        tbl = [{k: v for k, v in d.items() if k not in ("title", "path", "webpath")} for d in tbl]
         tbl = utils.col_resize(tbl, "title_path", 40)
         tbl = utils.col_naturalsize(tbl, "size")
         tbl = utils.col_naturaldate(tbl, "time_deleted")
         print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
         if utils.confirm(f"{len(matching_media)} media matching {p}. Add to blocklist?"):
             add_to_blocklist(args, p)
         else:
@@ -174,14 +173,14 @@
 
         paths_to_delete = [
             d["path"] for d in matching_media if d["time_deleted"] == 0 and not d["path"].startswith("http")
         ]
         if paths_to_delete:
             total_size = sum(d["size"] for d in matching_media if d["time_deleted"] == 0)
             if utils.confirm(
-                f"Would you like to delete these {len(paths_to_delete)} local files ({humanize.naturalsize(total_size)})?"
+                f"Would you like to delete these {len(paths_to_delete)} local files ({humanize.naturalsize(total_size)})?",
             ):
                 player.delete_media(args, paths_to_delete)
 
     if unmatched_playlists:
         log.error("Could not find media matching these URLs/words (rerun with --force to add a blocking rule):")
         log.error("  " + " ".join(t[0] for t in unmatched_playlists))
```

### Comparing `xklb-1.30.7/xklb/scripts/christen.py` & `xklb-1.31.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/cluster_sort.py` & `xklb-1.31.2/xklb/scripts/cluster_sort.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse, sys
+from pprint import pprint
 
 from xklb import usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
@@ -24,17 +25,15 @@
     lines = args.input_path.readlines()
     args.input_path.close()
 
     groups = utils.cluster_paths(lines, args.clusters)
     groups = sorted(groups, key=lambda d: (len(d["grouped_paths"]), -len(d["common_prefix"])))
 
     if args.groups:
-        from rich import print
-
-        print(groups)
+        pprint(groups)
     else:
         lines = utils.flatten(d["grouped_paths"] for d in groups)
         if args.output_path:
             with open(args.output_path, "w") as output_fd:
                 output_fd.writelines(lines)
         else:
             utils.pipe_lines(lines)
```

### Comparing `xklb-1.30.7/xklb/scripts/copy_play_counts.py` & `xklb-1.31.2/xklb/scripts/copy_play_counts.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         """
         SELECT
             *
         FROM
             src.media
         WHERE
             src.media.play_count > 0
+            or
+            src.media.playhead > 0
         """,
     )
 
     modified_row_count = 0
     with args.db.conn:
         for d in copy_counts:
             renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
```

### Comparing `xklb-1.30.7/xklb/scripts/dedupe.py` & `xklb-1.31.2/xklb/scripts/dedupe.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         const=DBType.audio,
         help="Dedupe database by artist + album + title",
     )
     profile.add_argument(
         "--tube-id",
         action="store_const",
         dest="profile",
-        const="tube_id",
-        help="Dedupe database by tube_id + ie_key",
+        const="extractor_id",
+        help="Dedupe database by extractor_id + extractor_key",
     )
     profile.add_argument(
         "--title",
         action="store_const",
         dest="profile",
         const="title",
         help="Dedupe database by title + uploader",
@@ -120,24 +120,26 @@
         -- , length(m1.path)-length(REPLACE(m1.path, '/', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
         , m2.path duplicate_path
         , m2.size duplicate_size
     FROM
         media m1
+    JOIN playlists p1 on p1.id = m1.playlist_id
+    JOIN playlists p2 on p2.id = m2.playlist_id
     JOIN media m2 on 1=1
-        and m1.tube_id = m2.tube_id
+        and m1.extractor_id = m2.extractor_id
         and m1.duration >= m2.duration - 4
         and m1.duration <= m2.duration + 4
-        and m1.ie_key in (m2.ie_key, 'Local')
+        and p1.extractor_key in (p2.extractor_key, 'Local')
         and m2.path != m1.path
     WHERE 1=1
         and m1.time_deleted = 0 and m2.time_deleted = 0
         and abs(m1.sparseness - 1) < 0.1
-        and m1.tube_id != '' and m1.ie_key != ''
+        and m1.extractor_id != '' and p1.extractor_key != ''
     ORDER BY 1=1
         , m1.video_count > 0 DESC
         , m1.subtitle_count > 0 DESC
         , m1.audio_count DESC
         , length(m1.path)-length(REPLACE(m1.path, '/', '')) DESC
         , length(m1.path)-length(REPLACE(m1.path, '.', ''))
         , length(m1.path)
@@ -193,15 +195,15 @@
 
 
 def dedupe() -> None:
     args = parse_args()
 
     if args.profile == DBType.audio:
         duplicates = get_music_duplicates(args)
-    elif args.profile == "tube_id":
+    elif args.profile == "extractor_id":
         duplicates = get_id_duplicates(args)
     elif args.profile == "title":
         duplicates = get_title_duplicates(args)
     elif args.profile == DBType.filesystem:
         print(
             """
         You should use `rmlint` instead:
```

### Comparing `xklb-1.30.7/xklb/scripts/download_status.py` & `xklb-1.31.2/xklb/scripts/download_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--errors", "-errors", "--error", action="store_true", help="Show only rows with errors")
     parser.add_argument("--delete", "--remove", "--erase", "--rm", "-rm", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
     parser.add_argument(
         "--retry-delay",
         "-r",
         default="14 days",
         help="Must be specified in SQLITE Modifiers format: N hours, days, months, or years",
@@ -94,29 +93,27 @@
     query, bindings = dl_extract.construct_query(args)
 
     count_paths = ""
     if "time_modified" in query:
         if args.safe:
             args.db.register_function(tube_backend.is_supported, deterministic=True)
             count_paths = (
-                ", count(*) FILTER(WHERE COALESCE(time_modified,0) = 0 and is_supported(path)) never_downloaded"
+                "count(*) FILTER(WHERE COALESCE(m.time_modified,0) = 0 and is_supported(path)) never_downloaded"
             )
         else:
-            count_paths = ", count(*) FILTER(WHERE COALESCE(time_modified,0) = 0) never_downloaded"
+            count_paths = "count(*) FILTER(WHERE COALESCE(m.time_modified,0) = 0) never_downloaded"
 
     query = f"""select
-        coalesce(category, "Playlist-less media") category
-        {', ie_key' if 'm.ie_key' in query else ''}
-        {', sum(duration) duration' if 'duration' in query else ''}
         {count_paths}
-        {', count(*) FILTER(WHERE COALESCE(time_modified,0) > 0 AND error IS NOT NULL) errors' if 'error' in query else ''}
-        {', group_concat(distinct error) error_descriptions' if args.errors or 'error' in query and args.verbose >= 1 else ''}
+        , extractor_key
+        {', sum(duration) duration' if 'duration' in query else ''}
+        {', count(*) FILTER(WHERE COALESCE(m.time_modified,0) > 0 AND error IS NOT NULL) errors' if 'error' in query else ''}
+        {', group_concat(distinct error) error_descriptions' if 'error' in query and args.verbose >= 1 else ''}
     from ({query}) m
     where 1=1
         and COALESCE(time_downloaded,0) = 0
         and COALESCE(time_deleted,0) = 0
-        {'and error is not null' if args.errors else ''}
-    group by category{', ie_key' if 'm.ie_key' in query else ''}{', error' if args.errors else ''}
-    order by {'errors,' if args.errors else ''} category nulls last"""
+    group by extractor_key
+    order by never_downloaded"""
 
     printer(args, query, bindings)
     return None
```

### Comparing `xklb-1.30.7/xklb/scripts/history.py` & `xklb-1.31.2/xklb/scripts/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,27 +67,27 @@
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def print_recent(tbl, time_column=None):
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "playhead")
     if time_column:
-        utils.col_naturaldate(tbl, time_column)
+        utils.col_naturaltime(tbl, time_column)
     tbl = [{"title_path": "\n".join(utils.concat(d["title"], d["path"])), **d} for d in tbl]
     tbl = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in tbl]
 
     tbl = utils.col_resize(tbl, "title_path", 40)
     tbl = utils.col_resize(tbl, "duration", 5)
     tbl = utils.col_resize(tbl, "playhead", 5)
     tbl = utils.list_dict_filter_bool(tbl)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def recent_media(args, time_column):
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
     query = f"""
     SELECT
         path
         {', title' if 'title' in m_columns else ''}
         {', duration' if 'duration' in m_columns else ''}
         {', subtitle_count' if 'subtitle_count' in m_columns else ''}
         , {time_column}
```

### Comparing `xklb-1.30.7/xklb/scripts/merge_dbs.py` & `xklb-1.31.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/merge_online_local.py` & `xklb-1.31.2/xklb/scripts/merge_online_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from copy import deepcopy
-from typing import List, Optional
+from typing import List
 
 from tabulate import tabulate
 
-from xklb import consts, db, usage, utils
+from xklb import consts, db, media, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("database")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
@@ -25,16 +25,20 @@
         SELECT
             *
         FROM
             media
         WHERE 1=1
             and id is not null
             and id != ""
-            and ie_key != 'Local'
             and time_deleted = 0
+            and playlist_id in (
+                SELECT id from playlists
+                WHERE extractor_key
+                    NOT IN ('Local', 'NBCStations', 'TedTalk', 'ThisAmericanLife', 'InfoQ', 'NFB', 'KickStarter')
+            )
     )
     SELECT
         m2.path keep_path
         , m1.path duplicate_path
         , m1.title
     FROM m1, (
         SELECT
@@ -44,35 +48,29 @@
             media
         WHERE 1=1
             and time_deleted = 0
             and id is null
             and title is null
     ) m2
     JOIN media_fts on m2.rowid = media_fts.rowid
-    WHERE m2.ie_key = 'Local'
-        AND m1.ie_key NOT IN ('NBCStations', 'TedTalk', 'ThisAmericanLife', 'InfoQ', 'NFB', 'KickStarter')
-        AND media_fts.path MATCH '"'||m1.tube_id||'"'
-        AND m2.PATH LIKE '%['||m1.tube_id||']%'
+    JOIN playlists p2 on p2.id = m2.playlist_id
+    WHERE p2.extractor_key = 'Local'
+        AND media_fts.path MATCH '"'||m1.extractor_id||'"'
+        AND m2.PATH LIKE '%['||m1.extractor_id||']%'
     ORDER BY 1=1
         , length(m2.path)-length(REPLACE(m2.path, '/', '')) desc
         , length(m2.path)-length(REPLACE(m2.path, '.', ''))
         , length(m2.path)
         , m2.time_modified desc
         , m2.time_created desc
         , m2.duration desc
         , m2.path desc
     """
 
-    media = list(args.db.query(query))
-    return media
-
-
-def get_dict(args, path) -> Optional[dict]:
-    known = list(args.db.query("select * from media where path=?", [path]))[0]
-    return utils.dict_filter_bool(known, keep_0=False)
+    return list(args.db.query(query))
 
 
 def merge_online_local() -> None:
     args = parse_args()
     args.db["media"].rebuild_fts()
     duplicates = get_duplicates(args)
     duplicates_count = len(duplicates)
@@ -91,28 +89,29 @@
         merged = []
         for d in duplicates:
             fspath = d["keep_path"]
             webpath = d["duplicate_path"]
             if webpath in merged or fspath == webpath:
                 continue
 
-            tube_entry = get_dict(args, webpath)
-            fs_tags = get_dict(args, fspath)
+            tube_entry = media.get(args, webpath)
+            fs_tags = media.get(args, fspath)
 
-            if not tube_entry or not fs_tags or tube_entry["tube_id"] not in fs_tags["path"]:
+            if not tube_entry or not fs_tags or tube_entry["extractor_id"] not in fs_tags["path"]:
                 continue
 
             if fs_tags["time_modified"] is None or fs_tags["time_modified"] == 0:
                 fs_tags["time_modified"] = consts.now()
             if fs_tags["time_downloaded"] is None or fs_tags["time_downloaded"] == 0:
                 fs_tags["time_downloaded"] = consts.APPLICATION_START
 
             entry = {**tube_entry, **fs_tags, "webpath": webpath}
-            args.db["media"].insert(utils.dict_filter_bool(entry), pk="id", alter=True, replace=True)  # type: ignore
-            args.db["media"].delete(webpath)
+            media._add(args, utils.dict_filter_bool(entry))  # type: ignore
+            with args.db.conn:
+                args.db.conn.execute("DELETE from media WHERE path = ?", [webpath])
             merged.append(webpath)
 
         print(len(merged), "merged")
 
 
 if __name__ == "__main__":
     merge_online_local()
```

### Comparing `xklb-1.30.7/xklb/scripts/move_list.py` & `xklb-1.31.2/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/optimize_db.py` & `xklb-1.31.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/playlists.py` & `xklb-1.31.2/xklb/scripts/playlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--errors", "-errors", "--error", action="store_true", help="Show only rows with errors")
     parser.add_argument("--delete", "--remove", "--erase", "--rm", "-rm", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
 
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
@@ -39,16 +38,15 @@
     log.info(utils.dict_filter_bool(args.__dict__))
 
     args.action = consts.SC.stats
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
-    utils.ensure_playlists_exists(args)
-    pl_columns = args.db["playlists"].columns_dict
+    pl_columns = db.columns(args, "playlists")
     args.filter_sql = []
     args.filter_bindings = {}
 
     args.filter_sql.extend([" and " + w for w in args.where])
 
     args.table = "playlists"
     if args.db["playlists"].detect_fts():
@@ -112,33 +110,33 @@
 
 def playlists() -> None:
     args = parse_args()
 
     if args.delete:
         return delete_playlists(args, args.delete)
 
-    pl_columns = args.db["playlists"].columns_dict
-    m_columns = args.db["media"].columns_dict
+    pl_columns = db.columns(args, "playlists")
+    m_columns = db.columns(args, "media")
     query, bindings = construct_query(args)
 
-    if "playlist_path" in m_columns:
+    if "playlist_id" in m_columns:
         query = f"""
         select
             coalesce(p.path, "Playlist-less media") path
-            {', p.ie_key' if 'ie_key' in pl_columns else ''}
+            , p.extractor_key
             {', p.title' if 'title' in pl_columns else ''}
             {', p.time_deleted' if 'time_deleted' in pl_columns else ''}
             {', count(*) FILTER(WHERE play_count>0) play_count' if 'play_count' in m_columns else ''}
             {', sum(m.duration) duration' if 'duration' in m_columns else ''}
             {', sum(m.size) size' if 'size' in m_columns else ''}
             , count(*) count
         from media m
-        left join ({query}) p on (p.path = m.playlist_path {"and p.ie_key = m.ie_key and m.ie_key != 'Local'" if 'ie_key' in m_columns else ''})
+        left join ({query}) p on p.id = m.playlist_id
         group by coalesce(p.path, "Playlist-less media")
-        order by count, p.category nulls last, p.path
+        order by count, p.path
         """
 
     if args.aggregate:
         query = f"""
         select
             'Aggregate of playlists' path
             {', count(*) FILTER(WHERE time_deleted>0) deleted_count' if 'time_deleted' in query else ''}
```

### Comparing `xklb-1.30.7/xklb/scripts/redownload.py` & `xklb-1.31.2/xklb/scripts/redownload.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,25 +82,26 @@
             AND time_downloaded > 0
         """
         media = list(args.db.query(query, (args.deleted_at,)))
     return media
 
 
 def mark_media_undownloaded(args, deleted_media) -> None:
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
 
     media = deepcopy(deleted_media)
     for d in media:
         d["time_deleted"] = 0
         d["time_modified"] = 0
         d["time_downloaded"] = 0
         d.pop("error", None)
 
         if "webpath" in m_columns and (d.get("webpath") or "").startswith("http"):
-            args.db["media"].delete(d["path"])  # type: ignore
+            with args.db.conn:
+                args.db.conn.execute("DELETE from media WHERE path = ?", d["path"])
 
             d["path"] = d["webpath"]
             args.db["media"].upsert(d, pk="id", alter=True)  # type: ignore
         else:
             args.db["media"].upsert(d, pk="id", alter=True)  # type: ignore
 
 
@@ -134,15 +135,15 @@
     else:
         deletions = list_deletions(args)
         print_deletions(args, deletions)
         raise SystemExit(0)
 
     print_deleted(args, deleted_media)
     paths = [d["path"] for d in deleted_media]
-    redownload_ids = [d["tube_id"] for d in deleted_media if d.get("tube_id")]
+    redownload_ids = [d["extractor_id"] for d in deleted_media if d.get("extractor_id")]
     print(len(redownload_ids), "tube ids found")
     if deleted_media and utils.confirm("Redownload media?"):  # type: ignore
         if len(redownload_ids) > 0:
             download_archive = Path(args.download_archive).expanduser().resolve()
             if download_archive.exists():
                 utils.filter_file(str(download_archive), redownload_ids)
```

### Comparing `xklb-1.30.7/xklb/scripts/relmv.py` & `xklb-1.31.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/scatter.py` & `xklb-1.31.2/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/streaming_tab_loader.py` & `xklb-1.31.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/mining/data.py` & `xklb-1.31.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/mining/extract_links.py` & `xklb-1.31.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/mining/nouns.py` & `xklb-1.31.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/mining/pushshift.py` & `xklb-1.31.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.31.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, html
 from typing import Set, Tuple
 from urllib.parse import urlparse
 
-from xklb import db, usage, utils
+from xklb import db, media, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library reddit-selftext", usage=usage.reddit_selftext)
     parser.add_argument("database")
     parser.add_argument("--verbose", "-v", action="count", default=0)
@@ -38,15 +38,15 @@
     return internal_links, external_links
 
 
 def reddit_selftext() -> None:
     from markdown import markdown
 
     args = parse_args()
-    m_columns = args.db["media"].columns_dict
+    m_columns = db.columns(args, "media")
 
     reddit_posts = list(
         args.db.query(
             f"""
             select path, selftext
             from reddit_posts
             where 1=1
@@ -59,12 +59,12 @@
         html_data = markdown(d["selftext"])
         internal_links, external_links = get_page_links(d["path"], html_data)
         if internal_links:
             for i_link in internal_links:
                 log.info(i_link)
 
         for e_link in external_links:
-            args.db["media"].upsert({**d, "path": e_link, "webpage": d["path"]}, pk="path", alter=True)
+            media._add(args, {**d, "path": e_link, "webpage": d["path"]})
 
 
 if __name__ == "__main__":
     reddit_selftext()
```

### Comparing `xklb-1.30.7/xklb/assets/kotobago.png` & `xklb-1.31.2/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/.gitignore` & `xklb-1.31.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/LICENSE` & `xklb-1.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.30.7/README.md` & `xklb-1.31.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 And you can always add more later--even from different websites.
 
     library tubeadd maker.db https://vimeo.com/terburg
 
 To prevent mistakes the default configuration is to download metadata for only
 the most recent 20,000 videos per playlist/channel.
 
-    library tubeadd maker.db --dl-config playlistend=1000
+    library tubeadd maker.db --extractor-config playlistend=1000
 
 Be aware that there are some YouTube Channels which have many items--for example
 the TEDx channel has about 180,000 videos. Some channels even have upwards of
 two million videos. More than you could likely watch in one sitting--maybe even one lifetime.
 On a high-speed connection (>500 Mbps), it can take up to five hours to download
 the metadata for 180,000 videos.
 
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.007)
+    xk media library subcommands (v1.31.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -167,14 +167,17 @@
       lb merge-dbs             Merge multiple SQLITE files
       lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
+      lb galleryadd            Create a gallery database; Add albums
+      lb galleryupdate         Fetch new images from saved playlists
+
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
@@ -570,33 +573,29 @@
 
 
 </details>
 
 <details><summary>Add online media (tubeadd)</summary>
 
     $ library tubeadd -h
-    usage: library tubeadd [-c CATEGORY] [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+    usage: library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
-    You can also include a category for file organization
-
-        library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
-
-    Files will be saved to <download prefix>/<tubeadd category>/
+    Files will be saved to <download prefix>/<extractor>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -655,15 +654,15 @@
 
 
 </details>
 
 <details><summary>Add tabs (tabsadd)</summary>
 
     $ library tabsadd -h
-    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
+    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -1165,15 +1164,15 @@
 
         library download dl.db --prefix ~/output/path/root/
 
     Download stuff in a random order, limited to the specified playlist URLs.
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
-    Files will be saved to <lb download prefix>/<lb download category>/
+    Files will be saved to <lb download prefix>/<extractor>/
 
         For example:
         library dladd Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Print list of queued up downloads
@@ -1183,71 +1182,67 @@
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
         library download-status audio.db
-        ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
-        │                     │            │ and 20 minutes   │                    │          │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
-        ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key     │ duration         │   never_downloaded │   errors │
+        ╞════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Soundcloud │                  │                 10 │        0 │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
+        │            │ and 20 minutes   │                    │          │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 7.68 minutes     │                 99 │        1 │
+        ╘════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
 <details><summary>Download Status (download-status)</summary>
 
     $ library download-status -h
     usage: library download-status DATABASE
 
     Print download queue groups
 
         library download-status video.db
-        ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
-        │                     │             │ and 6 minutes    │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Dailymotion         │ Dailymotion │                  │                186 │      198 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Uncategorized       │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Vimeo               │ Vimeo       │                  │                253 │       49 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Youtube             │ Youtube     │ 2 years, 4       │              51676 │      197 │
-        │                     │             │ months, 15 days  │                    │          │
-        │                     │             │ and 6 hours      │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
-        │                     │             │ days, 19 hours   │                    │          │
-        │                     │             │ and 33 minutes   │                    │          │
-        ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒═════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key      │ duration         │   never_downloaded │   errors │
+        ╞═════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                 53 │        0 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
+        │             │ and 6 minutes    │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                186 │      198 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Vimeo       │                  │                253 │       49 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 2 years, 4       │              51676 │      197 │
+        │             │ months, 15 days  │                    │          │
+        │             │ and 6 hours      │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 4 months, 23     │               2686 │        7 │
+        │             │ days, 19 hours   │                    │          │
+        │             │ and 33 minutes   │                    │          │
+        ╘═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
         library download-status video.db --safe
 
-    Show only download attempts with errors
-
-        library download-status video.db --errors
-
 
 </details>
 
 <details><summary>Update local media (fsupdate)</summary>
 
     $ library fsupdate -h
     usage: library fsupdate DATABASE
@@ -1258,24 +1253,20 @@
 
 
 </details>
 
 <details><summary>Update online media (tubeupdate)</summary>
 
     $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] [-c CATEGORY] DATABASE
+    usage: library tubeupdate [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
-    Or limit to specific categories...
-
-        library tubeupdate -c "Bob Ross" educational.db
-
     Run with --optimize to add indexes (might speed up searching but the size will increase):
 
         library tubeupdate --optimize examples/music.tl.db
 
     Fetch extra metadata:
 
         By default tubeupdate will quickly add media.
@@ -1285,15 +1276,15 @@
 
 
 </details>
 
 <details><summary>Update reddit media (redditupdate)</summary>
 
     $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 
 
 </details>
@@ -1326,24 +1317,24 @@
     $ library playlists -h
     usage: library playlists DATABASE [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
-        │ ie_key   │ title              │ path                                                                     │
+        │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╛
 
     Aggregate Report of Videos in each Playlist
 
         library playlists -p a
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╤═══════════════╤═════════╕
-        │ ie_key   │ title              │ path                                                                     │ duration      │   count │
+        │ extractor_key   │ title              │ path                                                                     │ duration      │   count │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╪═══════════════╪═════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │ 53.28 minutes │      15 │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╧═══════════════╧═════════╛
         1 playlist
         Total duration: 53.28 minutes
 
     Print only playlist urls:
@@ -1509,15 +1500,15 @@
 
     Merge database data and tables
 
         library merge-dbs --upsert --pk path video.db tv.db movies.db
         library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path audio-fts.db audio.db
 
         library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
-        library merge-dbs --only-new-rows --pk playlist_path,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 
 
 </details>
 
 <details><summary>Sort lines by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
```

### Comparing `xklb-1.30.7/pyproject.toml` & `xklb-1.31.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [project]
 authors = [
   {name = "Jacob Chapman", email = "7908073+chapmanjacobd@users.noreply.github.com"},
 ]
 dependencies = [
-  'sqlite-utils >=3.30',
-  'catt',
-  'ffmpeg-python',
-  'ftfy',
-  'gallery-dl',
-  'humanize',
-  'ipython',
-  'Markdown',
-  'mutagen',
-  'natsort',
-  'praw',
-  'pysubs2',
-  'python-mpv-jsonipc',
-  'regex',
-  'rich',
-  'screeninfo',
-  'subliminal',
-  'tabulate',
-  'tinytag',
-  'yt-dlp',
+    'sqlite-utils >=3.30',
+    'catt',
+    'ffmpeg-python',
+    'ftfy',
+    'gallery-dl',
+    'humanize',
+    'ipython',
+    'Markdown',
+    'mutagen',
+    'natsort',
+    'praw',
+    'pysubs2',
+    'python-mpv-jsonipc',
+    'regex',
+    'rich',
+    'screeninfo',
+    'subliminal',
+    'tabulate',
+    'tinytag',
+    'yt-dlp',
+    "python-dateutil",
 ]
 description = "xk library"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "xklb"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -78,22 +79,26 @@
 profile = "black"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/*" = ["ANN201", "PLR2004"]
 
 [tool.ruff]
+unfixable = ["F841"]
+
 ignore = [
   "ANN001",
   "ANN002",
   "ANN003",
   "ANN101",
   "ANN204",
   "BLE001",
+  "C400",
   "C401",
+  "C405",
   "C901",
   "D100",
   "D101",
   "D102",
   "D103",
   "D104",
   "D107",
```

### Comparing `xklb-1.30.7/PKG-INFO` & `xklb-1.31.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.30.7
+Version: 1.31.2
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -47,14 +47,15 @@
 Requires-Dist: humanize
 Requires-Dist: ipython
 Requires-Dist: markdown
 Requires-Dist: mutagen
 Requires-Dist: natsort
 Requires-Dist: praw
 Requires-Dist: pysubs2
+Requires-Dist: python-dateutil
 Requires-Dist: python-mpv-jsonipc
 Requires-Dist: regex
 Requires-Dist: rich
 Requires-Dist: screeninfo
 Requires-Dist: sqlite-utils>=3.30
 Requires-Dist: subliminal
 Requires-Dist: tabulate
@@ -141,15 +142,15 @@
 And you can always add more later--even from different websites.
 
     library tubeadd maker.db https://vimeo.com/terburg
 
 To prevent mistakes the default configuration is to download metadata for only
 the most recent 20,000 videos per playlist/channel.
 
-    library tubeadd maker.db --dl-config playlistend=1000
+    library tubeadd maker.db --extractor-config playlistend=1000
 
 Be aware that there are some YouTube Channels which have many items--for example
 the TEDx channel has about 180,000 videos. Some channels even have upwards of
 two million videos. More than you could likely watch in one sitting--maybe even one lifetime.
 On a high-speed connection (>500 Mbps), it can take up to five hours to download
 the metadata for 180,000 videos.
 
@@ -223,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.007)
+    xk media library subcommands (v1.31.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -251,14 +252,17 @@
       lb merge-dbs             Merge multiple SQLITE files
       lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
+      lb galleryadd            Create a gallery database; Add albums
+      lb galleryupdate         Fetch new images from saved playlists
+
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
@@ -654,33 +658,29 @@
 
 
 </details>
 
 <details><summary>Add online media (tubeadd)</summary>
 
     $ library tubeadd -h
-    usage: library tubeadd [-c CATEGORY] [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+    usage: library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
-    You can also include a category for file organization
-
-        library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
-
-    Files will be saved to <download prefix>/<tubeadd category>/
+    Files will be saved to <download prefix>/<extractor>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -739,15 +739,15 @@
 
 
 </details>
 
 <details><summary>Add tabs (tabsadd)</summary>
 
     $ library tabsadd -h
-    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
+    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -1249,15 +1249,15 @@
 
         library download dl.db --prefix ~/output/path/root/
 
     Download stuff in a random order, limited to the specified playlist URLs.
 
         library download dl.db https://www.youtube.com/c/BlenderFoundation/videos
 
-    Files will be saved to <lb download prefix>/<lb download category>/
+    Files will be saved to <lb download prefix>/<extractor>/
 
         For example:
         library dladd Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Print list of queued up downloads
@@ -1267,71 +1267,67 @@
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
         library download-status audio.db
-        ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
-        │                     │            │ and 20 minutes   │                    │          │
-        ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
-        ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key     │ duration         │   never_downloaded │   errors │
+        ╞════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Soundcloud │                  │                 10 │        0 │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
+        │            │ and 20 minutes   │                    │          │
+        ├────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube    │ 7.68 minutes     │                 99 │        1 │
+        ╘════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
 <details><summary>Download Status (download-status)</summary>
 
     $ library download-status -h
     usage: library download-status DATABASE
 
     Print download queue groups
 
         library download-status video.db
-        ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
-        │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
-        ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
-        │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ 75_MovieQueue       │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
-        │                     │             │ and 6 minutes    │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Dailymotion         │ Dailymotion │                  │                186 │      198 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Uncategorized       │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
-        │                     │             │ minutes          │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Vimeo               │ Vimeo       │                  │                253 │       49 │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Youtube             │ Youtube     │ 2 years, 4       │              51676 │      197 │
-        │                     │             │ months, 15 days  │                    │          │
-        │                     │             │ and 6 hours      │                    │          │
-        ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
-        │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
-        │                     │             │ days, 19 hours   │                    │          │
-        │                     │             │ and 33 minutes   │                    │          │
-        ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
+        ╒═════════════╤══════════════════╤════════════════════╤══════════╕
+        │ extractor_key      │ duration         │   never_downloaded │   errors │
+        ╞═════════════╪══════════════════╪════════════════════╪══════════╡
+        │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                 53 │        0 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 day, 18 hours  │                 30 │        0 │
+        │             │ and 6 minutes    │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Dailymotion │                  │                186 │      198 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 1 hour and 52.18 │                  1 │        0 │
+        │             │ minutes          │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Vimeo       │                  │                253 │       49 │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 2 years, 4       │              51676 │      197 │
+        │             │ months, 15 days  │                    │          │
+        │             │ and 6 hours      │                    │          │
+        ├─────────────┼──────────────────┼────────────────────┼──────────┤
+        │ Youtube     │ 4 months, 23     │               2686 │        7 │
+        │             │ days, 19 hours   │                    │          │
+        │             │ and 33 minutes   │                    │          │
+        ╘═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
         library download-status video.db --safe
 
-    Show only download attempts with errors
-
-        library download-status video.db --errors
-
 
 </details>
 
 <details><summary>Update local media (fsupdate)</summary>
 
     $ library fsupdate -h
     usage: library fsupdate DATABASE
@@ -1342,24 +1338,20 @@
 
 
 </details>
 
 <details><summary>Update online media (tubeupdate)</summary>
 
     $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] [-c CATEGORY] DATABASE
+    usage: library tubeupdate [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
-    Or limit to specific categories...
-
-        library tubeupdate -c "Bob Ross" educational.db
-
     Run with --optimize to add indexes (might speed up searching but the size will increase):
 
         library tubeupdate --optimize examples/music.tl.db
 
     Fetch extra metadata:
 
         By default tubeupdate will quickly add media.
@@ -1369,15 +1361,15 @@
 
 
 </details>
 
 <details><summary>Update reddit media (redditupdate)</summary>
 
     $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [-c CATEGORY] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 
 
 </details>
@@ -1410,24 +1402,24 @@
     $ library playlists -h
     usage: library playlists DATABASE [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
-        │ ie_key   │ title              │ path                                                                     │
+        │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╛
 
     Aggregate Report of Videos in each Playlist
 
         library playlists -p a
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╤═══════════════╤═════════╕
-        │ ie_key   │ title              │ path                                                                     │ duration      │   count │
+        │ extractor_key   │ title              │ path                                                                     │ duration      │   count │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╪═══════════════╪═════════╡
         │ Youtube  │ Highlights of Life │ https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n │ 53.28 minutes │      15 │
         ╘══════════╧════════════════════╧══════════════════════════════════════════════════════════════════════════╧═══════════════╧═════════╛
         1 playlist
         Total duration: 53.28 minutes
 
     Print only playlist urls:
@@ -1593,15 +1585,15 @@
 
     Merge database data and tables
 
         library merge-dbs --upsert --pk path video.db tv.db movies.db
         library merge-dbs --only-target-columns --only-new-rows --table media,playlists --pk path audio-fts.db audio.db
 
         library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
-        library merge-dbs --only-new-rows --pk playlist_path,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
+        library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 
 
 </details>
 
 <details><summary>Sort lines by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
```

