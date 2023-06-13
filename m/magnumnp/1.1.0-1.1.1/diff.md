# Comparing `tmp/magnumnp-1.1.0.tar.gz` & `tmp/magnumnp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnumnp-1.1.0.tar", last modified: Wed May 24 18:29:56 2023, max compression
+gzip compressed data, was "magnumnp-1.1.1.tar", last modified: Tue Jun 13 16:00:24 2023, max compression
```

## Comparing `magnumnp-1.1.0.tar` & `magnumnp-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.812390 magnumnp-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-24 18:29:41.000000 magnumnp-1.1.0/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35069 2023-05-24 18:29:41.000000 magnumnp-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7118 2023-05-24 18:29:56.811390 magnumnp-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6625 2023-05-24 18:29:41.000000 magnumnp-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.808390 magnumnp-1.1.0/magnumnp/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.809390 magnumnp-1.1.0/magnumnp/common/
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/decorated_tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/material.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     7251 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/state.py
--rw-rw-rw-   0 root         (0) root         (0)    38962 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/tabulate.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/time_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/common/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.810391 magnumnp-1.1.0/magnumnp/field_terms/
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/anisotropy.py
--rw-rw-rw-   0 root         (0) root         (0)     8459 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demag.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demagPBC.py
--rw-rw-rw-   0 root         (0) root         (0)     6698 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/demag_nonequidistant.py
--rw-rw-rw-   0 root         (0) root         (0)     8592 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/dmi.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/external.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/field_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     6357 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/oersted.py
--rw-rw-rw-   0 root         (0) root         (0)     4936 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/rkky.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/field_terms/spintorque.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.810391 magnumnp-1.1.0/magnumnp/loggers/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7570 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/loggers/scalar_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/solvers/
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/llg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4420 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/rkf45.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_ode.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_odeint.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/ode_solvers/torchdiffeq.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/solvers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.811390 magnumnp-1.1.0/magnumnp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/imaging_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-24 18:29:42.000000 magnumnp-1.1.0/magnumnp/utils/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:29:56.808390 magnumnp-1.1.0/magnumnp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7118 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1420 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 18:29:56.000000 magnumnp-1.1.0/magnumnp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 18:29:56.812390 magnumnp-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-24 18:29:51.000000 magnumnp-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.279124 magnumnp-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-13 16:00:09.000000 magnumnp-1.1.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35069 2023-06-13 16:00:09.000000 magnumnp-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-06-13 16:00:24.278124 magnumnp-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7002 2023-06-13 16:00:09.000000 magnumnp-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.275125 magnumnp-1.1.1/magnumnp/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.276125 magnumnp-1.1.1/magnumnp/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/decorated_tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/material.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/state.py
+-rw-rw-rw-   0 root         (0) root         (0)    38962 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/tabulate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/time_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/common/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.277125 magnumnp-1.1.1/magnumnp/field_terms/
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/anisotropy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8514 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demagPBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6734 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/demag_nonequidistant.py
+-rw-rw-rw-   0 root         (0) root         (0)     8592 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/dmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/external.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/field_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6437 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/oersted.py
+-rw-rw-rw-   0 root         (0) root         (0)     4936 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/rkky.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/rux.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/field_terms/spintorque.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.277125 magnumnp-1.1.1/magnumnp/loggers/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5829 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/loggers/scalar_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/solvers/
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/eigensolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/llg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4420 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/rkf45.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_odeint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/ode_solvers/torchdiffeq.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/solvers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.278124 magnumnp-1.1.1/magnumnp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/imaging_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-13 16:00:09.000000 magnumnp-1.1.1/magnumnp/utils/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:00:24.275125 magnumnp-1.1.1/magnumnp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 16:00:24.000000 magnumnp-1.1.1/magnumnp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 16:00:24.279124 magnumnp-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-06-13 16:00:19.000000 magnumnp-1.1.1/setup.py
```

### Comparing `magnumnp-1.1.0/LICENSE` & `magnumnp-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/PKG-INFO` & `magnumnp-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.0
+Version: 1.1.1
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-magnum.np 1.1.0
-===============
+![magnum.np](logo.png)
 
+magnum.np 1.1.1
+===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
 * Fast FFT Demagnetization-field computation optimized for small memory footprint
 * Fast FFT Oersted-field optimized for small memory footprint
-* Arbitrary Material Parameters variing in space and time
-* Spin-torque model by Zhang and Li, Slonczewski
+* Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
+* Non-Equidistant Mesh for Multilayer Structures
+* Arbitrary Material Parameters varying in space and time
+* Spin-torque model by Zhang and Li
+* Spin-Orbit torque (SOT)
 * Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
-* Seemingless VTK import / export via [pyvista](https://docs.pyvista.org/)
+* Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
 
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
@@ -43,28 +47,31 @@
    * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
    * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
    * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
    * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
    * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
-
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
 
     mkdir venv
     python -m venv venv
     source venv/bin/activate
 
 Finally install a release versions of magnum.np by means of pip:
 
-    pip install magnum.np
+    pip install magnumnp
+
+You can also easily install different versions from private repositories. E.g. use the following command to install the latest version of the main branch:
+
+    pip install git+https://gitlab.com/magnum.np/magnum.np@main
 
 
 ### from source code (gitlab.com)
 More advanced users can also install magnum.np from source code.
 It can be downloaded from https://gitlab.com/magnum.np/magnum.np .
 
 After activating the virtual environment magnum.np can be simply installed using pip. For example
```

### Comparing `magnumnp-1.1.0/README.md` & `magnumnp-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-magnum.np 1.1.0
-===============
+![magnum.np](logo.png)
 
+magnum.np 1.1.1
+===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
 * Fast FFT Demagnetization-field computation optimized for small memory footprint
 * Fast FFT Oersted-field optimized for small memory footprint
-* Arbitrary Material Parameters variing in space and time
-* Spin-torque model by Zhang and Li, Slonczewski
+* Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
+* Non-Equidistant Mesh for Multilayer Structures
+* Arbitrary Material Parameters varying in space and time
+* Spin-torque model by Zhang and Li
+* Spin-Orbit torque (SOT)
 * Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
-* Seemingless VTK import / export via [pyvista](https://docs.pyvista.org/)
+* Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
 
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
@@ -30,28 +34,31 @@
    * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
    * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
    * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
    * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
    * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
-
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
 
     mkdir venv
     python -m venv venv
     source venv/bin/activate
 
 Finally install a release versions of magnum.np by means of pip:
 
-    pip install magnum.np
+    pip install magnumnp
+
+You can also easily install different versions from private repositories. E.g. use the following command to install the latest version of the main branch:
+
+    pip install git+https://gitlab.com/magnum.np/magnum.np@main
 
 
 ### from source code (gitlab.com)
 More advanced users can also install magnum.np from source code.
 It can be downloaded from https://gitlab.com/magnum.np/magnum.np .
 
 After activating the virtual environment magnum.np can be simply installed using pip. For example
```

### Comparing `magnumnp-1.1.0/magnumnp/__init__.py` & `magnumnp-1.1.1/magnumnp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """magnum.np main module"""
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 import magnumnp.common.logging as logging
 import torch
 torch.set_default_dtype(torch.float64)
 
 # monkey patch torch versions < 2.0 or on Windows
 try:
```

### Comparing `magnumnp-1.1.0/magnumnp/common/__init__.py` & `magnumnp-1.1.1/magnumnp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/constants.py` & `magnumnp-1.1.1/magnumnp/common/constants.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/decorated_tensor.py` & `magnumnp-1.1.1/magnumnp/common/decorated_tensor.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/io.py` & `magnumnp-1.1.1/magnumnp/common/io.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/logging.py` & `magnumnp-1.1.1/magnumnp/common/logging.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/material.py` & `magnumnp-1.1.1/magnumnp/common/material.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/mesh.py` & `magnumnp-1.1.1/magnumnp/common/mesh.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/state.py` & `magnumnp-1.1.1/magnumnp/common/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import torch
 import os
 import subprocess
 import numpy as np
 from magnumnp.common import logging, DecoratedTensor, Material
 from magnumnp.common.io import write_vti, write_vtr
 
-__all__ = ["State"]
+__all__ = ["State", "complex_dtype"]
 
 complex_dtype = {
     torch.float: torch.complex,
     torch.float32: torch.complex64,
     torch.float64: torch.complex128
     }
 
@@ -160,18 +160,14 @@
             write_vtr(fields, filename + ".vtr", self)
 
     @property
     def dtype(self):
         return self._dtype
 
     @property
-    def complex_dtype(self):
-        return complex_dtype[self._dtype]
-
-    @property
     def cell_volumes(self):
         return self._cell_volumes
 
 
 
 def get_gpu_with_least_memory():
     if not torch.cuda.is_available():
```

### Comparing `magnumnp-1.1.0/magnumnp/common/tabulate.py` & `magnumnp-1.1.1/magnumnp/common/tabulate.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/time_interpolator.py` & `magnumnp-1.1.1/magnumnp/common/time_interpolator.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/common/timer.py` & `magnumnp-1.1.1/magnumnp/common/timer.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/__init__.py` & `magnumnp-1.1.1/magnumnp/field_terms/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 from magnumnp.field_terms.demagPBC import *
 from magnumnp.field_terms.dmi import *
 from magnumnp.field_terms.exchange import *
 from magnumnp.field_terms.external import *
 from magnumnp.field_terms.field_terms import *
 from magnumnp.field_terms.oersted import *
 from magnumnp.field_terms.rkky import *
+from magnumnp.field_terms.rux import *
 from magnumnp.field_terms.spintorque import *
 
 __all__ = (anisotropy.__all__ +
            demag.__all__ +
            demag_nonequidistant.__all__ +
            demagPBC.__all__ +
            dmi.__all__ +
            exchange.__all__ +
            external.__all__ +
            field_terms.__all__ +
            oersted.__all__ +
+           rux.__all__ +
            rkky.__all__ +
            spintorque.__all__)
```

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/anisotropy.py` & `magnumnp-1.1.1/magnumnp/field_terms/anisotropy.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/demag.py` & `magnumnp-1.1.1/magnumnp/field_terms/demag.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from magnumnp.common import logging, timedmethod, constants, Timer
+from magnumnp.common import logging, timedmethod, constants, Timer, complex_dtype
 from .field_terms import LinearFieldTerm
 import numpy as np
 import torch
 import torch.fft
 from torch import asinh, atan, sqrt, log, abs
 from time import time
 import os
@@ -126,15 +126,15 @@
         return s
 
     def _init_N_component(self, state, perm, func):
         dx = np.array(state.mesh.dx)
         dx /= dx.min() # rescale dx to avoid NaNs when using single precision
 
         shape = self._shape(state)
-        ij = [torch.fft.fftfreq(n,1/n).to(device=state._device) for n in shape] # local indices
+        ij = [torch.fft.fftfreq(n,1/n).to(dtype=state._dtype,device=state._device) for n in shape] # local indices
         ij = torch.meshgrid(*ij,indexing='ij')
         x, y, z = [ij[ind]*dx[ind] for ind in perm]
         Lx = [state.mesh.n[ind]*dx[ind] for ind in perm]
         dx = [dx[ind] for ind in perm]
 
         offsets = [state.arange(-state.mesh.pbc[ind], state.mesh.pbc[ind]+1) for ind in perm] # offset of pseudo PBC images
         offsets = torch.stack(torch.meshgrid(*offsets, indexing="ij"), dim=-1).flatten(end_dim=-2)
@@ -177,17 +177,17 @@
 
         if len(dim) == 0: # single spin   TODO: remove this when torch issue #96518 has been solved
             N = torch.stack([torch.stack(self._N[0], dim=-1),
                              torch.stack(self._N[1], dim=-1),
                              torch.stack(self._N[2], dim=-1)], dim=-1)
             return (N * state.m).sum(dim=-1)
 
-        hx = state.zeros(self._N[0][0].shape, dtype=state.complex_dtype)
-        hy = state.zeros(self._N[0][0].shape, dtype=state.complex_dtype)
-        hz = state.zeros(self._N[0][0].shape, dtype=state.complex_dtype)
+        hx = state.zeros(self._N[0][0].shape, dtype=complex_dtype[state.dtype])
+        hy = state.zeros(self._N[0][0].shape, dtype=complex_dtype[state.dtype])
+        hz = state.zeros(self._N[0][0].shape, dtype=complex_dtype[state.dtype])
         for ax in range(3):
             m_pad_fft1D = torch.fft.rfftn(state.material["Ms"] * state.m[:,:,:,(ax,)], dim = dim, s = s).squeeze(-1)
 
             hx += self._N[0][ax] * m_pad_fft1D
             hy += self._N[1][ax] * m_pad_fft1D
             hz += self._N[2][ax] * m_pad_fft1D
```

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/demagPBC.py` & `magnumnp-1.1.1/magnumnp/field_terms/demagPBC.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/demag_nonequidistant.py` & `magnumnp-1.1.1/magnumnp/field_terms/demag_nonequidistant.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from magnumnp.common import logging, timedmethod, constants, Timer
+from magnumnp.common import logging, timedmethod, constants, Timer, complex_dtype
 from .field_terms import LinearFieldTerm
 from . import demag_f, demag_g
 import numpy as np
 import torch
 from time import time
 import os
 
@@ -121,17 +121,17 @@
         if not hasattr(self, "_N"):
             self._init_N(state)
         dim = [i for i in range(2) if state.mesh.n[i] > 1]
         shape = self._shape(state)
         s = [shape[i] for i in dim]
 
         m_pad_fft = torch.fft.rfftn(state.material["Ms"] * state.m, dim = dim, s = s)
-        hx = state.zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
-        hy = state.zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
-        hz = state.zeros(m_pad_fft.shape[:-1], dtype=state.complex_dtype)
+        hx = state.zeros(m_pad_fft.shape[:-1], dtype=complex_dtype[state.dtype])
+        hy = state.zeros(m_pad_fft.shape[:-1], dtype=complex_dtype[state.dtype])
+        hz = state.zeros(m_pad_fft.shape[:-1], dtype=complex_dtype[state.dtype])
 
         for i_dst in range(state.mesh.n[2]):
             for i_src in range(state.mesh.n[2]):
                 for ax in range(3):
                     hx[:,:,i_src] += self._N[i_src][i_dst][0][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
                     hy[:,:,i_src] += self._N[i_src][i_dst][1][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
                     hz[:,:,i_src] += self._N[i_src][i_dst][2][ax][:,:,0]*m_pad_fft[:,:,i_dst,ax]
```

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/dmi.py` & `magnumnp-1.1.1/magnumnp/field_terms/dmi.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/exchange.py` & `magnumnp-1.1.1/magnumnp/field_terms/exchange.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/external.py` & `magnumnp-1.1.1/magnumnp/field_terms/external.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/field_terms.py` & `magnumnp-1.1.1/magnumnp/field_terms/field_terms.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/oersted.py` & `magnumnp-1.1.1/magnumnp/field_terms/oersted.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from magnumnp.common import logging, timedmethod, constants
+from magnumnp.common import logging, timedmethod, constants, complex_dtype
 from .field_terms import FieldTerm
 import numpy as np
 import torch
 import torch.fft
 from torch import asinh, atan, sqrt, log, abs
 import os
 from time import time
@@ -50,15 +50,14 @@
     res[mask] += (z/6. * x * (z**2 - 3.*y**2) * log(x+R))[mask]
 
     mask = (x**2+z**2).gt(0)
     res[mask] += (z/6. * y * (z**2 - 3.*x**2) * log(y+R))[mask]
 
     return res
 
-
 def dipole_g(points):
     x = points[:,:,:,0]
     y = points[:,:,:,1]
     z = points[:,:,:,2]
 
     R = sqrt(x**2 + y**2 + z**2)
     res = -z/R**3
@@ -112,33 +111,33 @@
 
         return torch.fft.rfftn(Kc, dim = [i for i in range(3) if state.mesh.n[i] > 1])#.real.clone()
 
     def _init_K(self, state):
         dtype = state._dtype
         state._dtype = torch.float64 # always use double precision
         time_kernel = time()
-        Kxy = self._init_K_component(state, [0,1,2], krueger_g, dipole_g).to(dtype=dtype)
-        Kyz = self._init_K_component(state, [1,2,0], krueger_g, dipole_g).to(dtype=dtype)
-        Kxz = self._init_K_component(state, [2,0,1], krueger_g, dipole_g).to(dtype=dtype)
+        Kxy = self._init_K_component(state, [0,1,2], krueger_g, dipole_g).to(dtype=complex_dtype[dtype])
+        Kyz = self._init_K_component(state, [1,2,0], krueger_g, dipole_g).to(dtype=complex_dtype[dtype])
+        Kxz = self._init_K_component(state, [2,0,1], krueger_g, dipole_g).to(dtype=complex_dtype[dtype])
 
         self._K = [[  0., -Kxy, +Kxz],
                    [+Kxy,   0., -Kyz],
                    [-Kxz, +Kyz,   0.]]
 
         logging.info(f"[OERSTED]: Time calculation of oersted kernel = {time() - time_kernel} s")
         state._dtype = dtype # restore dtype
 
     @timedmethod
     def h(self, state):
         if not hasattr(self, "_K"):
             self._init_K(state)
 
-        hx = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
-        hy = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
-        hz = state.zeros(list(self._K[0][1].shape), dtype=state.complex_dtype)
+        hx = state.zeros(list(self._K[0][1].shape), dtype=complex_dtype[state.dtype])
+        hy = state.zeros(list(self._K[0][1].shape), dtype=complex_dtype[state.dtype])
+        hz = state.zeros(list(self._K[0][1].shape), dtype=complex_dtype[state.dtype])
 
         for ax in range(3):
             j_pad_fft1D = torch.fft.rfftn(state.j[:,:,:,ax], dim = [i for i in range(3) if state.mesh.n[i] > 1], s = [2*state.mesh.n[i] for i in range(3) if state.mesh.n[i] > 1])
 
             hx += self._K[0][ax] * j_pad_fft1D
             hy += self._K[1][ax] * j_pad_fft1D
             hz += self._K[2][ax] * j_pad_fft1D
```

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/rkky.py` & `magnumnp-1.1.1/magnumnp/field_terms/rkky.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/field_terms/spintorque.py` & `magnumnp-1.1.1/magnumnp/field_terms/spintorque.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/loggers/__init__.py` & `magnumnp-1.1.1/magnumnp/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/loggers/field_logger.py` & `magnumnp-1.1.1/magnumnp/loggers/field_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 import os
 from magnumnp.common import logging, read_vti
-import xml.etree.cElementTree as ET
 from xml.etree import cElementTree
 from xml.dom import minidom
 from magnumnp.common.io import write_vti
 
 __all__ = ["FieldLogger"]
 
 class FieldLogger(object):
```

### Comparing `magnumnp-1.1.0/magnumnp/loggers/logger.py` & `magnumnp-1.1.1/magnumnp/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/loggers/scalar_logger.py` & `magnumnp-1.1.1/magnumnp/loggers/scalar_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/__init__.py` & `magnumnp-1.1.1/magnumnp/solvers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
+from magnumnp.solvers.eigensolver import *
 from magnumnp.solvers.llg import *
 from magnumnp.solvers.ode_solvers import *
 from magnumnp.solvers.string import *
 
-__all__ = (llg.__all__ +
+__all__ = (eigensolver.__all__ +
+           llg.__all__ +
            ode_solvers.__all__ +
            string.__all__)
```

### Comparing `magnumnp-1.1.0/magnumnp/solvers/llg.py` & `magnumnp-1.1.1/magnumnp/solvers/llg.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/__init__.py` & `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/rkf45.py` & `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/rkf45.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_ode.py` & `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_ode.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/scipy_odeint.py` & `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/scipy_odeint.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/ode_solvers/torchdiffeq.py` & `magnumnp-1.1.1/magnumnp/solvers/ode_solvers/torchdiffeq.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/solvers/string.py` & `magnumnp-1.1.1/magnumnp/solvers/string.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/utils/__init__.py` & `magnumnp-1.1.1/magnumnp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/utils/imaging_tools.py` & `magnumnp-1.1.1/magnumnp/utils/imaging_tools.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp/utils/misc.py` & `magnumnp-1.1.1/magnumnp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.0/magnumnp.egg-info/PKG-INFO` & `magnumnp-1.1.1/magnumnp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.0
+Version: 1.1.1
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-magnum.np 1.1.0
-===============
+![magnum.np](logo.png)
 
+magnum.np 1.1.1
+===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
 * Fast FFT Demagnetization-field computation optimized for small memory footprint
 * Fast FFT Oersted-field optimized for small memory footprint
-* Arbitrary Material Parameters variing in space and time
-* Spin-torque model by Zhang and Li, Slonczewski
+* Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
+* Non-Equidistant Mesh for Multilayer Structures
+* Arbitrary Material Parameters varying in space and time
+* Spin-torque model by Zhang and Li
+* Spin-Orbit torque (SOT)
 * Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
-* Seemingless VTK import / export via [pyvista](https://docs.pyvista.org/)
+* Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
 
 
 Documented Demos:
 -----------------
 Demo scripts for various applications are available in the [demo](demos/README.md) directory.
 
@@ -43,28 +47,31 @@
    * [Spin Orbit Torque](demos/sot/run.ipynb) ([Colab](https://colab.research.google.com/drive/1vfLhEUMGFCfJ-CB1QNKgZtLP6vkjf3hw))
    * [Standard Problem #4](demos/sp4/run.ipynb) ([Colab](https://colab.research.google.com/drive/1UNdTe5y41k_6HrZ7WsNASQSs5viUMzss))
    * [Standard Problem #5](demos/sp5/run.ipynb) ([Colab](https://colab.research.google.com/drive/1AR7ksZUbThvJAn3mTgFKh6ka7dgXbUOb))
    * [Standard Problem Domainwall Pinning](demos/sp_domainwall_pinning/run.ipynb) ([Colab](https://colab.research.google.com/drive/1tMKEFtOfg7NSCGYUONeHLa0nC0AXVGRP))
    * [Standard Problem FMR](demos/sp_FMR/run.ipynb) ([Colab](https://colab.research.google.com/drive/160QXXUkDEpd-GvZyI2PhLIdnSIDRVyG0))
 
 
-
 Installation
 ------------
 
 ### from Python Package Index (PyPi)
 For a clean and independent system, we start with a clean virtual python environment (this step could be omitted, if you would like to install magnum.np the available python environment)
 
     mkdir venv
     python -m venv venv
     source venv/bin/activate
 
 Finally install a release versions of magnum.np by means of pip:
 
-    pip install magnum.np
+    pip install magnumnp
+
+You can also easily install different versions from private repositories. E.g. use the following command to install the latest version of the main branch:
+
+    pip install git+https://gitlab.com/magnum.np/magnum.np@main
 
 
 ### from source code (gitlab.com)
 More advanced users can also install magnum.np from source code.
 It can be downloaded from https://gitlab.com/magnum.np/magnum.np .
 
 After activating the virtual environment magnum.np can be simply installed using pip. For example
```

### Comparing `magnumnp-1.1.0/magnumnp.egg-info/SOURCES.txt` & `magnumnp-1.1.1/magnumnp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 magnumnp/field_terms/demag_nonequidistant.py
 magnumnp/field_terms/dmi.py
 magnumnp/field_terms/exchange.py
 magnumnp/field_terms/external.py
 magnumnp/field_terms/field_terms.py
 magnumnp/field_terms/oersted.py
 magnumnp/field_terms/rkky.py
+magnumnp/field_terms/rux.py
 magnumnp/field_terms/spintorque.py
 magnumnp/loggers/__init__.py
 magnumnp/loggers/field_logger.py
 magnumnp/loggers/logger.py
 magnumnp/loggers/scalar_logger.py
 magnumnp/solvers/__init__.py
+magnumnp/solvers/eigensolver.py
 magnumnp/solvers/llg.py
 magnumnp/solvers/string.py
 magnumnp/solvers/ode_solvers/__init__.py
 magnumnp/solvers/ode_solvers/rkf45.py
 magnumnp/solvers/ode_solvers/scipy_ode.py
 magnumnp/solvers/ode_solvers/scipy_odeint.py
 magnumnp/solvers/ode_solvers/torchdiffeq.py
```

### Comparing `magnumnp-1.1.0/setup.py` & `magnumnp-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='magnumnp',
-      version='v1.1.0',
+      version='v1.1.1',
       description='magnum.np finite-difference package for the solution of micromagnetic problems',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Florian Bruckner',
       author_email='florian.bruckner@univie.ac.at',
       url='http://gitlab.com/magnum.np/magnum.np',
       project_urls = {'Documentation': 'https://magnum.np.gitlab.io/magnum.np/',
```

