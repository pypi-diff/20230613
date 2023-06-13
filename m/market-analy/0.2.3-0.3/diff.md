# Comparing `tmp/market_analy-0.2.3.tar.gz` & `tmp/market_analy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_analy-0.2.3.tar", last modified: Mon Apr 10 11:19:10 2023, max compression
+gzip compressed data, was "market_analy-0.3.tar", last modified: Tue Jun 13 10:10:07 2023, max compression
```

## Comparing `market_analy-0.2.3.tar` & `market_analy-0.3.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-10 11:18:52.000000 market_analy-0.2.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-10 11:18:52.000000 market_analy-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-10 11:18:52.000000 market_analy-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-10 11:18:52.000000 market_analy-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 11:18:52.000000 market_analy-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-10 11:18:52.000000 market_analy-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-10 11:19:10.189507 market_analy-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-10 11:18:52.000000 market_analy-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-10 11:18:52.000000 market_analy-0.2.3/docs/splash.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/etc/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements/why_here.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-10 11:18:52.000000 market_analy-0.2.3/etc/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-10 11:18:52.000000 market_analy-0.2.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-10 11:18:52.000000 market_analy-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 11:18:52.000000 market_analy-0.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:19:10.189507 market_analy-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-10 11:18:52.000000 market_analy-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.181507 market_analy-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.185507 market_analy-0.2.3/src/market_analy/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 11:19:09.000000 market_analy-0.2.3/src/market_analy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    42395 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66003 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18025 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/gui_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)    56989 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/src/market_analy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/bq_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27860 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/ipyvuetify_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/ipywidgets_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/maths_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/mkt_prices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-10 11:18:52.000000 market_analy-0.2.3/src/market_analy/utils/pandas_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:19:10.189507 market_analy-0.2.3/src/market_analy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 11:19:10.000000 market_analy-0.2.3/src/market_analy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.050400 market_analy-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 10:09:55.000000 market_analy-0.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-13 10:09:55.000000 market_analy-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 10:09:55.000000 market_analy-0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-13 10:09:55.000000 market_analy-0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 10:09:55.000000 market_analy-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 10:09:55.000000 market_analy-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-06-13 10:10:07.050400 market_analy-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-13 10:09:55.000000 market_analy-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.042400 market_analy-0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   113308 2023-06-13 10:09:55.000000 market_analy-0.3/docs/splash.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.042400 market_analy-0.3/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.042400 market_analy-0.3/etc/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-13 10:09:55.000000 market_analy-0.3/etc/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 10:09:55.000000 market_analy-0.3/etc/requirements/why_here.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-13 10:09:55.000000 market_analy-0.3/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-13 10:09:55.000000 market_analy-0.3/etc/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 10:09:55.000000 market_analy-0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-13 10:09:55.000000 market_analy-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-13 10:09:55.000000 market_analy-0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:10:07.050400 market_analy-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 10:09:55.000000 market_analy-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.042400 market_analy-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.046400 market_analy-0.3/src/market_analy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 10:10:06.000000 market_analy-0.3/src/market_analy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46103 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82823 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/gui_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70112 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/movements_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/trends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64750 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/trends_alt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/trends_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.046400 market_analy-0.3/src/market_analy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49222 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/bq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/ipyvuetify_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/ipywidgets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/maths_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/mkt_prices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-13 10:09:55.000000 market_analy-0.3/src/market_analy/utils/pandas_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:10:07.046400 market_analy-0.3/src/market_analy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-06-13 10:10:06.000000 market_analy-0.3/src/market_analy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 10:10:07.000000 market_analy-0.3/src/market_analy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:10:06.000000 market_analy-0.3/src/market_analy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 10:10:06.000000 market_analy-0.3/src/market_analy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 10:10:06.000000 market_analy-0.3/src/market_analy.egg-info/top_level.txt
```

### Comparing `market_analy-0.2.3/.flake8` & `market_analy-0.3/.flake8`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/.gitignore` & `market_analy-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/.pre-commit-config.yaml` & `market_analy-0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/.pylintrc` & `market_analy-0.3/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,19 @@
 [BASIC]
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i, j,
         x, y,
         k, v,
         d,
+        m,
         n, s, tt, bi,
         a, b,
         f,
+        to, px,
         df,
         ii,
         ts,
         tz,
         bv,
 
 [FORMAT]
```

### Comparing `market_analy-0.2.3/LICENSE.txt` & `market_analy-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/PKG-INFO` & `market_analy-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market_analy
-Version: 0.2.3
+Version: 0.3
 Summary: Analysis of exchange-listed financial instruments
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
 Project-URL: homepage, https://github.com/maread99/market_analy
 Project-URL: documentation, https://github.com/maread99/market_analy
 Project-URL: Issue Tracker, https://github.com/maread99/market_analy/issues
@@ -40,89 +40,106 @@
 
 -----------------
 
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-A python package to analyse financial instruments.
+A python package for interactive charting and analysis of financial instruments.
 
-There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
+Functionality includes **defining and visualising trends**.
 
-Some functionality is general, some is focused on defining and identifying trends. Interactive charting is offered via guis created from widgets of the bqplot, ipywidgets and ipyvuetify libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
+Interactive charting is offered via guis created from widgets of the [bqplot](https://github.com/bqplot/bqplot), [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) and [ipyvuetify](https://github.com/widgetti/ipyvuetify) libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
 
-The [demo video](https://vimeo.com/801302973) gives an overview of what´s on offer. All analyses are accessed via the classes `analysis.Analysis` (single instrument analyses) and `analysis.Compare` (to compare multiple instruments). For example:
+There's a load of great financial libraries out there. This library isn't reinventing the wheel (not intentionally anyway), rather it principally provides functions and interactive charting that I think are useful and couldn't find elsewhere.
+
+## Video tutorials
+
+The following videos cover what's on offer:
+* [General tutorial](https://vimeo.com/801302973) demonstrates the functionality as of the initial release (February 2023).
+* [Trends](https://vimeo.com/835495038) demonstrates functionality (added June 2023) to define and visualise trends.
+
+## Quickstart
+All analyses can be accessed via the classes `Analysis` (single instrument analyses) and `Compare` (to compare multiple instruments). For example:
 
 ```python
 from market_prices import PricesYahoo
 from market_analy import Analysis,  Compare
 
 prices = PricesYahoo("MSFT")
 analy = Analysis(prices)
 gui = analy.plot(days=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773777-df0d0bec-bbe1-45bb-b067-d679666450cd.mp4
 
 ```python
+trend_kwargs = {
+    "prd":60,
+    "ext_break":0.05,
+    "ext_limit":0.03,
+    "min_bars":5,
+}
+gui = analy.trends_chart(
+    "1D",
+    trend_kwargs,
+    years=3,
+)
+```
+https://github.com/maread99/market_analy/assets/56914820/998c7f46-20f5-43f1-8b82-c857c0702cee
+
+```python
 comp = Compare(PricesYahoo("MSFT, AMZN, TSLA"))
 gui = comp.plot(hours=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773790-1fdabf13-25bb-4205-acc2-6bac9b832dae.mp4
 
 ```python
 gui = comp.chg_every_interval("20T", days=5, chart=True)
 ```
 https://user-images.githubusercontent.com/56914820/220773802-ae329259-4a4e-4e5e-8d02-d4ee88b8b452.mp4
 
-
-For further documentation, see the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
+For further documentation see the [video tutorials](#Video-tutorials) and the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
 
 ## Installation and environment
 
 It's recommended that `market-analy` is installed to a new virtual environment created using `venv`.
 
 The package can be installed to the activated environment via pip:
 
 `$ pip install market-analy`
 
-Plots are intended to be created in a Jupyter Notebook or JupyterLab. The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
+Plots are intended to be created in JupyterLab (they will not load in a notebook opened in VSCode). The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
 
 `$ pip install market-analy[jupyter]`
 
-Then call:
-
-`jupyter nbextension enable --py --sys-prefix ipyvuetify`
-
-Alternatively, it's possible to use an existing Jupyter installation in a separate environment to that in which `market_analy` is installed. In this case:
-* The following dependencies should additionally be installed **in the environment to which Jupyter is installed**:
-  - `jupyterlab>=3.0`
+Alternatively, it's possible to use an existing JupyterLab installation (>=3.0) in a separate environment to that in which `market_analy` is installed. In this case:
+* The following dependencies should additionally be installed **in the environment to which JupyterLab is installed**:
   - `ipyvuetify`
   - `bqplot`
-* Jupyter should be called with the following arguments:
-  - `jupyter nbextension enable --py --sys-prefix ipyvuetify`
+* A kernel should be created for **the environment to which `market_analy` was installed**. Executing the following, with any virutal environment activated, will create a kernel and make it available to all installed versions of `jupyterlab`.
+  - `python -m ipykernel install --user --name mkt_analy --display-name "market analy env"`
 
-> :information_source: Unfortunately plots do not render in a VSCode notebook.
+> :warning: If starting JupyterLab from a different environment to the environment in which `market_analy` is installed then **the same versions of `ipyvuetify` and `bqplot` must be installed to both environments**. If either of these packages is subsequently upgraded in one environment then it must also be upgraded in the other. (This is due to the potential for conflicts between the versions in the JupyterLab environment, which are responsible for the frontend, and those in the `market_analy` environment where the backend is defined.)
 
 ### Color scheme
 The color scheme assumes the package is being used with the JupyterLab dark theme. There are no plans to provide a 'light theme' option (although a contribution would certainly be welcome from anyone seeking one).
 
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
 ## Release schedule, bugs, development and feedback
-
-The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+The first beta version of `market_analy` was released Feb 2023. Functionality to  define and visually interrogate trends was added in June 2023.
 
 The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
-The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
+The test suite is somewhat limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
 Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
 
 ## Disclaimers
 `market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
 
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `market_analy-0.2.3/README.md` & `market_analy-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,89 +5,106 @@
 
 -----------------
 
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-A python package to analyse financial instruments.
+A python package for interactive charting and analysis of financial instruments.
 
-There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
+Functionality includes **defining and visualising trends**.
 
-Some functionality is general, some is focused on defining and identifying trends. Interactive charting is offered via guis created from widgets of the bqplot, ipywidgets and ipyvuetify libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
+Interactive charting is offered via guis created from widgets of the [bqplot](https://github.com/bqplot/bqplot), [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) and [ipyvuetify](https://github.com/widgetti/ipyvuetify) libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
 
-The [demo video](https://vimeo.com/801302973) gives an overview of what´s on offer. All analyses are accessed via the classes `analysis.Analysis` (single instrument analyses) and `analysis.Compare` (to compare multiple instruments). For example:
+There's a load of great financial libraries out there. This library isn't reinventing the wheel (not intentionally anyway), rather it principally provides functions and interactive charting that I think are useful and couldn't find elsewhere.
+
+## Video tutorials
+
+The following videos cover what's on offer:
+* [General tutorial](https://vimeo.com/801302973) demonstrates the functionality as of the initial release (February 2023).
+* [Trends](https://vimeo.com/835495038) demonstrates functionality (added June 2023) to define and visualise trends.
+
+## Quickstart
+All analyses can be accessed via the classes `Analysis` (single instrument analyses) and `Compare` (to compare multiple instruments). For example:
 
 ```python
 from market_prices import PricesYahoo
 from market_analy import Analysis,  Compare
 
 prices = PricesYahoo("MSFT")
 analy = Analysis(prices)
 gui = analy.plot(days=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773777-df0d0bec-bbe1-45bb-b067-d679666450cd.mp4
 
 ```python
+trend_kwargs = {
+    "prd":60,
+    "ext_break":0.05,
+    "ext_limit":0.03,
+    "min_bars":5,
+}
+gui = analy.trends_chart(
+    "1D",
+    trend_kwargs,
+    years=3,
+)
+```
+https://github.com/maread99/market_analy/assets/56914820/998c7f46-20f5-43f1-8b82-c857c0702cee
+
+```python
 comp = Compare(PricesYahoo("MSFT, AMZN, TSLA"))
 gui = comp.plot(hours=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773790-1fdabf13-25bb-4205-acc2-6bac9b832dae.mp4
 
 ```python
 gui = comp.chg_every_interval("20T", days=5, chart=True)
 ```
 https://user-images.githubusercontent.com/56914820/220773802-ae329259-4a4e-4e5e-8d02-d4ee88b8b452.mp4
 
-
-For further documentation, see the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
+For further documentation see the [video tutorials](#Video-tutorials) and the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
 
 ## Installation and environment
 
 It's recommended that `market-analy` is installed to a new virtual environment created using `venv`.
 
 The package can be installed to the activated environment via pip:
 
 `$ pip install market-analy`
 
-Plots are intended to be created in a Jupyter Notebook or JupyterLab. The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
+Plots are intended to be created in JupyterLab (they will not load in a notebook opened in VSCode). The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
 
 `$ pip install market-analy[jupyter]`
 
-Then call:
-
-`jupyter nbextension enable --py --sys-prefix ipyvuetify`
-
-Alternatively, it's possible to use an existing Jupyter installation in a separate environment to that in which `market_analy` is installed. In this case:
-* The following dependencies should additionally be installed **in the environment to which Jupyter is installed**:
-  - `jupyterlab>=3.0`
+Alternatively, it's possible to use an existing JupyterLab installation (>=3.0) in a separate environment to that in which `market_analy` is installed. In this case:
+* The following dependencies should additionally be installed **in the environment to which JupyterLab is installed**:
   - `ipyvuetify`
   - `bqplot`
-* Jupyter should be called with the following arguments:
-  - `jupyter nbextension enable --py --sys-prefix ipyvuetify`
+* A kernel should be created for **the environment to which `market_analy` was installed**. Executing the following, with any virutal environment activated, will create a kernel and make it available to all installed versions of `jupyterlab`.
+  - `python -m ipykernel install --user --name mkt_analy --display-name "market analy env"`
 
-> :information_source: Unfortunately plots do not render in a VSCode notebook.
+> :warning: If starting JupyterLab from a different environment to the environment in which `market_analy` is installed then **the same versions of `ipyvuetify` and `bqplot` must be installed to both environments**. If either of these packages is subsequently upgraded in one environment then it must also be upgraded in the other. (This is due to the potential for conflicts between the versions in the JupyterLab environment, which are responsible for the frontend, and those in the `market_analy` environment where the backend is defined.)
 
 ### Color scheme
 The color scheme assumes the package is being used with the JupyterLab dark theme. There are no plans to provide a 'light theme' option (although a contribution would certainly be welcome from anyone seeking one).
 
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
 ## Release schedule, bugs, development and feedback
-
-The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+The first beta version of `market_analy` was released Feb 2023. Functionality to  define and visually interrogate trends was added in June 2023.
 
 The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
-The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
+The test suite is somewhat limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
 Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
 
 ## Disclaimers
 `market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
 
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `market_analy-0.2.3/etc/requirements/requirements.txt` & `market_analy-0.3/etc/requirements/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 #    pip-compile --output-file=./etc/requirements/requirements.txt pyproject.toml
 #
 asttokens==2.2.1
     # via stack-data
 backcall==0.2.0
     # via ipython
-bqplot==0.12.38
+bqplot==0.12.39
     # via market-analy (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 colorama==0.4.6
     # via
     #   ipython
     #   tqdm
@@ -24,110 +24,110 @@
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
-exchange-calendars==4.2.6
+exchange-calendars==4.2.8
     # via
     #   market-analy (pyproject.toml)
     #   market-prices
 executing==1.2.0
     # via stack-data
-fonttools==4.39.3
+fonttools==4.40.0
     # via matplotlib
 idna==3.4
     # via requests
-importlib-metadata==6.3.0
+importlib-metadata==6.6.0
     # via jupyter-client
 importlib-resources==5.12.0
     # via matplotlib
-ipykernel==6.22.0
+ipykernel==6.23.2
     # via ipywidgets
-ipython==8.12.0
+ipython==8.14.0
     # via
     #   ipykernel
     #   ipywidgets
-ipyvue==1.9.0
+ipyvue==1.9.1
     # via ipyvuetify
-ipyvuetify==1.8.5
+ipyvuetify==1.8.10
     # via market-analy (pyproject.toml)
 ipywidgets==8.0.6
     # via
     #   bqplot
     #   ipyvue
     #   market-analy (pyproject.toml)
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via market-analy (pyproject.toml)
-jupyter-client==8.1.0
+jupyter-client==8.2.0
     # via ipykernel
 jupyter-core==5.3.0
     # via
     #   ipykernel
     #   jupyter-client
 jupyterlab-widgets==3.0.7
     # via ipywidgets
 kiwisolver==1.4.4
     # via matplotlib
 korean-lunar-calendar==0.3.1
     # via exchange-calendars
 lxml==4.9.2
     # via yahooquery
-market-prices==0.10.2
+market-prices==0.10.3
     # via market-analy (pyproject.toml)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 matplotlib==3.7.1
     # via market-analy (pyproject.toml)
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 nest-asyncio==1.5.6
     # via ipykernel
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   bqplot
     #   contourpy
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   matplotlib
     #   pandas
-packaging==23.0
+packaging==23.1
     # via
     #   ipykernel
     #   matplotlib
-pandas==2.0.0
+pandas==2.0.2
     # via
     #   bqplot
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   yahooquery
 parso==0.8.3
     # via jedi
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
-platformdirs==3.2.0
+platformdirs==3.5.3
     # via jupyter-core
 prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
-pydantic==1.10.7
+pydantic==1.10.9
     # via market-prices
-pygments==2.14.0
+pygments==2.15.1
     # via ipython
 pyluach==2.2.0
     # via exchange-calendars
 pyparsing==3.0.9
     # via matplotlib
 python-dateutil==2.8.2
     # via
@@ -138,31 +138,31 @@
 pytz==2023.3
     # via
     #   exchange-calendars
     #   market-prices
     #   pandas
 # pywin32==306
     # via jupyter-core
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
-requests==2.28.2
+requests==2.31.0
     # via requests-futures
 requests-futures==1.0.0
     # via yahooquery
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
 stack-data==0.6.2
     # via ipython
 toolz==0.12.0
     # via exchange-calendars
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
 tqdm==4.65.0
     # via yahooquery
 traitlets==5.9.0
     # via
@@ -174,21 +174,21 @@
     #   jupyter-client
     #   jupyter-core
     #   market-analy (pyproject.toml)
     #   matplotlib-inline
     #   traittypes
 traittypes==0.2.1
     # via bqplot
-typing-extensions==4.5.0
+typing-extensions==4.6.3
     # via
     #   ipython
     #   pydantic
 tzdata==2023.3
     # via pandas
-urllib3==1.26.15
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 widgetsnbextension==4.0.7
     # via ipywidgets
 yahooquery==2.3.1
     # via market-prices
```

### Comparing `market_analy-0.2.3/etc/requirements_tests.txt` & `market_analy-0.3/etc/requirements_tests.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 asttokens==2.2.1
     # via stack-data
 backcall==0.2.0
     # via ipython
 black==23.3.0
     # via market-analy (pyproject.toml)
-bqplot==0.12.38
+bqplot==0.12.39
     # via market-analy (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via black
 colorama==0.4.6
     # via
@@ -32,142 +32,142 @@
     # via matplotlib
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 exceptiongroup==1.1.1
     # via pytest
-exchange-calendars==4.2.6
+exchange-calendars==4.2.8
     # via
     #   market-analy (pyproject.toml)
     #   market-prices
 executing==1.2.0
     # via stack-data
 flake8==6.0.0
     # via
     #   flake8-docstrings
     #   market-analy (pyproject.toml)
 flake8-docstrings==1.7.0
     # via market-analy (pyproject.toml)
-fonttools==4.39.3
+fonttools==4.40.0
     # via matplotlib
 idna==3.4
     # via requests
-importlib-metadata==6.3.0
+importlib-metadata==6.6.0
     # via jupyter-client
 importlib-resources==5.12.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.22.0
+ipykernel==6.23.2
     # via ipywidgets
-ipython==8.12.0
+ipython==8.14.0
     # via
     #   ipykernel
     #   ipywidgets
-ipyvue==1.9.0
+ipyvue==1.9.1
     # via ipyvuetify
-ipyvuetify==1.8.5
+ipyvuetify==1.8.10
     # via market-analy (pyproject.toml)
 ipywidgets==8.0.6
     # via
     #   bqplot
     #   ipyvue
     #   market-analy (pyproject.toml)
 jedi==0.18.2
     # via ipython
 jinja2==3.1.2
     # via market-analy (pyproject.toml)
-jupyter-client==8.1.0
+jupyter-client==8.2.0
     # via ipykernel
 jupyter-core==5.3.0
     # via
     #   ipykernel
     #   jupyter-client
 jupyterlab-widgets==3.0.7
     # via ipywidgets
 kiwisolver==1.4.4
     # via matplotlib
 korean-lunar-calendar==0.3.1
     # via exchange-calendars
 lxml==4.9.2
     # via yahooquery
-market-prices==0.10.2
+market-prices==0.10.3
     # via market-analy (pyproject.toml)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 matplotlib==3.7.1
     # via market-analy (pyproject.toml)
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
 mypy-extensions==1.0.0
     # via black
 nest-asyncio==1.5.6
     # via ipykernel
-numpy==1.24.2
+numpy==1.24.3
     # via
     #   bqplot
     #   contourpy
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   matplotlib
     #   pandas
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   ipykernel
     #   matplotlib
     #   pytest
-pandas==2.0.0
+pandas==2.0.2
     # via
     #   bqplot
     #   exchange-calendars
     #   market-analy (pyproject.toml)
     #   market-prices
     #   yahooquery
 parso==0.8.3
     # via jedi
 pathspec==0.11.1
     # via black
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
-platformdirs==3.2.0
+platformdirs==3.5.3
     # via
     #   black
     #   jupyter-core
 pluggy==1.0.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
-psutil==5.9.4
+psutil==5.9.5
     # via ipykernel
 pure-eval==0.2.2
     # via stack-data
 pycodestyle==2.10.0
     # via flake8
-pydantic==1.10.7
+pydantic==1.10.9
     # via market-prices
 pydocstyle==6.3.0
     # via flake8-docstrings
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.1
     # via ipython
 pyluach==2.2.0
     # via exchange-calendars
 pyparsing==3.0.9
     # via matplotlib
-pytest==7.3.0
+pytest==7.3.2
     # via
     #   market-analy (pyproject.toml)
     #   pytest-mock
 pytest-mock==3.10.0
     # via market-analy (pyproject.toml)
 python-dateutil==2.8.2
     # via
@@ -178,19 +178,19 @@
 pytz==2023.3
     # via
     #   exchange-calendars
     #   market-prices
     #   pandas
 # pywin32==306
     # via jupyter-core
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
-requests==2.28.2
+requests==2.31.0
     # via requests-futures
 requests-futures==1.0.0
     # via yahooquery
 six==1.16.0
     # via
     #   asttokens
     #   python-dateutil
@@ -200,15 +200,15 @@
     # via ipython
 tomli==2.0.1
     # via
     #   black
     #   pytest
 toolz==0.12.0
     # via exchange-calendars
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
 tqdm==4.65.0
     # via yahooquery
 traitlets==5.9.0
     # via
@@ -220,22 +220,22 @@
     #   jupyter-client
     #   jupyter-core
     #   market-analy (pyproject.toml)
     #   matplotlib-inline
     #   traittypes
 traittypes==0.2.1
     # via bqplot
-typing-extensions==4.5.0
+typing-extensions==4.6.3
     # via
     #   black
     #   ipython
     #   pydantic
 tzdata==2023.3
     # via pandas
-urllib3==1.26.15
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 widgetsnbextension==4.0.7
     # via ipywidgets
 yahooquery==2.3.1
     # via market-prices
```

### Comparing `market_analy-0.2.3/pyproject.toml` & `market_analy-0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,20 @@
     "black",
     "flake8",
     "flake8-docstrings",
     "pytest",
     "pytest-mock",
 ]
 dev = [
-    "market_analy[tests]",
+    "black",
+    "flake8",
+    "flake8-docstrings",
+    "pytest",
+    "pytest-mock",
+    "jupyterlab>=3.0",
     "pandas-stubs",
     "types-pytz",
     "mypy",
     "pip-tools",
     "pre-commit",
     "pylint",
 ]
```

### Comparing `market_analy-0.2.3/src/market_analy/__init__.py` & `market_analy-0.3/src/market_analy/__init__.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/analysis.py` & `market_analy-0.3/src/market_analy/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     Test for Compare class.
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta
 from collections.abc import Callable, Sequence
-from typing import Union, Literal, Any
+from typing import Union, Literal, Any, TYPE_CHECKING
 from datetime import datetime
 
 from exchange_calendars import ExchangeCalendar
 import market_prices as mp
 import matplotlib as mpl
 import pandas as pd
 from pandas.io.formats.style import Styler
@@ -98,14 +98,19 @@
 from market_analy.utils.pandas_utils import rebase_to_row
 from market_analy.utils.mkt_prices_utils import (
     request_daily_prices,
     period_string,
     range_string,
 )
 
+if TYPE_CHECKING:
+    from market_analy.movements_base import MovementsBase
+    from market_analy.trends_base import TrendsProto
+from market_analy import trends
+
 Date = Union[str, datetime, None]
 Calendar = Union[str, ExchangeCalendar]
 Symbols = Union[str, list[str]]
 ChartEngine = Literal["bqplot", "matplotlib"]
 
 
 def pct_chg_top_to_bot(pd_obj: pd.Series | pd.DataFrame) -> pd.Series | float:
@@ -935,14 +940,119 @@
         return style_df_grid(
             df,
             format="{:.2f}",
             caption=caption,
             gradient_kwargs={"cmap": "RdBu", "vmin": -1, "vmax": 1},
         )
 
+    def movements(
+        self,
+        interval: mp.intervals.RowInterval,
+        trend_kwargs: dict,
+        trend_cls: type[TrendsProto] = trends.Trends,
+        **kwargs,
+    ) -> MovementsBase:
+        """Evaluate trends over a given period.
+
+        Parameters
+        ----------
+        interval
+            Price data interval to use for analysis, as 'interval`
+            parameter described by `help(self.prices.get)`.
+
+        trend_kwargs
+            Kwargs to pass to the `trend_cls`. Do not include 'data' or
+            'interval'.
+
+            For the default `trend_cls` (`trends.Trends`) the kwargs are
+            'prd', 'ext_break', 'ext_limit' and 'min_bars'. See
+            documentation for trends class with
+            `help(trends.Trends.__doc__)`.
+
+        trend_cls
+            Class to use to evaluate trends. Must fulfil protocol described
+            by `trends_base.TrendsProto`.
+
+            Default is `trends.Trends`.
+
+        **kwargs:
+            Parameters to define period / price data to be analysed. See
+            module doc with `help(analysis.__doc__)`.
+        """
+        data = self.prices.get(interval, lose_single_symbol=True, **kwargs)
+        if isinstance(data.index, pd.IntervalIndex):
+            data.index = data.index.left
+        return trend_cls(data, interval, **trend_kwargs).get_movements()
+
+    def trends_chart(
+        self,
+        interval: mp.intervals.RowInterval,
+        trend_kwargs: dict,
+        gui_cls: type[guis.TrendsGuiBase] = trends.TrendsGui,
+        max_ticks: int | None = None,
+        log_scale: bool = True,
+        display: bool = True,
+        **kwargs,
+    ) -> guis.TrendsGuiBase:
+        """Visualise trends on an OHLC chart.
+
+        Underlying trends data can be accessed via the following attributes
+        of the returned object:
+            movements: Movements (will confrom with
+            `movements_base.MovementsChartProto`).
+
+            trends: Instance of trends class responsible for evaluating
+            movement (will confrom with `trends_base.TrendsProto`).
+
+        Parameters
+        ----------
+        interval
+            Price data interval to use for analysis, as 'interval`
+            parameter described by `help(self.prices.get)`.
+
+        trend_kwargs
+            Kwargs to pass to the `gui_cls`. Do not include 'analysis' or
+            'interval'.
+
+            For the default `gui_cls` (`trends.TrendsGui`) the kwargs are
+            'prd', 'ext_break', 'ext_limit' and 'min_bars'. See
+            documentation for associated trends class with
+            `help(trends.Trends.__doc__)`.
+
+        gui_cls
+            Class to use to create gui to visualise evaluated trends. Must
+            be a subclass of `guis.TrendsGuiBase`.
+
+            Default is `trends.TrendsGui`.
+
+        max_ticks
+            Maximum number of bars (x-axis ticks) that will shown by
+            default (more can be shown via slider). None for no limit.
+
+        log_scale
+            True to plot prices against a log scale. False to plot prices
+            against a linear scale.
+
+        display
+            False to not display the GUI.
+
+        **kwargs:
+            Parameters to define period / price data to be analysed. See
+            module doc with `help(analysis.__doc__)`.
+        """
+        return gui_cls(
+            self,
+            interval,
+            **trend_kwargs,
+            max_ticks=max_ticks,
+            log_scale=log_scale,
+            display=display,
+            **kwargs,
+        )
+
 
 class Compare(Base):
     """Analyse and compare multiple instruments.
 
     Properties
     ----------
     symbols -> list[str]:
```

### Comparing `market_analy-0.2.3/src/market_analy/charts.py` & `market_analy-0.3/src/market_analy/charts.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,45 +26,73 @@
 PctChgBarMult(_PctChgBarBase):
     Bar Chart displaying precentage changes of multiple instruments.
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
+from collections import defaultdict
 from collections.abc import Callable
 from copy import copy, deepcopy
-from functools import lru_cache
+from functools import lru_cache, cached_property
+import typing
 from typing import Any, Literal
 
 import bqplot as bq
 import IPython
 import ipywidgets as w
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 
 from market_analy.formatters import FORMATTERS, formatter_datetime
 import market_analy.utils.bq_utils as ubq
 import market_analy.utils.pandas_utils as upd
 from market_analy.utils.dict_utils import set_kwargs_from_dflt
 
+if typing.TYPE_CHECKING:
+    from market_analy.movements_base import MovementProto, MovementsChartProto
+from market_analy.config import COL_ADV, COL_DEC
+
 
 COLOR_CHART_TEXT = "lightyellow"
 CHART_TITLE_STYLE = {"font-size": "20px", "fill": COLOR_CHART_TEXT}
 
 TOOLTIP_STYLE = {
     "opacity": 0.8,
     "background-color": "black",
     "border-color": "white",
     "border-width": "1px",
 }
 
 AxesKwargs = dict[ubq.ScaleKeys, dict[str, Any]]
 
 
+def tooltip_html_style(**kwargs) -> str | None:
+    """HTML to define inline style for a tooltip.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Dictionary of style attributes, for example:
+            color='blue'
+        NB where style attribute has a hyphen, replace with underscore,
+        for example pass line-height as:
+            line_height = 3
+    """
+    if not kwargs:
+        return None
+    s = 'style="'
+    for k, v in kwargs.items():
+        k = k.replace("_", "-")
+        s += f"{k}: {str(v)}; "
+    s = s + '"'
+    return s
+
+
 def hold_mark_update(func) -> Callable:
     """Hold off syncing mark in frontend until `func` executed.
 
     Decorator to hold off syncing mark in frontend until decorated
     function has fully executed.
     """
 
@@ -483,43 +511,22 @@
 
             Should return HTML string to be displayed in tooltip when
             hovering over mark and index as provided by received
             parameters.
         """
         raise NotImplementedError("_tooltip_value is not implemented.")
 
-    def _tooltip_style(self, **kwargs) -> str | None:
-        """HTML to define inline style for a tooltip.
-
-        Parameters
-        ----------
-        **kwargs : dict
-            Dictionary of style attributes, for example:
-                color='blue'
-            NB where style attribute has a hyphen, replace with underscore,
-            for example pass line-height as:
-                line_height = 3
-        """
-        if not kwargs:
-            return None
-        s = 'style="'
-        for k, v in kwargs.items():
-            k = k.replace("_", "-")
-            s += f"{k}: {str(v)}; "
-        s = s + '"'
-        return s
-
     def _hover_handler(self, mark, data):
         self.mark.tooltip.value = self._tooltip_value(mark, data)
 
     @property
     def _has_tooltip(self) -> bool:
         """True if subclass handles mark hover."""
         try:
-            return self._tooltip_value()
+            return bool(self._tooltip_value())
         except BaseException as err:
             if isinstance(err, NotImplementedError):
                 return False
             else:
                 return True
 
     @abstractmethod
@@ -1712,15 +1719,15 @@
     def MarkCls(self) -> type[bq.Mark]:
         return bq.OHLC
 
     def _tooltip_value(self, mark: bq.OHLC, event: dict) -> str:
         i = event["data"]["index"]
         row = self.data.iloc[i]
         color = mark.colors[0] if row.close >= row.open else mark.colors[1]
-        style = self._tooltip_style(color=color, line_height=1.3)
+        style = tooltip_html_style(color=color, line_height=1.3)
         s = f"<p {style}>From: " + formatter_datetime(row.name.left)
         s += f"<br>To: {formatter_datetime(row.name.right)}"
         for line in ["open", "high", "low", "close"]:
             v = getattr(row, line)
             s += "<br>" + line.capitalize() + ": " + FORMATTERS[line](v)
         s += "</p>"
         return s
@@ -1925,15 +1932,15 @@
         return super()._axes_kwargs(axes_kwargs)
 
     def _tooltip_value(self, mark, data):
         i = data["data"]["index"]
         y = data["data"]["y"]
         color_i = 0 if y < 0 else -1
         color = mark.scales["color"].colors[color_i]
-        style = self._tooltip_style(color=color, line_height=1.3)
+        style = tooltip_html_style(color=color, line_height=1.3)
         s = f"<p {style}>Date: " + formatter_datetime(self.plotted_x_ticks[i])
         s += "<br>Chg: " + FORMATTERS["pct_chg"](y) + "</p>"
         return s
 
     def _create_mark(self, **_) -> bq.Mark:
         kwargs = {
             "color": self.pct_chgs,
@@ -2030,25 +2037,25 @@
 
     def _tooltip_value(self, mark, data):
         i = data["data"]["index"]
         ci = data["data"]["colorIndex"]
         row = self.data.iloc[i]
         s = (
             "<p"
-            + self._tooltip_style(color="white")
+            + tooltip_html_style(color="white")
             + ">Date: "
             + formatter_datetime(row.name.left)
         )
         for i, tup in enumerate(row.items()):
             symbol, y = tup
-            symbol_style = self._tooltip_style(color=mark.colors[i])
+            symbol_style = tooltip_html_style(color=mark.colors[i])
             symbol_span = f"<span {symbol_style}>{symbol}: </span>"
             chg = FORMATTERS["pct_chg"](y)
             chg_color = "crimson" if y < 0 else "darkgreen"
-            chg_style = self._tooltip_style(color=chg_color)
+            chg_style = tooltip_html_style(color=chg_color)
             chg_span = f"<span {chg_style}>{chg}</span>"
             ss = f"{symbol_span}{chg_span}"
             weight = "bold" if i == ci else "normal"
             div_style = f'style="line-height: 1.3; font-weight: {weight}"'
             ss = f"<div {div_style}>{ss}</div>"
             s += ss
         s += "</p>"
@@ -2065,7 +2072,466 @@
     def _create_figure(self, **kwargs) -> bq.Figure:
         kwargs.setdefault("legend_location", "top-right")
         return super()._create_figure(**kwargs)
 
     def cycle_legend(self):
         """Move legend to next location."""
         self._cycle_legend()
+
+
+class OHLCTrends(OHLC):
+    """OHLC and Trend analysis for single financial instrument.
+
+    OHLC chart with trend overlay. Trend dislayed as coloured line where
+    green indicates a rising trend, red indicates a falling trend and
+    yellow indicates no trend (consolidation).
+
+    For each movement described by `movements` a scatter mark denotes:
+        movement start (triangle)
+        movement end (cross)
+        bar when movement start confirmed (circle)
+        bar when movement end confirmed (square)
+
+    Scatter marks for advancing movements are green, those for declining
+    movements are red.
+
+    Handlers on `movements`, as defined on `MovementsChartProto`, will be
+    enabled.
+
+    Parameters
+    ----------
+    As for OHLC base class and additionally:
+
+    movements
+        Movements representing trends over period to be charted. Must
+        be passed.
+
+    click_trend_handler
+        Any client-defined handler to be additionally called when user
+        clicks on any scatter point representing a trend start. Should have
+        signature:
+            f(mark: bq.Scatter, event: dict)
+
+        NB handler will be called after any handlers defined on
+        `movements`.
+
+    inc_conf_marks
+        Whether to include scatter marks indicating the bar / price at
+        which movements were confirmed to have started and ended.
+    """
+
+    COLOR_MAP = ["yellow", COL_ADV, COL_DEC]  # 0 consol, 1 adv, -1 dec
+
+    def __init__(
+        self,
+        prices: pd.DataFrame,
+        title: str,
+        visible_x_ticks: pd.Interval | None = None,
+        max_ticks: int | None = None,
+        log_scale: bool = True,
+        display: bool = False,
+        movements: MovementsChartProto | None = None,
+        click_trend_handler: Callable | None = None,
+        inc_conf_marks: bool = True,
+    ):
+        if movements is None:
+            raise ValueError("'movements' is a required argument.")
+        self._widgets_temp: list[w.Widget] = []  # used by hold temporary widgets
+        self._client_click_trend_handler = click_trend_handler
+        self._inc_conf_marks = inc_conf_marks
+        self.movements = movements
+
+        self._current_move: MovementProto | None = None
+        self.mark_trend: bq.FlexLine  # set by _create_mark
+        self.mark_scatters: list[bq.Scatter] = []  # set by _create_mark
+
+        # set by add_marks and remove_marks
+        self._added_marks: defaultdict[str, list[bq.Mark]] = defaultdict(list)
+
+        super().__init__(prices, title, visible_x_ticks, max_ticks, log_scale, display)
+
+        if max_ticks is not None or visible_x_ticks is not None:
+            self.update_trend_mark()
+
+    @cached_property
+    def _y_trend(self) -> pd.Series:
+        """y data for all points on trend line."""
+        # set starts of advances as day low, starts of declines as day high, ends
+        # of advances (that do not conincide with a subsequent trend start) as day
+        # high, ends of declines (that do not conincide with a subsequent trend
+        # start) as day low, otherwise as day close.
+        y = self.prices.close.copy()
+        subset = self.movements.starts_adv
+        y[subset] = self.prices.low[subset]
+        subset = self.movements.starts_dec
+        y[subset] = self.prices.high[subset]
+        subset = self.movements.ends_adv_solo
+        y[subset] = self.prices.high[subset]
+        subset = self.movements.ends_dec_solo
+        y[subset] = self.prices.low[subset]
+        return y
+
+    @cached_property
+    def _cols_trend(self) -> list[str]:
+        """color data for all points on trend line."""
+        return [self.COLOR_MAP[t] for t in self.movements.trend.values]
+
+    def _create_scales(self) -> dict[ubq.ScaleKeys, bq.Scale]:
+        scales = super()._create_scales()
+        scales["width"] = bq.LinearScale()
+        return scales
+
+    def create_scatter(
+        self,
+        x: pd.DatetimeIndex,
+        y: pd.Series,
+        color: str,
+        marker: str,
+        hover_handler: Callable | None,
+        click_handler: Callable | None = None,
+    ) -> bq.Scatter:
+        """Convenience method to create a scatter mark.
+
+        Parameters
+        ----------
+        x
+            `pd.DatetimeIndex` representing x values of scatter points.
+
+        y
+            y values of scatter points.
+
+        color
+            Scatter point color, for example "skyblue".
+
+        marker
+            Scatter point marker, for example "circle".
+
+        hover_handler
+            Callback to call if a scatter point is hovered over.
+
+        click_handler
+            Callback to call if a scatter point is LMB clicked.
+        """
+        mark = bq.Scatter(
+            scales=self.scales,
+            colors=[color],
+            x=x,
+            y=y,
+            marker=marker,
+            opacities=[0.65],
+            tooltip=w.HTML(value="<p>placeholder</p>"),
+            tooltip_style=TOOLTIP_STYLE,
+        )
+        if hover_handler is not None:
+            mark.on_hover(hover_handler)
+        if click_handler is not None:
+            mark.on_element_click(click_handler)
+        return mark
+
+    def _add_scatter(
+        self,
+        x: pd.DatetimeIndex,
+        y: pd.Series,
+        color: str,
+        marker: str,
+        hover_handler: Callable | None,
+        click_handler: Callable | None = None,
+    ) -> bq.Scatter:
+        """Add a scatter mark to `self.mark_scatters`."""
+        mark = self.create_scatter(x, y, color, marker, hover_handler, click_handler)
+        self.mark_scatters.append(mark)
+        return mark
+
+    def hide_scatters(self):
+        """Hide scatter marks.
+
+        Hides scatter marks denoting movements' starts, ends and, if
+        applicable, bars when movements' starts and ends were confirmed.
+        """
+        for m in self.mark_scatters:
+            m.visible = False
+
+    def show_scatters(self):
+        """Show scatter marks.
+
+        Shows scatter marks denoting movements' starts, ends and, if
+        applicable, bars when movements' starts and ends were confirmed.
+        """
+        for m in self.mark_scatters:
+            m.visible = True
+
+    @property
+    def current_move(self) -> MovementProto | None:
+        """Last selected movement."""
+        return self._current_move
+
+    def _handler_click_trend(self, mark: bq.Scatter, event: dict):
+        """Handler for clicking a scatter representing start of a trend."""
+        self._current_move = self.movements.mark_to_move(mark, event)
+        self.movements.handler_click_trend(self, mark, event)
+        if self._client_click_trend_handler is not None:
+            self._client_click_trend_handler(mark, event)
+
+    def _create_mark(self, **_) -> bq.OHLC:
+        """Create all marks.
+
+        Retains OHLC as principle mark, creating via subclass.
+
+        Adds FlexLine mark to represent trend.
+
+        Adds Scatter marks to represent, for each trend:
+            Start (triangle-up/triangle-down for adv/dec).
+            End (cross) only if does not coincide with subsequent
+                trend start.
+        If `inc_conf_marks` passed as True (default) to constructor then
+        will also iadd scattern marks to represent, for each trend:
+            Conf Start (circle)
+            Conf End (square).
+        """
+        self.mark_trend = bq.FlexLine(
+            scales=self.scales,
+            colors=self._cols_trend,
+            x=self._x_data,
+            y=self._y_trend,
+            stroke_width=2,
+        )
+
+        movements = self.movements
+
+        # scatter for starts of advancing trends
+        subset = movements.starts_adv
+        self._mark_scatter_starts_adv = self._add_scatter(
+            subset,
+            self._y_trend[subset],
+            COL_ADV,
+            "triangle-up",
+            movements.handler_hover_start,
+            self._handler_click_trend,
+        )
+        # scatter for starts of declining trends
+        subset = movements.starts_dec
+        self._mark_scatter_starts_dec = self._add_scatter(
+            subset,
+            self._y_trend[subset],
+            COL_DEC,
+            "triangle-down",
+            movements.handler_hover_start,
+            self._handler_click_trend,
+        )
+        # scatters for ends of trends, only if do not coincide with subsequent trend start
+        handler = movements.handler_hover_end
+        subset = movements.ends_adv_solo
+        self._add_scatter(subset, self._y_trend[subset], COL_ADV, "cross", handler)
+        subset = movements.ends_dec_solo
+        self._add_scatter(subset, self._y_trend[subset], COL_DEC, "cross", handler)
+
+        if self._inc_conf_marks:
+            # scatters for confirmed starts of trends
+            handler = movements.handler_hover_conf_start
+            self._add_scatter(
+                movements.starts_conf_adv,
+                movements.starts_conf_adv_px,
+                COL_ADV,
+                "circle",
+                handler,
+            )
+            self._add_scatter(
+                movements.starts_conf_dec,
+                movements.starts_conf_dec_px,
+                COL_DEC,
+                "circle",
+                handler,
+            )
+            # scatters for confirmed ends of trends
+            handler = movements.handler_hover_conf_end
+            self._add_scatter(
+                movements.ends_conf_adv,
+                movements.ends_conf_adv_px,
+                COL_ADV,
+                "square",
+                handler,
+            )
+            self._add_scatter(
+                movements.ends_conf_dec,
+                movements.ends_conf_dec_px,
+                COL_DEC,
+                "square",
+                handler,
+            )
+
+        opacities = [0.7] * len(self.prices)
+        return super()._create_mark(opacities=opacities)
+
+    def _create_figure(self, **_) -> bq.Figure:
+        marks = [self.mark, self.mark_trend] + self.mark_scatters
+        return super()._create_figure(marks=marks)
+
+    def update_trend_mark(self, *_):
+        """Update trend mark to reflect plotted x ticks.
+
+        Notes
+        -----
+        Like for the OHLC class, the OHLC mark is not updated to reflect changes
+        to the plotted data (`_update_mark_data_attr_to_reflect_plotted` is False
+        for the class) as the nature of the mark (discrete renders rather than a
+        continuous line) does not result in any side-effects when the visible
+        domain is shorter than that the mark data. The same is true (more or less)
+        for the Scatter marks. However, it is necessary to update the FlexLine
+        to reflect the plotted data to avoid the line doubling back over the render
+        as it tries to plot the 'next point after the visible range' to the start
+        of the x-axis.
+
+        This method serves as a handler which should be called by a client
+        whenever the plotted dates are changed. To handle everything within this
+        class had originally overriden the `self._x_domain_chg_handler` method
+        which is invoked whenever the x scales domain is changed (i.e. whenever
+        the plotted dates are changed), however, and regardless of whether
+        holding off the sync to the frontend of not, the 'wrapped back round'
+        line could continue to be left and other rendering issues were more
+        common than with the implemented solution.
+
+        An alternative approach to resolving the 'wrapped around line' is to set
+        line widths to 0 for the segments prior to the first and subsequent to the
+        last plotted interval. This still leaves a thin trace, for which also set
+        the colour of these segments to the same as the background colour. It's an
+        option, although found it rendered less smoothly that the implemented
+        approach (i.e. updating the marks values to reflect the plotted intervals).
+        """
+        self.mark_trend.x = self.plotted_x_ticks
+        self.mark_trend.y = self._y_trend[self._domain_bv]
+        self.mark_trend.colors = [
+            col for col, b in zip(self._cols_trend, self._domain_bv) if b
+        ]
+
+        index = next(
+            (i for i, m in enumerate(self.figure.marks) if m.name == "Flexible lines")
+        )
+        self.figure.marks = [m for m in self.figure.marks if m.name != "Flexible lines"]
+        self.figure.marks = (
+            self.figure.marks[:index] + [self.mark_trend] + self.figure.marks[index:]
+        )
+
+    def add_marks(self, marks: list[bq.Mark], group: str, under: bool = False):
+        """Add marks to the chart.
+
+        Parameters
+        ----------
+        marks
+            Marks to add.
+
+        group
+            Name of group to which to add marks. This can be subsequently
+            be passed to `remove_added_marks` to remove the added marks.
+
+        under
+            True: place marks under existing marks.
+            False: place marks on top of existing marks.
+        """
+        self._added_marks[group].extend(marks)
+        if under:
+            self.figure.marks = marks + [m for m in self.figure.marks]
+        else:
+            self.figure.marks = [m for m in self.figure.marks] + marks
+
+    def added_marks(self, group: str) -> list[bq.Mark]:
+        """Marks that have been added to the chart.
+
+        Parameters
+        ----------
+        group
+            Name of group of marks to return.
+
+        See Also
+        --------
+        add_marks : Add marks to the chart.
+        added_marks_groups : Names of groups of added marks.
+        remove_added_marks : Remove from the chart all marks in a group.
+        """
+        return self._added_marks[group]
+
+    @property
+    def added_marks_groups(self) -> list[str]:
+        """Names of groups of added marks."""
+        return list(self._added_marks.keys())
+
+    def remove_added_marks(self, group: str):
+        """Remove all marks in `group`."""
+        marks = self._added_marks[group]
+        for m in marks:
+            m.close()
+        self.figure.marks = [m for m in self.figure.marks if m not in marks]
+        del self._added_marks[group]
+
+    def remove_all_added_marks(self):
+        """Remove all added marks."""
+        for group in self.added_marks_groups:
+            self.remove_added_marks(group)
+
+    def reset_marks(self, reset_current_move: bool = True):
+        """Reset marks.
+
+        Removes all added marks. Makes all other marks visible.
+
+        Parameters
+        ----------
+        reset_current_move
+            If True (default), sets current_move to None.
+        """
+        self.remove_all_added_marks()
+        self.show_scatters()
+        if reset_current_move:
+            self._current_move = None
+
+    def close(self):
+        """Close all chart widgets."""
+        for marks in self._added_marks.values():
+            for m in marks:
+                m.close()
+        super().close()
+
+    def delete(self):
+        """Delete all chart widgets."""
+        self.remove_all_added_marks()
+        super().delete()
+
+    def _click_starts_adv(self, index: int):
+        """Simulate clicking an element of scatter representing advances starts."""
+        event = {"data": {"index": index}}
+        self._handler_click_trend(self._mark_scatter_starts_adv, event)
+
+    def _click_starts_dec(self, index: int):
+        """Simulate clicking an element of scatter representing declines starts."""
+        event = {"data": {"index": index}}
+        self._handler_click_trend(self._mark_scatter_starts_dec, event)
+
+    def show_next_move(self):
+        """Select movement that follows the currently selected movement.
+
+        If no movement is currently selected then selects first movement.
+        """
+        move = self.current_move
+        i = 0 if move is None else self.movements.get_index(move) + 1
+        if i == len(self.movements.moves):
+            return  # current movement is last movement
+
+        next_move = self.movements.moves[i]
+        i_ = 0 if move is None else self.movements.get_index(next_move, direction=True)
+        f = self._click_starts_adv if next_move.is_adv else self._click_starts_dec
+        f(i_)
+
+    def show_previous_move(self):
+        """Select movement prior to the currently selected movement.
+
+        If no movement is currently selected then selects last movement.
+        """
+        move = self.current_move
+        if move is not None:
+            i = self.movements.get_index(move) - 1
+            if i == -1:
+                return  # current movement is first movement
+        else:
+            i = -1
+
+        prev_move = self.movements.moves[i]
+        i_ = 0 if move is None else self.movements.get_index(prev_move, direction=True)
+        f = self._click_starts_adv if prev_move.is_adv else self._click_starts_dec
+        f(i_)
```

### Comparing `market_analy-0.2.3/src/market_analy/formatters.py` & `market_analy-0.3/src/market_analy/formatters.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/gui_parts.py` & `market_analy-0.3/src/market_analy/gui_parts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Definitions of widgets to contribute to GUI.
 
 Widgets define the GUI, they do NOT define any event handling.
 
 Functions
 ---------
-loading_overlay() -> vue.Overlay:
+loading_overlay() -> v.Overlay:
     Overlay application with transparent sheet with loading symbol.
 
 close_but() -> wu.ButtonIcon:
     Return 'Close' icon button.
 
 legend_but() -> vu.IconButton:
     Return `IconButton` to cycle legend location.
@@ -46,15 +46,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from contextlib import contextmanager
 import re
 
 import ipywidgets as w
-import ipyvuetify as vue
+import ipyvuetify as v
 from market_prices import intervals
 
 import market_analy.utils.ipywidgets_utils as wu
 import market_analy.utils.ipyvuetify_utils as vu
 from market_analy.utils.dict_utils import set_kwargs_from_dflt
 
 ICON_DIM = "35px"
@@ -149,18 +149,18 @@
 
     def set_value_unobserved(self, value: intervals.PTInterval):
         """Set value without triggering any handler."""
         with self._handler_disabled():
             self.value = value
 
 
-def loading_overlay() -> vue.Overlay:
+def loading_overlay() -> v.Overlay:
     """Overlay application with opaque sheet with loading symbol."""
-    prog = vue.ProgressCircular(indeterminate=True, color="white", size=30)
-    return vue.Overlay(color="grey", value=False, absolute=True, children=[prog])
+    prog = v.ProgressCircular(indeterminate=True, color="white", size=30)
+    return v.Overlay(color="grey", value=False, absolute=True, children=[prog])
 
 
 class Dialog(vu.Dialog):
     """Dialog box.
 
     Pass instance as child of component to be overlaid and within which
     dialog box to appear.
@@ -203,15 +203,15 @@
         tooltips = ["Max dates", "Reset", "Resize Chart", "Close"]
         if has_3_handlers:
             tooltips.remove("Reset")
         for i, child in enumerate(self.children):
             child.tooltip = tooltips[i]
 
 
-class TabsControl(vue.Tabs):
+class TabsControl(v.Tabs):
     """Tabs widget.
 
     Includes:
         Cursor tab, one row:
             ToggleIcons[+ - IconBut] // Divider // Lightbulb IconBut
                 // Trash IconBut
         Selector tab, one row:
@@ -231,21 +231,21 @@
     but_arrow_up: `IconBut`
     but_arrow_down: `IconBut`
     """
 
     _tab_container_class_ = "d-flex justify-center align-center"
 
     def __init__(self):
-        self.cursor_objs: vue.Layout
+        self.cursor_objs: v.Layout
         self.cursor_toggle: vu.ToggleIcons
         self.but_lightbulb: vu.IconBut
         self.but_trash: vu.IconBut
         self._create_cursor_tab_content()
 
-        self.slctr_objs: vue.Layout
+        self.slctr_objs: v.Layout
         self.but_zoom: vu.IconBut
         self.but_arrow_up: vu.IconBut
         self.but_arrow_down: vu.IconBut
         self._create_slctr_tab_content()
 
         tab_class_ = "text-lowercase font-weight-regular " + BG
 
@@ -258,15 +258,15 @@
         for text, tt, tt_kwargs in zip(texts, tooltips, tts_kwargs):
             tab_tt = vu.TabTt(
                 children=[text], class_=tab_class_, tooltip=tt, tt_kwargs=tt_kwargs
             ).tt
             tab_tt_list.append(tab_tt)
 
         tab_items = [
-            vue.TabItem(children=[layout], class_=BG)
+            v.TabItem(children=[layout], class_=BG)
             for layout in [self.cursor_objs, self.slctr_objs]
         ]
 
         tabs_class_ = "d-flex flex-column align-center flex-grow-0 " + BG
         super().__init__(
             v_model=0,
             children=tab_tt_list + tab_items,
@@ -315,15 +315,15 @@
         set_kwargs_from_dflt(tt_kwargs, TT_KWARGS_DFLT)
         self.but_trash = vu.IconBut(
             "fa-trash", color=color, tooltip=tt, tt_kwargs=tt_kwargs
         )
 
         cursor_buts = [self.but_lightbulb.tt, self.but_trash.tt]
         children = self.cursor_toggle.contain_me + [divider] + cursor_buts
-        self.cursor_objs = vue.Layout(
+        self.cursor_objs = v.Layout(
             children=children, class_=self._tab_container_class_
         )
 
     def _create_slctr_tab_content(self):
         def get_but(icon_name: str, color: str, tooltip: str) -> vu.IconBut:
             class_ = "mx-4 mb-2 mt-4"
             tt_kwargs = {"color": color}
@@ -343,15 +343,15 @@
         tt = "Evalute maximum advance over selected period"
         self.but_arrow_up = get_but("fa-arrow-circle-up", "light-green lighten-1", tt)
 
         tt = "Evalute maximum decline over selected period"
         self.but_arrow_down = get_but("fa-arrow-circle-down", "red lighten-1", tt)
 
         buts = [self.but_zoom.tt, self.but_arrow_up.tt, self.but_arrow_down.tt]
-        self.slctr_objs = vue.Layout(children=buts, class_=self._tab_container_class_)
+        self.slctr_objs = v.Layout(children=buts, class_=self._tab_container_class_)
 
     def reset(self):
         self.v_model = 0
         self.cursor_toggle.deselect()
 
 
 class HtmlOutput(w.HBox):
@@ -365,21 +365,24 @@
         )
         self._close_but.on_click(self._close_button_handler)
         self._hide_close_button()
 
         super().__init__(
             children=[self._html, self._close_but],
             layout=w.Layout(
-                justify_content="center", align_self="center", grid_gap="10px"
+                justify_content="center",
+                align_self="center",
+                grid_gap="10px",
+                margin="20px 0 0 0",
             ),
         )
 
     def _show_close_button(self):
         self._close_but.layout.visibility = "visible"
-        self._close_but.layout.margin = "25px 0 0 0"
+        self._close_but.layout.margin = "0 0 0 0"  # "25px 0 0 0"
 
     def _hide_close_button(self):
         self._close_but.layout.visibility = "hidden"
         self._close_but.layout.margin = "0 0 0 0"
 
     def display(self, html: str, add_padding: int = 0):
         """Display html.
@@ -576,20 +579,175 @@
         tooltip="Rebase prices",
         color="orange",
         handler=handler,
         **kwargs,
     )
 
 
-class PctChgIconRowMult(vue.Layout):
+class PctChgIconRowMult(v.Layout):
     """Percent change bar chart options for multiple instruments."""
 
     def __init__(self):
         self.bar_type_tog = BarTypeToggle()
         self.legend_cycle_but = legend_but()
 
         children = [
-            vue.Layout(children=self.bar_type_tog.contain_me, class_="flex-grow-0"),
+            v.Layout(children=self.bar_type_tog.contain_me, class_="flex-grow-0"),
             self.legend_cycle_but.tt,
         ]
 
         super().__init__(children=children, class_=BG, justify_space_around=True)
+
+
+class TrendControls(v.Layout):
+    """Container of controls for selecting and viewing trend movements.
+
+    Client should directly assign handlers to exposed buttons after
+    creating instance.
+
+    Includes vu.IconBut arranged as:
+
+                        but_next  //  but_prev
+        but_show_all //                           // but_ruler
+                        but_narrow  //  but_wide
+    """
+
+    _TURN_OFF_COLOR = "#CD853F"
+
+    def __init__(self):
+        self.but_show_all: vu.IconBut
+        self.but_next: vu.IconBut
+        self.but_prev: vu.IconBut
+        self.but_narrow: vu.IconBut
+        self.but_wide: vu.IconBut
+        self.but_ruler: vu.IconBut
+        self._buts: list[vu.IconBut] = []
+        self._dark = True
+
+        super().__init__(
+            children=[
+                self._create_show_all_container(),
+                self._create_trend_container(),
+                self._create_ruler_container(),
+            ],
+            class_="d-flex justify-start ml-2",
+        )
+
+    def _create_iconbut(
+        self,
+        icon_name: str,
+        tooltip: str,
+        color: str,
+        class_="mr-2",
+        dark: bool | None = None,
+    ) -> vu.IconBut:
+        if dark is None:
+            dark = self._dark
+        but = create_icon_but(
+            icon_name=icon_name,
+            tooltip=tooltip,
+            color=color,
+            class_=class_,
+            dark_color="grey",
+            dark=dark,
+        )
+        self._buts.append(but)
+        return but
+
+    def _create_show_all_container(self) -> v.Layout:
+        self.but_show_all = self._create_iconbut(
+            icon_name="mdi-chart-scatter-plot",
+            tooltip="Toggle visibilty of trend marks",
+            color="yellow",
+            class_="flex-grow-0 align-self-center",
+            dark=False,
+        )
+        return v.Layout(
+            children=[
+                v.Layout(
+                    children=[self.but_show_all.tt],
+                    class_="d-flex justify-start flex-grow-0 mr-2",
+                )
+            ],
+            class_="d-flex justify-start flex-grow-0",
+        )
+
+    def _create_prev_next_container(self) -> v.Layout:
+        self.but_prev = self._create_iconbut(
+            "mdi-arrow-left-circle", "Select previous movement", "#F0E68C"
+        )
+        self.but_next = self._create_iconbut(
+            "mdi-arrow-right-circle", "Select next movement", "#FFD700"
+        )
+        return v.Layout(
+            children=[self.but_prev.tt, self.but_next.tt],
+            class_="d-flex justify-start mb-2",
+        )
+
+    def _create_narrow_wide_view_container(self) -> v.Layout:
+        self.but_narrow = self._create_iconbut(
+            "mdi-arrow-expand-horizontal",
+            "Narrow view around selected movement",
+            "#BDB76B",
+        )
+        self.but_wide = self._create_iconbut(
+            "mdi-arrow-left-right", "Wide view around selected movement", "#BDB76B"
+        )
+        return v.Layout(
+            children=[self.but_narrow.tt, self.but_wide.tt],
+            class_="d-flex justify-start",
+        )
+
+    def _create_trend_container(self) -> v.Layout:
+        contain_prev_next = self._create_prev_next_container()
+        contain_narrow_wide = self._create_narrow_wide_view_container()
+        return v.Layout(
+            children=[contain_prev_next, contain_narrow_wide],
+            class_="d-flex flex-column justify-center flex-grow-0 ml-2",
+        )
+
+    def but_ruler_handler(self, but: vu.IconBut, event: str, data: dict):
+        """Handler to toggle ruler but color light/red if group not dark."""
+        if but.is_dark:
+            return
+        if but.is_light:
+            but.icon_color = self._TURN_OFF_COLOR
+            return
+        f = but.darken if self.is_dark_single_trend else but.lighten
+        f()
+
+    def _create_ruler_container(self) -> v.Layout:
+        self.but_ruler = self._create_iconbut(
+            icon_name="mdi-ruler",
+            tooltip="Show ruler with width of trend period",
+            color="yellow",
+            class_="flex-grow-0 align-self-center",
+        )
+        self.but_ruler.on_event("click", self.but_ruler_handler)
+        return v.Layout(
+            children=[self.but_ruler.tt],
+            class_="d-flex justify-start flex-grow-1",
+        )
+
+    @property
+    def is_dark_single_trend(self) -> bool:
+        """Query if icons for single-trend actions are dark."""
+        return self._dark
+
+    def darken_single_trend(self):
+        """Darken icon buttons for single-trend actions.
+
+        Will not darken any icon waiting to be switched off.
+        """
+        for but in self._buts:
+            if (but.icon_color == self._TURN_OFF_COLOR) or but is self.but_show_all:
+                continue
+            but.darken()
+        self._dark = True
+
+    def lighten_single_trend(self):
+        """Lighten icon buttons for single-trend actions."""
+        for but in self._buts:
+            if but is self.but_show_all:
+                continue
+            but.lighten()
+        self._dark = False
```

### Comparing `market_analy-0.2.3/src/market_analy/guis.py` & `market_analy-0.3/src/market_analy/guis.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,33 +28,37 @@
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable
 from contextlib import contextmanager
-from typing import Literal
+from typing import Literal, TYPE_CHECKING
 
 import bqplot as bq
 from bqplot.interacts import Selector
 import exchange_calendars as xcals
 import IPython
 import ipyvuetify as v
 import ipywidgets as w
 import market_prices as mp
 from market_prices.intervals import TDInterval, PTInterval, to_ptinterval, ONE_DAY
 import pandas as pd
 
 from market_analy import charts, gui_parts, analysis
-from market_analy.utils.bq_utils import Crosshairs, FastIntervalSelectorDD
+from market_analy.trends_base import TrendsProto
+from market_analy.utils.bq_utils import Crosshairs, FastIntervalSelectorDD, HFixedRule
 from market_analy.utils.dict_utils import set_kwargs_from_dflt
 import market_analy.utils.ipyvuetify_utils as vu
 import market_analy.utils.ipywidgets_utils as wu
 import market_analy.utils.pandas_utils as upd
 
+if TYPE_CHECKING:
+    from market_analy.movements_base import MovementProto, MovementsChartProto
+
 # CONSTANTS
 HIGHLIGHT_COLOR = "lightyellow"
 
 
 class Base(metaclass=ABCMeta):
     """ABC for creating GUI.
 
@@ -642,27 +646,28 @@
             described by `help(analysis.prices.get)`.
 
         max_ticks
             Maximum number of x-axis ticks that will shown by default (client
             can choose to show more via slider). None for no limit.
 
         log_scale
-            True to chart prices against a log scale.
+            True to plot prices against a log scale. False to plot prices
+            against a linear scale.
 
         display
             True to display created GUI.
 
         chart_kwargs
             Any kwargs to pass on to the chart class.
 
         **kwargs
             Period for which to plot prices. Passed as period parameters as
-            described by market-prices documentation for `PricesCls.get`
-            method where `PricesCls` is the class that was passed to
-            `PricesCls` parameter of `mkt_anlaysis.Analysis` to intantiate
+            described by market-prices documentation for 'PricesCls.get'
+            method where 'PricesCls' is the class that was passed to
+            'PricesCls' parameter of `mkt_anlaysis.Analysis` to intantiate
             `analysis`.
         """
         assert issubclass(self.ChartCls, charts.BasePrice)
         chart_kwargs = {} if chart_kwargs is None else chart_kwargs
         ptinterval = None if interval is None else to_ptinterval(interval)
         self._analysis = analysis
         self._initial_price_params: dict  # set by _get_initial_prices
@@ -1258,24 +1263,25 @@
             if True will rebase prices following zoom.
 
         max_ticks
             Maximum number of x-axis ticks that will shown by default
             (client can choose to show more via slider). None for no limit.
 
         log_scale
-            True to chart prices against a log scale.
+            True to plot prices against a log scale. False to plot prices
+            against a linear scale.
 
         display
             True to display created GUI.
 
         **kwargs
             Period for which to plot prices. Passed as period parameters as
-            described by market-prices documentation for `PricesCls.get`
-            method where `PricesCls` is the class that was passed to
-            `PricesCls` parameter of `mkt_anlaysis.Compare` to intantiate
+            described by market-prices documentation for 'PricesCls.get'
+            method where 'PricesCls' is the class that was passed to
+            'PricesCls' parameter of `mkt_anlaysis.Compare` to intantiate
             `analysis`.
         """
         self._rebase_on_zoom = rebase_on_zoom
         self._labels: list[str]  # set by --_get_initial_prices--
         super().__init__(analysis, interval, max_ticks, log_scale, display, **kwargs)
 
     @property
@@ -1545,15 +1551,15 @@
             i += 1
             higher = data[index][1] > data[index - i][1]
             lower = data[index][2] < data[index - i][2]
             if i == 100:
                 raise StopIteration("breaking infinite loop.")
         y = data[index][1] if higher else data[index][2]
 
-        self.add_crosshair(x=x, y=y)
+        self.add_crosshair(x=x, y=y, existing_mark=mark)
 
     def _display_mark_data(self, mark: bq.OHLC, event: dict):
         s = self.chart._tooltip_value(mark, event)
         self.html_output.display(s)
 
     @property
     def last_selected(self) -> pd.Series:
@@ -1685,7 +1691,354 @@
         super()._create_gui_parts()
         self._icon_row = self._create_icon_row()
         self._set_icon_row_handlers()
 
     @property
     def _gui_box_contents(self) -> list[w.Widget]:
         return super()._gui_box_contents + [self._icon_row]
+
+
+class TrendsGuiBase(ChartOHLC):
+    """GUI to display and interact with trend analysis over OHLC Chart.
+
+    Parameters
+    ----------
+    analysis
+        Analysis instance representing instrument to be plotted.
+
+    interval
+        Interval covered by one bar (i.e. one x-axis tick). As 'interval`
+        parameter described by `help(analysis.prices.get)`.
+
+    trend_cls
+        Class to use to analyse trends. Must conform with
+        `trends_base.TrendsProto`, for example, `trends.Trends`.
+
+    trend_kwargs
+        Arguments to pass to `trend_cls`. Do not include `data` or
+        `interval`.
+
+    max_ticks
+        Maximum number of bars (x-axis ticks) that will shown by default
+        (client can choose to show more via slider). None for no limit.
+
+    log_scale
+        True to plot prices against a log scale. False to plot prices
+        against a linear scale.
+
+    display
+        True to display created GUI.
+
+    narrow_view
+        When displaying a movement in 'narrow' view, the number of bars
+        that should be shown before the bar representing the movement's
+        start and after the bar representing the movement's confirmed end.
+
+    wide_view
+        When displaying a movement in 'wide' view, the number of bars that
+        should be shown before the bar representing the movement's start
+        and after the bar representing the movement's confirmed end.
+
+    chart_kwargs
+        Any kwargs to pass on to the chart class.
+
+    **kwargs
+        Period for which to plot prices. Passed as period parameters as
+        described by market-prices documentation for 'PricesCls.get'
+        method where 'PricesCls' is the class that was passed to
+        'PricesCls' parameter of `mkt_anlaysis.Analysis` to intantiate
+        `analysis` (for example, documenation for
+        'market_prices.PricesYahoo.get').
+
+    Notes
+    -----
+    -- Subclass Implementation --
+
+    This base class can be subclassed, including for the purposes of:
+
+        Passing through the required `trend_cls` and concreting in its own
+        constructor arguments passed on to this base as `trend_kwargs`.
+
+        Concrete constructor arguments such as `narrow_view`, `wide_view`
+        etc.
+
+        Defining the `_gui_click_trend_handler` method to customise the
+        handling, at a gui level, of clicking a mark representing the start
+        of a trend. NB Alternatively a handler can be passed within
+        `chart_kwargs` with the key 'click_trend_handler'.
+
+    -- Horrible Hack --
+
+    This class current incorporates at least one horrible hack.
+
+    The trend movements must be based on the same data as the chart.
+    However, the initial chart data is requested within the `BasePrice`
+    subclass' contribution to the constructor. This happens shortly before
+    the chart is created by the `_create_chart` method as defined on the
+    `Base` class and which isn't intended to be extended. So, how to get
+    access to the chart data between these two points in order to be able
+    to evaluate the Movements and pass them to the chart class along with
+    its data? Yup, extend the `_create_chart` method.
+
+    The `BasePrice` class exists not so much to be able to get the initial
+    price data, but to be able to make subsequent calls to get data at
+    different intervals. This behaviour is not required for this
+    `TrendsGuiBase` class which is intended to house a chart based on
+    static data. However, as the OHLC class inherits from `BasePrice`,
+    so must this `TrendsGuiBase` class.
+
+    I suspect the preferable approach to all this would be to lose the
+    inheritance and instead go with a pick-n-mix composition
+    implementation. Could define components as isolated classes, the
+    constructor of each making requirements in terms of attibutes or
+    methods of other components that it requires in order to work. Classes
+    could include the likes of:
+        Prices
+            To administer all things prices, requesting and updating the
+            chart to reflect the changes. Would only be required by GUIs
+            that provide for updating / changing the data. The interval
+            selector buttons would either be included to this component
+            or defined as its own dedicated component.
+
+        Selector
+            To select periods.
+
+        Crosshairs
+            To administer crosshairs.
+
+        TabsControl
+            UI to create crosshairs and undertake analysis.
+
+        DataSlider
+            To scross through plot dates.
+
+    Before diving in would need to have a look at the current
+    implementation and have a think about how to best implement a
+    compositional approach.
+    """
+
+    _HAS_INTERVAL_SELECTOR = False
+
+    def __init__(
+        self,
+        analysis: analysis.Analysis,
+        interval: mp.intervals.RowInterval,
+        trend_cls: type[TrendsProto],
+        trend_kwargs: dict,
+        max_ticks: int | None = None,
+        log_scale: bool = True,
+        display: bool = True,
+        narrow_view: int = 10,
+        wide_view: int = 10,
+        chart_kwargs: dict | None = None,
+        **kwargs,
+    ):
+        self.movements: MovementsChartProto  # set by _create_chart
+        self.trends: TrendsProto  # set by _create_chart
+        self._trends_cls = trend_cls
+        self._trends_kwargs = trend_kwargs
+        self._narrow_view = narrow_view
+        self._wide_view = wide_view
+        chart_kwargs = {} if chart_kwargs is None else chart_kwargs
+        chart_kwargs.setdefault("click_trend_handler", self._gui_click_trend_handler)
+        super().__init__(
+            analysis, interval, max_ticks, log_scale, display, chart_kwargs, **kwargs
+        )
+        self._rulers: list = []
+
+    @property
+    def ChartCls(self) -> type[charts.Base]:
+        return charts.OHLCTrends
+
+    @property
+    def _chart_title(self) -> str:
+        return self._analysis.symbol + " Trend Analysis"
+
+    def _create_chart(
+        self, data: pd.DataFrame | pd.Series, title: str | None, **kwargs
+    ) -> charts.Base:
+        """Create chart.
+
+        Notes
+        -----
+        This is a horrible hack, see the Notes section of the class doc.
+        """
+        data_moves = data.copy()
+        if isinstance(data_moves.index, pd.IntervalIndex):
+            data_moves.index = data_moves.index.left
+            if data_moves.index.tz is not None:
+                data_moves.index = data_moves.index.tz_localize(None)
+        interval = self._initial_price_params["interval"]
+        self.trends = self._trends_cls(data_moves, interval, **self._trends_kwargs)
+        self.movements = self.trends.get_movements()
+        kwargs.setdefault("movements", self.movements)
+        return super()._create_chart(data, title, **kwargs)
+
+    @property
+    def _icon_row_top_handlers(self) -> list[Callable]:
+        return [self._max_x_ticks, self._resize_chart, self.close]
+
+    def _show_all_but_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_light:
+            self.chart.hide_scatters()
+            but.darken()
+            return
+
+        if self.current_move is not None:
+            self.chart.reset_marks()
+            self.trends_controls_container.darken_single_trend()
+        else:
+            self.chart.show_scatters()
+        but.lighten()
+
+    def _show_next_move_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_dark:
+            return
+        self.chart.show_next_move()
+
+    def _show_prev_move_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_dark:
+            return
+        self.chart.show_previous_move()
+
+    def _set_slider_to_current_move(self, bars: int):
+        """Set slider to focus on currently selected movement.
+
+        Parameters
+        ----------
+        bars
+            Number of bars to view prior to movement start and following
+            movement's confirmed end.
+        """
+        if self.current_move is None:
+            return
+        index = self.movements.data.index
+        start = max(index.get_loc(self.current_move.start) - bars, 0)
+        end = self.current_move.end_conf
+        if end is None:
+            stop = len(index) - 1
+        else:
+            stop = min(index.get_loc(end) + bars, len(index) - 1)
+        self.date_slider.interval = pd.Interval(index[start], index[stop], "both")
+
+    def _narrow_view_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_dark:
+            return
+        self._set_slider_to_current_move(self._narrow_view)
+
+    def _wide_view_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_dark:
+            return
+        self._set_slider_to_current_move(self._wide_view)
+
+    def _close_rulers(self):
+        for ruler in self._rulers:
+            ruler.close()
+        self._rulers = []
+
+    def _add_rulers(self):
+        self._close_rulers()  # close any existing
+        ohlc_mark = next(m for m in self.chart.figure.marks if isinstance(m, bq.OHLC))
+        self._rulers.append(
+            HFixedRule(
+                level=self.current_move.start_px,
+                scales=self.chart.scales,
+                figure=self.chart.figure,
+                start=self.current_move.start.asm8,
+                length=self.current_move.params["prd"],
+                color="yellow",
+                draggable=True,
+                ordinal_values=list(ohlc_mark.x),
+                stroke_width=5,
+            )
+        )
+
+    def _ruler_handler(self, but: vu.IconBut, event: str, data: dict):
+        if but.is_dark:
+            return
+        f = self._add_rulers if but.is_light else self._close_rulers
+        f()
+        # chain handlers...
+        self.trends_controls_container.but_ruler_handler(but, event, data)
+
+    def _create_trends_controls_container(self) -> v.Layout:
+        controls = gui_parts.TrendControls()
+        controls.but_show_all.on_event("click", self._show_all_but_handler)
+        controls.but_next.on_event("click", self._show_next_move_handler)
+        controls.but_prev.on_event("click", self._show_prev_move_handler)
+        controls.but_narrow.on_event("click", self._narrow_view_handler)
+        controls.but_wide.on_event("click", self._wide_view_handler)
+        controls.but_ruler.on_event("click", self._ruler_handler)
+        return controls
+
+    def _create_controls_container(self) -> v.Layout:
+        self._tabs_control_container = v.Layout(
+            children=[self.tabs_control], class_="d-flex justify-end mr-2"
+        )
+        self.trends_controls_container = self._create_trends_controls_container()
+        return v.Layout(
+            children=[self._tabs_control_container, self.trends_controls_container],
+            class_="d-flex align-center justify-center",
+        )
+
+    def _create_gui_parts(self):
+        super()._create_gui_parts()
+        self._controls_container = self._create_controls_container()
+
+    @property
+    def _gui_box_contents(self) -> list[w.Widget]:
+        contents = [
+            self._icon_row_top,
+            self.chart.figure,
+            self.date_slider,
+            self._controls_container,
+            self.html_output,
+        ]
+        return contents
+
+    def _create_date_slider(self, **kwargs):
+        ds = super()._create_date_slider(**kwargs)
+        ds.slider.observe(self.chart.update_trend_mark, ["index"])
+        return ds
+
+    @property
+    def current_move(self) -> MovementProto | None:
+        """Currently selected Movement.
+
+        None if no movement has been selected.
+        """
+        return self.chart.current_move
+
+    def _gui_click_trend_handler(self, mark: bq.Scatter, event: dict):
+        """Gui level handler for clicking marker representing trend start.
+
+        Subclass should define if required
+        """
+
+    @contextmanager
+    def _handler_disabled(self):
+        """Undertake an operation within context of disabled handler.
+
+        Undertake an operation with context of slider's handlers being
+        disabled.
+
+        Notes
+        -----
+        Messily overrides method defined on `BaseVariableDates` subclass to
+        include the additional `self.chart.update_trend_mark` handler.
+        """
+        self._slider.unobserve(self._set_chart_x_ticks_to_slider, ["index"])
+        self._slider.unobserve(self.chart.update_trend_mark, ["index"])
+        yield
+        self._slider.observe(self._set_chart_x_ticks_to_slider, ["index"])
+        self._slider.observe(self.chart.update_trend_mark, ["index"])
+
+    def _max_x_ticks(self):
+        """Show data for all plottable x-ticks (bars).
+
+        Notes
+        -----
+        Overrides inherited method to ensure trend mark is also updated.
+        """
+        self.chart.reset_x_ticks()
+        self._set_slider_limits_to_all_plottable_x_ticks()
+        self.chart.update_trend_mark()
```

### Comparing `market_analy-0.2.3/src/market_analy/utils/dict_utils.py` & `market_analy-0.3/src/market_analy/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/utils/ipyvuetify_utils.py` & `market_analy-0.3/src/market_analy/utils/ipyvuetify_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,24 @@
         """Darken icon color."""
         self.icon_color = self.color_dark
 
     def lighten(self):
         """Lighten icon color."""
         self.icon_color = self.color_light
 
+    @property
+    def is_dark(self) -> bool:
+        """Query if icon is dark."""
+        return self.icon_color == self.color_dark
+
+    @property
+    def is_light(self) -> bool:
+        """Query if icon is light."""
+        return self.icon_color == self.color_light
+
 
 class ToggleIcon(IconBut):
     """Selectable `IconBut`.
 
     Clicking `IconBut` toggles selection. Optionally:
         Define selected and unselected icon colors.
         Set selecting/deselecting handlers.
```

### Comparing `market_analy-0.2.3/src/market_analy/utils/ipywidgets_utils.py` & `market_analy-0.3/src/market_analy/utils/ipywidgets_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/utils/list_utils.py` & `market_analy-0.3/src/market_analy/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/utils/mkt_prices_utils.py` & `market_analy-0.3/src/market_analy/utils/mkt_prices_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy/utils/pandas_utils.py` & `market_analy-0.3/src/market_analy/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `market_analy-0.2.3/src/market_analy.egg-info/PKG-INFO` & `market_analy-0.3/src/market_analy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-analy
-Version: 0.2.3
+Version: 0.3
 Summary: Analysis of exchange-listed financial instruments
 Author: Marcus Read
 Author-email: marcusaread@gmail.com
 License: MIT License
 Project-URL: homepage, https://github.com/maread99/market_analy
 Project-URL: documentation, https://github.com/maread99/market_analy
 Project-URL: Issue Tracker, https://github.com/maread99/market_analy/issues
@@ -40,89 +40,106 @@
 
 -----------------
 
 # market_analy
 
 [![PyPI](https://img.shields.io/pypi/v/market-analy)](https://pypi.org/project/market-analy/) ![Python Support](https://img.shields.io/pypi/pyversions/market-analy) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-A python package to analyse financial instruments.
+A python package for interactive charting and analysis of financial instruments.
 
-There's a load of great financial libraries out there for Technical Analysis, Charting, Backtesting, Portfolio Analysis etc. This library isn't reinventing the wheel (not intentionally anyway), rather it provides functions and interactive charting that I think are useful and couldn't find elsewhere. It's not comprehensive, but rather fills some of the gaps.
+Functionality includes **defining and visualising trends**.
 
-Some functionality is general, some is focused on defining and identifying trends. Interactive charting is offered via guis created from widgets of the bqplot, ipywidgets and ipyvuetify libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
+Interactive charting is offered via guis created from widgets of the [bqplot](https://github.com/bqplot/bqplot), [ipywidgets](https://github.com/jupyter-widgets/ipywidgets) and [ipyvuetify](https://github.com/widgetti/ipyvuetify) libraries. Users can use the underlying parts to develop their own interactive charts and analyses. Contributions very much welcome! This is a WIP and it's anticipated that further analyses will be added.
 
-The [demo video](https://vimeo.com/801302973) gives an overview of what´s on offer. All analyses are accessed via the classes `analysis.Analysis` (single instrument analyses) and `analysis.Compare` (to compare multiple instruments). For example:
+There's a load of great financial libraries out there. This library isn't reinventing the wheel (not intentionally anyway), rather it principally provides functions and interactive charting that I think are useful and couldn't find elsewhere.
+
+## Video tutorials
+
+The following videos cover what's on offer:
+* [General tutorial](https://vimeo.com/801302973) demonstrates the functionality as of the initial release (February 2023).
+* [Trends](https://vimeo.com/835495038) demonstrates functionality (added June 2023) to define and visualise trends.
+
+## Quickstart
+All analyses can be accessed via the classes `Analysis` (single instrument analyses) and `Compare` (to compare multiple instruments). For example:
 
 ```python
 from market_prices import PricesYahoo
 from market_analy import Analysis,  Compare
 
 prices = PricesYahoo("MSFT")
 analy = Analysis(prices)
 gui = analy.plot(days=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773777-df0d0bec-bbe1-45bb-b067-d679666450cd.mp4
 
 ```python
+trend_kwargs = {
+    "prd":60,
+    "ext_break":0.05,
+    "ext_limit":0.03,
+    "min_bars":5,
+}
+gui = analy.trends_chart(
+    "1D",
+    trend_kwargs,
+    years=3,
+)
+```
+https://github.com/maread99/market_analy/assets/56914820/998c7f46-20f5-43f1-8b82-c857c0702cee
+
+```python
 comp = Compare(PricesYahoo("MSFT, AMZN, TSLA"))
 gui = comp.plot(hours=30)
 ```
 https://user-images.githubusercontent.com/56914820/220773790-1fdabf13-25bb-4205-acc2-6bac9b832dae.mp4
 
 ```python
 gui = comp.chg_every_interval("20T", days=5, chart=True)
 ```
 https://user-images.githubusercontent.com/56914820/220773802-ae329259-4a4e-4e5e-8d02-d4ee88b8b452.mp4
 
-
-For further documentation, see the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
+For further documentation see the [video tutorials](#Video-tutorials) and the [analysis](https://github.com/maread99/market_analy/blob/master/src/market_analy/analysis.py) module.
 
 ## Installation and environment
 
 It's recommended that `market-analy` is installed to a new virtual environment created using `venv`.
 
 The package can be installed to the activated environment via pip:
 
 `$ pip install market-analy`
 
-Plots are intended to be created in a Jupyter Notebook or JupyterLab. The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
+Plots are intended to be created in JupyterLab (they will not load in a notebook opened in VSCode). The 'jupyter' optional dependencies can be specified to additionally install `jupyter` and `jupyterlab` to the target environment.
 
 `$ pip install market-analy[jupyter]`
 
-Then call:
-
-`jupyter nbextension enable --py --sys-prefix ipyvuetify`
-
-Alternatively, it's possible to use an existing Jupyter installation in a separate environment to that in which `market_analy` is installed. In this case:
-* The following dependencies should additionally be installed **in the environment to which Jupyter is installed**:
-  - `jupyterlab>=3.0`
+Alternatively, it's possible to use an existing JupyterLab installation (>=3.0) in a separate environment to that in which `market_analy` is installed. In this case:
+* The following dependencies should additionally be installed **in the environment to which JupyterLab is installed**:
   - `ipyvuetify`
   - `bqplot`
-* Jupyter should be called with the following arguments:
-  - `jupyter nbextension enable --py --sys-prefix ipyvuetify`
+* A kernel should be created for **the environment to which `market_analy` was installed**. Executing the following, with any virutal environment activated, will create a kernel and make it available to all installed versions of `jupyterlab`.
+  - `python -m ipykernel install --user --name mkt_analy --display-name "market analy env"`
 
-> :information_source: Unfortunately plots do not render in a VSCode notebook.
+> :warning: If starting JupyterLab from a different environment to the environment in which `market_analy` is installed then **the same versions of `ipyvuetify` and `bqplot` must be installed to both environments**. If either of these packages is subsequently upgraded in one environment then it must also be upgraded in the other. (This is due to the potential for conflicts between the versions in the JupyterLab environment, which are responsible for the frontend, and those in the `market_analy` environment where the backend is defined.)
 
 ### Color scheme
 The color scheme assumes the package is being used with the JupyterLab dark theme. There are no plans to provide a 'light theme' option (although a contribution would certainly be welcome from anyone seeking one).
 
 ### `market-prices` dependency
 `market-analy` depends on the [market-prices][market-prices] library for price data. This provides for functionality including:
 * defining analysis periods in terms of number of sessions and trading minutes rather than calendar days and times.
 * complete data sets regardless of liquidity (regular data points during market hours, no data points outside of market hours).
 
 Most of the arguments available to the market-prices `get` function can be passed directly to the `market_analy` functions. See the [market-prices][market-prices] documentation for further info.
 
 ## Release schedule, bugs, development and feedback
-
-The first beta version of `market_analy` was released Feb 2023. It's anticipated that functionality to define and visually interrogate trends will be added later in 2023.
+The first beta version of `market_analy` was released Feb 2023. Functionality to  define and visually interrogate trends was added in June 2023.
 
 The project is immature. Whilst it's not anticipated that major changes will be made to the existing public side, they could be. All that's under-the-bonnet is subject to change as the project evolves. The `guis` module in particular won't permit much further development without overhauling the current inheritance-based approach to a compositional one.
 
-The test suite is limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
+The test suite is somewhat limited. It's pretty much guaranteed that there are bugs. Please raise an [issue](https://github.com/maread99/market_analy/issues) if you find one or come across unexpected behaviour.
 
 Please use [discussions](https://github.com/maread99/market_analy/discussions) to make any suggestions and offer general feedback.
 
 ## Disclaimers
 `market-analy` should not be assumed sufficiently reliable to undertake analysis intended to inform investment decisions. Users should inspect the source code and the test suite of the library and its dependencies in order to make their own assessment of the packages' suitability for their purposes. **The `market-analy` package is used entirely at the user's own risk.**
 
 The default `market_prices.PricesYahoo` class gets data from publically available Yahoo APIs. **See the [Disclaimers section of the market-prices README](https://github.com/maread99/market_prices#disclaimers) for conditions of use**, including restrictions.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `market_analy-0.2.3/src/market_analy.egg-info/SOURCES.txt` & `market_analy-0.3/src/market_analy.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 etc/requirements_tests.txt
 etc/requirements/requirements.txt
 etc/requirements/why_here.txt
 src/market_analy/__init__.py
 src/market_analy/_version.py
 src/market_analy/analysis.py
 src/market_analy/charts.py
+src/market_analy/config.py
 src/market_analy/formatters.py
 src/market_analy/gui_parts.py
 src/market_analy/guis.py
+src/market_analy/movements_base.py
+src/market_analy/trends.py
+src/market_analy/trends_alt.py
+src/market_analy/trends_base.py
 src/market_analy.egg-info/PKG-INFO
 src/market_analy.egg-info/SOURCES.txt
 src/market_analy.egg-info/dependency_links.txt
 src/market_analy.egg-info/requires.txt
 src/market_analy.egg-info/top_level.txt
 src/market_analy/utils/__init__.py
 src/market_analy/utils/bq_utils.py
```

