# Comparing `tmp/tdameritrade-0.1.1.tar.gz` & `tmp/tdameritrade-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tdameritrade-0.1.1.tar", last modified: Mon Jul  6 14:50:44 2020, max compression
+gzip compressed data, was "tdameritrade-0.2.0.tar", last modified: Tue Jun 13 15:26:32 2023, max compression
```

## Comparing `tdameritrade-0.1.1.tar` & `tdameritrade-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/
--rw-r--r--   0 theocean154   (501) staff       (20)      401 2020-06-17 03:19:09.000000 tdameritrade-0.1.1/.bumpversion.cfg
--rw-r--r--   0 theocean154   (501) staff       (20)    11357 2018-08-01 16:25:58.000000 tdameritrade-0.1.1/LICENSE
--rw-r--r--   0 theocean154   (501) staff       (20)      344 2019-12-27 21:33:37.000000 tdameritrade-0.1.1/MANIFEST.in
--rw-r--r--   0 theocean154   (501) staff       (20)     1390 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/Makefile
--rw-r--r--   0 theocean154   (501) staff       (20)     3304 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)     2293 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/README.md
--rw-r--r--   0 theocean154   (501) staff       (20)      106 2019-12-27 21:33:50.000000 tdameritrade-0.1.1/pyproject.toml
--rw-r--r--   0 theocean154   (501) staff       (20)      170 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/setup.cfg
--rw-r--r--   0 theocean154   (501) staff       (20)     1752 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/setup.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/
--rw-r--r--   0 theocean154   (501) staff       (20)       91 2019-12-27 21:53:49.000000 tdameritrade-0.1.1/tdameritrade/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      581 2020-06-17 03:19:09.000000 tdameritrade-0.1.1/tdameritrade/_version.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/auth/
--rw-r--r--   0 theocean154   (501) staff       (20)     3948 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/auth/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)       61 2018-12-31 23:42:18.000000 tdameritrade-0.1.1/tdameritrade/auth/__main__.py
--rw-r--r--   0 theocean154   (501) staff       (20)    25464 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/client.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2351 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/enums.py
--rw-r--r--   0 theocean154   (501) staff       (20)      975 2020-04-08 23:03:03.000000 tdameritrade-0.1.1/tdameritrade/exceptions.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2729 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/order.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/orders/
--rw-r--r--   0 theocean154   (501) staff       (20)      457 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)     5737 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/constants.py
--rw-r--r--   0 theocean154   (501) staff       (20)     1333 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/leg_builder.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/orders/models/
--rw-r--r--   0 theocean154   (501) staff       (20)      128 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      734 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/activities.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2155 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/base.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2162 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/instruments.py
--rw-r--r--   0 theocean154   (501) staff       (20)      458 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/json_encoder.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2943 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/leg.py
--rw-r--r--   0 theocean154   (501) staff       (20)     2088 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/models/orders.py
--rw-r--r--   0 theocean154   (501) staff       (20)     4947 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/orders/order_builder.py
--rw-r--r--   0 theocean154   (501) staff       (20)     1641 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/session.py
--rw-r--r--   0 theocean154   (501) staff       (20)        0 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/streaming.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/tests/
--rw-r--r--   0 theocean154   (501) staff       (20)      314 2020-03-20 13:52:17.000000 tdameritrade-0.1.1/tdameritrade/tests/JSONS.py
--rw-r--r--   0 theocean154   (501) staff       (20)       42 2018-07-12 15:56:19.000000 tdameritrade-0.1.1/tdameritrade/tests/test_all.py
--rw-r--r--   0 theocean154   (501) staff       (20)     5771 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/test_client.py
--rw-r--r--   0 theocean154   (501) staff       (20)      429 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/tests/test_exceptions.py
--rw-r--r--   0 theocean154   (501) staff       (20)     1805 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/tests/test_session.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/
--rw-r--r--   0 theocean154   (501) staff       (20)        0 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/__init__.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/models/
--rw-r--r--   0 theocean154   (501) staff       (20)        0 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/models/__init__.py
--rw-r--r--   0 theocean154   (501) staff       (20)      178 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/models/test_base.py
--rw-r--r--   0 theocean154   (501) staff       (20)      158 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/test_constants.py
--rw-r--r--   0 theocean154   (501) staff       (20)     3284 2020-06-17 03:18:55.000000 tdameritrade-0.1.1/tdameritrade/tests/unit/orders/test_order_builder.py
--rw-r--r--   0 theocean154   (501) staff       (20)     6701 2020-04-30 14:38:45.000000 tdameritrade-0.1.1/tdameritrade/urls.py
-drwxr-xr-x   0 theocean154   (501) staff       (20)        0 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/
--rw-r--r--   0 theocean154   (501) staff       (20)     3304 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/PKG-INFO
--rw-r--r--   0 theocean154   (501) staff       (20)     1430 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/SOURCES.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/dependency_links.txt
--rw-r--r--   0 theocean154   (501) staff       (20)       62 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/entry_points.txt
--rw-r--r--   0 theocean154   (501) staff       (20)        1 2020-03-20 13:53:06.000000 tdameritrade-0.1.1/tdameritrade.egg-info/not-zip-safe
--rw-r--r--   0 theocean154   (501) staff       (20)      285 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/requires.txt
--rw-r--r--   0 theocean154   (501) staff       (20)       13 2020-07-06 14:50:44.000000 tdameritrade-0.1.1/tdameritrade.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.858173 tdameritrade-0.2.0/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      292 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11357 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      344 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1305 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2699 2023-06-13 15:26:32.858237 tdameritrade-0.2.0/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2137 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)      106 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)      236 2023-06-13 15:26:32.858467 tdameritrade-0.2.0/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1550 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.854059 tdameritrade-0.2.0/tdameritrade/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       66 2023-06-13 15:26:29.000000 tdameritrade-0.2.0/tdameritrade/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.855093 tdameritrade-0.2.0/tdameritrade/auth/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4111 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/auth/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       62 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/auth/__main__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    26183 2023-06-13 15:15:32.000000 tdameritrade-0.2.0/tdameritrade/client.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2351 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/enums.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1347 2023-06-13 15:15:32.000000 tdameritrade-0.2.0/tdameritrade/exceptions.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2671 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/order.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.855674 tdameritrade-0.2.0/tdameritrade/orders/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      457 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5737 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/constants.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1363 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/leg_builder.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.856628 tdameritrade-0.2.0/tdameritrade/orders/models/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      128 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      698 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/activities.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2155 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/base.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2047 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/instruments.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      458 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/json_encoder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2936 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/leg.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2146 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/models/orders.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5031 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/orders/order_builder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1647 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/session.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/streaming.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857323 tdameritrade-0.2.0/tdameritrade/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      315 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/JSONS.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       42 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_all.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5783 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_client.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      430 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_exceptions.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1810 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/test_session.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857470 tdameritrade-0.2.0/tdameritrade/tests/unit/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.857773 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.858031 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      178 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/models/test_base.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      158 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_constants.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3284 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_order_builder.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6569 2023-06-13 15:00:28.000000 tdameritrade-0.2.0/tdameritrade/urls.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-06-13 15:26:32.854852 tdameritrade-0.2.0/tdameritrade.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2699 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1405 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       61 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)      335 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       13 2023-06-13 15:26:32.000000 tdameritrade-0.2.0/tdameritrade.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tdameritrade-0.1.1/LICENSE` & `tdameritrade-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.1.1/Makefile` & `tdameritrade-0.2.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 tests: ## Make unit tests
-	python3.7 -m pytest -v tdameritrade/tests --cov=tdameritrade  --junitxml=python_junit.xml --cov-report=xml --cov-branch
+	python -m pytest -v tdameritrade/tests --cov=tdameritrade  --junitxml=python_junit.xml --cov-report=xml --cov-branch
 
 testall: ## run the tests including those that hit the actual api
-	@ python3.7 -m pytest -v tdameritrade/tests --cov=tdameritrade  --junitxml=python_junit.xml --cov-report=xml --cov-branch
+	@ python -m pytest -v tdameritrade/tests --cov=tdameritrade  --junitxml=python_junit.xml --cov-report=xml --cov-branch
 
 lint: ## run linter
-	flake8 tdameritrade 
+	python -m flake8 tdameritrade setup.py
 
 fix:  ## run autopep8/tslint fix
-	autopep8 --in-place -r -a -a tdameritrade/
-
-annotate: ## MyPy type annotation check
-	mypy -s tdameritrade
-
-annotate_l: ## MyPy type annotation check - count only
-	mypy -s tdameritrade | wc -l 
+	python -m black tdameritrade/ setup.py
 
 clean: ## clean the repository
 	find . -name "__pycache__" | xargs  rm -rf 
 	find . -name "*.pyc" | xargs rm -rf 
 	rm -rf .coverage cover htmlcov logs build dist *.egg-info
 	make -C ./docs clean
 
 docs:  ## make documentation
 	make -C ./docs html
 	open ./docs/_build/html/index.html
 
-dist:  ## dist to pypi
+dist:  ## create dists
 	rm -rf dist build
-	python3 setup.py sdist
-	python3 setup.py bdist_wheel
-	twine check dist/* && twine upload dist/*
+	python setup.py sdist bdist_wheel
+	python -m twine check dist/*
+	
+publish: dist  ## dist to pypi
+	python -m twine upload dist/* --skip-existing
 
 install:  ## install to site-packages
-	pip3 install .
+	python -m pip install .
 
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
```

### Comparing `tdameritrade-0.1.1/PKG-INFO` & `tdameritrade-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 Metadata-Version: 2.1
 Name: tdameritrade
-Version: 0.1.1
+Version: 0.2.0
 Summary: APIs for TD Ameritrade
 Home-page: https://github.com/timkpaine/tdameritrade
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
-Description: # tdameritrade
-        Python interface to TD Ameritrade Api
-        
-        [![Build Status](https://dev.azure.com/tpaine154/tdameritrade/_apis/build/status/timkpaine.tdameritrade?branchName=master)](https://dev.azure.com/tpaine154/tdameritrade/_build/latest?definitionId=8&branchName=master)
-        [![Coverage](https://img.shields.io/azure-devops/coverage/tpaine154/tdameritrade/8)]()
-        [![License](https://img.shields.io/github/license/timkpaine/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
-        [![PyPI](https://img.shields.io/pypi/v/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
-        [![Docs](https://img.shields.io/readthedocs/tdameritrade.svg)](https://tdameritrade.readthedocs.io)
-        
-        
-        
-        ## Getting Started
-        
-        ### Install
-        Install from pip
-        
-        `pip install tdameritrade`
-        
-        or from source
-        
-        `python setup.py install`
-        
-        
-        ### Docs
-        Major changes in the v0.1.0 update to the way tokens are handled.  
-        You will still need the original authentication instructions, but the TDClient now takes the refresh token and client
-        id, not the access token. A new session class handles token expiration and will automatically call a new token as
-        needed. 
-        
-        It is recommended that you store these as environmental variables.  
-        
-        ```
-        client_id = os.getenv('TDAMERITRADE_CLIENT_ID')
-        account_id = os.getenv('TDAMERITRADE_ACCOUNT_ID')
-        refresh_token = os.getenv('TDAMERITRADE_REFRESH_TOKEN')
-        
-        tdclient = tdameritrade.TDClient(client_id=client_id, refresh_token=refresh_token, account_ids=[account_id])
-        ``` 
-        
-        See the tests\test_client.py file for examples on current usage. 
-        
-        [Read the docs!](http://tdameritrade.readthedocs.io/en/latest/index.html)
-        
-        All functionality is available as methods on the `TDClient` object. For most methods, there is a convenience method to return the result as a pandas DataFrame.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/client.png)
-        
-        Most data fetching methods accept the symbol as argument. For equities, this is just the ticker.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/quote.png)
-        
-        For different assets, utilize the `search` and `instrument` methods to lookup symbols. For options, you can utilize the options method.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/options.png)
-        
-        
 Keywords: finance data
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# tdameritrade
+Python interface to TD Ameritrade Api
+
+[![Build Status](https://github.com/timkpaine/tdameritrade/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/tdameritrade/actions?query=workflow%3A%22Build+Status%22)
+[![Coverage](https://codecov.io/gh/timkpaine/tdameritrade/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/tdameritrade)
+[![License](https://img.shields.io/github/license/timkpaine/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
+[![PyPI](https://img.shields.io/pypi/v/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
+
+
+
+## Getting Started
+
+### Install
+Install from pip
+
+`pip install tdameritrade`
+
+or from source
+
+`python setup.py install`
+
+
+### Docs
+Major changes in the v0.1.0 update to the way tokens are handled.  
+You will still need the original authentication instructions, but the TDClient now takes the refresh token and client
+id, not the access token. A new session class handles token expiration and will automatically call a new token as
+needed. 
+
+It is recommended that you store these as environmental variables.  
+
+```
+client_id = os.getenv('TDAMERITRADE_CLIENT_ID')
+account_id = os.getenv('TDAMERITRADE_ACCOUNT_ID')
+refresh_token = os.getenv('TDAMERITRADE_REFRESH_TOKEN')
+
+tdclient = tdameritrade.TDClient(client_id=client_id, refresh_token=refresh_token, account_ids=[account_id])
+``` 
+
+See the tests\test_client.py file for examples on current usage. 
+
+All functionality is available as methods on the `TDClient` object. For most methods, there is a convenience method to return the result as a pandas DataFrame.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/client.png)
+
+Most data fetching methods accept the symbol as argument. For equities, this is just the ticker.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/quote.png)
+
+For different assets, utilize the `search` and `instrument` methods to lookup symbols. For options, you can utilize the options method.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/options.png)
+
```

### Comparing `tdameritrade-0.1.1/README.md` & `tdameritrade-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # tdameritrade
 Python interface to TD Ameritrade Api
 
-[![Build Status](https://dev.azure.com/tpaine154/tdameritrade/_apis/build/status/timkpaine.tdameritrade?branchName=master)](https://dev.azure.com/tpaine154/tdameritrade/_build/latest?definitionId=8&branchName=master)
-[![Coverage](https://img.shields.io/azure-devops/coverage/tpaine154/tdameritrade/8)]()
+[![Build Status](https://github.com/timkpaine/tdameritrade/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/tdameritrade/actions?query=workflow%3A%22Build+Status%22)
+[![Coverage](https://codecov.io/gh/timkpaine/tdameritrade/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/tdameritrade)
 [![License](https://img.shields.io/github/license/timkpaine/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
 [![PyPI](https://img.shields.io/pypi/v/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
-[![Docs](https://img.shields.io/readthedocs/tdameritrade.svg)](https://tdameritrade.readthedocs.io)
 
 
 
 ## Getting Started
 
 ### Install
 Install from pip
@@ -35,21 +34,19 @@
 refresh_token = os.getenv('TDAMERITRADE_REFRESH_TOKEN')
 
 tdclient = tdameritrade.TDClient(client_id=client_id, refresh_token=refresh_token, account_ids=[account_id])
 ``` 
 
 See the tests\test_client.py file for examples on current usage. 
 
-[Read the docs!](http://tdameritrade.readthedocs.io/en/latest/index.html)
-
 All functionality is available as methods on the `TDClient` object. For most methods, there is a convenience method to return the result as a pandas DataFrame.
 
-![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/client.png)
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/client.png)
 
 Most data fetching methods accept the symbol as argument. For equities, this is just the ticker.
 
-![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/quote.png)
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/quote.png)
 
 For different assets, utilize the `search` and `instrument` methods to lookup symbols. For options, you can utilize the options method.
 
-![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/options.png)
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/options.png)
```

### Comparing `tdameritrade-0.1.1/tdameritrade/auth/__init__.py` & `tdameritrade-0.2.0/tdameritrade/auth/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,91 +6,120 @@
 from shutil import which
 
 import requests
 
 
 def authentication(client_id, redirect_uri, tdauser=None, tdapass=None):
     from selenium import webdriver
-    client_id = client_id + '@AMER.OAUTHAP'
-    url = 'https://auth.tdameritrade.com/auth?response_type=code&redirect_uri=' + up.quote(redirect_uri) + '&client_id=' + up.quote(client_id)
+    from selenium.webdriver.common.by import By
+
+    client_id = client_id + "@AMER.OAUTHAP"
+    url = (
+        "https://auth.tdameritrade.com/auth?response_type=code&redirect_uri="
+        + up.quote(redirect_uri)
+        + "&client_id="
+        + up.quote(client_id)
+    )
 
     options = webdriver.ChromeOptions()
 
-    if sys.platform == 'darwin':
+    if sys.platform == "darwin":
         # MacOS
-        if os.path.exists("/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"):
-            options.binary_location = "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
+        if os.path.exists(
+            "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
+        ):
+            options.binary_location = (
+                "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
+            )
         elif os.path.exists("/Applications/Chrome.app/Contents/MacOS/Google Chrome"):
-            options.binary_location = "/Applications/Chrome.app/Contents/MacOS/Google Chrome"
-    elif 'linux' in sys.platform:
+            options.binary_location = (
+                "/Applications/Chrome.app/Contents/MacOS/Google Chrome"
+            )
+    elif "linux" in sys.platform:
         # Linux
-        options.binary_location = which('google-chrome') or which('chrome') or which('chromium')
+        options.binary_location = (
+            which("google-chrome") or which("chrome") or which("chromium")
+        )
 
     else:
         # Windows
-        if os.path.exists('C:/Program Files (x86)/Google/Chrome/Application/chrome.exe'):
-            options.binary_location = 'C:/Program Files (x86)/Google/Chrome/Application/chrome.exe'
-        elif os.path.exists('C:/Program Files/Google/Chrome/Application/chrome.exe'):
-            options.binary_location = 'C:/Program Files/Google/Chrome/Application/chrome.exe'
+        if os.path.exists(
+            "C:/Program Files (x86)/Google/Chrome/Application/chrome.exe"
+        ):
+            options.binary_location = (
+                "C:/Program Files (x86)/Google/Chrome/Application/chrome.exe"
+            )
+        elif os.path.exists("C:/Program Files/Google/Chrome/Application/chrome.exe"):
+            options.binary_location = (
+                "C:/Program Files/Google/Chrome/Application/chrome.exe"
+            )
 
-    chrome_driver_binary = which('chromedriver') or "/usr/local/bin/chromedriver"
+    chrome_driver_binary = which("chromedriver") or "/usr/local/bin/chromedriver"
     driver = webdriver.Chrome(chrome_driver_binary, chrome_options=options)
 
     driver.get(url)
 
     # Set tdauser and tdapass from environemnt if TDAUSER and TDAPASS environment variables were defined
-    tdauser = tdauser or os.environ.get('TDAUSER', '')
-    tdapass = tdapass or os.environ.get('TDAPASS', '')
+    tdauser = tdauser or os.environ.get("TDAUSER", "")
+    tdapass = tdapass or os.environ.get("TDAPASS", "")
 
-    # Fully automated oauth2 authentication (if tdauser and tdapass were intputed into the function, or found as
+    # Fully automated oauth2 authentication (if tdauser and tdapass were inputed into the function, or found as
     # environment variables)
     if tdauser and tdapass:
-        ubox = driver.find_element_by_id('username')
-        pbox = driver.find_element_by_id('password')
+        ubox = driver.find_element(By.ID, "username")
+        pbox = driver.find_element(By.ID, "password")
         ubox.send_keys(tdauser)
         pbox.send_keys(tdapass)
-        driver.find_element_by_id('accept').click()
+        driver.find_element(By.ID, "accept").click()
 
-        driver.find_element_by_id('accept').click()
+        driver.find_element(By.ID, "accept").click()
         while True:
             try:
-                code = up.unquote(driver.current_url.split('code=')[1])
-                if code != '':
+                code = up.unquote(driver.current_url.split("code=")[1])
+                if code != "":
                     break
                 else:
                     time.sleep(2)
             except (TypeError, IndexError):
                 pass
     else:
-        input('after giving access, hit enter to continue')
-        code = up.unquote(driver.current_url.split('code=')[1])
+        input("after giving access, hit enter to continue")
+        code = up.unquote(driver.current_url.split("code=")[1])
 
     driver.close()
 
-    resp = requests.post('https://api.tdameritrade.com/v1/oauth2/token',
-                         headers={'Content-Type': 'application/x-www-form-urlencoded'},
-                         data={'grant_type': 'authorization_code',
-                               'refresh_token': '',
-                               'access_type': 'offline',
-                               'code': code,
-                               'client_id': client_id,
-                               'redirect_uri': redirect_uri})
+    resp = requests.post(
+        "https://api.tdameritrade.com/v1/oauth2/token",
+        headers={"Content-Type": "application/x-www-form-urlencoded"},
+        data={
+            "grant_type": "authorization_code",
+            "refresh_token": "",
+            "access_type": "offline",
+            "code": code,
+            "client_id": client_id,
+            "redirect_uri": redirect_uri,
+        },
+    )
     if resp.status_code != 200:
-        raise Exception('Could not authenticate!')
+        raise Exception("Could not authenticate!")
     return resp.json()
 
 
 def access_token(refresh_token, client_id):
-    resp = requests.post('https://api.tdameritrade.com/v1/oauth2/token',
-                         headers={'Content-Type': 'application/x-www-form-urlencoded'},
-                         data={'grant_type': 'refresh_token',
-                               'refresh_token': refresh_token,
-                               'client_id': client_id})
+    resp = requests.post(
+        "https://api.tdameritrade.com/v1/oauth2/token",
+        headers={"Content-Type": "application/x-www-form-urlencoded"},
+        data={
+            "grant_type": "refresh_token",
+            "refresh_token": refresh_token,
+            "client_id": client_id,
+        },
+    )
     if resp.status_code != 200:
-        raise Exception('Could not authenticate!')
+        raise Exception("Could not authenticate!")
     return resp.json()
 
 
 def main():
-    client_id = input('client id:')
-    redirect_uri = input('redirect uri:')
+    client_id = input("client id:")
+    redirect_uri = input("redirect uri:")
     print(authentication(client_id, redirect_uri))
```

### Comparing `tdameritrade-0.1.1/tdameritrade/client.py` & `tdameritrade-0.2.0/tdameritrade/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,232 +62,271 @@
     CREATE_WATCHLIST,
     DELETE_WATCHLIST,
     GET_WATCHLIST,
     # GET_WATCHLISTS_MULTIPLE_ACCOUNTS,
     GET_WATCHLISTS,
     GET_WATCHLISTS_MULTIPLE_ACCOUNTS,
     REPLACE_WATCHLIST,
-    UPDATE_WATCHLIST)
+    UPDATE_WATCHLIST,
+)
 
 
 def response_is_valid(resp):
-    return resp.status_code in (200, 201)
+    return resp.status_code in (200, 201, 204)
 
 
 class TDClient(object):
     def __init__(self, client_id=None, refresh_token=None, account_ids=None):
-        self._clientId = client_id or os.environ['TDAMERITRADE_CLIENT_ID']
-        self._refreshToken = refresh_token or os.environ['TDAMERITRADE_REFRESH_TOKEN']
+        self._clientId = client_id or os.environ["TDAMERITRADE_CLIENT_ID"]
+        self._refreshToken = refresh_token or os.environ["TDAMERITRADE_REFRESH_TOKEN"]
         self.accountIds = account_ids or []
         self.session = TDASession(self._refreshToken, self._clientId)
 
     def _request(self, url, method="GET", params=None, *args, **kwargs):
         resp = self.session.request(method, url, params=params, *args, **kwargs)
         if not response_is_valid(resp):
             handle_error_response(resp)
         return resp
 
     def accounts(self, positions=False, orders=False):
-        '''get user accounts. caches account ids in accountIds if not provided during initialization
+        """get user accounts. caches account ids in accountIds if not provided during initialization
 
         Args:
             positions (bool): include position information
             orders (bool): include order information
-        '''
+        """
         ret = {}
 
         if positions or orders:
-            params = {'fields': []}
+            params = {"fields": []}
 
             if positions:
-                params['fields'].append('positions')
+                params["fields"].append("positions")
             if orders:
-                params['fields'].append('orders')
-            params['fields'] = ','.join(params['fields'])
+                params["fields"].append("orders")
+            params["fields"] = ",".join(params["fields"])
         else:
             params = {}
 
         if self.accountIds:
             for acc in self.accountIds:
                 resp = self._request(GET_ACCOUNT.format(accountId=acc), params=params)
                 ret[acc] = resp.json()
         else:
             resp = self._request(GET_ACCOUNTS, params=params)
             for account in resp.json():
-                ret[account['securitiesAccount']['accountId']] = account
+                ret[account["securitiesAccount"]["accountId"]] = account
             self.accountIds = [int(accountId) for accountId in ret]
         return ret
 
     def accountsDF(self):
-        '''get accounts as dataframe'''
+        """get accounts as dataframe"""
         data = self.accounts()
         account_dataframes = []
         for accountId, value in data.items():
-            account_dataframes.append(pd.io.json.json_normalize(value))
-            account_dataframes[-1].columns = [c.replace('securitiesAccount.', '') for c in account_dataframes[-1].columns]
+            account_dataframes.append(pd.json_normalize(value))
+            account_dataframes[-1].columns = [
+                c.replace("securitiesAccount.", "")
+                for c in account_dataframes[-1].columns
+            ]
         return pd.concat(account_dataframes)
 
-    def transactions(self, accountId=None, type=None, symbol=None, startDate=None, endDate=None):
-        '''get transactions by account
+    def transactions(
+        self, accountId=None, type=None, symbol=None, startDate=None, endDate=None
+    ):
+        """get transactions by account
 
         Args:
             accountId (int): account id (defaults to client's ids)
             type (str): transaction type, in ('ALL', 'TRADE', 'BUY_ONLY', 'SELL_ONLY', 'CASH_IN_OR_CASH_OUT', 'CHECKING', 'DIVIDEND', 'INTEREST', 'OTHER', 'ADVISOR_FEES')
             symbol (str): transactions for given symbol
             start_date (str): start date as string yyyy-MM-dd
             end_date (str): end date as string yyyy-MM-dd
-        '''
+        """
         if accountId:
             accounts = [accountId]
         else:
             accounts = self.accountIds
 
         if type not in GET_TRANSCATION_TYPE_VALUES:
-            raise TDAAPIError('Transaction type must be in {}'.format(GET_TRANSCATION_TYPE_VALUES))
+            raise TDAAPIError(
+                "Transaction type must be in {}".format(GET_TRANSCATION_TYPE_VALUES)
+            )
 
         ret = {}
         for account in accounts:
             transactions = GET_ACCOUNT.format(accountId=account) + "/transactions"
-            ret[account] = self._request(transactions,
-                                         params={
-                                             'type': type,
-                                             'symbol': symbol,
-                                             'startDate': startDate,
-                                             'endDate': endDate
-                                         }).json()
+            ret[account] = self._request(
+                transactions,
+                params={
+                    "type": type,
+                    "symbol": symbol,
+                    "startDate": startDate,
+                    "endDate": endDate,
+                },
+            ).json()
         return ret
 
-    def transactionsDF(self, accountId=None, type=None, symbol=None, startDate=None, endDate=None):
-        '''get transaction information as Dataframe'''
-        return pd.json_normalize(self.transactions(accountId=accountId, type=type, symbol=symbol, startDate=startDate, endDate=endDate))
+    def transactionsDF(
+        self, accountId=None, type=None, symbol=None, startDate=None, endDate=None
+    ):
+        """get transaction information as Dataframe"""
+        return pd.json_normalize(
+            self.transactions(
+                accountId=accountId,
+                type=type,
+                symbol=symbol,
+                startDate=startDate,
+                endDate=endDate,
+            )
+        )
 
-    def search(self, symbol, projection='symbol-search'):
-        '''Search for a symbol
+    def search(self, symbol, projection="symbol-search"):
+        """Search for a symbol
 
         Args:
             symbol (sring): string to search for
             projection (string): projection to use, in ('symbol-search', 'symbol-regex', 'desc-search', 'desc-regex', 'fundamental')
-        '''
+        """
         if projection not in SEARCH_INSTRUMENT_PROJECTION:
-            raise TDAAPIError('Projection must be in {}'.format(SEARCH_INSTRUMENT_PROJECTION))
+            raise TDAAPIError(
+                "Projection must be in {}".format(SEARCH_INSTRUMENT_PROJECTION)
+            )
+
+        return self._request(
+            SEARCH_INSTRUMENTS, params={"symbol": symbol, "projection": projection}
+        ).json()
 
-        return self._request(SEARCH_INSTRUMENTS,
-                             params={'symbol': symbol,
-                                     'projection': projection}).json()
-
-    def searchDF(self, symbol, projection='symbol-search'):
-        '''search for symbol as a dataframe'''
+    def searchDF(self, symbol, projection="symbol-search"):
+        """search for symbol as a dataframe"""
         ret = []
         dat = self.search(symbol, projection)
         for symbol in dat:
             ret.append(dat[symbol])
 
         return pd.DataFrame(ret)
 
     def fundamentalSearch(self, symbol):
-        '''helper to search for a symbol using fundamental projection'''
-        return self.search(symbol, 'fundamental')
+        """helper to search for a symbol using fundamental projection"""
+        return self.search(symbol, "fundamental")
 
     def fundamentalSearchDF(self, symbol):
-        '''helper to search for a symbol using fundamental projection and return DF'''
-        return self.searchDF(symbol, 'fundamental')
+        """helper to search for a symbol using fundamental projection and return DF"""
+        return self.searchDF(symbol, "fundamental")
 
     def instrument(self, cusip):
-        '''get instrument info from cusip
+        """get instrument info from cusip
 
         Args:
             cusip (str): the cusip to use, can find it by looking up in search
-        '''
+        """
         return self._request(GET_INSTRUMENT.format(cusip=cusip)).json()
 
     def instrumentDF(self, cusip):
-        '''get instrument info from cusip as dataframe'''
+        """get instrument info from cusip as dataframe"""
         return pd.DataFrame(self.instrument(cusip))
 
     def quote(self, symbol):
-        '''get quote for symbol
+        """get quote for symbol
 
         Args:
             symbol (str): symbol to get quote for
-        '''
+        """
         if not isinstance(symbol, list):
             symbol = [symbol]
 
-        return self._request(GET_QUOTES,
-                             params={'symbol': [s.upper() for s in symbol]}).json()
+        return self._request(
+            GET_QUOTES, params={"symbol": [s.upper() for s in symbol]}
+        ).json()
 
     def quoteDF(self, symbol):
-        '''get quote, format as dataframe'''
+        """get quote, format as dataframe"""
         x = self.quote(symbol)
 
         return pd.DataFrame(x).T.reset_index(drop=True)
 
-    def history(self, symbol,
-                periodType=None, period=None,
-                frequencyType=None, frequency=None,
-                endDate=None, startDate=None,
-                needExtendedHoursData=True):
-        '''get price history
+    def history(
+        self,
+        symbol,
+        periodType=None,
+        period=None,
+        frequencyType=None,
+        frequency=None,
+        endDate=None,
+        startDate=None,
+        needExtendedHoursData=True,
+    ):
+        """get price history
 
         Args:
             symbol (str): symbol to get price history for
             periodType (str): period type to request
             period (int): period to use
             frequencyType (str): frequency type to use
             frequency (int): frequency to use
             endDate (int): End date as milliseconds since epoch. If startDate and endDate are provided, period should not be provided. Default is previous trading day.
             startDate (int): Start date as milliseconds since epoch. If startDate and endDate are provided, period should not be provided.
             needExtendedHoursData (bool): true to return extended hours data, false for regular market hours only. Default is true
-        '''
+        """
         params = {}
         if periodType or period:
             if periodType not in PERIOD_TYPE_VALUES:
-                raise TDAAPIError('Period type must be in {}'.format(PERIOD_TYPE_VALUES))
-            params['period'] = period
-            params['periodType'] = periodType
+                raise TDAAPIError(
+                    "Period type must be in {}".format(PERIOD_TYPE_VALUES)
+                )
+            params["period"] = period
+            params["periodType"] = periodType
         if frequencyType or frequency:
             if frequencyType not in FREQUENCY_TYPE_VALUES:
-                raise TDAAPIError('Frequency type must be in {}'.format(FREQUENCY_TYPE_VALUES))
-            params['frequency'] = frequency
-            params['frequencyType'] = frequencyType
+                raise TDAAPIError(
+                    "Frequency type must be in {}".format(FREQUENCY_TYPE_VALUES)
+                )
+            params["frequency"] = frequency
+            params["frequencyType"] = frequencyType
 
         if startDate:
-            params['startDate'] = startDate
+            params["startDate"] = startDate
 
         if endDate:
-            params['endDate'] = endDate
+            params["endDate"] = endDate
+
+        params["needExtendedHoursData"] = needExtendedHoursData
 
-        return self._request(GET_PRICE_HISTORY.format(symbol=symbol), params=params).json()
+        return self._request(
+            GET_PRICE_HISTORY.format(symbol=symbol), params=params
+        ).json()
 
     def historyDF(self, symbol, **kwargs):
-        '''get history as dataframe'''
+        """get history as dataframe"""
         x = self.history(symbol, **kwargs)
-        df = pd.DataFrame(x['candles'])
-        df['datetime'] = pd.to_datetime(df['datetime'], unit='ms')
+        df = pd.DataFrame(x["candles"])
+        df["datetime"] = pd.to_datetime(df["datetime"], unit="ms")
 
         return df
 
-    def options(self,
-                symbol,
-                contractType='ALL',
-                strikeCount=-1,
-                includeQuotes=False,
-                strategy='SINGLE',
-                interval=None,
-                strike=None,
-                range='ALL',
-                fromDate=None,
-                toDate=None,
-                volatility=None,
-                underlyingPrice=None,
-                interestRate=None,
-                daysToExpiration=None,
-                expMonth='ALL',
-                optionType='ALL'):
-        '''request option chain information
+    def options(
+        self,
+        symbol,
+        contractType="ALL",
+        strikeCount=-1,
+        includeQuotes=False,
+        strategy="SINGLE",
+        interval=None,
+        strike=None,
+        range="ALL",
+        fromDate=None,
+        toDate=None,
+        volatility=None,
+        underlyingPrice=None,
+        interestRate=None,
+        daysToExpiration=None,
+        expMonth="ALL",
+        optionType="ALL",
+    ):
+        """request option chain information
 
         Args:
             symbol (str): Enter one symbol
             contractType (str): Type of contracts to return in the chain. Can be CALL, PUT, or ALL. Default is ALL.
             strikeCount (int): The number of strikes to return above and below the at-the-money price.
             includeQuotes (bool): Include quotes for options in the option chain. Can be TRUE or FALSE. Default is FALSE.
             strategy (str): Passing a value returns a Strategy Chain. Possible values are SINGLE, ANALYTICAL (allows use of the volatility, underlyingPrice, interestRate, and daysToExpiration params to calculate theoretical values), COVERED, VERTICAL, CALENDAR, STRANGLE, STRADDLE, BUTTERFLY, CONDOR, DIAGONAL, COLLAR, or ROLL. Default is SINGLE.
@@ -312,328 +351,398 @@
                                 Example: JAN
                                 Default is ALL.
             optionType (str): Type of contracts to return. Possible values are:
                                 S: Standard contracts
                                 NS: Non-standard contracts
                                 ALL: All contracts
                                 Default is ALL.
-        '''
-        params = {'symbol': symbol}
+        """
+        params = {"symbol": symbol}
 
         if contractType not in CONTRACT_TYPE_VALUES:
-            raise TDAAPIError('Contract type must be in {}'.format(CONTRACT_TYPE_VALUES))
-        params['contractType'] = contractType
+            raise TDAAPIError(
+                "Contract type must be in {}".format(CONTRACT_TYPE_VALUES)
+            )
+        params["contractType"] = contractType
 
         if strikeCount:
-            params['strikeCount'] = strikeCount
+            params["strikeCount"] = strikeCount
 
-        params['includeQuotes'] = includeQuotes
+        params["includeQuotes"] = includeQuotes
 
         if strategy not in STRATEGY_VALUES:
-            raise TDAAPIError('Strategy must be in {}'.format(STRATEGY_VALUES))
+            raise TDAAPIError("Strategy must be in {}".format(STRATEGY_VALUES))
 
-        params['strategy'] = strategy
+        params["strategy"] = strategy
 
         if interval:
-            params['interval'] = interval
+            params["interval"] = interval
 
         if strike:
-            params['strike'] = strike
+            params["strike"] = strike
 
         if range not in RANGE_VALUES:
-            raise TDAAPIError('Range must be in {}'.format(RANGE_VALUES))
-            params['range'] = range
+            raise TDAAPIError("Range must be in {}".format(RANGE_VALUES))
+
+        params["range"] = range
 
         if fromDate:
-            params['fromDate'] = fromDate
+            params["fromDate"] = fromDate
 
         if toDate:
-            params['toDate'] = toDate
+            params["toDate"] = toDate
 
-        if strategy == 'ANALYTICAL':
+        if strategy == "ANALYTICAL":
             if volatility:
-                params['volatility'] = volatility
+                params["volatility"] = volatility
             if underlyingPrice:
-                params['underlyingPrice'] = underlyingPrice
+                params["underlyingPrice"] = underlyingPrice
             if interestRate:
-                params['interestRate'] = interestRate
+                params["interestRate"] = interestRate
             if daysToExpiration:
-                params['daysToExpiration'] = daysToExpiration
+                params["daysToExpiration"] = daysToExpiration
 
         if expMonth not in OPTION_EXPMONTH_VALUES:
-            raise TDAAPIError('Expiration month must be in {}'.format(OPTION_EXPMONTH_VALUES))
-        params['expMonth'] = expMonth
+            raise TDAAPIError(
+                "Expiration month must be in {}".format(OPTION_EXPMONTH_VALUES)
+            )
+        params["expMonth"] = expMonth
 
         if optionType not in OPTION_TYPE_VALUES:
-            raise TDAAPIError('Option type must be in {}'.format(OPTION_TYPE_VALUES))
+            raise TDAAPIError("Option type must be in {}".format(OPTION_TYPE_VALUES))
 
         return self._request(GET_OPTION_CHAIN, params=params).json()
 
-    def optionsDF(self,
-                  symbol,
-                  contractType='ALL',
-                  strikeCount=-1,
-                  includeQuotes=False,
-                  strategy='SINGLE',
-                  interval=None,
-                  strike=None,
-                  range='ALL',
-                  fromDate=None,
-                  toDate=None,
-                  volatility=None,
-                  underlyingPrice=None,
-                  interestRate=None,
-                  daysToExpiration=None,
-                  expMonth='ALL',
-                  optionType='ALL'):
-        '''return options chain as dataframe'''
+    def optionsDF(
+        self,
+        symbol,
+        contractType="ALL",
+        strikeCount=-1,
+        includeQuotes=False,
+        strategy="SINGLE",
+        interval=None,
+        strike=None,
+        range="ALL",
+        fromDate=None,
+        toDate=None,
+        volatility=None,
+        underlyingPrice=None,
+        interestRate=None,
+        daysToExpiration=None,
+        expMonth="ALL",
+        optionType="ALL",
+    ):
+        """return options chain as dataframe"""
         ret = []
-        dat = self.options(symbol=symbol,
-                           contractType=contractType,
-                           strikeCount=strikeCount,
-                           includeQuotes=includeQuotes,
-                           strategy=strategy,
-                           interval=interval,
-                           strike=strike,
-                           range=range,
-                           fromDate=fromDate,
-                           toDate=toDate,
-                           volatility=volatility,
-                           underlyingPrice=underlyingPrice,
-                           interestRate=interestRate,
-                           daysToExpiration=daysToExpiration,
-                           expMonth=expMonth,
-                           optionType=optionType)
-        for date in dat['callExpDateMap']:
-            for strike in dat['callExpDateMap'][date]:
-                ret.extend(dat['callExpDateMap'][date][strike])
-        for date in dat['putExpDateMap']:
-            for strike in dat['putExpDateMap'][date]:
-                ret.extend(dat['putExpDateMap'][date][strike])
-
-        df = pd.DataFrame(ret)
-        for col in ('tradeTimeInLong', 'quoteTimeInLong',
-                    'expirationDate', 'lastTradingDay'):
-            df[col] = pd.to_datetime(df[col], unit='ms')
-
-        return df
+        dat = self.options(
+            symbol=symbol,
+            contractType=contractType,
+            strikeCount=strikeCount,
+            includeQuotes=includeQuotes,
+            strategy=strategy,
+            interval=interval,
+            strike=strike,
+            range=range,
+            fromDate=fromDate,
+            toDate=toDate,
+            volatility=volatility,
+            underlyingPrice=underlyingPrice,
+            interestRate=interestRate,
+            daysToExpiration=daysToExpiration,
+            expMonth=expMonth,
+            optionType=optionType,
+        )
+
+        if dat["status"] == "SUCCESS":
+            for date in dat["callExpDateMap"]:
+                for strike in dat["callExpDateMap"][date]:
+                    ret.extend(dat["callExpDateMap"][date][strike])
+            for date in dat["putExpDateMap"]:
+                for strike in dat["putExpDateMap"][date]:
+                    ret.extend(dat["putExpDateMap"][date][strike])
+
+            df = pd.DataFrame(ret)
+            for col in (
+                "tradeTimeInLong",
+                "quoteTimeInLong",
+                "expirationDate",
+                "lastTradingDay",
+            ):
+                df[col] = pd.to_datetime(df[col], unit="ms")
+
+            for col in (
+                "interestRate",
+                "underlyingPrice",
+            ):
+                if col in dat:
+                    df[col] = dat[col]
+            return df
+        raise (Exception(dat))
 
-    def movers(self, index, direction='up', change='percent'):
-        '''request market movers
+    def movers(self, index, direction="up", change="percent"):
+        """request market movers
 
         Args:
             index (str): index to look for movers in
             direction (str): up or down
             change (str): percent or value
-        '''
+        """
         params = {}
         if direction not in DIRECTION_VALUES:
-            raise TDAAPIError('Direction must be in {}'.format(DIRECTION_VALUES))
-        params['direction'] = direction
+            raise TDAAPIError("Direction must be in {}".format(DIRECTION_VALUES))
+        params["direction"] = direction
 
         if change not in CHANGE_VALUES:
-            raise TDAAPIError('Change mus be in {}'.format(CHANGE_VALUES))
-        params['change'] = change
+            raise TDAAPIError("Change mus be in {}".format(CHANGE_VALUES))
+        params["change"] = change
 
         return self._request(MOVERS.format(index=index), params=params).json()
 
-    def orders(self,
-               accountId=None,
-               orderId=None,
-               maxResults=-1,
-               fromEnteredTime=None,
-               toEnteredTime=None,
-               status=None):
-        '''get order
+    def orders(
+        self,
+        accountId=None,
+        orderId=None,
+        maxResults=-1,
+        fromEnteredTime=None,
+        toEnteredTime=None,
+        status=None,
+    ):
+        """get order
 
         Args:
             accountId (int): account id
             orderId (int): orderId
             maxResults (int): max number of results to return
             fromEnteredTime (str): yyyy-MM-dd to filter by
             toEnteredTime (str): yyyy-MM-dd to filter by
             status (str): only return orders with this status
-        '''
+        """
         params = {}
         if status and status not in STATUS_VALUES:
-            raise TDAAPIError('Status must be in {}'.format(STATUS_VALUES))
+            raise TDAAPIError("Status must be in {}".format(STATUS_VALUES))
         elif status:
-            params['status'] = status
+            params["status"] = status
 
         if accountId:
-            params['accountId'] = accountId
+            params["accountId"] = accountId
         if orderId:
-            params['orderId'] = orderId
+            params["orderId"] = orderId
         if maxResults:
-            params['maxResults'] = maxResults
+            params["maxResults"] = maxResults
         if fromEnteredTime:
-            params['fromEnteredTime'] = fromEnteredTime
+            params["fromEnteredTime"] = fromEnteredTime
         if toEnteredTime:
-            params['toEnteredTime'] = toEnteredTime
-        return self._request(GET_ORDER_BY_QUERY, params=params).json()
+            params["toEnteredTime"] = toEnteredTime
+        return self._request(GET_ORDER_BY_QUERY, json=params).json()
 
     def cancelOrder(self, accountId, orderId):
-        '''cancel the given order
+        """cancel the given order
 
         Args:
             accountId (int): account id the order is under
             orderId (int): order id of order to cancel
-        '''
-        return self._request(CANCEL_ORDER.format(accountId=accountId, orderId=orderId), method='DELETE').json()
+        """
+        return self._request(
+            CANCEL_ORDER.format(accountId=accountId, orderId=orderId), method="DELETE"
+        )
 
     def placeOrder(self, accountId, order):
-        '''place an order
+        """place an order
 
         Args:
             accountId (int): id of account to place order under
             order (JSON): order instance to place
-        '''
-        return self._request(PLACE_ORDER.format(accountId=accountId), method='POST', data=order).json()
+        """
+        return self._request(
+            PLACE_ORDER.format(accountId=accountId), method="POST", data=order
+        )
 
     def replaceOrder(self, accountId, orderId, order):
-        '''place an order
+        """place an order
 
         Args:
             accountId (int): id of account to place order under
             orderId (int): id of order to replace
             order (JSON): order instance to place
-        '''
-        return self._request(REPLACE_ORDER.format(accountId=accountId, orderId=orderId), method='PUT', data=order).json()
+        """
+        return self._request(
+            REPLACE_ORDER.format(accountId=accountId, orderId=orderId),
+            method="PUT",
+            data=order,
+        ).json()
 
     def savedOrders(self, accountId=None, savedOrderId=None):
-        '''get saved orders
+        """get saved orders
 
         Args:
             accountId (int): id of account to get saved orders from
             savedOrderId (int): id of saved order
-        '''
+        """
         if not accountId and savedOrderId:
-            raise TDAAPIError('Must provide account id if attempting to lookup by savedOrderId')
+            raise TDAAPIError(
+                "Must provide account id if attempting to lookup by savedOrderId"
+            )
 
         if not accountId:
             ret = {}
             for account in self.accountIds:
-                ret[account] = self._request(GET_SAVED_ORDER_BY_PATH.format(accountId=account)).json()
+                ret[account] = self._request(
+                    GET_SAVED_ORDER_BY_PATH.format(accountId=account)
+                ).json()
             return ret
 
         if savedOrderId:
-            return self._request(GET_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId)).json()
+            return self._request(
+                GET_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId)
+            ).json()
         return self._request(GET_SAVED_ORDER_BY_PATH.format(accountId=accountId)).json()
 
     def createSavedOrder(self, accountId, order):
-        '''create a saved order
+        """create a saved order
 
         Args:
             accountId (int): id of account to place order under
             order (JSON): order instance to place
-        '''
-        return self._request(CREATE_SAVED_ORDER.format(accountId=accountId), method='POST', data=order).json()
+        """
+        return self._request(
+            CREATE_SAVED_ORDER.format(accountId=accountId), method="POST", data=order
+        ).json()
 
     def deleteSavedOrder(self, accountId, savedOrderId):
-        '''delete a saved order
+        """delete a saved order
 
         Args:
             accountId (int): id of account to place order under
             savedOrderId (int): id of order instance to delete
-        '''
-        return self._request(DELETE_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId), method='DELETE').json()
+        """
+        return self._request(
+            DELETE_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId),
+            method="DELETE",
+        ).json()
 
     def replaceSavedOrder(self, accountId, savedOrderId, order):
-        '''create a saved order
+        """create a saved order
 
         Args:
             accountId (int): id of account to place order under
             savedOrderId (int): id of order instance to delete
             order (JSON): order instance to place
-        '''
-        return self._request(REPLACE_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId), method='PUT', data=order).json()
+        """
+        return self._request(
+            REPLACE_SAVED_ORDER.format(accountId=accountId, savedOrderId=savedOrderId),
+            method="PUT",
+            data=order,
+        ).json()
 
     def hours(self, market="EQUITY", date=None):
-        '''get market hours
+        """get market hours
 
         Args:
             market (str): market to get hours for, in ('EQUITY', 'OPTION', 'FUTURE', 'BOND', 'FOREX')
             date (str): date to get hours for, yyyy-MM-dd or yyyy-MM-dd'T'HH:mm::ssz
-        '''
+        """
         if date:
-            params = {'date': date}
+            params = {"date": date}
         else:
             params = {}
 
         if market:
             if market not in MARKETS_VALUES:
-                raise TDAAPIError('Markets must be in {}'.format(MARKETS_VALUES))
-            return self._request(GET_HOURS_FOR_SINGLE_MARKET.format(market=market), params=params).json()
+                raise TDAAPIError("Markets must be in {}".format(MARKETS_VALUES))
+            return self._request(
+                GET_HOURS_FOR_SINGLE_MARKET.format(market=market), params=params
+            ).json()
         return self._request(GET_HOURS_FOR_MULTIPLE_MARKETS, params=params).json()
 
     def preferences(self, accountId=None):
-        '''get preferences for account
+        """get preferences for account
 
         Args:
             accountId (int): account to get preferences for
-        '''
+        """
         if not accountId:
             ret = {}
             for account in self.accountIds:
-                ret[account] = self._request(GET_PREFERENCES.format(accountId=account)).json()
+                ret[account] = self._request(
+                    GET_PREFERENCES.format(accountId=account)
+                ).json()
             return ret
         return self._request(GET_PREFERENCES.format(accountId=accountId)).json()
 
     def updatePreferences(self, accountId, preferences):
-        '''update preferences for account
+        """update preferences for account
 
         Args:
             accountId (int): account to get preferences for
             preferences (JSON): preferences to update
-        '''
-        return self._request(UPDATE_PREFERENCES.format(accountId=accountId), method='PUT', data=preferences).json()
+        """
+        return self._request(
+            UPDATE_PREFERENCES.format(accountId=accountId),
+            method="PUT",
+            data=preferences,
+        ).json()
 
     def watchlists(self, accountId=None, watchlistId=None):
-        '''get watchlist for account
+        """get watchlist for account
 
         Args:
             accountId (int): account to get watchlist for
             watchlistId (int): watchlist to get
-        '''
+        """
         if not accountId:
             return self._request(GET_WATCHLISTS_MULTIPLE_ACCOUNTS).json()
         if watchlistId:
-            return self._request(GET_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId)).json()
+            return self._request(
+                GET_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId)
+            ).json()
         return self._request(GET_WATCHLISTS.format(accountId=accountId)).json()
 
     def createWatchlist(self, accountId, watchlist):
-        '''create watchlist for account
+        """create watchlist for account
 
         Args:
             accountId (int): account to get watchlist for
             watchlist (JSON): watchlist to create
-        '''
-        return self._request(CREATE_WATCHLIST.format(accountId=accountId), method='POST', data=watchlist).json()
+        """
+        return self._request(
+            CREATE_WATCHLIST.format(accountId=accountId), method="POST", json=watchlist
+        )
 
     def updateWatchlist(self, accountId, watchlistId, watchlist):
-        '''update watchlist for account
+        """update watchlist for account
 
         Args:
             accountId (int): account to get watchlist for
             watchlistId (int): watchlist to update
             watchlist (JSON): watchlist to update with
-        '''
-        return self._request(UPDATE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId), method='PATCH', data=watchlist).json()
+        """
+        return self._request(
+            UPDATE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId),
+            method="PATCH",
+            json=watchlist,
+        )
 
     def replaceWatchlist(self, accountId, watchlistId, watchlist):
-        '''update watchlist for account
+        """update watchlist for account
 
         Args:
             accountId (int): account to get watchlist for
             watchlistId (int): watchlist to update
             watchlist (JSON): watchlist to update with
-        '''
-        return self._request(REPLACE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId), method='PATCH', data=watchlist).json()
+        """
+        return self._request(
+            REPLACE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId),
+            method="PUT",
+            json=watchlist,
+        )
 
     def deleteWatchlist(self, accountId, watchlistId):
-        '''delete watchlist for account
+        """delete watchlist for account
 
         Args:
             accountId (int): account to delete watchlist from
             watchlistId (int): watchlist to delete
-        '''
-        return self._request(DELETE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId), method='DELETE').json()
+        """
+        return self._request(
+            DELETE_WATCHLIST.format(accountId=accountId, watchlistId=watchlistId),
+            method="DELETE",
+        )
```

### Comparing `tdameritrade-0.1.1/tdameritrade/order.py` & `tdameritrade-0.2.0/tdameritrade/order.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 from .exceptions import TDAAPIError
 from .enums import DURATION
+
 # from .enums import DURATION, ORDER_TYPE, COMPLEX_ORDER_STRATEGY_TYPE, LEG_TYPE
 
 
 class OrderBuilder(object):
-    def __init__(self,
-                 quantity,
-                 price,
-                 duration='DAY',
-                 orderType='MARKET',
-                 orderStrategyType='SINGLE',
-                 complexOrderStrategyType='NONE',
-                 specialInstruction=None,
-                 requestedDestination='AUTO',
-                 priceLinkBasis=None,
-                 priceLinkType=None,
-                 stopPrice=0.0,
-                 stopPriceLinkBasis=None,
-                 stopPriceLinkType=None,
-                 stopType=None,
-                 taxLotMethod=None
-                 ):
+    def __init__(
+        self,
+        quantity,
+        price,
+        duration="DAY",
+        orderType="MARKET",
+        orderStrategyType="SINGLE",
+        complexOrderStrategyType="NONE",
+        specialInstruction=None,
+        requestedDestination="AUTO",
+        priceLinkBasis=None,
+        priceLinkType=None,
+        stopPrice=0.0,
+        stopPriceLinkBasis=None,
+        stopPriceLinkType=None,
+        stopType=None,
+        taxLotMethod=None,
+    ):
         if duration not in DURATION:
-            raise TDAAPIError('Duration must be in {}'.format(duration))
+            raise TDAAPIError("Duration must be in {}".format(duration))
 
         self._rep = {
-            'duration': duration,
-            'orderType': orderType,
-            'complexOrderStrategyType': complexOrderStrategyType,
-            'requestedDestination': requestedDestination,
-            'stopPrice': 0,
-            'stopPriceLinkBasis': stopPriceLinkBasis,
-            'stopPriceLinkType': stopPriceLinkType,
-            'stopPriceOffset': 0,
-            'stopType': stopType,
-            'priceLinkBasis': priceLinkBasis,
-            'priceLinkType': priceLinkType,
-            'price': price,
-            'taxLotMethod': taxLotMethod,
-            'orderLegCollection': [],
-            'specialInstruction': specialInstruction,
-            'orderStrategyType': orderStrategyType,
+            "duration": duration,
+            "orderType": orderType,
+            "complexOrderStrategyType": complexOrderStrategyType,
+            "requestedDestination": requestedDestination,
+            "stopPrice": 0,
+            "stopPriceLinkBasis": stopPriceLinkBasis,
+            "stopPriceLinkType": stopPriceLinkType,
+            "stopPriceOffset": 0,
+            "stopType": stopType,
+            "priceLinkBasis": priceLinkBasis,
+            "priceLinkType": priceLinkType,
+            "price": price,
+            "taxLotMethod": taxLotMethod,
+            "orderLegCollection": [],
+            "specialInstruction": specialInstruction,
+            "orderStrategyType": orderStrategyType,
         }
 
-    def addLeg(self, assetType, symbol, instruction, positionEffect, quantity, quantityType, type=None, putCall=None):
+    def addLeg(
+        self,
+        assetType,
+        symbol,
+        instruction,
+        positionEffect,
+        quantity,
+        quantityType,
+        type=None,
+        putCall=None,
+    ):
         leg = {
-            'orderLegType': assetType,
-            'instrument': {
-                'assetType': assetType,
-                'symbol': symbol,
+            "orderLegType": assetType,
+            "instrument": {
+                "assetType": assetType,
+                "symbol": symbol,
             },
-            'instruction': instruction,
-            'positionEffect': positionEffect,
-            'quantity': quantity,
-            'quantityType': quantityType,
+            "instruction": instruction,
+            "positionEffect": positionEffect,
+            "quantity": quantity,
+            "quantityType": quantityType,
         }
 
         # if assetType == 'OPTION':
         #     leg['instrument']['type'] = type
         #     leg['instrument']['putCall'] = putCall
         # elif assetType == 'MUTUAL_FUND':
         #     leg['instrument']['type'] = type
         # elif assetType == 'CASH_EQUIVALENT':
         #     leg['instrument']['type'] = type
         # elif assetType == 'FIXED_INCOME':
         #     leg['instrument']['maturityDate'] = maturityDate
         #     leg['instrument']['variableRate'] = variableRate
         #     leg['instrument']['factor'] = factor
-        self._rep['orderLegCollection'].append(leg)
+        self._rep["orderLegCollection"].append(leg)
 
     def to_json(self):
         return self._rep
```

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/constants.py` & `tdameritrade-0.2.0/tdameritrade/orders/constants.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/leg_builder.py` & `tdameritrade-0.2.0/tdameritrade/orders/leg_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from .constants import Instruction, InstrumentAssetType
 from .models.instruments import EquityInstrument, OptionInstrument
 from .models.leg import OrderLeg
 
 
 def create_equity_order_leg(
-    instruction, quantity, symbol, description=None, cusip=None, **order_leg_kwargs,
+    instruction,
+    quantity,
+    symbol,
+    description=None,
+    cusip=None,
+    **order_leg_kwargs,
 ):
-    """Creates OrderLeg for equity orders
-    """
+    """Creates OrderLeg for equity orders"""
     valid_instructions = [
         Instruction("BUY"),
         Instruction("SELL"),
         Instruction("BUY_TO_COVER"),
         Instruction("SELL_SHORT"),
     ]
 
@@ -28,18 +32,22 @@
         quantity=quantity,
         instrument=instrument,
         **order_leg_kwargs,
     )
 
 
 def create_option_order_leg(
-    instruction, quantity, symbol, description=None, cusip=None, **order_leg_kwargs,
+    instruction,
+    quantity,
+    symbol,
+    description=None,
+    cusip=None,
+    **order_leg_kwargs,
 ):
-    """Creates Option OrderLeg
-    """
+    """Creates Option OrderLeg"""
     asset_type = InstrumentAssetType.OPTION
 
     instrument = OptionInstrument(symbol=symbol, assetType=asset_type)
 
     return OrderLeg(
         instruction=instruction,
         quantity=quantity,
```

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/models/base.py` & `tdameritrade-0.2.0/tdameritrade/orders/models/base.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/models/instruments.py` & `tdameritrade-0.2.0/tdameritrade/orders/models/instruments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 from dataclasses import dataclass
 from typing import List
 
-from ..constants import (CashEquivalentType, InstrumentAssetType,
-                         MutualFundType, OptionDeliverableCurrencyType,
-                         OptionPutCall, OptionType)
+from ..constants import (
+    CashEquivalentType,
+    InstrumentAssetType,
+    MutualFundType,
+    OptionDeliverableCurrencyType,
+    OptionPutCall,
+    OptionType,
+)
 from .base import BaseOrder
 
 
 @dataclass
 class Instrument(BaseOrder):
-    """Base Instrument class
-    """
+    """Base Instrument class"""
 
     pass
 
 
-@dataclass(frozen=True)
+@dataclass
 class EquityInstrument(Instrument):
-    """Equity Instrument
-    """
+    """Equity Instrument"""
 
     assetType: InstrumentAssetType = None
     cusip: str = None
     symbol: str = None
     description: str = None
 
 
-@dataclass(frozen=True)
+@dataclass
 class FixedIncomeInstrument(Instrument):
-    """Fixed Income Instrument
-    """
+    """Fixed Income Instrument"""
 
     assetType: InstrumentAssetType = None
     cusip: str = None
     symbol: str = None
     description: str = None
     maturityDate: str = None
     variableRate: int = None
     factor: int = None
 
 
-@dataclass(frozen=True)
+@dataclass
 class MutualFundInstrument(Instrument):
-    """Mutual Fund Instrument
-    """
+    """Mutual Fund Instrument"""
 
     assetType: InstrumentAssetType = None
     cusip: str = None
     symbol: str = None
     description: str = None
     type: MutualFundType = None
 
 
-@dataclass(frozen=True)
+@dataclass
 class CashEquivalentInstrument(Instrument):
-    """Cash Equivalent Instrument
-    """
+    """Cash Equivalent Instrument"""
 
     assetType: InstrumentAssetType = None
     cusip: str = None
     symbol: str = None
     description: str = None
     type: CashEquivalentType = None
 
 
-@dataclass(frozen=True)
+@dataclass
 class OptionDeliverable(BaseOrder):
     """Option Deliverable in Option's optionDeliverables list
 
     This class is not an instrument itself
     """
 
     symbol: str = None
     deliverableUnits: int = None
     currencyType: OptionDeliverableCurrencyType = None
     assetType: InstrumentAssetType = None
 
 
-@dataclass(frozen=True)
+@dataclass
 class OptionInstrument(Instrument):
-    """Option Instrument
-    """
+    """Option Instrument"""
 
     assetType: InstrumentAssetType = None
     cusip: str = None
     symbol: str = None
     description: str = None
     type: OptionType = None
     putCall: OptionPutCall = None
     underlyingSymbol: str = None
     optionMultiplier: int = None
-    optionDeliverables: List = None  # List[OptionDeliverable]. Issue with List[type] formatting
+    optionDeliverables: List = (
+        None  # List[OptionDeliverable]. Issue with List[type] formatting
+    )
```

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/models/leg.py` & `tdameritrade-0.2.0/tdameritrade/orders/models/leg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Order Leg usedin in Orders API
 """
 from dataclasses import dataclass
 
-from ..constants import (Instruction, InstrumentAssetType, OrderLegType,
-                         PositionEffect, QuantityType)
+from ..constants import (
+    Instruction,
+    InstrumentAssetType,
+    OrderLegType,
+    PositionEffect,
+    QuantityType,
+)
 from .base import BaseOrder
 from .instruments import EquityInstrument, Instrument, OptionInstrument
 
 
 class InvalidInstructionError(Exception):
     pass
 
 
 @dataclass
 class OrderLeg(BaseOrder):
-    """OrderLeg used in orderLegCollection
-    """
+    """OrderLeg used in orderLegCollection"""
 
     orderLegType: OrderLegType = None
     legId: int = None
     instrument: Instrument = None
     instruction: Instruction = None
     positionEffect: PositionEffect = None
     quantity: int = None
```

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/models/orders.py` & `tdameritrade-0.2.0/tdameritrade/orders/models/orders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 from dataclasses import dataclass
 from typing import List
 
 from ..constants import (
-    ComplexOrderStrategyType, Duration, OrderStrategyType, OrderType,
-    PriceLinkBasis, PriceLinkType, RequestedDestination, Session,
-    SpecialInstruction, Status, StopPriceLinkBasis, StopPriceLinkType,
-    StopType, TaxLotMethod)
+    ComplexOrderStrategyType,
+    Duration,
+    OrderStrategyType,
+    OrderType,
+    PriceLinkBasis,
+    PriceLinkType,
+    RequestedDestination,
+    Session,
+    SpecialInstruction,
+    Status,
+    StopPriceLinkBasis,
+    StopPriceLinkType,
+    StopType,
+    TaxLotMethod,
+)
 from .base import BaseOrder
 
 
 @dataclass
 class CancelTime(BaseOrder):
     date: str = None
     shortFormat: bool = None
@@ -52,11 +63,13 @@
     orderId: int = None
     cancelable: bool = None
     editable: bool = None
     status: Status = None
     enteredTime: str = None
     closeTime: str = None
     accountId: int = None
-    orderActivityCollection: List = None  # List[OrderActivity]. Issue with List[type] formatting
+    orderActivityCollection: List = (
+        None  # List[OrderActivity]. Issue with List[type] formatting
+    )
     replacingOrderCollection: List = None  # List[Order]
     childOrderStrategies: List = None  # List[Order]
     statusDescription: str = None
```

### Comparing `tdameritrade-0.1.1/tdameritrade/orders/order_builder.py` & `tdameritrade-0.2.0/tdameritrade/orders/order_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from .constants import (ComplexOrderStrategyType, Duration, Instruction,
-                        OrderStrategyType, OrderType, Session)
+from .constants import (
+    ComplexOrderStrategyType,
+    Duration,
+    Instruction,
+    OrderStrategyType,
+    OrderType,
+    Session,
+)
 from .leg_builder import create_equity_order_leg, create_option_order_leg
 from .models.orders import Order
 
 
 def build_buy_market_stock_order(symbol, quantity):
     """Build Buy Market Stock Order
 
-    Buy {quantity} shares of {smybol} at the Market good for the Day.
+    Buy {quantity} shares of {symbol} at the Market good for the Day.
 
     Simple sample from https://developer.tdameritrade.com/content/place-order-samples
 
     Args:
         symbol: symbol you want to trade
         quantity: How much of the stock to trade
     """
@@ -20,15 +26,17 @@
     session = Session.NORMAL
     duration = Duration.DAY
     order_strategy_type = OrderStrategyType.SINGLE
     # Can be changed to handle Buy and Sell for Equities
     _instruction = Instruction.BUY
 
     _order_leg = create_equity_order_leg(
-        instruction=_instruction, quantity=quantity, symbol=symbol,
+        instruction=_instruction,
+        quantity=quantity,
+        symbol=symbol,
     )
     order_leg_collection = [_order_leg]
 
     return Order(
         orderType=order_type,
         session=session,
         duration=duration,
@@ -36,15 +44,15 @@
         orderLegCollection=order_leg_collection,
     )
 
 
 def build_buy_limit_option_order(symbol, quantity, price):
     """Build Buy Limit: Single Option
 
-    Buy to open {quanity} contracts of the {symbol with date and option info}
+    Buy to open {quantity} contracts of the {symbol with date and option info}
     at a Limit of {price} good for the Day.
 
     Args:
         symbol: symbol you want to trade.  Includes date e.g., XYZ_032015C49
         quantity: Amount you want to buy
         price: Amount you want to buy the option for
 
@@ -57,15 +65,17 @@
     order_type = OrderType.LIMIT
     session = Session.NORMAL
     duration = Duration.DAY
     order_strategy_type = OrderStrategyType.SINGLE
     _instruction = Instruction.BUY_TO_OPEN
 
     _order_leg = create_option_order_leg(
-        instruction=_instruction, quantity=quantity, symbol=symbol,
+        instruction=_instruction,
+        quantity=quantity,
+        symbol=symbol,
     )
     order_leg_collection = [_order_leg]
 
     return Order(
         complexOrderStrategyType=complex_order_strategy_type,
         orderType=order_type,
         session=session,
@@ -94,19 +104,23 @@
     # Constants
     order_type = OrderType.NET_DEBIT
     session = Session.NORMAL
     duration = Duration.DAY
     order_strategy_type = OrderStrategyType.SINGLE
 
     _buy_order_leg = create_option_order_leg(
-        instruction=Instruction.BUY_TO_OPEN, quantity=quantity, symbol=buy_symbol,
+        instruction=Instruction.BUY_TO_OPEN,
+        quantity=quantity,
+        symbol=buy_symbol,
     )
 
     _sell_order_leg = create_option_order_leg(
-        instruction=Instruction.SELL_TO_OPEN, quantity=quantity, symbol=sell_symbol,
+        instruction=Instruction.SELL_TO_OPEN,
+        quantity=quantity,
+        symbol=sell_symbol,
     )
 
     order_leg_collection = [
         _buy_order_leg,
         _sell_order_leg,
     ]
 
@@ -132,15 +146,17 @@
     order_strategy_type = OrderStrategyType.SINGLE
     order_type = OrderType.MARKET
     session = Session.NORMAL
     duration = Duration.DAY
     complex_order_strategy_type = ComplexOrderStrategyType.CUSTOM
 
     _buy_order_leg = create_option_order_leg(
-        instruction=Instruction.BUY_TO_OPEN, quantity=buy_quantity, symbol=buy_symbol,
+        instruction=Instruction.BUY_TO_OPEN,
+        quantity=buy_quantity,
+        symbol=buy_symbol,
     )
 
     _sell_order_leg = create_option_order_leg(
         instruction=Instruction.SELL_TO_OPEN,
         quantity=sell_quantity,
         symbol=sell_symbol,
     )
```

### Comparing `tdameritrade-0.1.1/tdameritrade/session.py` & `tdameritrade-0.2.0/tdameritrade/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import requests
 import time
 from . import auth
 
 
 class TDASession(requests.Session):
-
     def __init__(self, refresh_token=None, client_id=None):
         super().__init__()
-        self._refreshToken = {'token': refresh_token}
-        self._accessToken = {'token': '',
-                             'created_at': time.time(),
-                             'expires_in': -1}  # Set to -1 so that it gets refreshed immediately and its age tracked.
+        self._refreshToken = {"token": refresh_token}
+        self._accessToken = {
+            "token": "",
+            "created_at": time.time(),
+            "expires_in": -1,
+        }  # Set to -1 so that it gets refreshed immediately and its age tracked.
         self._client_id = client_id
         self._headers = {}
 
     def _set_header_auth(self):
-        self._headers.update({'Authorization': 'Bearer ' + self._accessToken['token']})
+        self._headers.update({"Authorization": "Bearer " + self._accessToken["token"]})
 
     def request(self, *args, **kwargs):
         self._refresh_token_if_invalid()
         return super().request(headers=self._headers, *args, **kwargs)
 
     def _is_token_invalid(self):
-        if not self._accessToken['token'] or \
-                self._access_token_age_secs() >= self._accessToken['expires_in'] - 60:
+        if (
+            not self._accessToken["token"]
+            or self._access_token_age_secs() >= self._accessToken["expires_in"] - 60
+        ):
             return True
         else:
             return False
 
     def _refresh_token_if_invalid(self):
         # Expire the token one minute before its expiration time to be safe
         if self._is_token_invalid():
-            token = auth.access_token(self._refreshToken['token'], self._client_id)
+            token = auth.access_token(self._refreshToken["token"], self._client_id)
             self._set_access_token(token)
 
     def _set_access_token(self, token):
-        self._accessToken['token'] = token['access_token']
-        self._accessToken['created_at'] = time.time()
-        self._accessToken['expires_in'] = token['expires_in']
+        self._accessToken["token"] = token["access_token"]
+        self._accessToken["created_at"] = time.time()
+        self._accessToken["expires_in"] = token["expires_in"]
         self._set_header_auth()
 
     def _access_token_age_secs(self):
-        return time.time() - self._accessToken['created_at']
+        return time.time() - self._accessToken["created_at"]
```

### Comparing `tdameritrade-0.1.1/tdameritrade/tests/test_client.py` & `tdameritrade-0.2.0/tdameritrade/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 from mock import MagicMock, patch
 
 
 @pytest.fixture
 def tdclient():
     from tdameritrade import TDClient
-    tdc = TDClient(client_id=123,
-                   refresh_token='reftoken',
-                   account_ids=[1, 2])
+
+    tdc = TDClient(client_id=123, refresh_token="reftoken", account_ids=[1, 2])
     return tdc
 
 
 class TestExtension:
     def setup(self):
         pass
         # setup() before each test method
@@ -31,100 +30,106 @@
 
     @classmethod
     def teardown_class(cls):
         pass
         # teardown_class() after any methods in this class
 
     def test_init(self, tdclient):
-        assert (tdclient._refreshToken == 'reftoken')
+        assert tdclient._refreshToken == "reftoken"
 
     def test_request(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
             m.return_value.json.return_value = [MagicMock()]
             tdclient._request("http://goodurl.com", None)
 
     def test_request_exception(self, tdclient):
         from tdameritrade.exceptions import InvalidAuthToken
-        with patch('tdameritrade.session.TDASession.request') as m:
+
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 401
             with pytest.raises(InvalidAuthToken):
                 tdclient._request("http://goodurl.com", None)
 
     def test_accounts(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
             m.return_value.json.return_value = [MagicMock()]
             tdclient.accounts()
-            m.return_value.json.return_value = [{'test': 1, 'test2': 2}]
+            m.return_value.json.return_value = [{"test": 1, "test2": 2}]
             tdclient.accounts(positions=True)
             tdclient.accounts(positions=True, orders=True)
             tdclient.accounts(orders=True)
             tdclient.accountsDF()
-            m.return_value.json.return_value = [{'test': 1}]
+            m.return_value.json.return_value = [{"test": 1}]
             tdclient.accountsDF()
 
-
     def test_accounts_no_accountIDs(self):
         from tdameritrade import TDClient
-        with patch('tdameritrade.session.TDASession.request') as m:
+
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
             m.return_value.json.return_value = [MagicMock()]
-            tdc = TDClient(client_id=123,
-                           refresh_token='reftoken',)
+            tdc = TDClient(
+                client_id=123,
+                refresh_token="reftoken",
+            )
             tdc.accounts()
 
     def test_search(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            m.return_value.json.return_value = {'aapl': {'test': 1, 'test2': 2}}
-            tdclient.search('aapl')
-            tdclient.searchDF('aapl')
+            m.return_value.json.return_value = {"aapl": {"test": 1, "test2": 2}}
+            tdclient.search("aapl")
+            tdclient.searchDF("aapl")
 
     def test_fundementalSearch(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            tdclient.fundamentalSearch('aapl')
-            tdclient.fundamentalSearch('aapl')
+            tdclient.fundamentalSearch("aapl")
+            tdclient.fundamentalSearch("aapl")
 
     def test_instrument(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            m.return_value.json.return_value = {'aapl': {'test': 1, 'test2': 2}}
-            tdclient.instrument('aapl')
-            tdclient.instrumentDF('aapl')
+            m.return_value.json.return_value = {"aapl": {"test": 1, "test2": 2}}
+            tdclient.instrument("aapl")
+            tdclient.instrumentDF("aapl")
 
     def test_quote(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            m.return_value.json.return_value = {'aapl': {'test': 1, 'test2': 2}}
-            tdclient.quote('aapl')
-            tdclient.quoteDF('aapl')
+            m.return_value.json.return_value = {"aapl": {"test": 1, "test2": 2}}
+            tdclient.quote("aapl")
+            tdclient.quoteDF("aapl")
 
     def test_history(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            m.return_value.json.return_value = {'candles': [{'datetime': 1, 'test2': 2}]}
-            tdclient.history('aapl')
-            tdclient.historyDF('aapl')
-            tdclient.history('aapl', periodType="day")
+            m.return_value.json.return_value = {
+                "candles": [{"datetime": 1, "test2": 2}]
+            }
+            tdclient.history("aapl")
+            tdclient.historyDF("aapl")
+            tdclient.history("aapl", periodType="day")
             with pytest.raises(TDAAPIError):
-                tdclient.history('aapl', periodType="daily")
+                tdclient.history("aapl", periodType="daily")
             with pytest.raises(TDAAPIError):
-                tdclient.history('aapl', frequency="invalid")
+                tdclient.history("aapl", frequency="invalid")
 
     def test_hours(self, tdclient):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
             tdclient.hours()
 
     def test_movers(self):
-        with patch('tdameritrade.session.TDASession.request') as m:
+        with patch("tdameritrade.session.TDASession.request") as m:
             m.return_value.status_code = 200
-            m.return_value.json.return_value = {'aapl': {'test'}}
+            m.return_value.json.return_value = {"aapl": {"test"}}
+
 
 #    @pytest.fixture
 #    def json_order(self):
 #        from tdameritrade.tests.JSONS import TEST_BUY_MARKET_STOCK
 
 #    def test_place_order(self, json_order, tdclient):
 #        with patch('tdameritrade.session.TDASession.request') as m:
```

### Comparing `tdameritrade-0.1.1/tdameritrade/tests/test_session.py` & `tdameritrade-0.2.0/tdameritrade/tests/test_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from mock import patch
 import time
 
 
-@patch('tdameritrade.auth.access_token')
+@patch("tdameritrade.auth.access_token")
 class TestSession:
-
     def test_init(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
-        assert s._accessToken['expires_in'] == -1
+        assert s._accessToken["expires_in"] == -1
 
     def test_request_headers(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
-        s._accessToken['token'] = "testToken"
+        s._accessToken["token"] = "testToken"
         s._set_header_auth()
-        assert s._headers['Authorization'] == 'Bearer testToken'
+        assert s._headers["Authorization"] == "Bearer testToken"
 
     def test_token_age(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
-        s._accessToken['created_at'] = time.time() - 60
+        s._accessToken["created_at"] = time.time() - 60
         assert s._access_token_age_secs() > 59
         assert s._access_token_age_secs() < 61
 
     def test_is_token_invalid_returns_true(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
         assert s._is_token_invalid()
-        s._accessToken['token'] = "testToken"
-        s._accessToken['created_at'] = time.time() - 61
-        s._accessToken['expires_in'] = 60
+        s._accessToken["token"] = "testToken"
+        s._accessToken["created_at"] = time.time() - 61
+        s._accessToken["expires_in"] = 60
         assert s._is_token_invalid()
 
     def test_is_token_invalid_returns_false(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
-        s._accessToken['token'] = "testToken"
-        s._accessToken['created_at'] = time.time() - 60
-        s._accessToken['expires_in'] = time.time() + 1
+        s._accessToken["token"] = "testToken"
+        s._accessToken["created_at"] = time.time() - 60
+        s._accessToken["expires_in"] = time.time() + 1
         assert s._is_token_invalid() == 0
 
     def test_update_access_token_if_expired(self, mocked_auth):
         from tdameritrade import session
+
         s = session.TDASession()
-        with patch('tdameritrade.auth.access_token') as mock:
+        with patch("tdameritrade.auth.access_token") as mock:
             s._refresh_token_if_invalid()
-            mock.assert_called_with(s._refreshToken['token'], s._client_id)
+            mock.assert_called_with(s._refreshToken["token"], s._client_id)
```

### Comparing `tdameritrade-0.1.1/tdameritrade/tests/unit/orders/test_order_builder.py` & `tdameritrade-0.2.0/tdameritrade/tests/unit/orders/test_order_builder.py`

 * *Files identical despite different names*

### Comparing `tdameritrade-0.1.1/tdameritrade/urls.py` & `tdameritrade-0.2.0/tdameritrade/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,166 +1,233 @@
-BASE = 'https://api.tdameritrade.com/v1/'
+BASE = "https://api.tdameritrade.com/v1/"
 
 ########################
 # Accounts and Trading #
 ########################
 # https://developer.tdameritrade.com/account-access/apis
 
 # ORDERS
-CANCEL_ORDER = BASE + 'accounts/{accountId}/orders/{orderId}'  # DELETE
-GET_ORDER = BASE + 'accounts/{accountId}/orders/{orderId}'  # GET
-GET_ORDERS_BY_PATH = BASE + 'accounts/{accountId}/orders'  # GET
-GET_ORDER_BY_QUERY = BASE + 'orders'  # GET
-PLACE_ORDER = BASE + 'accounts/{accountId}/orders'  # POST
-REPLACE_ORDER = BASE + 'accounts/{accountId}/orders/{orderId}'  # PUT
-GET_ORDER_BY_PATH_ARGS = ('maxResults', 'fromEnteredTime', 'toEnteredTime', 'status')
-GET_ORDER_BY_QUERY_ARGS = ('accountId', 'maxResults', 'fromEnteredTime', 'toEnteredTime', 'status')
+CANCEL_ORDER = BASE + "accounts/{accountId}/orders/{orderId}"  # DELETE
+GET_ORDER = BASE + "accounts/{accountId}/orders/{orderId}"  # GET
+GET_ORDERS_BY_PATH = BASE + "accounts/{accountId}/orders"  # GET
+GET_ORDER_BY_QUERY = BASE + "orders"  # GET
+PLACE_ORDER = BASE + "accounts/{accountId}/orders"  # POST
+REPLACE_ORDER = BASE + "accounts/{accountId}/orders/{orderId}"  # PUT
+GET_ORDER_BY_PATH_ARGS = ("maxResults", "fromEnteredTime", "toEnteredTime", "status")
+GET_ORDER_BY_QUERY_ARGS = (
+    "accountId",
+    "maxResults",
+    "fromEnteredTime",
+    "toEnteredTime",
+    "status",
+)
 STATUS_VALUES = (
-    'AWAITING_PARENT_ORDER',
-    'AWAITING_CONDITION',
-    'AWAITING_MANUAL_REVIEW',
-    'ACCEPTED',
-    'AWAITING_UR_OUT',
-    'PENDING_ACTIVATION',
-    'QUEUED',
-    'WORKING',
-    'REJECTED',
-    'PENDING_CANCEL',
-    'CANCELED',
-    'PENDING_REPLACE',
-    'REPLACED',
-    'FILLED',
-    'EXPIRED')
+    "AWAITING_PARENT_ORDER",
+    "AWAITING_CONDITION",
+    "AWAITING_MANUAL_REVIEW",
+    "ACCEPTED",
+    "AWAITING_UR_OUT",
+    "PENDING_ACTIVATION",
+    "QUEUED",
+    "WORKING",
+    "REJECTED",
+    "PENDING_CANCEL",
+    "CANCELED",
+    "PENDING_REPLACE",
+    "REPLACED",
+    "FILLED",
+    "EXPIRED",
+)
 # maxResults: int
 # fromEnteredTime: yyyy-MM-dd
 # toEnteredTime: yyyy-MM-dd
 # status: STATUS_VALUES
 
 # SAVED ORDERS
-CREATE_SAVED_ORDER = BASE + 'accounts/{accountId}/savedorders'  # POST
-DELETE_SAVED_ORDER = BASE + 'accounts/{accountId}/savedorders/{savedOrderId}'  # DELETE
-GET_SAVED_ORDER = BASE + 'accounts/{accountId}/savedorders/{savedOrderId}'  # GET
-GET_SAVED_ORDER_BY_PATH = BASE + 'accounts/{accountId}/savedorders'  # GET
-REPLACE_SAVED_ORDER = BASE + 'accounts/{accountId}/savedorders/{savedOrderId}'  # PUT
+CREATE_SAVED_ORDER = BASE + "accounts/{accountId}/savedorders"  # POST
+DELETE_SAVED_ORDER = BASE + "accounts/{accountId}/savedorders/{savedOrderId}"  # DELETE
+GET_SAVED_ORDER = BASE + "accounts/{accountId}/savedorders/{savedOrderId}"  # GET
+GET_SAVED_ORDER_BY_PATH = BASE + "accounts/{accountId}/savedorders"  # GET
+REPLACE_SAVED_ORDER = BASE + "accounts/{accountId}/savedorders/{savedOrderId}"  # PUT
 
 # ACCOUNTS
-GET_ACCOUNT = BASE + 'accounts/{accountId}'  # GET
-GET_ACCOUNTS = BASE + 'accounts'  # GET
+GET_ACCOUNT = BASE + "accounts/{accountId}"  # GET
+GET_ACCOUNTS = BASE + "accounts"  # GET
 
 ##################
 # AUTHENTICATION #
 ##################
 # https://developer.tdameritrade.com/authentication/apis
-ACCESS_TOKEN = BASE + 'oauth2/token'  # POST
-ACCESS_TOKEN_ARGS = ('grant_type', 'refresh_token', 'access_type', 'code', 'client_id', 'redirect_uri')
+ACCESS_TOKEN = BASE + "oauth2/token"  # POST
+ACCESS_TOKEN_ARGS = (
+    "grant_type",
+    "refresh_token",
+    "access_type",
+    "code",
+    "client_id",
+    "redirect_uri",
+)
 
 ###############
 # INSTRUMENTS #
 ###############
 # https://developer.tdameritrade.com/instruments/apis
-SEARCH_INSTRUMENTS = BASE + 'instruments'  # GET
-SEARCH_INSTRUMENTS_ARGS = ('symbol', 'projection')
-SEARCH_INSTRUMENT_PROJECTION = ('symbol-search', 'symbol-regex', 'desc-search', 'desc-regex', 'fundamental')
-GET_INSTRUMENT = BASE + 'instruments/{cusip}'  # GET
+SEARCH_INSTRUMENTS = BASE + "instruments"  # GET
+SEARCH_INSTRUMENTS_ARGS = ("symbol", "projection")
+SEARCH_INSTRUMENT_PROJECTION = (
+    "symbol-search",
+    "symbol-regex",
+    "desc-search",
+    "desc-regex",
+    "fundamental",
+)
+GET_INSTRUMENT = BASE + "instruments/{cusip}"  # GET
 
 ################
 # MARKET HOURS #
 ################
 # https://developer.tdameritrade.com/market-hours/apis
-GET_HOURS_FOR_MULTIPLE_MARKETS = BASE + 'marketdata/hours'  # GET
-GET_HOURS_FOR_MULTIPLE_MARKETS_ARGS = ('markets', 'date')
-MARKETS_VALUES = ('EQUITY', 'OPTION', 'FUTURE', 'BOND', 'FOREX')
-GET_HOURS_FOR_SINGLE_MARKET = BASE + 'marketdata/{market}/hours'  # GET
-GET_HOURS_FOR_SINGLE_MARKET_ARGS = ('date')
+GET_HOURS_FOR_MULTIPLE_MARKETS = BASE + "marketdata/hours"  # GET
+GET_HOURS_FOR_MULTIPLE_MARKETS_ARGS = ("markets", "date")
+MARKETS_VALUES = ("EQUITY", "OPTION", "FUTURE", "BOND", "FOREX")
+GET_HOURS_FOR_SINGLE_MARKET = BASE + "marketdata/{market}/hours"  # GET
+GET_HOURS_FOR_SINGLE_MARKET_ARGS = "date"
 # date: yyyy-MM-dd or yyyy-MM-dd'T'HH:mm::ssz
 
 ##########
 # MOVERS #
 ##########
 # https://developer.tdameritrade.com/movers/apis
-MOVERS = BASE + 'marketdata/{index}/movers'  # GET
-MOVERS_ARGS = ('direction', 'change')
-DIRECTION_VALUES = ('up', 'down')
-CHANGE_VALUES = ('value', 'percent')
+MOVERS = BASE + "marketdata/{index}/movers"  # GET
+MOVERS_ARGS = ("direction", "change")
+DIRECTION_VALUES = ("up", "down")
+CHANGE_VALUES = ("value", "percent")
 
 #################
 # OPTION CHAINS #
 #################
 # https://developer.tdameritrade.com/option-chains/apis
-GET_OPTION_CHAIN = BASE + 'marketdata/chains'  # GET
-OPTION_CHAIN_ARGS = ('symbol',
-                     'contractType',
-                     'strikeCount',
-                     'includeQuotes',
-                     'strategy',
-                     'interval',
-                     'strike',
-                     'range',
-                     'fromDate',
-                     'toDate',
-                     'volatility',
-                     'underlyingPrice',
-                     'interestRate',
-                     'daysToExpiration',
-                     'expMonth',
-                     'optionType')
-CONTRACT_TYPE_VALUES = ('CALL', 'PUT', 'ALL')
-STRATEGY_VALUES = ('SINGLE', 'ANALYTICAL', 'COVERED', 'VERTICAL', 'CALENDAR', 'STRANGLE', 'STRADDLE', 'BUTTERFLY', 'CONDOR', 'DIAGONAL', 'COLLAR', 'ROLL')
-RANGE_VALUES = ('ITM', 'NTM', 'OTM', 'SAK', 'SBK', 'SNK', 'ALL')
-OPTION_TYPE_VALUES = ('S', 'NS', 'ALL')
-OPTION_EXPMONTH_VALUES = ('JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC', 'ALL')
+GET_OPTION_CHAIN = BASE + "marketdata/chains"  # GET
+OPTION_CHAIN_ARGS = (
+    "symbol",
+    "contractType",
+    "strikeCount",
+    "includeQuotes",
+    "strategy",
+    "interval",
+    "strike",
+    "range",
+    "fromDate",
+    "toDate",
+    "volatility",
+    "underlyingPrice",
+    "interestRate",
+    "daysToExpiration",
+    "expMonth",
+    "optionType",
+)
+CONTRACT_TYPE_VALUES = ("CALL", "PUT", "ALL")
+STRATEGY_VALUES = (
+    "SINGLE",
+    "ANALYTICAL",
+    "COVERED",
+    "VERTICAL",
+    "CALENDAR",
+    "STRANGLE",
+    "STRADDLE",
+    "BUTTERFLY",
+    "CONDOR",
+    "DIAGONAL",
+    "COLLAR",
+    "ROLL",
+)
+RANGE_VALUES = ("ITM", "NTM", "OTM", "SAK", "SBK", "SNK", "ALL")
+OPTION_TYPE_VALUES = ("S", "NS", "ALL")
+OPTION_EXPMONTH_VALUES = (
+    "JAN",
+    "FEB",
+    "MAR",
+    "APR",
+    "MAY",
+    "JUN",
+    "JUL",
+    "AUG",
+    "SEP",
+    "OCT",
+    "NOV",
+    "DEC",
+    "ALL",
+)
 
 #################
 # PRICE HISTORY #
 #################
 # https://developer.tdameritrade.com/price-history/apis
-GET_PRICE_HISTORY = BASE + 'marketdata/{symbol}/pricehistory'  # GET
-GET_PRICE_HISTORY_ARGS = ('periodType',
-                          'period',
-                          'frequencyType',
-                          'frequency',
-                          'endDate',
-                          'startDate',
-                          'needExtendedHoursData')
-PERIOD_TYPE_VALUES = ('day', 'month', 'year', 'ytd')
-FREQUENCY_TYPE_VALUES = ('minute', 'daily', 'weekly', 'monthly')
+GET_PRICE_HISTORY = BASE + "marketdata/{symbol}/pricehistory"  # GET
+GET_PRICE_HISTORY_ARGS = (
+    "periodType",
+    "period",
+    "frequencyType",
+    "frequency",
+    "endDate",
+    "startDate",
+    "needExtendedHoursData",
+)
+PERIOD_TYPE_VALUES = ("day", "month", "year", "ytd")
+FREQUENCY_TYPE_VALUES = ("minute", "daily", "weekly", "monthly")
 
 ##########
 # QUOTES #
 ##########
 # https://developer.tdameritrade.com/quotes/apis
-GET_QUOTE = BASE + 'marketdata/{symbol}/quotes'  # GET
-GET_QUOTES = BASE + 'marketdata/quotes'  # GET
-GET_QUOTES_ARGS = ('symbol',)
+GET_QUOTE = BASE + "marketdata/{symbol}/quotes"  # GET
+GET_QUOTES = BASE + "marketdata/quotes"  # GET
+GET_QUOTES_ARGS = ("symbol",)
 
 #######################
 # TRANSACTION HISTORY #
 #######################
 # https://developer.tdameritrade.com/transaction-history/apis
-GET_TRANSACTION = BASE + 'accounts/{accountId}/transactions/{transactionId}'  # GET
-GET_TRANSACTIONS = BASE + 'accounts/{accountId}/transactions'  # GET
-GET_TRANSACTIONS_ARGS = ('type', 'symbol', 'startDate', 'endDate')
-GET_TRANSCATION_TYPE_VALUES = ('ALL', 'TRADE', 'BUY_ONLY', 'SELL_ONLY', 'CASH_IN_OR_CASH_OUT', 'CHECKING', 'DIVIDEND', 'INTEREST', 'OTHER', 'ADVISOR_FEES')
+GET_TRANSACTION = BASE + "accounts/{accountId}/transactions/{transactionId}"  # GET
+GET_TRANSACTIONS = BASE + "accounts/{accountId}/transactions"  # GET
+GET_TRANSACTIONS_ARGS = ("type", "symbol", "startDate", "endDate")
+GET_TRANSCATION_TYPE_VALUES = (
+    "ALL",
+    "TRADE",
+    "BUY_ONLY",
+    "SELL_ONLY",
+    "CASH_IN_OR_CASH_OUT",
+    "CHECKING",
+    "DIVIDEND",
+    "INTEREST",
+    "OTHER",
+    "ADVISOR_FEES",
+)
 
 ###################
 # User Info/Prefs #
 ###################
 # https://developer.tdameritrade.com/user-principal/apis
-GET_PREFERENCES = BASE + 'accounts/{accountId}/preferences'  # GET
-GET_STREAMER_SUBSCRIPTION_KEYS = BASE + 'userprincipals/streamersubscriptionkeys'  # GET
-GET_STREAMER_SUBSCRIPTION_KEYS_ARGS = ('accountIds',)
-GET_USER_PRINCIPALS = BASE + 'userprincipals'  # GET
-GET_USER_PRINCIPALS_ARGS = ('fields',)
-USER_PRINCIPALS_FIELDS_VALUES = ('streamerSubscriptionKeys', 'streamerConnectionInfo', 'preferences', 'surrogateIds')
-UPDATE_PREFERENCES = BASE + 'accounts/{accountId}/preferences'  # PUT
+GET_PREFERENCES = BASE + "accounts/{accountId}/preferences"  # GET
+GET_STREAMER_SUBSCRIPTION_KEYS = BASE + "userprincipals/streamersubscriptionkeys"  # GET
+GET_STREAMER_SUBSCRIPTION_KEYS_ARGS = ("accountIds",)
+GET_USER_PRINCIPALS = BASE + "userprincipals"  # GET
+GET_USER_PRINCIPALS_ARGS = ("fields",)
+USER_PRINCIPALS_FIELDS_VALUES = (
+    "streamerSubscriptionKeys",
+    "streamerConnectionInfo",
+    "preferences",
+    "surrogateIds",
+)
+UPDATE_PREFERENCES = BASE + "accounts/{accountId}/preferences"  # PUT
 
 #############
 # WATCHLIST #
 #############
 # https://developer.tdameritrade.com/watchlist/apis
-CREATE_WATCHLIST = BASE + 'accounts/{accountId}/watchlists'  # POST
-DELETE_WATCHLIST = BASE + 'accounts/{accountId}/watchlists/{watchlistId}'  # DELETE
-GET_WATCHLIST = BASE + 'accounts/{accountId}/watchlists/{watchlistId}'  # GET
-GET_WATCHLISTS_MULTIPLE_ACCOUNTS = BASE + 'accounts/watchlists'  # GET
-GET_WATCHLISTS = BASE + 'accounts/{accountId}/watchlists'  # GET
-REPLACE_WATCHLIST = BASE + 'accounts/{accountId}/watchlists/{watchlistId}'  # PUT
-UPDATE_WATCHLIST = BASE + 'accounts/{accountId}/watchlists/{watchlistId}'  # PATCH
+CREATE_WATCHLIST = BASE + "accounts/{accountId}/watchlists"  # POST
+DELETE_WATCHLIST = BASE + "accounts/{accountId}/watchlists/{watchlistId}"  # DELETE
+GET_WATCHLIST = BASE + "accounts/{accountId}/watchlists/{watchlistId}"  # GET
+GET_WATCHLISTS_MULTIPLE_ACCOUNTS = BASE + "accounts/watchlists"  # GET
+GET_WATCHLISTS = BASE + "accounts/{accountId}/watchlists"  # GET
+REPLACE_WATCHLIST = BASE + "accounts/{accountId}/watchlists/{watchlistId}"  # PUT
+UPDATE_WATCHLIST = BASE + "accounts/{accountId}/watchlists/{watchlistId}"  # PATCH
```

### Comparing `tdameritrade-0.1.1/tdameritrade.egg-info/PKG-INFO` & `tdameritrade-0.2.0/tdameritrade.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 Metadata-Version: 2.1
 Name: tdameritrade
-Version: 0.1.1
+Version: 0.2.0
 Summary: APIs for TD Ameritrade
 Home-page: https://github.com/timkpaine/tdameritrade
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
-Description: # tdameritrade
-        Python interface to TD Ameritrade Api
-        
-        [![Build Status](https://dev.azure.com/tpaine154/tdameritrade/_apis/build/status/timkpaine.tdameritrade?branchName=master)](https://dev.azure.com/tpaine154/tdameritrade/_build/latest?definitionId=8&branchName=master)
-        [![Coverage](https://img.shields.io/azure-devops/coverage/tpaine154/tdameritrade/8)]()
-        [![License](https://img.shields.io/github/license/timkpaine/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
-        [![PyPI](https://img.shields.io/pypi/v/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
-        [![Docs](https://img.shields.io/readthedocs/tdameritrade.svg)](https://tdameritrade.readthedocs.io)
-        
-        
-        
-        ## Getting Started
-        
-        ### Install
-        Install from pip
-        
-        `pip install tdameritrade`
-        
-        or from source
-        
-        `python setup.py install`
-        
-        
-        ### Docs
-        Major changes in the v0.1.0 update to the way tokens are handled.  
-        You will still need the original authentication instructions, but the TDClient now takes the refresh token and client
-        id, not the access token. A new session class handles token expiration and will automatically call a new token as
-        needed. 
-        
-        It is recommended that you store these as environmental variables.  
-        
-        ```
-        client_id = os.getenv('TDAMERITRADE_CLIENT_ID')
-        account_id = os.getenv('TDAMERITRADE_ACCOUNT_ID')
-        refresh_token = os.getenv('TDAMERITRADE_REFRESH_TOKEN')
-        
-        tdclient = tdameritrade.TDClient(client_id=client_id, refresh_token=refresh_token, account_ids=[account_id])
-        ``` 
-        
-        See the tests\test_client.py file for examples on current usage. 
-        
-        [Read the docs!](http://tdameritrade.readthedocs.io/en/latest/index.html)
-        
-        All functionality is available as methods on the `TDClient` object. For most methods, there is a convenience method to return the result as a pandas DataFrame.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/client.png)
-        
-        Most data fetching methods accept the symbol as argument. For equities, this is just the ticker.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/client/quote.png)
-        
-        For different assets, utilize the `search` and `instrument` methods to lookup symbols. For options, you can utilize the options method.
-        
-        ![](https://raw.githubusercontent.com/timkpaine/tdameritrade/master/docs/img/options.png)
-        
-        
 Keywords: finance data
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# tdameritrade
+Python interface to TD Ameritrade Api
+
+[![Build Status](https://github.com/timkpaine/tdameritrade/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/tdameritrade/actions?query=workflow%3A%22Build+Status%22)
+[![Coverage](https://codecov.io/gh/timkpaine/tdameritrade/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/tdameritrade)
+[![License](https://img.shields.io/github/license/timkpaine/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
+[![PyPI](https://img.shields.io/pypi/v/tdameritrade.svg)](https://pypi.python.org/pypi/tdameritrade/)
+
+
+
+## Getting Started
+
+### Install
+Install from pip
+
+`pip install tdameritrade`
+
+or from source
+
+`python setup.py install`
+
+
+### Docs
+Major changes in the v0.1.0 update to the way tokens are handled.  
+You will still need the original authentication instructions, but the TDClient now takes the refresh token and client
+id, not the access token. A new session class handles token expiration and will automatically call a new token as
+needed. 
+
+It is recommended that you store these as environmental variables.  
+
+```
+client_id = os.getenv('TDAMERITRADE_CLIENT_ID')
+account_id = os.getenv('TDAMERITRADE_ACCOUNT_ID')
+refresh_token = os.getenv('TDAMERITRADE_REFRESH_TOKEN')
+
+tdclient = tdameritrade.TDClient(client_id=client_id, refresh_token=refresh_token, account_ids=[account_id])
+``` 
+
+See the tests\test_client.py file for examples on current usage. 
+
+All functionality is available as methods on the `TDClient` object. For most methods, there is a convenience method to return the result as a pandas DataFrame.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/client.png)
+
+Most data fetching methods accept the symbol as argument. For equities, this is just the ticker.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/client/quote.png)
+
+For different assets, utilize the `search` and `instrument` methods to lookup symbols. For options, you can utilize the options method.
+
+![](https://raw.githubusercontent.com/timkpaine/tdameritrade/main/docs/img/options.png)
+
```

### Comparing `tdameritrade-0.1.1/tdameritrade.egg-info/SOURCES.txt` & `tdameritrade-0.2.0/tdameritrade.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tdameritrade/__init__.py
-tdameritrade/_version.py
 tdameritrade/client.py
 tdameritrade/enums.py
 tdameritrade/exceptions.py
 tdameritrade/order.py
 tdameritrade/session.py
 tdameritrade/streaming.py
 tdameritrade/urls.py
```

