# Comparing `tmp/udn_songbook-1.1.5.tar.gz` & `tmp/udn_songbook-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udn_songbook-1.1.5.tar", max compression
+gzip compressed data, was "udn_songbook-1.1.6.tar", max compression
```

## Comparing `udn_songbook-1.1.5.tar` & `udn_songbook-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1662 2023-06-13 21:16:36.155514 udn_songbook-1.1.5/CHANGELOG.md
--rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1476 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       91 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/__init__.py
--rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/book.py
--rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.5/udn_songbook/filters.py
--rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.5/udn_songbook/renderer.py
--rw-r--r--   0        0        0    19925 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/song.py
--rw-r--r--   0        0        0     2771 2023-05-05 10:02:10.537804 udn_songbook-1.1.5/udn_songbook/stylesheets/pdf.css
--rw-r--r--   0        0        0     3517 2023-05-05 10:02:10.537804 udn_songbook-1.1.5/udn_songbook/stylesheets/responsive.css
--rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.5/udn_songbook/stylesheets/ukedown_elements.css
--rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/templates/base.html.j2
--rw-r--r--   0        0        0     1062 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/templates/index.html.j2
--rw-r--r--   0        0        0     1298 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/templates/song.html.j2
--rwxr-xr-x   0        0        0     2778 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/tools/makesheet.py
--rwxr-xr-x   0        0        0     1990 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/tools/transpose.py
--rw-r--r--   0        0        0     1037 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/utils.py
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 udn_songbook-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1662 2023-06-13 21:42:22.016696 udn_songbook-1.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     1731 2023-05-03 20:57:17.787425 udn_songbook-1.1.6/README.md
+-rw-r--r--   0        0        0     1500 2023-06-13 21:44:59.278514 udn_songbook-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/__init__.py
+-rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.6/udn_songbook/book.py
+-rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.6/udn_songbook/filters.py
+-rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.6/udn_songbook/renderer.py
+-rw-r--r--   0        0        0    19925 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/song.py
+-rw-r--r--   0        0        0     2771 2023-05-05 10:02:10.537804 udn_songbook-1.1.6/udn_songbook/stylesheets/pdf.css
+-rw-r--r--   0        0        0     3517 2023-05-05 10:02:10.537804 udn_songbook-1.1.6/udn_songbook/stylesheets/responsive.css
+-rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.6/udn_songbook/stylesheets/ukedown_elements.css
+-rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.6/udn_songbook/templates/base.html.j2
+-rw-r--r--   0        0        0     1062 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/templates/index.html.j2
+-rw-r--r--   0        0        0     1298 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/templates/song.html.j2
+-rwxr-xr-x   0        0        0     2778 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/tools/makesheet.py
+-rwxr-xr-x   0        0        0     1990 2023-06-13 21:42:22.018696 udn_songbook-1.1.6/udn_songbook/tools/transpose.py
+-rw-r--r--   0        0        0     1037 2023-06-13 21:16:36.157514 udn_songbook-1.1.6/udn_songbook/utils.py
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 udn_songbook-1.1.6/PKG-INFO
```

### Comparing `udn_songbook-1.1.5/CHANGELOG.md` & `udn_songbook-1.1.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/LICENSE.txt` & `udn_songbook-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/pyproject.toml` & `udn_songbook-1.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "udn-songbook"
-version = "1.1.5"
+version = "1.1.6"
 description = "songbook and songsheet management for songsheets in ukedown format"
 authors = ["Stuart Sears <stuart@sjsears.com>"]
 include = ["CHANGELOG.md"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/lanky/udn-songbook"
-
+readme = [ "README.md" ]
 [tool.poetry.scripts]
 udn_transpose = "udn_songbook.tools.transpose:main"
 udn_songsheet = "udn_songbook.tools.makesheet:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ukedown = "^2.0.0"
```

### Comparing `udn_songbook-1.1.5/udn_songbook/book.py` & `udn_songbook-1.1.6/udn_songbook/book.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/filters.py` & `udn_songbook-1.1.6/udn_songbook/filters.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/renderer.py` & `udn_songbook-1.1.6/udn_songbook/renderer.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/song.py` & `udn_songbook-1.1.6/udn_songbook/song.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/stylesheets/pdf.css` & `udn_songbook-1.1.6/udn_songbook/stylesheets/pdf.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/stylesheets/responsive.css` & `udn_songbook-1.1.6/udn_songbook/stylesheets/responsive.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/stylesheets/ukedown_elements.css` & `udn_songbook-1.1.6/udn_songbook/stylesheets/ukedown_elements.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/templates/base.html.j2` & `udn_songbook-1.1.6/udn_songbook/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/templates/index.html.j2` & `udn_songbook-1.1.6/udn_songbook/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/templates/song.html.j2` & `udn_songbook-1.1.6/udn_songbook/templates/song.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/tools/makesheet.py` & `udn_songbook-1.1.6/udn_songbook/tools/makesheet.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/tools/transpose.py` & `udn_songbook-1.1.6/udn_songbook/tools/transpose.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.5/udn_songbook/utils.py` & `udn_songbook-1.1.6/udn_songbook/utils.py`

 * *Files identical despite different names*

