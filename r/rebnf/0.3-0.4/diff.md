# Comparing `tmp/rebnf-0.3.tar.gz` & `tmp/rebnf-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebnf-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rebnf-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rebnf-0.3.tar` & `rebnf-0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.3/LICENSE.md
--rw-r--r--   0        0        0     2678 2023-06-13 15:30:49.042837 rebnf-0.3/README.md
--rw-r--r--   0        0        0      592 2023-06-13 16:28:03.581041 rebnf-0.3/pyproject.toml
--rw-r--r--   0        0        0     1813 2023-06-13 16:11:30.112109 rebnf-0.3/rebnf/__init__.py
--rw-r--r--   0        0        0     1474 2023-06-13 16:12:48.740888 rebnf-0.3/rebnf/__main__.py
--rw-r--r--   0        0        0     3347 2023-06-13 16:20:46.776221 rebnf-0.3/rebnf/lexers.py
--rw-r--r--   0        0        0     4272 2023-06-13 15:44:42.734837 rebnf-0.3/rebnf/parsers.py
--rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 rebnf-0.3/PKG-INFO
+-rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.4/LICENSE.md
+-rw-r--r--   0        0        0     2783 2023-06-13 17:12:31.751347 rebnf-0.4/README.md
+-rw-r--r--   0        0        0      598 2023-06-13 16:35:44.463249 rebnf-0.4/pyproject.toml
+-rw-r--r--   0        0        0     1813 2023-06-13 17:12:23.407555 rebnf-0.4/rebnf/__init__.py
+-rw-r--r--   0        0        0     1474 2023-06-13 16:12:48.740888 rebnf-0.4/rebnf/__main__.py
+-rw-r--r--   0        0        0     3347 2023-06-13 16:20:46.776221 rebnf-0.4/rebnf/lexers.py
+-rw-r--r--   0        0        0     4272 2023-06-13 15:44:42.734837 rebnf-0.4/rebnf/parsers.py
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 rebnf-0.4/PKG-INFO
```

### Comparing `rebnf-0.3/LICENSE.md` & `rebnf-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rebnf-0.3/README.md` & `rebnf-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,49 @@
-<p align="center">
-  <a href="https://gitlab.com/opsocket/rebnf">
-    <img alt="opsocket" height="100" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
+Metadata-Version: 2.1
+Name: rebnf
+Version: 0.4
+Summary: __init__.py - Package for the rebnf language
+Author-email: opsocket <opsocket@pm.me>
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Dist: ply
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: twine ; extra == "dev"
+Project-URL: Repository, https://gitlab.com/opsocket/rebnf.git
+Provides-Extra: dev
+Provides-Extra: docs
+
+# ReBNF
+
+<div>
+  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.4-ec3832.svg?color=ec3832&style=flat"/></a>
+  <a href="https://opsocket.com" style="text-decoration: none;">
+    <img alt="opsocket" height="42" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
   </a>
-  <br>
-  <br>
-  <img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.0.3-ec3832.svg?color=ec3832&style=flat" />
-</p>
+</div>
+
+
+**ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to define the
+syntax of a language using regular expressions.
+
+It is an extension of the EBNF (Extended Backus-Naur Form) notation, allowing
+for more flexibility and ease of use.
 
 ```
 ooooooooo.             oooooooooo.  ooooo      ooo oooooooooooo 
 `888   `Y88.           `888'   `Y8b `888b.     `8' `888'     `8 
  888   .d88'  .ooooo.   888     888  8 `88b.    8   888         
  888ooo88P'  d88' `88b  888oooo888'  8   `88b.  8   888oooo8    
  888`88b.    888ooo888  888    `88b  8     `88b.8   888    "    
  888  `88b.  888    .o  888    .88P  8       `888   888         
 o888o  o888o `Y8bod8P' o888bood8P'  o8o        `8  o888o       
 ```
 
-ReBNF (Regexes for Extended Backus-Naur Form) is a notation used to define the
-syntax of a language using regular expressions. 
-
-It is an extension of the EBNF (Extended Backus-Naur Form) notation, allowing
-for more flexibility and ease of use.
-
 ## Table of Contents
 
 - [Syntax](#syntax)
 - [Example](#example)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
@@ -70,8 +87,12 @@
 
 Contributions are welcome! If you have suggestions, improvements, or new ideas
 related to the **ReBNF** notation, please feel free to open an issue or submit a
 pull request.
 
 ## License
 
-This project is licensed under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) license - see [LICENSE.md](LICENSE.md) for details..
+This project is licensed under the [GPLv3][#gplv3] license - see [LICENSE.md][#license] for details..
+
+[#gplv3]: https://www.gnu.org/licenses/gpl-3.0.html
+[#license]: https://gitlab.com/opsocket/rebnf/-/blob/main/LICENSE.md
+
```

#### html2text {}

```diff
@@ -1,32 +1,40 @@
-                                  [opsocket]
-
-          [https://img.shields.io/badge/%F0%9F%94%96%20Version-0.0.3-
-                      ec3832.svg?color=ec3832&style=flat]
-``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88. `888' `Y8b `888b.
-`8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888 888ooo88P' d88' `88b
-888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b 8 `88b.8 888 " 888
-`88b. 888 .o 888 .88P 8 `888 888 o888o o888o `Y8bod8P' o888bood8P' o8o `8 o888o
-``` ReBNF (Regexes for Extended Backus-Naur Form) is a notation used to define
-the syntax of a language using regular expressions. It is an extension of the
-EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility and
-ease of use. ## Table of Contents - [Syntax](#syntax) - [Example](#example) -
-[Usage](#usage) - [Contributing](#contributing) - [License](#license) ## Syntax
-The **ReBNF** notation uses regular expressions to define the structure of a
-language. Each *rule* consists of a *left-hand side* (non-terminal) and a
-*right-hand side* separated by an **assignment operator** (either `::=`, `:=`
-or `=`). The general syntax of a **ReBNF** rule is as follows: ```  ::= r"[a-
-zA-Z0-9]" ; # any alphanumeric characters ``` ## Example Here's a short example
-of a **ReBNF** definition for a simple arithmetic expression language: ```
-expression = term { ('+' | '-') term } term = factor { ('*' | '/') factor }
-factor = number | expression number = r'\d+' ``` ## Usage **ReBNF** notation is
-used to define the syntax of programming languages, configuration file formats,
-or any other formal language. It provides a concise and powerful way to express
-language structures with a addition of regular expressions. > Note that the
-functions in this module are only designed to parse syntactically valid
-**ReBNF** code (code that does not raise when parsed using `parse()`). The
-behavior of the functions in this module is undefined when providing invalid
-**ReBNF** code and it can change at any point. ## Contributing Contributions
-are welcome! If you have suggestions, improvements, or new ideas related to the
-**ReBNF** notation, please feel free to open an issue or submit a pull request.
-## License This project is licensed under the [GPLv3](https://www.gnu.org/
-licenses/gpl-3.0.html) license - see [LICENSE.md](LICENSE.md) for details..
+Metadata-Version: 2.1 Name: rebnf Version: 0.4 Summary: __init__.py - Package
+for the rebnf language Author-email: opsocket
+pm.me> Description-Content-Type: text/markdown Classifier: License :: OSI
+Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist: ply
+Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev" Requires-Dist: twine ; extra == "dev"
+Project-URL: Repository, https://gitlab.com/opsocket/rebnf.git Provides-Extra:
+dev Provides-Extra: docs # ReBNF
+[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.4-
+ec3832.svg?color=ec3832&style=flat] [opsocket]
+**ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to
+define the syntax of a language using regular expressions. It is an extension
+of the EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility
+and ease of use. ``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88.
+`888' `Y8b `888b. `8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888
+888ooo88P' d88' `88b 888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b
+8 `88b.8 888 " 888 `88b. 888 .o 888 .88P 8 `888 888 o888o o888o `Y8bod8P'
+o888bood8P' o8o `8 o888o ``` ## Table of Contents - [Syntax](#syntax) -
+[Example](#example) - [Usage](#usage) - [Contributing](#contributing) -
+[License](#license) ## Syntax The **ReBNF** notation uses regular expressions
+to define the structure of a language. Each *rule* consists of a *left-hand
+side* (non-terminal) and a *right-hand side* separated by an **assignment
+operator** (either `::=`, `:=` or `=`). The general syntax of a **ReBNF** rule
+is as follows: ```  ::= r"[a-zA-Z0-9]" ; # any alphanumeric characters ``` ##
+Example Here's a short example of a **ReBNF** definition for a simple
+arithmetic expression language: ``` expression = term { ('+' | '-') term } term
+= factor { ('*' | '/') factor } factor = number | expression number = r'\d+'
+``` ## Usage **ReBNF** notation is used to define the syntax of programming
+languages, configuration file formats, or any other formal language. It
+provides a concise and powerful way to express language structures with a
+addition of regular expressions. > Note that the functions in this module are
+only designed to parse syntactically valid **ReBNF** code (code that does not
+raise when parsed using `parse()`). The behavior of the functions in this
+module is undefined when providing invalid **ReBNF** code and it can change at
+any point. ## Contributing Contributions are welcome! If you have suggestions,
+improvements, or new ideas related to the **ReBNF** notation, please feel free
+to open an issue or submit a pull request. ## License This project is licensed
+under the [GPLv3][#gplv3] license - see [LICENSE.md][#license] for details..
+[#gplv3]: https://www.gnu.org/licenses/gpl-3.0.html [#license]: https://
+gitlab.com/opsocket/rebnf/-/blob/main/LICENSE.md
```

### Comparing `rebnf-0.3/pyproject.toml` & `rebnf-0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,11 +21,11 @@
   "black",
   "flake8",
   "flit",
   "twine"
 ]
 
 [project.urls]
-repo = "https://gitlab.com/opsocket/rebnf.git"
+Repository = "https://gitlab.com/opsocket/rebnf.git"
 
 [project.scripts]
 tokenize = "rebnf.__main__:main"
```

### Comparing `rebnf-0.3/rebnf/__init__.py` & `rebnf-0.4/rebnf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from . import lexers
 from . import parsers
 
 assert all((lexers, parsers))
 
 __author__ = "opsocket <opsocket@pm.me>"
 __description__ = "Lexer and parser for the ReBNF metasyntax language"
-__version__ = "0.3"
+__version__ = "0.4"
 __ascii__ = """
 ooooooooo.             oooooooooo.  ooooo      ooo oooooooooooo 
 `888   `Y88.           `888'   `Y8b `888b.     `8' `888'     `8 
  888   .d88'  .ooooo.   888     888  8 `88b.    8   888         
  888ooo88P'  d88' `88b  888oooo888'  8   `88b.  8   888oooo8    
  888`88b.    888ooo888  888    `88b  8     `88b.8   888    "    
  888  `88b.  888    .o  888    .88P  8       `888   888
```

### Comparing `rebnf-0.3/rebnf/__main__.py` & `rebnf-0.4/rebnf/__main__.py`

 * *Files identical despite different names*

### Comparing `rebnf-0.3/rebnf/lexers.py` & `rebnf-0.4/rebnf/lexers.py`

 * *Files identical despite different names*

### Comparing `rebnf-0.3/rebnf/parsers.py` & `rebnf-0.4/rebnf/parsers.py`

 * *Files identical despite different names*

