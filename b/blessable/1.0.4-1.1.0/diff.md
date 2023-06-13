# Comparing `tmp/blessable-1.0.4.tar.gz` & `tmp/blessable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blessable-1.0.4.tar", last modified: Mon Jun 12 02:54:26 2023, max compression
+gzip compressed data, was "blessable-1.1.0.tar", last modified: Tue Jun 13 00:51:38 2023, max compression
```

## Comparing `blessable-1.0.4.tar` & `blessable-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.262496 blessable-1.0.4/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1905 2023-06-12 02:54:26.262356 blessable-1.0.4/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1533 2023-06-12 02:54:11.000000 blessable-1.0.4/README.md
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.261413 blessable-1.0.4/blessable/
--rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.0.4/blessable/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)      624 2023-06-12 01:36:31.000000 blessable-1.0.4/blessable/blessable.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    15184 2023-06-12 00:48:54.000000 blessable-1.0.4/blessable/colormap.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.262158 blessable-1.0.4/blessable.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1905 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/top_level.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-12 02:54:26.262545 blessable-1.0.4/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      603 2023-06-12 02:54:23.000000 blessable-1.0.4/setup.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-13 00:51:38.636863 blessable-1.1.0/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1708 2023-06-13 00:51:38.636717 blessable-1.1.0/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1336 2023-06-13 00:51:28.000000 blessable-1.1.0/README.md
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-13 00:51:38.635921 blessable-1.1.0/blessable/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.1.0/blessable/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      564 2023-06-13 00:51:28.000000 blessable-1.1.0/blessable/blessable.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)    15261 2023-06-13 00:51:28.000000 blessable-1.1.0/blessable/colormap.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-13 00:51:38.636546 blessable-1.1.0/blessable.egg-info/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1708 2023-06-13 00:51:38.000000 blessable-1.1.0/blessable.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-13 00:51:38.000000 blessable-1.1.0/blessable.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-13 00:51:38.000000 blessable-1.1.0/blessable.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-13 00:51:38.000000 blessable-1.1.0/blessable.egg-info/requires.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-13 00:51:38.000000 blessable-1.1.0/blessable.egg-info/top_level.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-13 00:51:38.636911 blessable-1.1.0/setup.cfg
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      603 2023-06-13 00:51:28.000000 blessable-1.1.0/setup.py
```

### Comparing `blessable-1.0.4/PKG-INFO` & `blessable-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blessable
-Version: 1.0.4
+Version: 1.1.0
 Summary: "Blessable" - a simple markup language for Blessings.
 Home-page: https://github.com/fakerybakery/blessable
 Author: www.mrfake.name
 Project-URL: Bug Reports, https://github.com/fakerybakery/blessable/issues
 Project-URL: Source, https://github.com/fakerybakery/blessable
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, install the packages:
+First, install the package:
 
 ```python
 pip install blessable # or python -m pip install blessable
 ```
 
 Then, import the `blessable` module:
 
@@ -58,35 +58,17 @@
 
 ```html
 The Blessed library is truly <red>amazing</red>, with <blue>Windows, Mac, and Linux Support</blue> all built-in!
 ```
 
 ## Supported Colors
 
-The following colors are supported, as well as `color_on_color`, e.g. `white_on_blue`:
-
- - `black`
- - `red`
- - `green`
- - `yellow`
- - `blue`
- - `magenta`
- - `cyan`
- - `white`
- - `bright_black`
- - `bright_red`
- - `bright_green`
- - `bright_yellow`
- - `bright_blue`
- - `bright_magenta`
- - `bright_cyan`
- - `bright_white`
-
-In addition to these colors, we also supports the following non-colors:
-
- - `bold` (alias `b`)
- - `italic` (alias `i`)
- - `underline` (alias `u`)
+[Supported colors have been moved to our Wiki](https://github.com/fakerybakery/blessable/wiki/Documentation#supported-colors).
 
 ## To Do
 
  - [ ] Support nested styling
+ - [ ] Support escaping tags
+
+## FAQs
+
+Please see the [Wiki](https://github.com/fakerybakery/blessable/wiki) for FAQs, comparisons, and more.
```

### Comparing `blessable-1.0.4/README.md` & `blessable-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, install the packages:
+First, install the package:
 
 ```python
 pip install blessable # or python -m pip install blessable
 ```
 
 Then, import the `blessable` module:
 
@@ -48,35 +48,17 @@
 
 ```html
 The Blessed library is truly <red>amazing</red>, with <blue>Windows, Mac, and Linux Support</blue> all built-in!
 ```
 
 ## Supported Colors
 
-The following colors are supported, as well as `color_on_color`, e.g. `white_on_blue`:
-
- - `black`
- - `red`
- - `green`
- - `yellow`
- - `blue`
- - `magenta`
- - `cyan`
- - `white`
- - `bright_black`
- - `bright_red`
- - `bright_green`
- - `bright_yellow`
- - `bright_blue`
- - `bright_magenta`
- - `bright_cyan`
- - `bright_white`
-
-In addition to these colors, we also supports the following non-colors:
-
- - `bold` (alias `b`)
- - `italic` (alias `i`)
- - `underline` (alias `u`)
+[Supported colors have been moved to our Wiki](https://github.com/fakerybakery/blessable/wiki/Documentation#supported-colors).
 
 ## To Do
 
  - [ ] Support nested styling
+ - [ ] Support escaping tags
+
+## FAQs
+
+Please see the [Wiki](https://github.com/fakerybakery/blessable/wiki) for FAQs, comparisons, and more.
```

### Comparing `blessable-1.0.4/blessable/blessable.py` & `blessable-1.1.0/blessable/blessable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from .colormap import color_map
-
 class Blessable:
-    # def __init__(self):
-        # self.term = Terminal()
-
     def bless(self, markup):
         parts = markup.split('<')
         converted_markup = ''
         for part in parts:
             if '>' in part:
                 color_tag, text = part.split('>', 1)
                 color_tag = color_tag.strip()
                 if color_tag in color_map:
                     converted_markup += color_map[color_tag](text)
                 else:
                     converted_markup += text
             else:
                 converted_markup += part
-        return converted_markup
+        return converted_markup
```

### Comparing `blessable-1.0.4/blessable/colormap.py` & `blessable-1.1.0/blessable/colormap.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 color_map = {
     "bold": term.bold,
     "italic": term.italic,
     "underline": term.underline,
     "b": term.bold,
     "i": term.italic,
     "u": term.underline,
+    "left": term.ljust,
+    "right": term.rjust,
+    "center": term.center,
     "black": term.black,
     "black_on_black": term.black_on_black,
     "black_on_red": term.black_on_red,
     "black_on_green": term.black_on_green,
     "black_on_yellow": term.black_on_yellow,
     "black_on_blue": term.black_on_blue,
     "black_on_magenta": term.black_on_magenta,
@@ -275,8 +278,8 @@
     "bright_white_on_bright_red": term.bright_white_on_bright_red,
     "bright_white_on_bright_green": term.bright_white_on_bright_green,
     "bright_white_on_bright_yellow": term.bright_white_on_bright_yellow,
     "bright_white_on_bright_blue": term.bright_white_on_bright_blue,
     "bright_white_on_bright_magenta": term.bright_white_on_bright_magenta,
     "bright_white_on_bright_cyan": term.bright_white_on_bright_cyan,
     "bright_white_on_bright_white": term.bright_white_on_bright_white,
-}
+}
```

### Comparing `blessable-1.0.4/blessable.egg-info/PKG-INFO` & `blessable-1.1.0/blessable.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blessable
-Version: 1.0.4
+Version: 1.1.0
 Summary: "Blessable" - a simple markup language for Blessings.
 Home-page: https://github.com/fakerybakery/blessable
 Author: www.mrfake.name
 Project-URL: Bug Reports, https://github.com/fakerybakery/blessable/issues
 Project-URL: Source, https://github.com/fakerybakery/blessable
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, install the packages:
+First, install the package:
 
 ```python
 pip install blessable # or python -m pip install blessable
 ```
 
 Then, import the `blessable` module:
 
@@ -58,35 +58,17 @@
 
 ```html
 The Blessed library is truly <red>amazing</red>, with <blue>Windows, Mac, and Linux Support</blue> all built-in!
 ```
 
 ## Supported Colors
 
-The following colors are supported, as well as `color_on_color`, e.g. `white_on_blue`:
-
- - `black`
- - `red`
- - `green`
- - `yellow`
- - `blue`
- - `magenta`
- - `cyan`
- - `white`
- - `bright_black`
- - `bright_red`
- - `bright_green`
- - `bright_yellow`
- - `bright_blue`
- - `bright_magenta`
- - `bright_cyan`
- - `bright_white`
-
-In addition to these colors, we also supports the following non-colors:
-
- - `bold` (alias `b`)
- - `italic` (alias `i`)
- - `underline` (alias `u`)
+[Supported colors have been moved to our Wiki](https://github.com/fakerybakery/blessable/wiki/Documentation#supported-colors).
 
 ## To Do
 
  - [ ] Support nested styling
+ - [ ] Support escaping tags
+
+## FAQs
+
+Please see the [Wiki](https://github.com/fakerybakery/blessable/wiki) for FAQs, comparisons, and more.
```

### Comparing `blessable-1.0.4/setup.py` & `blessable-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open('README.md', 'r') as f:
     longdesc = f.read()
 setup(
     name='blessable',
-    version='1.0.4',
+    version='1.1.0',
     author='www.mrfake.name',
     description='"Blessable" - a simple markup language for Blessings.',
     long_description=longdesc,
     long_description_content_type='text/markdown',
     url='https://github.com/fakerybakery/blessable',
     packages=['blessable'],
     install_requires=['blessed'],
```

