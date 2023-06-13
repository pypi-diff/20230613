# Comparing `tmp/lyrics_client-0.0.1.tar.gz` & `tmp/lyrics_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_client-0.0.1.tar", max compression
+gzip compressed data, was "lyrics_client-0.0.2.tar", max compression
```

## Comparing `lyrics_client-0.0.1.tar` & `lyrics_client-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     2085 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/README.md
--rw-r--r--   0        0        0      440 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/__init__.py
--rw-r--r--   0        0        0      159 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/__init__.py
--rw-r--r--   0        0        0      355 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/clients/__init__.py
--rw-r--r--   0        0        0     3975 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/clients/abstract_lyrics_client.py
--rw-r--r--   0        0        0     2723 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/clients/azlyrics_lyrics_client.py
--rw-r--r--   0        0        0     2575 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/clients/genius_lyrics_client.py
--rw-r--r--   0        0        0     2165 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/clients/musixmatch_lyrics_client.py
--rw-r--r--   0        0        0      245 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/fetch_lyrics_command.py
--rw-r--r--   0        0        0      209 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/classes/fetch_lyrics_result.py
--rw-r--r--   0        0        0       83 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/di/__init__.py
--rw-r--r--   0        0        0      520 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/di/dependency_injector.py
--rw-r--r--   0        0        0      211 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/errors/__init__.py
--rw-r--r--   0        0        0       71 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/errors/bad_format_error.py
--rw-r--r--   0        0        0       79 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/errors/bad_title_match_error.py
--rw-r--r--   0        0        0       69 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/errors/no_result_error.py
--rw-r--r--   0        0        0       81 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/interfaces/__init__.py
--rw-r--r--   0        0        0      240 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/interfaces/base_lyrics_client.py
--rw-r--r--   0        0        0      841 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/main.py
--rw-r--r--   0        0        0        0 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/lyrics_client/py.typed
--rw-r--r--   0        0        0     1341 2023-06-10 09:46:36.753299 lyrics_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 lyrics_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2093 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/README.md
+-rw-r--r--   0        0        0      440 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/__init__.py
+-rw-r--r--   0        0        0     3975 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/abstract_lyrics_client.py
+-rw-r--r--   0        0        0     2723 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/azlyrics_lyrics_client.py
+-rw-r--r--   0        0        0     2575 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/genius_lyrics_client.py
+-rw-r--r--   0        0        0     2165 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/clients/musixmatch_lyrics_client.py
+-rw-r--r--   0        0        0      245 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/fetch_lyrics_command.py
+-rw-r--r--   0        0        0      209 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/classes/fetch_lyrics_result.py
+-rw-r--r--   0        0        0       83 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/di/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/di/dependency_injector.py
+-rw-r--r--   0        0        0      211 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/bad_format_error.py
+-rw-r--r--   0        0        0       79 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/bad_title_match_error.py
+-rw-r--r--   0        0        0       69 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/errors/no_result_error.py
+-rw-r--r--   0        0        0       81 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/interfaces/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/interfaces/base_lyrics_client.py
+-rw-r--r--   0        0        0      841 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/lyrics_client/py.typed
+-rw-r--r--   0        0        0     1341 2023-06-13 14:20:45.805362 lyrics_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 lyrics_client-0.0.2/PKG-INFO
```

### Comparing `lyrics_client-0.0.1/LICENSE` & `lyrics_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/README.md` & `lyrics_client-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,23 @@
  - Possible to use via DI integration
 
 ## Installation
 
 ### Pip
 
 ```
-pip install taipan-di
+pip install lyrics-client
 ```
 
 ### Poetry
 
 [Poetry](https://python-poetry.org/) is a Python dependency management and packaging tool. I actually use it for this project.
 
 ```
-poetry add taipan-di
+poetry add lyrics-client
 ```
 
 ## Usage
 
 There are 2 ways to use this library : using the LyricsClient object or via the DI.
 
 ### Using LyricsClient
```

### Comparing `lyrics_client-0.0.1/lyrics_client/classes/clients/abstract_lyrics_client.py` & `lyrics_client-0.0.2/lyrics_client/classes/clients/abstract_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/lyrics_client/classes/clients/azlyrics_lyrics_client.py` & `lyrics_client-0.0.2/lyrics_client/classes/clients/azlyrics_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/lyrics_client/classes/clients/genius_lyrics_client.py` & `lyrics_client-0.0.2/lyrics_client/classes/clients/genius_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/lyrics_client/classes/clients/musixmatch_lyrics_client.py` & `lyrics_client-0.0.2/lyrics_client/classes/clients/musixmatch_lyrics_client.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/lyrics_client/di/dependency_injector.py` & `lyrics_client-0.0.2/lyrics_client/di/dependency_injector.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/lyrics_client/main.py` & `lyrics_client-0.0.2/lyrics_client/main.py`

 * *Files identical despite different names*

### Comparing `lyrics_client-0.0.1/pyproject.toml` & `lyrics_client-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "A generic client to fetch lyrics from a song's data"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["lyrics client", "lyrics", "python", "genius", "azlyrics, musixmatch"]
```

### Comparing `lyrics_client-0.0.1/PKG-INFO` & `lyrics_client-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A generic client to fetch lyrics from a song's data
 Home-page: https://github.com/Billuc/lyrics-client
 License: MIT
 Keywords: lyrics client,lyrics,python,genius,azlyrics, musixmatch
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -41,23 +41,23 @@
  - Possible to use via DI integration
 
 ## Installation
 
 ### Pip
 
 ```
-pip install taipan-di
+pip install lyrics-client
 ```
 
 ### Poetry
 
 [Poetry](https://python-poetry.org/) is a Python dependency management and packaging tool. I actually use it for this project.
 
 ```
-poetry add taipan-di
+poetry add lyrics-client
 ```
 
 ## Usage
 
 There are 2 ways to use this library : using the LyricsClient object or via the DI.
 
 ### Using LyricsClient
```

