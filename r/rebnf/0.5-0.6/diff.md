# Comparing `tmp/rebnf-0.5.tar.gz` & `tmp/rebnf-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebnf-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rebnf-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rebnf-0.5.tar` & `rebnf-0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.5/LICENSE.md
--rw-r--r--   0        0        0     2783 2023-06-13 17:14:47.808448 rebnf-0.5/README.md
--rw-r--r--   0        0        0      598 2023-06-13 16:35:44.463249 rebnf-0.5/pyproject.toml
--rw-r--r--   0        0        0     1813 2023-06-13 17:23:10.303213 rebnf-0.5/rebnf/__init__.py
--rw-r--r--   0        0        0     1474 2023-06-13 16:12:48.740888 rebnf-0.5/rebnf/__main__.py
--rw-r--r--   0        0        0     3347 2023-06-13 16:20:46.776221 rebnf-0.5/rebnf/lexers.py
--rw-r--r--   0        0        0     4272 2023-06-13 15:44:42.734837 rebnf-0.5/rebnf/parsers.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 rebnf-0.5/PKG-INFO
+-rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.6/LICENSE.md
+-rw-r--r--   0        0        0     2783 2023-06-13 18:23:17.917564 rebnf-0.6/README.md
+-rw-r--r--   0        0        0     1159 2023-06-13 18:25:15.789248 rebnf-0.6/pyproject.toml
+-rw-r--r--   0        0        0     1813 2023-06-13 18:23:51.905464 rebnf-0.6/rebnf/__init__.py
+-rw-r--r--   0        0        0     1474 2023-06-13 16:12:48.740888 rebnf-0.6/rebnf/__main__.py
+-rw-r--r--   0        0        0     3347 2023-06-13 16:20:46.776221 rebnf-0.6/rebnf/lexers.py
+-rw-r--r--   0        0        0     4272 2023-06-13 15:44:42.734837 rebnf-0.6/rebnf/parsers.py
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rebnf-0.6/PKG-INFO
```

### Comparing `rebnf-0.5/LICENSE.md` & `rebnf-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rebnf-0.5/README.md` & `rebnf-0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ReBNF
 
 <div>
-  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.5-ec3832.svg?color=ec3832&style=flat"/></a>
+  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.6-ec3832.svg?color=ec3832&style=flat"/></a>
   <a href="https://opsocket.com" style="text-decoration: none;">
     <img alt="opsocket" height="42" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
   </a>
 </div>
 
 
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to define the
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # ReBNF
-[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.5-
+[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.6-
 ec3832.svg?color=ec3832&style=flat] [opsocket]
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to
 define the syntax of a language using regular expressions. It is an extension
 of the EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility
 and ease of use. ``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88.
 `888' `Y8b `888b. `8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888
 888ooo88P' d88' `88b 888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b
```

### Comparing `rebnf-0.5/rebnf/__init__.py` & `rebnf-0.6/rebnf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from . import lexers
 from . import parsers
 
 assert all((lexers, parsers))
 
 __author__ = "opsocket <opsocket@pm.me>"
 __description__ = "Lexer and parser for the ReBNF metasyntax language"
-__version__ = "0.5"
+__version__ = "0.6"
 __ascii__ = """
 ooooooooo.             oooooooooo.  ooooo      ooo oooooooooooo 
 `888   `Y88.           `888'   `Y8b `888b.     `8' `888'     `8 
  888   .d88'  .ooooo.   888     888  8 `88b.    8   888         
  888ooo88P'  d88' `88b  888oooo888'  8   `88b.  8   888oooo8    
  888`88b.    888ooo888  888    `88b  8     `88b.8   888    "    
  888  `88b.  888    .o  888    .88P  8       `888   888
```

### Comparing `rebnf-0.5/rebnf/__main__.py` & `rebnf-0.6/rebnf/__main__.py`

 * *Files identical despite different names*

### Comparing `rebnf-0.5/rebnf/lexers.py` & `rebnf-0.6/rebnf/lexers.py`

 * *Files identical despite different names*

### Comparing `rebnf-0.5/rebnf/parsers.py` & `rebnf-0.6/rebnf/parsers.py`

 * *Files identical despite different names*

### Comparing `rebnf-0.5/PKG-INFO` & `rebnf-0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: rebnf
-Version: 0.5
+Version: 0.6
 Summary: ReBNF: Regexes for Extended Backus-Naur Form
+Keywords: backus-naur form,bnf,context-free grammar,ebnf,extended backus-naur form,formal language,grammar,language,lexer,metasyntax,parser,parsing,rebnf,regex,regexes,syntax,text processing
 Author-email: opsocket <opsocket@pm.me>
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Topic :: Text Processing
 Requires-Dist: ply
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Project-URL: Repository, https://gitlab.com/opsocket/rebnf.git
 Provides-Extra: dev
 Provides-Extra: docs
 
 # ReBNF
 
 <div>
-  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.5-ec3832.svg?color=ec3832&style=flat"/></a>
+  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.6-ec3832.svg?color=ec3832&style=flat"/></a>
   <a href="https://opsocket.com" style="text-decoration: none;">
     <img alt="opsocket" height="42" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
   </a>
 </div>
 
 
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to define the
```

#### html2text {}

```diff
@@ -1,16 +1,23 @@
-Metadata-Version: 2.1 Name: rebnf Version: 0.5 Summary: ReBNF: Regexes for
-Extended Backus-Naur Form Author-email: opsocket
-pm.me> Description-Content-Type: text/markdown Classifier: License :: OSI
-Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist: ply
+Metadata-Version: 2.1 Name: rebnf Version: 0.6 Summary: ReBNF: Regexes for
+Extended Backus-Naur Form Keywords: backus-naur form,bnf,context-free
+grammar,ebnf,extended backus-naur form,formal
+language,grammar,language,lexer,metasyntax,parser,parsing,rebnf,regex,regexes,syntax,text
+processing Author-email: opsocket
+pm.me> Description-Content-Type: text/markdown Classifier: Development Status
+:: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
+OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Topic :: Software Development :: Libraries Classifier: Topic
+:: Software Development Classifier: Topic :: Text Processing Requires-Dist: ply
 Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev" Requires-Dist: twine ; extra == "dev"
 Project-URL: Repository, https://gitlab.com/opsocket/rebnf.git Provides-Extra:
 dev Provides-Extra: docs # ReBNF
-[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.5-
+[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.6-
 ec3832.svg?color=ec3832&style=flat] [opsocket]
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to
 define the syntax of a language using regular expressions. It is an extension
 of the EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility
 and ease of use. ``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88.
 `888' `Y8b `888b. `8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888
 888ooo88P' d88' `88b 888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b
```

