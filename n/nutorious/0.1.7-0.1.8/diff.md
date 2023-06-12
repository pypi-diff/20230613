# Comparing `tmp/nutorious-0.1.7.tar.gz` & `tmp/nutorious-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutorious-0.1.7.tar", max compression
+gzip compressed data, was "nutorious-0.1.8.tar", max compression
```

## Comparing `nutorious-0.1.7.tar` & `nutorious-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-06-12 00:02:39.371817 nutorious-0.1.7/LICENSE
--rw-r--r--   0        0        0     6727 2023-06-12 00:02:39.371817 nutorious-0.1.7/README.md
--rw-r--r--   0        0        0      879 2023-06-12 00:02:39.375817 nutorious-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/__init__.py
--rw-r--r--   0        0        0      770 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/cli/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/config/__init__.py
--rw-r--r--   0        0        0      376 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/config/default.yml
--rw-r--r--   0        0        0      203 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/context/__init__.py
--rw-r--r--   0        0        0     4430 2023-06-12 00:02:39.375817 nutorious-0.1.7/src/nutorious/journal/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/base.py
--rw-r--r--   0        0        0     2555 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/daily.py
--rw-r--r--   0        0        0        0 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/report/diff.py
--rw-r--r--   0        0        0     1094 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/ui/__init__.py
--rw-r--r--   0        0        0      336 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/utils/collections.py
--rw-r--r--   0        0        0      570 2023-06-12 00:02:39.379817 nutorious-0.1.7/src/nutorious/utils/commons.py
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 nutorious-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 22:39:28.357649 nutorious-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6727 2023-06-12 22:39:28.357649 nutorious-0.1.8/README.md
+-rw-r--r--   0        0        0      879 2023-06-12 22:39:28.357649 nutorious-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1559 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/cli/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-12 22:39:28.357649 nutorious-0.1.8/src/nutorious/config/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/config/default.yml
+-rw-r--r--   0        0        0      204 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/context/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/journal/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/__init__.py
+-rw-r--r--   0        0        0     1457 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/base.py
+-rw-r--r--   0        0        0     2556 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/daily.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/report/diff.py
+-rw-r--r--   0        0        0     1094 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/ui/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/utils/collections.py
+-rw-r--r--   0        0        0      570 2023-06-12 22:39:28.361649 nutorious-0.1.8/src/nutorious/utils/commons.py
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 nutorious-0.1.8/PKG-INFO
```

### Comparing `nutorious-0.1.7/LICENSE` & `nutorious-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/README.md` & `nutorious-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/pyproject.toml` & `nutorious-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nutorious"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Dzmitry Paulenka"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dzmitry-paulenka/nutorious"
 
 [tool.poetry.dependencies]
```

### Comparing `nutorious-0.1.7/src/nutorious/__init__.py` & `nutorious-0.1.8/src/nutorious/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from datetime import datetime
 
 import click
 from cattrs import transform_error
 from cattrs.errors import BaseValidationError
+
 from nutorious.cli import option_date, option_journal_path, option_watch
 from nutorious.report.daily import DailyReportOptions, display_daily_report
 from nutorious.utils.commons import mkstring
 
 
 @click.group()
 def nutorious_cli():
```

### Comparing `nutorious-0.1.7/src/nutorious/cli/__init__.py` & `nutorious-0.1.8/src/nutorious/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/src/nutorious/config/__init__.py` & `nutorious-0.1.8/src/nutorious/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from importlib.resources import files
 from pathlib import Path
 
 import cattrs
 import yaml
 from attrs import define, field
+
 from nutorious.utils.collections import merge_dicts
 from nutorious.utils.commons import load_yaml_data
 
 
 @define
 class Config:
     meals: list[str]
```

### Comparing `nutorious-0.1.7/src/nutorious/journal/__init__.py` & `nutorious-0.1.8/src/nutorious/journal/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import re
 from datetime import date
 from datetime import datetime
 from pathlib import Path
 
 import cattrs
 from attrs import Factory, define
+from pydash import py_
+
 from nutorious.config import Config
 from nutorious.model import Journal, Day, Food, Meal
 from nutorious.utils.commons import load_yaml_data
-from pydash import py_
 
 ItemData = list[str]
 DayData = dict[str, ItemData]
 Data = dict[date, DayData]
 
 weight_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?)g$")
 count_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?)x$")
-ingredient_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?) ([\w-]+)$")
+ingredient_spec_pattern = re.compile(r"^(\d+(?:\.\d+)?) (\S+)$", re.U)
 
 
 @define
 class FoodRegistry:
     foods: dict[str, Food] = Factory(dict)
 
     def register(self, food: Food):
@@ -136,18 +137,14 @@
         amount=food.amount,
         countable=food.countable,
         weight=food.weight,
         ingredients=food.ingredients,
     )
 
 
-def lookup_journal_day(journal: Journal, dt: date) -> Day:
-    ...
-
-
 def __cattrs_date_structure_hook(raw, _) -> date:
     if type(raw) == date:
         return raw
     elif type(raw) == datetime:
         return raw.date()
     elif type(raw) == str:
         return datetime.strptime(raw, "%Y-%m-%d")
```

### Comparing `nutorious-0.1.7/src/nutorious/model/__init__.py` & `nutorious-0.1.8/src/nutorious/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/src/nutorious/report/base.py` & `nutorious-0.1.8/src/nutorious/report/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from typing import Callable
 
 from attrs import define
-from nutorious.config import load_config
-from nutorious.context import Context
-from nutorious.journal import load_journal
 from rich.console import Console
 from rich.live import Live
 from watchfiles import watch
 from watchfiles.filters import DefaultFilter
 
+from nutorious.config import load_config
+from nutorious.context import Context
+from nutorious.journal import load_journal
+
 
 @define
 class BaseOptions:
     journal_path: str
     watch: bool
 
 
@@ -23,15 +24,14 @@
         return path.endswith(".yml") and super().__call__(change, path)
 
 
 def display_report(options: BaseOptions, build_report_table_fn: Callable[[Context], Table]):
     context = __load_context(options)
 
     if options.watch:
-        ch_cnt = 0
         with Live(build_report_table_fn(context), auto_refresh=False) as live:
             for changes in watch(options.journal_path, watch_filter=YmlFilesFilter()):
                 context = __load_context(options)
                 live.update(build_report_table_fn(context), refresh=True)
     else:
         console = Console()
         try:
```

### Comparing `nutorious-0.1.7/src/nutorious/report/daily.py` & `nutorious-0.1.8/src/nutorious/report/daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from datetime import date
 
 from attrs import define
+from pydash import py_
+from rich import box
+from rich.table import Table
+
 from nutorious.config import ColumnConfig, Config
 from nutorious.context import Context
 from nutorious.model import Day, Meal, Food
 from nutorious.report.base import BaseOptions, display_report
 from nutorious.ui import create_tree_row
-from pydash import py_
-from rich import box
-from rich.table import Table
 
 
 @define
 class DailyReportOptions(BaseOptions):
     dt: date
```

### Comparing `nutorious-0.1.7/src/nutorious/ui/__init__.py` & `nutorious-0.1.8/src/nutorious/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/src/nutorious/utils/commons.py` & `nutorious-0.1.8/src/nutorious/utils/commons.py`

 * *Files identical despite different names*

### Comparing `nutorious-0.1.7/PKG-INFO` & `nutorious-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutorious
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/dzmitry-paulenka/nutorious
 License: MIT
 Author: Dzmitry Paulenka
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

