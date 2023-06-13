# Comparing `tmp/pmm_cfg_gen-0.2.3.tar.gz` & `tmp/pmm_cfg_gen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmm_cfg_gen-0.2.3.tar", max compression
+gzip compressed data, was "pmm_cfg_gen-0.2.4.tar", max compression
```

## Comparing `pmm_cfg_gen-0.2.3.tar` & `pmm_cfg_gen-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.3/LICENSE
--rw-r--r--   0        0        0     1167 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.3/README.md
--rw-r--r--   0        0        0     1182 2023-04-07 18:07:58.094977 pmm_cfg_gen-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/.gitignore
--rw-r--r--   0        0        0     1183 2023-04-06 17:50:16.037839 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/__init__.py
--rw-r--r--   0        0        0      956 2023-04-06 15:40:40.048972 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/config_default.yaml
--rw-r--r--   0        0        0     1375 2023-04-05 12:16:46.728346 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/logging.yaml
--rw-r--r--   0        0        0       27 2023-04-07 02:15:04.147528 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/library.json.j2
--rw-r--r--   0        0        0       24 2023-04-07 01:57:28.613322 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.collection.json.j2
--rw-r--r--   0        0        0      662 2023-04-07 02:15:57.419845 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.collection.yml.j2
--rw-r--r--   0        0        0      111 2023-04-07 01:57:33.917353 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.metadata.json.j2
--rw-r--r--   0        0        0      724 2023-04-04 21:44:17.294489 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/movies.metadata.yml.j2
--rw-r--r--   0        0        0     1392 2023-04-06 13:30:45.584955 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/thePosterDatabase.html.j2
--rw-r--r--   0        0        0      142 2023-04-06 18:10:09.861502 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/thePosterDatabase.json.j2
--rw-r--r--   0        0        0       24 2023-04-07 01:57:43.117406 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.collection.json.j2
--rw-r--r--   0        0        0      617 2023-04-07 02:16:07.491905 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.collection.yml.j2
--rw-r--r--   0        0        0      111 2023-04-07 01:57:47.097429 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.metadata.json.j2
--rw-r--r--   0        0        0      777 2023-04-03 22:53:32.103146 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/templates/tvshows.metadata.yml.j2
--rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/__init__.py
--rw-r--r--   0        0        0     1408 2023-04-06 17:50:16.029839 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/cli_args.py
--rw-r--r--   0        0        0     1194 2023-04-05 11:47:03.681025 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/fileutils.py
--rw-r--r--   0        0        0     1578 2023-04-05 23:36:11.177668 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/logging.py
--rw-r--r--   0        0        0    17405 2023-04-07 17:13:05.095676 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex.py
--rw-r--r--   0        0        0     1992 2023-04-07 17:07:15.268609 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_stats.py
--rw-r--r--   0        0        0     2653 2023-04-07 12:49:38.861227 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_utils.py
--rw-r--r--   0        0        0     2735 2023-04-06 13:30:45.588955 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/pmm_cfg_manager.py
--rw-r--r--   0        0        0    11455 2023-04-06 17:50:16.313841 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/settings_yml.py
--rw-r--r--   0        0        0     5211 2023-04-07 02:13:17.834897 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/template_manager.py
--rwxr-xr-x   0        0        0     4019 2023-04-07 19:44:51.546772 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/time_span.py
--rw-r--r--   0        0        0     2663 2023-04-07 18:44:27.163668 pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/timer.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 09:59:32.119583 pmm_cfg_gen-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1810 2023-04-24 17:17:02.023284 pmm_cfg_gen-0.2.4/README.md
+-rw-r--r--   0        0        0     1246 2023-06-13 01:20:51.816201 pmm_cfg_gen-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-04 21:44:17.290489 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/.gitignore
+-rw-r--r--   0        0        0     1691 2023-04-24 15:14:53.409283 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/__init__.py
+-rw-r--r--   0        0        0     5242 2023-06-08 14:36:04.841456 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/config_default.yaml
+-rw-r--r--   0        0        0     2809 2023-06-12 17:14:55.748774 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/logging.yaml
+-rw-r--r--   0        0        0       27 2023-04-25 13:15:00.359814 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/library.json.j2
+-rw-r--r--   0        0        0       24 2023-04-25 13:14:55.063789 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/movie.collection.json.j2
+-rw-r--r--   0        0        0     3855 2023-06-13 12:28:08.719838 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/movie.collection.yaml.j2
+-rw-r--r--   0        0        0       25 2023-04-21 20:29:02.908227 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/movie.metadata.json.j2
+-rw-r--r--   0        0        0     3396 2023-06-13 12:58:26.728929 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/movie.metadata.yaml.j2
+-rw-r--r--   0        0        0       24 2023-04-25 13:14:34.303691 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/show.collection.json.j2
+-rw-r--r--   0        0        0     3854 2023-06-13 12:50:38.818656 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/show.collection.yaml.j2
+-rw-r--r--   0        0        0       24 2023-04-21 20:28:17.955980 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/show.metadata.json.j2
+-rw-r--r--   0        0        0     3733 2023-06-13 12:58:33.560963 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/show.metadata.yaml.j2
+-rw-r--r--   0        0        0     1107 2023-05-11 19:57:56.303215 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/templates/template.collection.yaml.j2
+-rw-r--r--   0        0        0        0 2023-04-03 13:48:27.869541 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/__init__.py
+-rw-r--r--   0        0        0     2592 2023-06-08 14:35:32.685306 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/cli_args.py
+-rw-r--r--   0        0        0     1956 2023-05-10 00:07:32.747680 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/file_utils.py
+-rw-r--r--   0        0        0     1778 2023-04-13 17:07:10.794833 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/logging_utils.py
+-rw-r--r--   0        0        0    36895 2023-06-13 12:26:52.555452 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/plex.py
+-rw-r--r--   0        0        0     2951 2023-06-12 16:23:04.350525 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/plex_cache.py
+-rw-r--r--   0        0        0     2150 2023-06-12 16:23:51.874774 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/plex_stats.py
+-rw-r--r--   0        0        0    17322 2023-06-13 00:41:25.266381 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/plex_utils.py
+-rwxr-xr-x   0        0        0    14285 2023-06-13 12:50:09.094516 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/pmm_utils.py
+-rw-r--r--   0        0        0    18201 2023-06-08 15:54:52.364845 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/settings_utils_v1.py
+-rw-r--r--   0        0        0    10122 2023-06-13 02:22:42.005047 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/template_filters.py
+-rw-r--r--   0        0        0     5057 2023-06-13 01:24:01.797107 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/template_manager.py
+-rwxr-xr-x   0        0        0     4443 2023-05-11 12:21:27.849258 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/time_span.py
+-rw-r--r--   0        0        0     2691 2023-04-10 21:13:51.972712 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/timer.py
+-rw-r--r--   0        0        0     2579 2023-04-26 13:50:19.226275 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/tmdb_utils.py
+-rw-r--r--   0        0        0     1361 2023-04-24 15:15:17.785439 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/trakt_utils.py
+-rw-r--r--   0        0        0     1514 2023-04-10 21:13:52.064713 pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/tvdb_utils.py
+-rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 pmm_cfg_gen-0.2.4/PKG-INFO
```

### Comparing `pmm_cfg_gen-0.2.3/LICENSE` & `pmm_cfg_gen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pmm_cfg_gen-0.2.3/pyproject.toml` & `pmm_cfg_gen-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pmm-cfg-gen"
-version = "0.2.3"
+version = "0.2.4"
 description = "A script to help automatically generate Plex Meta Manager configuration files for your libraries"
 license = "GPL-3.0-or-later"
 authors = ["Shawn Anderson <sanderson@eye-catcher.com>"]
 readme = "README.md"
 homepage = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 repository = "https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator"
 keywords = [ "pmm", "plex-meta-manager", "plex" ]
@@ -13,24 +13,27 @@
 ]
 packages = [
     {include = "pmm_cfg_gen", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-jsonpickle = "*"
 plexapi = "*"
 jinja2 = "*"
 ruamel-yaml = "^0.17.21"
 expandvars = "^0.9.0"
 python-dotenv = "^1.0.0"
 confuse = "^2.0.1"
 importlib-resources = "^5.12.0"
 coloredlogs = "^15.0.1"
 readchar = "^4.0.5"
+jsonpickle = "^3.0.1"
+json-fix = "^0.5.2"
+themoviedb = "^0.3.3"
+dotty-dict = "*"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 scriv = {extras = ["toml"], version = "^1.2.1"}
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/__init__.py` & `pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 
 #######################################################################
 
 import logging
 import os
 import readchar
 import signal
+import jsonpickle
 
 from pmm_cfg_gen.utils.cli_args import globalArgs
-from pmm_cfg_gen.utils.logging import setup_logging
+from pmm_cfg_gen.utils.settings_utils_v1 import globalSettingsMgr
+from pmm_cfg_gen.utils.logging_utils import setup_logging
 from pmm_cfg_gen.utils.plex import PlexLibraryProcessor
-from pmm_cfg_gen.utils.settings_yml import globalSettingsMgr
+
+#######################################################################
+
+jsonpickle.set_preferred_backend("json")
+
+#######################################################################
 
 
 def handler(signum, frame):
     msg = "Ctrl-c was pressed. Do you really want to exit? y/n "
     print(msg, end="", flush=True)
     res = readchar.readchar()
     if res == "y":
@@ -24,24 +31,31 @@
         print("", end="\r", flush=True)
         print(" " * len(msg), end="", flush=True)  # clear the printed line
         print("    ", end="\r", flush=True)
 
 
 signal.signal(signal.SIGINT, handler)
 
+#######################################################################
+
 setup_logging(
     str(globalSettingsMgr.modulePath.joinpath("logging.yaml")),
 )
 
 logger = logging.getLogger("pmm_cfg_gen")
 logger.setLevel(getattr(logging, globalArgs.logLevel))
 
 globalSettingsMgr.loadFromFile("config.yaml", globalArgs)
 
+#######################################################################
+
 
 def cli():
     plexMoveLibraryProcessor = PlexLibraryProcessor()
     plexMoveLibraryProcessor.process()
 
 
+#######################################################################
+#######################################################################
+
 if __name__ == "__main__":
     cli()
```

### Comparing `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/logging.py` & `pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging.config
 import logging.handlers
 import os
 
 import coloredlogs
 import yaml
 
+###################################################################################################
 
 class RollingFileHanderEx(logging.handlers.RotatingFileHandler):
     def __init__(
         self,
         filename,
         mode: str = "a",
         maxBytes: int = 0,
@@ -21,14 +22,15 @@
         delay: bool = False,
         errors: str | None = None,
     ) -> None:
         os.makedirs(os.path.dirname(filename), exist_ok=True)
 
         super().__init__(filename, mode, maxBytes, backupCount, encoding, delay, errors)
 
+###################################################################################################
 
 def setup_logging(
     default_path="logging.yaml", default_level=logging.INFO, env_key="LOG_CFG"
 ):
     """
     | **@author:** Prathyush SP
     | Logging Setup
```

### Comparing `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/plex_stats.py` & `pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/plex_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 from pmm_cfg_gen.utils.timer import timer
 
 ###################################################################################################
 
 class PlexStatsTotals:
     total: int
     processed: int
+    skipped: int
 
     def __init__(self) -> None:
         self.total = 0
         self.processed = 0
+        self.skipped = 0
 
     def _addStats(self, stats):
         self.total += stats.total
         self.processed += stats.processed
+        self.skipped += stats.skipped
+
 
 class PlexStatsLibraryTotals:
     totals: PlexStatsTotals
 
     collections: PlexStatsTotals
     items: PlexStatsTotals
 
@@ -29,14 +33,16 @@
         self.totals = PlexStatsTotals()
         self.collections = PlexStatsTotals()
         self.items = PlexStatsTotals()
 
     def calcTotals(self):
         self.totals.total = self.collections.total + self.items.total
         self.totals.processed = self.collections.processed + self.items.processed
+        self.totals.skipped = self.collections.skipped + self.items.skipped
+
 
 class PlexStats:
     timerProgram: timer
     timerLibraries: dict[str, timer]
 
     countsProgram: PlexStatsLibraryTotals
     countsLibraries: dict[str, PlexStatsLibraryTotals]
```

### Comparing `pmm_cfg_gen-0.2.3/src/pmm_cfg_gen/utils/timer.py` & `pmm_cfg_gen-0.2.4/src/pmm_cfg_gen/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 #######################################################################
 # timer.py
 
 import time
-import datetime
 from contextlib import ContextDecorator
 from dataclasses import dataclass, field
 from typing import Any, Callable, ClassVar, Dict, Optional
 from pmm_cfg_gen.utils.time_span import timespan
 
 #######################################################################
 
+
 class timer_exception(Exception):
     """A custom exception used to report errors in use of Timer class"""
 
+
 @dataclass
 class timer(ContextDecorator):
     """Time your code using a class, context manager, or decorator"""
 
     timers: ClassVar[Dict[str, float]] = {}
     name: Optional[str] = None
     text: str = "Elapsed time: {:0.4f} seconds"
@@ -60,19 +61,23 @@
     @property
     def elapsed_time(self) -> float:
         return self._elapsed_time.total_seconds
 
     @property
     def elapsed_time_ts(self) -> timespan:
         return self._elapsed_time
-    
+
     def __enter__(self) -> "timer":
         """Start a new timer as a context manager"""
         self.start()
         return self
 
     def __exit__(self, *exc_info: Any) -> None:
         """Stop the context manager timer"""
         self.stop()
 
     def to_dict(self):
-        return { "start": self._start_time, "end": self._end_time, "elapsed": self._elapsed_time.to_dict() }
+        return {
+            "start": self._start_time,
+            "end": self._end_time,
+            "elapsed": self._elapsed_time.to_dict(),
+        }
```

### Comparing `pmm_cfg_gen-0.2.3/PKG-INFO` & `pmm_cfg_gen-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,100 @@
 Metadata-Version: 2.1
 Name: pmm-cfg-gen
-Version: 0.2.3
+Version: 0.2.4
 Summary: A script to help automatically generate Plex Meta Manager configuration files for your libraries
 Home-page: https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator
 License: GPL-3.0-or-later
 Keywords: pmm,plex-meta-manager,plex
 Author: Shawn Anderson
 Author-email: sanderson@eye-catcher.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: confuse (>=2.0.1,<3.0.0)
+Requires-Dist: dotty-dict
 Requires-Dist: expandvars (>=0.9.0,<0.10.0)
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
 Requires-Dist: jinja2
-Requires-Dist: jsonpickle
+Requires-Dist: json-fix (>=0.5.2,<0.6.0)
+Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
 Requires-Dist: plexapi
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: readchar (>=4.0.5,<5.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: themoviedb (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/ravensorb/Plex-Meta-Manager-Config-Generator
 Description-Content-Type: text/markdown
 
-# Plex-Meta-Mnager-Config-Generator
+# Plex-Meta-Manager-Config-Generator
+
+[![PyPI version](https://badge.fury.io/py/pmm-cfg-gen.svg)](https://badge.fury.io/py/pmm-cfg-gen)
+
 A python script to automatically generate Plex Meta Manager configuration files based on your plex libraries.
 
-Install:
-```pip install pmm-cfg-gen```
+## Install
+
+```shell
+pip install pmm-cfg-gen
+```
 
-**Running from command line**
+## Running from command line
 
 Usage:
-```
-pmm-cfg-gen
-pmm-cfg-gen -h | --help
-pmm-cfg-gen --plex.serverUrl <plex server url> --plex.token <plex auth token> --plex.libraries <libray names> --output.path <path to store output> [--logLevel <log level>]
-```
 
-Options:
-```
--h --help           Show this help
---plex.serverUrl    The Fully Qualified Name for your Plex Server (ex: https://plex:32400)
---plex.token        The Plex Auth token (not the claim token)
---plex.library      Comma delimited list of library names
---output.path       Set the output path (default: ./data)
---logLevel          Logging Level (INFO, WARN, DEBUG, CRITICAL)
+```shell
+usage: pmm-cfg-gen [-h] [--plex.serverUrl PLEX.SERVERURL] [--plex.token PLEX.TOKEN] [--plex.lbraries [PLEX.LBRARIES ...]] [--output.path OUTPUT.PATH] [--logLevel {INFO,WARN,DEBUG,CRITICAL}]
+
+options:
+  -h, --help            show this help message and exit
+  --plex.serverUrl PLEX.SERVERURL
+                        Plex Server fully qualifed URL
+  --plex.token PLEX.TOKEN
+                        Authentication Token (not claim token) for the plex server
+  --plex.lbraries [PLEX.LBRARIES ...]
+                        Comma delimited list of libraries to process
+  --output.path OUTPUT.PATH
+                        Root path to store generated files (default: ./data)
+  --logLevel {INFO,WARN,DEBUG,CRITICAL}
+                        Logging Level (default: INFO)
+
 ```
 
-**Configuration File**
+## Configuration File
 
-All of the configuration can be stored in a ```config.yaml``` file that uses the following format.
+All of the configuration can be stored in a ```config.yaml``` file that uses the following format (with the exception of logLevel).
 
 config.yaml:
+
+```yaml
+plex:
+  serverUrl: <plex server>
+  token: <plex token>
+  libraries:
+    - <plex library name>
+    - <plex library name>
+    - <plex library name>
+    
+theMovieDatabase:
+  apiKey: <api key for tmdb>
+
+output:
+    path: <path to store generated output>
 ```
+
+Notes:
+
+* It is possible to use ENV variables (standard bash syntax supported).
+* If The Movia Database API Key is set, collection details are looked up realtime
+
+Example:
+
+```yaml
 plex:
-    serverUrl: <plex server>
-    token: <plex token>
-    libraries:
-        - <library 1>
-        - <library 2>
+    serverUrl: ${PLEX_SERVER:-https://plex:32400}
+    token: ${PLEX_TOKEN}
 ```
-Note: It is possible to use ENV variables (standard bash syntax supported).
```

