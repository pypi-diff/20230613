# Comparing `tmp/gtrending-0.4.0.tar.gz` & `tmp/gtrending-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtrending-0.4.0.tar", last modified: Fri Jan 20 07:36:16 2023, max compression
+gzip compressed data, was "gtrending-0.5.0.tar", max compression
```

## Comparing `gtrending-0.4.0.tar` & `gtrending-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:36:16.666217 gtrending-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-20 07:36:07.000000 gtrending-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-01-20 07:36:16.666217 gtrending-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-01-20 07:36:07.000000 gtrending-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:36:16.666217 gtrending-0.4.0/gtrending/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-20 07:36:07.000000 gtrending-0.4.0/gtrending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-20 07:36:07.000000 gtrending-0.4.0/gtrending/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-01-20 07:36:07.000000 gtrending-0.4.0/gtrending/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-01-20 07:36:07.000000 gtrending-0.4.0/gtrending/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-01-20 07:36:07.000000 gtrending-0.4.0/gtrending/paramutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 07:36:16.666217 gtrending-0.4.0/gtrending.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-20 07:36:16.000000 gtrending-0.4.0/gtrending.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 07:36:16.666217 gtrending-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-20 07:36:07.000000 gtrending-0.4.0/setup.py
+-rw-r--r--   0        0        0     1066 2023-01-20 02:44:28.865068 gtrending-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7429 2023-01-20 07:45:35.602367 gtrending-0.5.0/README.md
+-rw-r--r--   0        0        0      622 2023-06-13 03:21:00.648434 gtrending-0.5.0/gtrending/__init__.py
+-rw-r--r--   0        0        0       30 2023-01-16 00:50:57.980133 gtrending-0.5.0/gtrending/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:19:32.537961 gtrending-0.5.0/gtrending/_data/__init__.py
+-rw-r--r--   0        0        0    19555 2023-06-13 03:19:32.538467 gtrending-0.5.0/gtrending/_data/languages.json
+-rw-r--r--   0        0        0     7287 2023-06-13 03:19:32.538766 gtrending-0.5.0/gtrending/_data/spoken_languages.json
+-rw-r--r--   0        0        0     5489 2023-01-20 02:44:28.868035 gtrending-0.5.0/gtrending/cli.py
+-rw-r--r--   0        0        0     4948 2023-06-13 09:23:18.744939 gtrending-0.5.0/gtrending/fetch.py
+-rw-r--r--   0        0        0    12525 2023-06-13 04:00:38.154485 gtrending-0.5.0/gtrending/paramutils.py
+-rw-r--r--   0        0        0     5163 2023-06-13 03:30:50.396559 gtrending-0.5.0/gtrending/scrape.py
+-rw-r--r--   0        0        0      639 2023-06-13 06:57:46.881313 gtrending-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8054 1970-01-01 00:00:00.000000 gtrending-0.5.0/PKG-INFO
```

### Comparing `gtrending-0.4.0/LICENSE` & `gtrending-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtrending-0.4.0/PKG-INFO` & `gtrending-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: gtrending
-Version: 0.4.0
-Summary: Trending repositories and developers on GitHub
-Home-page: https://github.com/hedyhli/gtrending
-Author: hedyhli
-Author-email: hedy@tilde.cafe
+Version: 0.5.0
+Summary: Trending repositories and developers on GitHu
 License: MIT
+Author: hedy
+Author-email: hedy@tilde.cafe
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # `gtrending`
 
 ![checks](https://github.com/hedyhli/gtrending/workflows/checks/badge.svg)
 [![codecov](https://codecov.io/gh/hedyhli/gtrending/branch/master/graph/badge.svg?token=J19AQKEO4W)](https://codecov.io/gh/hedyhli/gtrending)
 [![docs status](https://readthedocs.org/projects/gtrending/badge/?version=latest)](https://gtrending.readthedocs.io/en/latest/)
 [![pypi version](https://img.shields.io/pypi/v/gtrending)](https://pypi.org/project/gtrending/)
@@ -75,15 +74,20 @@
 ```
 
 You get the idea.
 
 
 ## Usage
 
-Documentation: [Read the docs](https://gtrending.readthedocs.io/)
+Documentation: [Read the docs (online)](https://gtrending.readthedocs.io/)
+
+You can also download the PDF documentation build from the [latest
+release](https://github.com/hedyhli/gtrending/releases) or get it from [read the
+docs' downloads](https://readthedocs.org/projects/gtrending/downloads/).
+
 
 ### `fetch_repos()`
 
 Parameters:
 * `language (str, optional)`:  Filtering by language, eg: python
 * `spoken_language_code (str, optional)`: The spoken language, eg: en for
   english
@@ -154,28 +158,31 @@
     'avatar': 'https://avatars.githubusercontent.com/u/2230985',
     'name': 'Connor Peet',
     'repo': {
       'description': 'A resilience and transient-fault-handling library '
                      'that allows developers to express policies such as '
                      'Backoff, Retry, Circuit Breaker, Tim…',
       'name': 'cockatiel',
-      'url': 'https://github.com/connor4312/cockatiel'},
-      'sponsorUrl': None,
-      'url': 'https://github.com/connor4312',
-      'username': 'connor4312'
+      'url': 'https://github.com/connor4312/cockatiel'
+    },
+    'sponsorUrl': None,
+    'url': 'https://github.com/connor4312',
+    'username': 'connor4312'
   },
   {
     'avatar': 'https://avatars.githubusercontent.com/u/13049130',
     'name': 'Robert Soriano',
-    'repo': {'description': 'End-to-end typesafe APIs in Nuxt applications.',
+    'repo': {
+      'description': 'End-to-end typesafe APIs in Nuxt applications.',
       'name': 'trpc-nuxt',
-      'url': 'https://github.com/wobsoriano/trpc-nuxt'},
-      'sponsorUrl': None,
-      'url': 'https://github.com/wobsoriano',
-      'username': 'wobsoriano'
+      'url': 'https://github.com/wobsoriano/trpc-nuxt'
+    },
+    'sponsorUrl': None,
+    'url': 'https://github.com/wobsoriano',
+    'username': 'wobsoriano'
   },
   ...
 ]
 ```
 
 <br>
 
@@ -345,7 +352,8 @@
 ```
 
 ## Uses
 
 * [github-trending-api](https://github.com/huchenme/github-trending-api) —
   JavaScript library with web API
 * requests — Making API requests
+
```

### Comparing `gtrending-0.4.0/README.md` & `gtrending-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,20 @@
 ```
 
 You get the idea.
 
 
 ## Usage
 
-Documentation: [Read the docs](https://gtrending.readthedocs.io/)
+Documentation: [Read the docs (online)](https://gtrending.readthedocs.io/)
+
+You can also download the PDF documentation build from the [latest
+release](https://github.com/hedyhli/gtrending/releases) or get it from [read the
+docs' downloads](https://readthedocs.org/projects/gtrending/downloads/).
+
 
 ### `fetch_repos()`
 
 Parameters:
 * `language (str, optional)`:  Filtering by language, eg: python
 * `spoken_language_code (str, optional)`: The spoken language, eg: en for
   english
@@ -135,28 +140,31 @@
     'avatar': 'https://avatars.githubusercontent.com/u/2230985',
     'name': 'Connor Peet',
     'repo': {
       'description': 'A resilience and transient-fault-handling library '
                      'that allows developers to express policies such as '
                      'Backoff, Retry, Circuit Breaker, Tim…',
       'name': 'cockatiel',
-      'url': 'https://github.com/connor4312/cockatiel'},
-      'sponsorUrl': None,
-      'url': 'https://github.com/connor4312',
-      'username': 'connor4312'
+      'url': 'https://github.com/connor4312/cockatiel'
+    },
+    'sponsorUrl': None,
+    'url': 'https://github.com/connor4312',
+    'username': 'connor4312'
   },
   {
     'avatar': 'https://avatars.githubusercontent.com/u/13049130',
     'name': 'Robert Soriano',
-    'repo': {'description': 'End-to-end typesafe APIs in Nuxt applications.',
+    'repo': {
+      'description': 'End-to-end typesafe APIs in Nuxt applications.',
       'name': 'trpc-nuxt',
-      'url': 'https://github.com/wobsoriano/trpc-nuxt'},
-      'sponsorUrl': None,
-      'url': 'https://github.com/wobsoriano',
-      'username': 'wobsoriano'
+      'url': 'https://github.com/wobsoriano/trpc-nuxt'
+    },
+    'sponsorUrl': None,
+    'url': 'https://github.com/wobsoriano',
+    'username': 'wobsoriano'
   },
   ...
 ]
 ```
 
 <br>
```

### Comparing `gtrending-0.4.0/gtrending/__init__.py` & `gtrending-0.5.0/gtrending/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,11 +17,11 @@
     check_spoken_language_code,
     check_spoken_language,
     check_since,
     convert_spoken_language_name_to_code,
     convert_language_name_to_param,
 )
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __url__ = "https://github.com/hedyhli/gtrending"
 __author__ = "hedyhli"
 __author_email__ = "hedy@tilde.cafe"
```

### Comparing `gtrending-0.4.0/gtrending/cli.py` & `gtrending-0.5.0/gtrending/cli.py`

 * *Files identical despite different names*

### Comparing `gtrending-0.4.0/gtrending/fetch.py` & `gtrending-0.5.0/gtrending/fetch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """
 Fetch trending repositories and developers using github-trending-api
 """
 
 from urllib.parse import quote as urlquote
 from typing import List, Optional
 
-import requests
-
 from .paramutils import (
     check_language,
     check_spoken_language_code,
     check_since,
     convert_language_name_to_param,
 )
+from .scrape import scrape_repos, scrape_developers
 
 
 def fetch_repos(
     language: Optional[str] = "",
     spoken_language_code: Optional[str] = "",
     since: Optional[str] = "daily",
 ) -> List[dict]:
     """Fetch trending repositories on GitHub.
 
     Parameters:
         language (str, optional):  Filtering by language, eg: python, common-lisp
         spoken_language_code (str, optional): The spoken language, eg: en for english
         since (str, optional): The time range, choose from: [daily, weekly, monthly].
-        Defaults to "daily".
+                               Defaults to "daily".
 
     Note:
         spoken_language_code argument must be the language code ("en" and not
         "english"). To convert language name to language code, use
         convert_spoken_language_name_to_code().
 
         Likewise, language argument must be the parameter value ("common-lisp"
@@ -71,23 +70,18 @@
 
     if not isinstance(since, (str, type(None))) or since and not check_since(since):
         raise ValueError(
             f"Invalid since argument (must be 'daily', 'weekly' or 'monthly'): {since}"
         )
     since = since or "daily"
 
-    url: str = (
-        "https://gtrend.yapie.me/repositories?"
-        f"language={language_param}&since={since}&spoken_language_code={spoken_language_code}"
-    )
-
-    res = requests.get(url).json()
+    res = scrape_repos(language_param, spoken_language_code, since)
     repos = []
     for repo in res:
-        repo["fullname"] = f"{repo['author']}/{repo['name']}"
+        # repo["fullname"] = f"{repo['author']}/{repo['name']}"
         repo_language = repo.get("language")
         # Edge cases
         if language:
             if (
                 not repo_language
                 or convert_language_name_to_param(repo_language).lower()
                 != language.lower()
@@ -101,35 +95,40 @@
             repo["currentPeriodStars"] = 0  # pragma: no cover
 
         repos.append(repo)
     return repos
 
 
 def fetch_developers(
-    language: Optional[str] = "", since: Optional[str] = "daily"
+    language: Optional[str] = "",
+    since: Optional[str] = "daily",
+    sponsorable: Optional[bool] = False,
 ) -> List[dict]:
     """Fetch trending developers on GitHub.
 
     Parameters:
         language (str, optional): The programming language, eg: python
         since (str, optional): The time range, choose from [daily, weekly, monthly].
-        Defaults to "daily".
+                               Defaults to "daily".
+        sponsorable (bool, optional): Whether to only search for developers with sponsor URLs.
+                                      Defaults to False.
 
     Returns:
         list(dict): A list of dictionaries containing information for each trending developer found
 
     Raises:
         ValueError: When any of the arguments are invalid
 
     Examples:
         ::
 
             fetch_developers()
             fetch_repos(language="python")
             fetch_repos("C", since="monthly")
+            fetch_repos("python", sponsorable=True)
     """
 
     if (
         not isinstance(language, (str, type(None)))
         or language
         and not check_language(language)
     ):
@@ -137,13 +136,14 @@
     language_param = urlquote(language, safe="+") if language else ""
 
     if not isinstance(since, (str, type(None))) or since and not check_since(since):
         raise ValueError(
             f"Invalid since argument (must be 'daily', 'weekly' or 'monthly'): {since}"
         )
 
-    url: str = (
-        f"https://gtrend.yapie.me/developers?language={language_param}&since={since}"
-    )
+    if not isinstance(sponsorable, (bool, type(None))):
+        raise ValueError(
+            f"Invalid sponsorable argument (must be True/False/None): {sponsorable}"
+        )
 
-    res = requests.get(url).json()
+    res = scrape_developers(language_param, since, sponsorable)
     return res
```

### Comparing `gtrending-0.4.0/gtrending/paramutils.py` & `gtrending-0.5.0/gtrending/paramutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Parameter utility functions"""
 
 from urllib.parse import unquote as urlunquote
 from typing import List
+import json
+import importlib.resources as pkg_resources
 
-import requests
+from . import _data
 
 
-"""Tuple of valid arguments for the `since` parameter"""
 SINCE_PARAM = ("daily", "weekly", "monthly")
+"""Tuple of valid arguments for the `since` parameter"""
 
 
 def languages_list() -> List[dict]:
     """Fetch programming languages.
 
     Example:
         ::
@@ -37,28 +39,23 @@
                 {'name': 'IRC log', 'param': 'irc-log'},
                 ...
             ]
 
     Returns:
         list(dict): A list of dictionaries containing languages, mapping the param value to its name
     """
-    url: str = "https://gtrend.yapie.me/languages"
-    response = requests.get(url).json()
-
-    # Rename key urlParam to param
-    for i in response:
-        # https://stackoverflow.com/questions/54637847/how-to-change-dictionary-keys-in-a-list-of-dictionaries
-        i["param"] = urlunquote(i.pop("urlParam"))
-        # urlParam values returned by API shows values that should be used as
-        # url query values, these are converted to %-decoded values for use as
-        # a python library.
-        #
-        # (For check_language()):
-
-    return response
+    # https://stackoverflow.com/a/20885799  for Python >=3.7
+    try:
+        file = pkg_resources.files(_data) / "languages.json"  # type: ignore
+        f = file.open()
+    except AttributeError:
+        f = pkg_resources.open_text(_data, "languages.json")  # type: ignore
+    res = json.load(f)
+    f.close()
+    return res
 
 
 def spoken_languages_list() -> List[dict]:
     """Fetch spoken languages.
 
     Example:
         ::
@@ -86,24 +83,22 @@
                 {'code': 'el', 'name': ['Greek', 'Modern']},
                 ...
             ]
 
     Returns:
         list(dict): A list dictionaries of spoken languages, mapping the code to the name
     """
-    url: str = "https://gtrend.yapie.me/spoken_languages"
-    response = requests.get(url).json()
-
-    # Rename key urlParam to code
-    for i in response:
-        # https://stackoverflow.com/questions/54637847/how-to-change-dictionary-keys-in-a-list-of-dictionaries
-        i["code"] = i.pop("urlParam")
-        i["name"] = i["name"].split(", ")
-
-    return response
+    try:
+        file = pkg_resources.files(_data) / "spoken_languages.json"  # type: ignore
+        f = file.open()
+    except AttributeError:
+        f = pkg_resources.open_text(_data, "spoken_languages.json")  # type: ignore
+    res = json.load(f)
+    f.close()
+    return res
 
 
 def check_language(language: str) -> bool:
     """Check if the language parameter is valid.
 
     Value that is already url-encoded would not be accepted.
```

