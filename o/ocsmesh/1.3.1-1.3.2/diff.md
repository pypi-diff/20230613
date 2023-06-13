# Comparing `tmp/ocsmesh-1.3.1.tar.gz` & `tmp/ocsmesh-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsmesh-1.3.1.tar", last modified: Tue May 16 17:28:18 2023, max compression
+gzip compressed data, was "ocsmesh-1.3.2.tar", last modified: Tue Jun 13 16:24:26 2023, max compression
```

## Comparing `ocsmesh-1.3.1.tar` & `ocsmesh-1.3.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.048067 ocsmesh-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.032068 ocsmesh-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.036068 ocsmesh-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.github/workflows/functional_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.github/workflows/functional_test_2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-16 17:28:18.048067 ocsmesh-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.036068 ocsmesh-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/noaa_33879_DS1.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.040068 ocsmesh-1.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/ocsmesh.command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/ocsmesh.geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/ocsmesh.mesh.rst
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/ocsmesh.size_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/ocsmesh.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.040068 ocsmesh-1.3.1/ocsmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.040068 ocsmesh-1.3.1/ocsmesh/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/mesh_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/remesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/remesh_by_shape_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23104 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cli/subset_n_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.040068 ocsmesh-1.3.1/ocsmesh/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/linefeature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/features/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/ocsmesh/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/geom/shapely.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/ocsmesh/hfun/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/hfun/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/ocsmesh/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/ocsmesh/mesh/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/parsers/grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/mesh/parsers/sms2dm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/ocsmesh/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/ops/combine_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/ops/combine_hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    62966 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/ocsmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.040068 ocsmesh-1.3.1/ocsmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-16 17:28:17.000000 ocsmesh-1.3.1/ocsmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-16 17:28:18.000000 ocsmesh-1.3.1/ocsmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:28:17.000000 ocsmesh-1.3.1/ocsmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 17:28:17.000000 ocsmesh-1.3.1/ocsmesh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-16 17:28:17.000000 ocsmesh-1.3.1/ocsmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 17:28:17.000000 ocsmesh-1.3.1/ocsmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:28:18.048067 ocsmesh-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.032068 ocsmesh-1.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.044067 ocsmesh-1.3.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30824 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/hfun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:28:18.048067 ocsmesh-1.3.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/cli/build_geom.sh
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/cli/build_hfun.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 17:28:05.000000 ocsmesh-1.3.1/tests/cli/remesh_by_dem.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.460197 ocsmesh-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/functional_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/functional_test_2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)  2851126 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/noaa_33879_DS1.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.468197 ocsmesh-1.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.mesh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.size_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/ocsmesh.utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.468197 ocsmesh-1.3.2/ocsmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/mesh_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/remesh_by_shape_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23104 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cli/subset_n_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/linefeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/features/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/geom/shapely.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh/hfun/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81400 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59651 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/hfun/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74313 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/mesh/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/mesh/parsers/sms2dm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/ocsmesh/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/combine_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/ops/combine_hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64799 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68014 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/ocsmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.472197 ocsmesh-1.3.2/ocsmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 16:24:26.000000 ocsmesh-1.3.2/ocsmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.464197 ocsmesh-1.3.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30865 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/hfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:24:26.476198 ocsmesh-1.3.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/build_geom.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/build_hfun.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:24:13.000000 ocsmesh-1.3.2/tests/cli/remesh_by_dem.sh
```

### Comparing `ocsmesh-1.3.1/.github/workflows/documentation.yml` & `ocsmesh-1.3.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/.github/workflows/functional_test.yml` & `ocsmesh-1.3.2/.github/workflows/functional_test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name: Python ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
-        python-version: [ '3.8', '3.9', '3.10' ]
+        python-version: [ '3.9', '3.10', '3.11' ]
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Setup Mamba environment for Python
       uses: mamba-org/provision-with-micromamba@main
       with:
```

### Comparing `ocsmesh-1.3.1/.github/workflows/functional_test_2.yml` & `ocsmesh-1.3.2/.github/workflows/functional_test_2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name: Python ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
-        python-version: [ '3.8', '3.9', '3.10' ]
+        python-version: [ '3.9', '3.10', '3.11' ]
 
     steps:
     - name: Checkout 
       uses: actions/checkout@v3
 
     - name: OS binaries
       shell: bash -l {0}
```

### Comparing `ocsmesh-1.3.1/.github/workflows/pylint.yml` & `ocsmesh-1.3.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/.github/workflows/release.yml` & `ocsmesh-1.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/.gitignore` & `ocsmesh-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/.pylintrc` & `ocsmesh-1.3.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/LICENSE` & `ocsmesh-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/PKG-INFO` & `ocsmesh-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
@@ -124,15 +124,15 @@
             Work.
          d. Affirmer understands and acknowledges that Creative Commons is not a
             party to this document and has no duty or obligation with respect to
             this CC0 or use of the Work.
         
 Project-URL: Documentation, https://noaa-ocs-modeling.github.io/OCSMesh/
 Project-URL: Source, https://github.com/noaa-ocs-modeling/OCSMesh/
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: documentation
 License-File: LICENSE
 
 ![lint workflow](https://github.com/noaa-ocs-modeling/OCSMesh/actions/workflows/pylint.yml/badge.svg?branch=main)
 ![fnc workflow](https://github.com/noaa-ocs-modeling/OCSMesh/actions/workflows/functional_test.yml/badge.svg?branch=main)
```

### Comparing `ocsmesh-1.3.1/README.md` & `ocsmesh-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/docs/Makefile` & `ocsmesh-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/docs/make.bat` & `ocsmesh-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/docs/noaa_33879_DS1.pdf` & `ocsmesh-1.3.2/docs/noaa_33879_DS1.pdf`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/docs/source/conf.py` & `ocsmesh-1.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/__init__.py` & `ocsmesh-1.3.2/ocsmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/__main__.py` & `ocsmesh-1.3.2/ocsmesh/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cli/cli.py` & `ocsmesh-1.3.2/ocsmesh/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cli/mesh_upgrader.py` & `ocsmesh-1.3.2/ocsmesh/cli/mesh_upgrader.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cli/remesh.py` & `ocsmesh-1.3.2/ocsmesh/cli/remesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cli/remesh_by_shape_factor.py` & `ocsmesh-1.3.2/ocsmesh/cli/remesh_by_shape_factor.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cli/subset_n_combine.py` & `ocsmesh-1.3.2/ocsmesh/cli/subset_n_combine.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/cmd.py` & `ocsmesh-1.3.2/ocsmesh/cmd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/db.py` & `ocsmesh-1.3.2/ocsmesh/db.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/driver.py` & `ocsmesh-1.3.2/ocsmesh/driver.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/features/channel.py` & `ocsmesh-1.3.2/ocsmesh/features/channel.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/features/constraint.py` & `ocsmesh-1.3.2/ocsmesh/features/constraint.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/features/contour.py` & `ocsmesh-1.3.2/ocsmesh/features/contour.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/features/linefeature.py` & `ocsmesh-1.3.2/ocsmesh/features/linefeature.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/features/patch.py` & `ocsmesh-1.3.2/ocsmesh/features/patch.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/figures.py` & `ocsmesh-1.3.2/ocsmesh/figures.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/base.py` & `ocsmesh-1.3.2/ocsmesh/geom/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/collector.py` & `ocsmesh-1.3.2/ocsmesh/geom/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/geom.py` & `ocsmesh-1.3.2/ocsmesh/geom/geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/mesh.py` & `ocsmesh-1.3.2/ocsmesh/geom/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/raster.py` & `ocsmesh-1.3.2/ocsmesh/geom/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/geom/shapely.py` & `ocsmesh-1.3.2/ocsmesh/geom/shapely.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/hfun/base.py` & `ocsmesh-1.3.2/ocsmesh/hfun/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/hfun/collector.py` & `ocsmesh-1.3.2/ocsmesh/hfun/collector.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/hfun/hfun.py` & `ocsmesh-1.3.2/ocsmesh/hfun/hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/hfun/mesh.py` & `ocsmesh-1.3.2/ocsmesh/hfun/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/hfun/raster.py` & `ocsmesh-1.3.2/ocsmesh/hfun/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/interp.py` & `ocsmesh-1.3.2/ocsmesh/interp.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/mesh/base.py` & `ocsmesh-1.3.2/ocsmesh/mesh/base.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/mesh/mesh.py` & `ocsmesh-1.3.2/ocsmesh/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/mesh/parsers/grd.py` & `ocsmesh-1.3.2/ocsmesh/mesh/parsers/grd.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/mesh/parsers/sms2dm.py` & `ocsmesh-1.3.2/ocsmesh/mesh/parsers/sms2dm.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/ops/combine_geom.py` & `ocsmesh-1.3.2/ocsmesh/ops/combine_geom.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/ops/combine_hfun.py` & `ocsmesh-1.3.2/ocsmesh/ops/combine_hfun.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/raster.py` & `ocsmesh-1.3.2/ocsmesh/raster.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/ocsmesh/utils.py` & `ocsmesh-1.3.2/ocsmesh/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import jigsawpy
 from jigsawpy import jigsaw_msh_t  # type: ignore[import]
 from matplotlib.path import Path  # type: ignore[import]
 import matplotlib.pyplot as plt  # type: ignore[import]
 from matplotlib.tri import Triangulation  # type: ignore[import]
 import numpy as np  # type: ignore[import]
 import numpy.typing as npt
+import rasterio as rio
 from pyproj import CRS, Transformer  # type: ignore[import]
 from scipy.interpolate import (  # type: ignore[import]
     RectBivariateSpline, griddata)
 from scipy import sparse, constants
 from shapely.geometry import ( # type: ignore[import]
         Polygon, MultiPolygon,
         box, GeometryCollection, Point, MultiPoint,
@@ -73,14 +74,63 @@
         # TODO: Keep IDTag?
         setattr(mesh, etype, np.array(
                 [(idx, 0) for idx in elem_new_idx],
                 dtype=getattr(
                     jigsawpy.jigsaw_msh_t, f'{etype.upper()}_t')))
 
 
+def cleanup_duplicates(mesh):
+
+    """Cleanup duplicate nodes and elements
+
+    Notes
+    -----
+    Elements and nodes are duplicate if they fully overlapping (not
+    partially)
+    """
+
+    _, cooidx, coorev = np.unique(
+        mesh.vert2['coord'],
+        axis=0,
+        return_index=True,
+        return_inverse=True
+    )
+    nd_map = {e: i for e, i in enumerate(coorev)}
+    mesh.vert2 = mesh.vert2.take(cooidx, axis=0)
+
+    for etype, otype in MESH_TYPES.items():
+        cnn = getattr(mesh, etype)['index']
+
+        n_node = cnn.shape[1]
+
+        cnn_renu = np.array(
+            [nd_map[i] for i in cnn.flatten()]
+        ).reshape(-1, n_node)
+
+        _, cnnidx = np.unique(
+            np.sort(cnn_renu, axis=1),
+            axis=0,
+            return_index=True
+        )
+        mask = np.zeros(len(cnn_renu), dtype=bool)
+        mask[cnnidx] = True
+        adj_cnn = cnn_renu[mask]
+
+        setattr(
+            mesh,
+            etype,
+            np.array(
+                [(idx, 0) for idx in adj_cnn],
+                dtype=getattr(jigsaw_msh_t, otype)
+            )
+        )
+
+    if len(mesh.value) > 0:
+        mesh.value = mesh.value.take(sorted(cooidx), axis=0)
+
 def put_edge2(mesh):
     tri = Triangulation(
         mesh.vert2['coord'][:, 0],
         mesh.vert2['coord'][:, 1],
         mesh.tria3['index'])
     mesh.edge2 = np.array(
         [(edge, 0) for edge in tri.edges], dtype=jigsaw_msh_t.EDGE2_t)
@@ -379,14 +429,15 @@
             no_op = False
             _sieve_by_mask(mesh, sieve_mask)
 
         if no_op:
             break
 
     cleanup_isolates(mesh)
+    cleanup_duplicates(mesh)
     put_id_tags(mesh)
 
 
 def remesh_small_elements(opts, geom, mesh, hfun):
 
     """
     This function uses all the inputs for a given jigsaw meshing
@@ -752,15 +803,15 @@
     pt_series = gpd.GeoSeries(gpd.points_from_xy(
         mesh.vert2['coord'][:,0], mesh.vert2['coord'][:,1]))
     shp_series = gpd.GeoSeries(shape)
 
     # We need point indices in the shapes, not the shape indices
     # query bulk returns all combination of intersections in case
     # input shape results in multi-row series
-    in_shp_idx = pt_series.sindex.query_bulk(
+    in_shp_idx = pt_series.sindex.query(
             shp_series, predicate="intersects")[1]
 
     in_shp_idx = select_adjacent(mesh, in_shp_idx, num_layers=num_adjacent)
 
     return in_shp_idx
 
 def select_adjacent(mesh, in_indices, num_layers):
@@ -1982,7 +2033,158 @@
     particle_velocity = estimate_particle_velocity_from_depth(depth, wave_amplitude)
     characteristic_velocity_magnitude = (
         particle_velocity + np.sqrt(constants.g * np.abs(depth))
     )
     # For overland where h < nu the characteristic velocity is 2 * sqrt(g*h)
     characteristic_velocity_magnitude[~depth_mask] = 2 * particle_velocity[~depth_mask]
     return characteristic_velocity_magnitude * timestep / element_size
+
+
+def create_rectangle_mesh(
+    nx,
+    ny,
+    holes,
+    x_extent=None,
+    y_extent=None,
+    quads=None,
+):
+    # pylint: disable=W1401
+    """
+    Note:
+        x = x-index
+        y = y-index
+
+        holes or quads count starting at 1 from bottom corner square
+
+        node-index(node-id)
+
+              25(26)             29(30)
+          5     *---*---*---*---*
+                | \ | \ | \ | \ |
+          4     *---*---*---*---*
+                | \ | \ | \ | \ |
+          3     *---*---*---*---*
+                | \ |   | \ | \ |
+          2     *---*---*---*---*
+                | \ | \ | # | \ |
+          1     *---*---*---*---*
+                | \ | \ | \ | \ |
+          0     *---*---*---*---*
+              0(1)               4(5)
+
+                0   1   2   3   4
+    """
+
+    if x_extent is None:
+        x_range = range(nx)
+    else:
+        x_range = np.linspace(x_extent[0], x_extent[1], nx)
+
+    if y_extent is None:
+        y_range = range(ny)
+    else:
+        y_range = np.linspace(y_extent[0], y_extent[1], ny)
+
+    if quads is None:
+        quads = []
+
+    X, Y = np.meshgrid(x_range, y_range)
+    verts = np.array(list(zip(X.ravel(), Y.ravel())))
+    tria3 = []
+    quad4 = []
+    for j in range(ny - 1):
+        for i in range(nx - 1):
+            is_quad = (i + 1) + ((nx-1) * j) in quads
+            is_hole = (i + 1) + ((nx-1) * j) in holes
+            if is_hole:
+                continue
+            if is_quad:
+                quad4.append([
+                    j * nx + i,
+                    j * nx + (i + 1),
+                    (j + 1) * nx + (i + 1),
+                    (j + 1) * nx + i
+                ])
+            else: # is tria
+                tria3.append([j * nx + i, j * nx + (i + 1), (j + 1) * nx + i])
+                tria3.append([j * nx + (i + 1), (j + 1) * nx + (i + 1), (j + 1) * nx + i])
+
+
+
+    # NOTE: Everywhere is above 0 (auto: land) unless modified later
+    vals = np.ones((len(verts), 1)) * 10
+
+    mesh_msht = msht_from_numpy(
+        coordinates=verts,
+        triangles=tria3,
+        quadrilaterals=quad4 if len(quad4) > 0 else None,
+        crs=None
+    )
+
+    # Drop unused verts (e.g. 4 connected holes)
+    cleanup_isolates(mesh_msht)
+    mesh_msht.value = np.array(
+        vals, dtype=jigsaw_msh_t.REALS_t
+    )
+
+    return mesh_msht
+
+
+def raster_from_numpy(
+    filename,
+    data,
+    mgrid,
+    crs=CRS.from_epsg(4326)
+) -> None:
+    x = mgrid[0][:, 0]
+    y = mgrid[1][0, :]
+    res_x = (x[-1] - x[0]) / data.shape[1]
+    res_y = (y[-1] - y[0]) / data.shape[0]
+    # TODO: Mistake in transformation if x and y extent are different?
+    transform = rio.transform.Affine.translation(
+        x[0], y[0]
+    ) * rio.transform.Affine.scale(res_x, res_y)
+    if not isinstance(crs, CRS):
+        crs = CRS.from_user_input(crs)
+
+    with rio.open(
+        filename,
+        'w',
+        driver='GTiff',
+        height=data.shape[0],
+        width=data.shape[1],
+        count=1,
+        dtype=data.dtype,
+        crs=crs,
+        transform=transform,
+    ) as dst:
+        dst.write(data, 1)
+
+
+def msht_from_numpy(
+    coordinates,
+    triangles,
+    quadrilaterals=None,
+    crs=CRS.from_epsg(4326)
+):
+    mesh = jigsaw_msh_t()
+    mesh.mshID = 'euclidean-mesh'
+    mesh.ndims = +2
+    if crs is not None:
+        if not isinstance(crs, CRS):
+            crs = CRS.from_user_input(crs)
+        mesh.crs = crs
+    mesh.vert2 = np.array(
+        [(coord, 0) for coord in coordinates],
+        dtype=jigsaw_msh_t.VERT2_t
+        )
+    mesh.tria3 = np.array(
+        [(index, 0) for index in triangles],
+        dtype=jigsaw_msh_t.TRIA3_t
+        )
+    if quadrilaterals is not None:
+        mesh.quad4 = np.array(
+            [(index, 0) for index in quadrilaterals],
+            dtype=jigsaw_msh_t.QUAD4_t
+            )
+
+    return mesh
```

### Comparing `ocsmesh-1.3.1/ocsmesh.egg-info/PKG-INFO` & `ocsmesh-1.3.2/ocsmesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsmesh
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package to generate computational unstructured meshes from planetary modeling.
 Author-email: Jaime R Calzada <jreniel@gmail.com>, Soroosh Mani <soroosh.mani@noaa.gov>
 Maintainer-email: Soroosh Mani <soroosh.mani@noaa.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
@@ -124,15 +124,15 @@
             Work.
          d. Affirmer understands and acknowledges that Creative Commons is not a
             party to this document and has no duty or obligation with respect to
             this CC0 or use of the Work.
         
 Project-URL: Documentation, https://noaa-ocs-modeling.github.io/OCSMesh/
 Project-URL: Source, https://github.com/noaa-ocs-modeling/OCSMesh/
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: documentation
 License-File: LICENSE
 
 ![lint workflow](https://github.com/noaa-ocs-modeling/OCSMesh/actions/workflows/pylint.yml/badge.svg?branch=main)
 ![fnc workflow](https://github.com/noaa-ocs-modeling/OCSMesh/actions/workflows/functional_test.yml/badge.svg?branch=main)
```

### Comparing `ocsmesh-1.3.1/ocsmesh.egg-info/SOURCES.txt` & `ocsmesh-1.3.2/ocsmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/pyproject.toml` & `ocsmesh-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 maintainers = [
     {name = "Soroosh Mani", email = "soroosh.mani@noaa.gov"}
 ]
 description = "Package to generate computational unstructured meshes from planetary modeling."
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = '>=3.8, <3.11' # 3.11 no supported by numba
+requires-python = '>=3.9' # 3.8 not supported by scipy
 dependencies = [
     "colored-traceback", "fiona", "geoalchemy2", "geopandas",
     "jigsawpy", "matplotlib", "netCDF4", "numba",
     "numpy>=1.21", # introduce npt.NDArray
     "pyarrow", "rtree", "pyproj>=3.0", "rasterio", "requests", "scipy",
     "shapely", "tqdm", "typing_extensions", "utm",
     ]
```

### Comparing `ocsmesh-1.3.1/setup.py` & `ocsmesh-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/tests/api/driver.py` & `ocsmesh-1.3.2/tests/api/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import rasterio as rio
 import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
-    raster_from_numpy,
-    create_rectangle_mesh,
     topo_2rast_1mesh,
 )
 
 
 class Driver(unittest.TestCase):
 
     def setUp(self):
```

### Comparing `ocsmesh-1.3.1/tests/api/features.py` & `ocsmesh-1.3.2/tests/api/features.py`

 * *Files identical despite different names*

### Comparing `ocsmesh-1.3.1/tests/api/geom.py` & `ocsmesh-1.3.2/tests/api/geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import rasterio as rio
 import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
-    raster_from_numpy,
-    create_rectangle_mesh,
     topo_2rast_1mesh,
 )
 
 
 class GeomType(unittest.TestCase):
     def setUp(self):
         self.tdir = Path(tempfile.mkdtemp())
@@ -28,19 +26,19 @@
         self.rast = self.tdir / 'rast_1.tif'
         self.mesh = self.tdir / 'mesh_1.gr3'
 
         rast_xy = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
         rast_xy = np.mgrid[0:1.1:0.1, -0.7:0.1:0.1]
         rast_z = np.ones_like(rast_xy[0]) * 10
 
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast, rast_z, rast_xy, 4326
         )
 
-        msh_t = create_rectangle_mesh(
+        msh_t = ocsmesh.utils.create_rectangle_mesh(
             nx=17, ny=7, holes=[40, 41], x_extent=(-1, 1), y_extent=(0, 1))
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 'ignore', category=UserWarning, message='Input mesh has no CRS information'
             )
             mesh = ocsmesh.Mesh(msh_t)
```

### Comparing `ocsmesh-1.3.1/tests/api/hfun.py` & `ocsmesh-1.3.2/tests/api/hfun.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 import rasterio as rio
 import requests
 from shapely import geometry
 
 import ocsmesh
 
 from tests.api.common import (
-    raster_from_numpy,
-    msht_from_numpy,
-    create_rectangle_mesh,
     topo_2rast_1mesh,
 )
 
 
 class SizeFunctionType(unittest.TestCase):
     def setUp(self):
         self.tdir = Path(tempfile.mkdtemp())
@@ -30,19 +27,19 @@
         self.rast = self.tdir / 'rast_1.tif'
         self.mesh = self.tdir / 'mesh_1.gr3'
 
         rast_xy = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
         rast_xy = np.mgrid[0:1.1:0.1, -0.7:0.1:0.1]
         rast_z = np.ones_like(rast_xy[0])
 
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast, rast_z, rast_xy, 4326
         )
 
-        msh_t = create_rectangle_mesh(
+        msh_t = ocsmesh.utils.create_rectangle_mesh(
             nx=17, ny=7, holes=[40, 41], x_extent=(-1, 1), y_extent=(0, 1))
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 'ignore', category=UserWarning, message='Input mesh has no CRS information'
             )
             mesh = ocsmesh.Mesh(msh_t)
@@ -625,18 +622,18 @@
         self.feat1 = self.tdir / 'feature_1'
         self.feat2 = self.tdir / 'feature_2'
 
         rast_xy_1 = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
         rast_xy_2 = np.mgrid[0:1.1:0.1, -0.7:0.1:0.1]
         rast_z_1 = np.ones_like(rast_xy_1[0])
 
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast1, rast_z_1, rast_xy_1, 4326
         )
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast2, rast_z_1, rast_xy_2, 4326
         )
 
         crd = np.array([
             [-1, 0],
             [-0.1, 0],
             [-0.5, 0.2],
@@ -652,15 +649,15 @@
             [2, 1, 3],
             [2, 3, 5],
             [2, 6, 7],
             [2, 7, 5],
             [0, 2, 6],
             [5, 4, 7],
         ])
-        msh_t = msht_from_numpy(crd, tria, crs=4326)
+        msh_t = ocsmesh.utils.msht_from_numpy(crd, tria, crs=4326)
         mesh = ocsmesh.Mesh(msh_t)
         mesh.write(str(self.mesh1), format='grd', overwrite=False)
 
         self.shape1 = geometry.LineString([
             [-1, 0], [1, 0]
         ])
 
@@ -834,22 +831,22 @@
         self.rast2 = self.tdir / 'rast_2.tif'
         self.mesh1 = self.tdir / 'mesh_1.gr3'
 
         rast_xy_1 = np.mgrid[-1:0.1:0.1, -0.7:0.1:0.1]
         rast_xy_2 = np.mgrid[0:1.1:0.1, -0.7:0.1:0.1]
         rast_z_1 = np.ones_like(rast_xy_1[0])
 
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast1, rast_z_1, rast_xy_1, 4326
         )
-        raster_from_numpy(
+        ocsmesh.utils.raster_from_numpy(
             self.rast2, rast_z_1, rast_xy_2, 4326
         )
 
-        msh_t = create_rectangle_mesh(
+        msh_t = ocsmesh.utils.create_rectangle_mesh(
             nx=17, ny=7, holes=[40, 41], x_extent=(-1, 1), y_extent=(0, 1))
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 'ignore', category=UserWarning, message='Input mesh has no CRS information'
             )
             mesh = ocsmesh.Mesh(msh_t)
```

### Comparing `ocsmesh-1.3.1/tests/api/mesh.py` & `ocsmesh-1.3.2/tests/api/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import warnings
 from pathlib import Path
 
 import numpy as np
 from jigsawpy import jigsaw_msh_t
 from shapely import geometry
 
+from ocsmesh import utils
 from ocsmesh.mesh.mesh import Mesh
 
-from tests.api.common import create_rectangle_mesh
 
 
 def edge_at (x, y):
     return geometry.Point(x, y).buffer(0.05)
 
 class BoundaryExtraction(unittest.TestCase):
 
@@ -40,15 +40,15 @@
           0     *---*---*---*---*
               0(1)               4(5)
 
                 0   1   2   3   4
         """
 
         # x and y coords are the same as index (in value)
-        mesh_msht = create_rectangle_mesh(nx=5, ny=6, holes=[10])
+        mesh_msht = utils.create_rectangle_mesh(nx=5, ny=6, holes=[10])
 
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 'ignore', category=UserWarning, message='Input mesh has no CRS information'
             )
 
             self.mesh = Mesh(mesh_msht)
```

