# Comparing `tmp/udn_songbook-1.1.4.tar.gz` & `tmp/udn_songbook-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udn_songbook-1.1.4.tar", max compression
+gzip compressed data, was "udn_songbook-1.1.5.tar", max compression
```

## Comparing `udn_songbook-1.1.4.tar` & `udn_songbook-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      988 2023-06-13 21:37:23.946422 udn_songbook-1.1.4/CHANGELOG.md
--rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1458 2023-06-13 21:37:23.946422 udn_songbook-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       78 2023-06-13 21:37:23.947422 udn_songbook-1.1.4/udn_songbook/__init__.py
--rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.4/udn_songbook/book.py
--rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.4/udn_songbook/filters.py
--rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.4/udn_songbook/renderer.py
--rw-r--r--   0        0        0    19903 2023-06-13 21:37:23.947422 udn_songbook-1.1.4/udn_songbook/song.py
--rw-r--r--   0        0        0     2771 2023-05-05 10:02:10.537804 udn_songbook-1.1.4/udn_songbook/stylesheets/pdf.css
--rw-r--r--   0        0        0     3517 2023-05-05 10:02:10.537804 udn_songbook-1.1.4/udn_songbook/stylesheets/responsive.css
--rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.4/udn_songbook/stylesheets/ukedown_elements.css
--rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.4/udn_songbook/templates/base.html.j2
--rw-r--r--   0        0        0     1062 2023-06-13 21:16:36.156515 udn_songbook-1.1.4/udn_songbook/templates/index.html.j2
--rw-r--r--   0        0        0     1298 2023-06-13 21:16:36.157514 udn_songbook-1.1.4/udn_songbook/templates/song.html.j2
--rwxr-xr-x   0        0        0     1800 2023-06-13 21:37:23.947422 udn_songbook-1.1.4/udn_songbook/tools/makesheet.py
--rwxr-xr-x   0        0        0     1990 2023-06-13 21:16:36.157514 udn_songbook-1.1.4/udn_songbook/tools/transpose.py
--rw-r--r--   0        0        0     1037 2023-06-13 21:16:36.157514 udn_songbook-1.1.4/udn_songbook/utils.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 udn_songbook-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1662 2023-06-13 21:16:36.155514 udn_songbook-1.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0    35150 2023-05-03 20:57:17.787425 udn_songbook-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     1476 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/__init__.py
+-rw-r--r--   0        0        0     6944 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/book.py
+-rw-r--r--   0        0        0     1043 2023-05-05 10:02:10.536805 udn_songbook-1.1.5/udn_songbook/filters.py
+-rw-r--r--   0        0        0     3629 2023-05-25 22:09:08.574890 udn_songbook-1.1.5/udn_songbook/renderer.py
+-rw-r--r--   0        0        0    19925 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/song.py
+-rw-r--r--   0        0        0     2771 2023-05-05 10:02:10.537804 udn_songbook-1.1.5/udn_songbook/stylesheets/pdf.css
+-rw-r--r--   0        0        0     3517 2023-05-05 10:02:10.537804 udn_songbook-1.1.5/udn_songbook/stylesheets/responsive.css
+-rw-r--r--   0        0        0     1270 2023-05-05 10:02:10.538804 udn_songbook-1.1.5/udn_songbook/stylesheets/ukedown_elements.css
+-rw-r--r--   0        0        0     1517 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/templates/base.html.j2
+-rw-r--r--   0        0        0     1062 2023-06-13 21:16:36.156515 udn_songbook-1.1.5/udn_songbook/templates/index.html.j2
+-rw-r--r--   0        0        0     1298 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/templates/song.html.j2
+-rwxr-xr-x   0        0        0     2778 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/tools/makesheet.py
+-rwxr-xr-x   0        0        0     1990 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/tools/transpose.py
+-rw-r--r--   0        0        0     1037 2023-06-13 21:16:36.157514 udn_songbook-1.1.5/udn_songbook/utils.py
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 udn_songbook-1.1.5/PKG-INFO
```

### Comparing `udn_songbook-1.1.4/LICENSE.txt` & `udn_songbook-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/pyproject.toml` & `udn_songbook-1.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "udn-songbook"
-version = "1.1.4"
+version = "1.1.5"
 description = "songbook and songsheet management for songsheets in ukedown format"
 authors = ["Stuart Sears <stuart@sjsears.com>"]
 include = ["CHANGELOG.md"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/lanky/udn-songbook"
 
 [tool.poetry.scripts]
 udn_transpose = "udn_songbook.tools.transpose:main"
-udn_render = "udn_songbook.tools.makesheet:main"
+udn_songsheet = "udn_songbook.tools.makesheet:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ukedown = "^2.0.0"
 beautifulsoup4 = "^4.10.0"
 PyYAML = ">= 6"
 WeasyPrint = ">= 54.2"
 Markdown = "^3.3.6"
 Jinja2 = "^3.1.1"
 lxml = "^4.8.0"
 pychord = "^1.0.0"
 dynaconf = "^3.1.12"
 more-itertools = "^9.1.0"
+bs4 = "^0.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pre-commit = "^2.17.0"
 black = "^22.3.0"
 flake8 = "^4.0.1"
```

### Comparing `udn_songbook-1.1.4/udn_songbook/book.py` & `udn_songbook-1.1.5/udn_songbook/book.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/filters.py` & `udn_songbook-1.1.5/udn_songbook/filters.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/renderer.py` & `udn_songbook-1.1.5/udn_songbook/renderer.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/song.py` & `udn_songbook-1.1.5/udn_songbook/song.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,23 +104,23 @@
             self._filename = Path(os.path.basename(src))
             self._fsize = os.path.getsize(src)
             #
         else:
             # presume we've been given content
             self._markup = src
             self._fsize = len(src)
-
-        # does nothing yet
-        self._filename = src
-        self.__parse(markup=self._markup)
         # arbitrary metadata, some of which will have meaning
         self._meta = {}
         # tags are separate
         self._tags = set([])
 
+        # does nothing yet
+        self._filename = src
+        self.__parse(markup=self._markup)
+
         # update with any parameters...
         for key, val in kwargs.items():
             setattr(self, key, val)
 
         if self._filename is None:
             self._filename = ("{0.title}_-_{0.artist}.udn".format(self)).lower()
 
@@ -146,15 +146,15 @@
 
         sets:
             self._markup(str): text content, amy include metadata
             self._mod_time(datetime): last modified time, if any
             self.fsize(int): size of input in bytes.
         """
         try:
-            with codecs.open(sourcefile, mode="r", encoding="utf-8") as src:
+            with open(sourcefile, mode="r", encoding="utf-8") as src:
                 self._markup = src.read()
                 self._mod_time = datetime.datetime.fromtimestamp(
                     os.path.getmtime(sourcefile)
                 )
                 self.fsize = os.path.getsize(sourcefile)
 
         except (IOError, OSError) as E:
@@ -279,15 +279,16 @@
                 tail = m.groups()[1]
                 chord_locations.append([crd, m.end(), tail if tail is not None else ""])
                 if crd not in chordlist:
                     chordlist.append(crd)
             except ValueError:
                 # raised when this is not a recognised chord
                 print(
-                    f"Unable to parse chord {m.match} at position {m.start()} in song {self.filename}"
+                    f"""Unable to parse chord {m.match} at position {m.start()} 
+                        in song {self.filename}"""
                 )
                 raise
 
         # set attributes so we can access these elsewhere
         self._chord_locations = chord_locations
         self._chords = chordlist
```

### Comparing `udn_songbook-1.1.4/udn_songbook/stylesheets/pdf.css` & `udn_songbook-1.1.5/udn_songbook/stylesheets/pdf.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/stylesheets/responsive.css` & `udn_songbook-1.1.5/udn_songbook/stylesheets/responsive.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/stylesheets/ukedown_elements.css` & `udn_songbook-1.1.5/udn_songbook/stylesheets/ukedown_elements.css`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/templates/base.html.j2` & `udn_songbook-1.1.5/udn_songbook/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/templates/index.html.j2` & `udn_songbook-1.1.5/udn_songbook/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/templates/song.html.j2` & `udn_songbook-1.1.5/udn_songbook/templates/song.html.j2`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/udn_songbook/tools/makesheet.py` & `udn_songbook-1.1.5/udn_songbook/tools/transpose.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 #!/usr/bin/env python3
+# vim: set ts=4 sts=4 sw=4 et ci nu ft=python:
 import argparse
 import sys
-from pathlib import Path
 from typing import List
 
-from udn_songbook import Song
+from .song import Song
 
+"""
+A tool using the `udn_songbook` mechanisms to transpose songs by a given number of semitones
+"""
 
-def parse_cmdline(argv: List[str]) -> argparse.Namespace:
+
+def parse_cmdline(argv: List[str] = []) -> argparse.Namespace:
     """
-    Process commandline options and arguments, provide help
+    process commandline options and arguments
     """
-
-    preamble = """
-    Generates a PDF or HTML songsheet from a UDN input file
-
-    Files are generated in your CWD (current working directory),
-    unless you specify a path to an output file.
+    desc = """A tool using the `udn_songbook` toolset to transpose ukedown 
+    songsheets by a given number of semitones.
+    Can overwrite existing files if you want it to.
     """
+    parser = argparse.ArgumentParser(description=desc)
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument("filename", help="path to a filename in UDN format")
+    parser.add_argument(
+        "filenames", nargs="+", help="filename(s) in UDN(ukedown) format to transpose"
+    )
+    parser.add_argument(
+        "-t",
+        "--semitones",
+        type=int,
+        help="number of semitones to shift each chord by, can be negative",
+    )
     parser.add_argument(
         "-o",
         "--output",
-        help="name of output file, autogenerated from input filename if omitted",
+        help="output filename, will dump to stdout` if not specified."
+        "Will not work with more than one inputfile, for hopefully obvious reasons",
     )
-
     parser.add_argument(
-        "--html",
+        "-i",
+        "--in-place",
         action="store_true",
         default=False,
-        help="Create a songsheet in HTML format, rather than the default PDF",
-    )
-
-    parser.add_argument(
-        "--singers",
-        action="store_false",
-        default=True,
-        dest="chords",
-        help="Generate a singer's sheet (no chords)",
+        help="overwrite the input file with the transposed version. "
+        "Use this only if you are sure you want to",
     )
 
     opts = parser.parse_args(argv)
 
-    if opts.output:
-        opts.output = Path(opts.output)
-    else:
-        opts.output = (
-            Path(opts.filename).with_suffix(".html" if opts.html else ".pdf").name
+    if opts.output and len(opts.filenames) > 1:
+        raise argparse.ArgumentError(
+            "Cannot use --output with more than one input file."
         )
 
+    # sanity checking to be added
     return opts
 
 
 def main():
     """
-    Main functionality
+    Main script entrypoint
     """
     opts = parse_cmdline(sys.argv[1:])
 
-    song = Song(Path(opts.filename))
+    for fname in opts.filenames:
+        s = Song(fname)
+        s.transpose(opts.semitones)
+
+        if opts.in_place:
+            s.save(fname)
+
+        elif opts.output:
+            s.save(opts.output)
 
-    if opts.output.exists():
-        print(f"output file {opts.output} already exists")
-        sys.exit(1)
-
-    if opts.html:
-        with open(opts.output, "w") as dest:
-            dest.write(song.html(standalone=True))
-    else:
-        song.pdf(destfile=opts.output, chords=opts.chords)
+        else:
+            print(s.markup)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `udn_songbook-1.1.4/udn_songbook/utils.py` & `udn_songbook-1.1.5/udn_songbook/utils.py`

 * *Files identical despite different names*

### Comparing `udn_songbook-1.1.4/PKG-INFO` & `udn_songbook-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udn-songbook
-Version: 1.1.4
+Version: 1.1.5
 Summary: songbook and songsheet management for songsheets in ukedown format
 Home-page: https://github.com/lanky/udn-songbook
 License: GPL-3.0-or-later
 Author: Stuart Sears
 Author-email: stuart@sjsears.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.1,<4.0.0)
 Requires-Dist: Markdown (>=3.3.6,<4.0.0)
 Requires-Dist: PyYAML (>=6)
 Requires-Dist: WeasyPrint (>=54.2)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: pychord (>=1.0.0,<2.0.0)
 Requires-Dist: ukedown (>=2.0.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/lanky/udn-songbook/issues
 Project-URL: Repository, https://github.com/lanky/udn-songbook
```

