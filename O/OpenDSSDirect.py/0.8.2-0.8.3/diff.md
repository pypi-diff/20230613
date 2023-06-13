# Comparing `tmp/OpenDSSDirect.py-0.8.2.tar.gz` & `tmp/OpenDSSDirect.py-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenDSSDirect.py-0.8.2.tar", last modified: Thu Apr 13 12:26:03 2023, max compression
+gzip compressed data, was "OpenDSSDirect.py-0.8.3.tar", last modified: Tue Jun 13 04:36:53 2023, max compression
```

## Comparing `OpenDSSDirect.py-0.8.2.tar` & `OpenDSSDirect.py-0.8.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/
--rw-r--r--   0 meira     (1000) users      (100)     2442 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/LICENSE
--rw-r--r--   0 meira     (1000) users      (100)      197 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/MANIFEST.in
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/
--rw-r--r--   0 meira     (1000) users      (100)     4022 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/PKG-INFO
--rw-r--r--   0 meira     (1000) users      (100)     2006 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/SOURCES.txt
--rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/dependency_links.txt
--rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/not-zip-safe
--rw-r--r--   0 meira     (1000) users      (100)      124 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/requires.txt
--rw-r--r--   0 meira     (1000) users      (100)       14 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/top_level.txt
--rw-r--r--   0 meira     (1000) users      (100)     4022 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/PKG-INFO
--rw-r--r--   0 meira     (1000) users      (100)     3035 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/README.md
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/docs/
--rw-r--r--   0 meira     (1000) users      (100)      909 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/Makefile
--rw-r--r--   0 meira     (1000) users      (100)     5331 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/conf.py
--rw-r--r--   0 meira     (1000) users      (100)      534 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/index.rst
--rw-r--r--   0 meira     (1000) users      (100)      819 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/make.bat
--rw-r--r--   0 meira     (1000) users      (100)     6968 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/opendssdirect.rst
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/opendssdirect/
--rw-r--r--   0 meira     (1000) users      (100)     2417 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ActiveClass.py
--rw-r--r--   0 meira     (1000) users      (100)     6913 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Basic.py
--rw-r--r--   0 meira     (1000) users      (100)     6752 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Bus.py
--rw-r--r--   0 meira     (1000) users      (100)     5352 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CNData.py
--rw-r--r--   0 meira     (1000) users      (100)     5846 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CapControls.py
--rw-r--r--   0 meira     (1000) users      (100)     3527 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Capacitors.py
--rw-r--r--   0 meira     (1000) users      (100)     8072 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Circuit.py
--rw-r--r--   0 meira     (1000) users      (100)    11293 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CktElement.py
--rw-r--r--   0 meira     (1000) users      (100)     1595 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CmathLib.py
--rw-r--r--   0 meira     (1000) users      (100)     2173 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CtrlQueue.py
--rw-r--r--   0 meira     (1000) users      (100)       88 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSCore.py
--rw-r--r--   0 meira     (1000) users      (100)       28 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSEvents.py
--rw-r--r--   0 meira     (1000) users      (100)      323 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSimComs.py
--rw-r--r--   0 meira     (1000) users      (100)     1053 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Element.py
--rw-r--r--   0 meira     (1000) users      (100)     1855 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Error.py
--rw-r--r--   0 meira     (1000) users      (100)     1209 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Executive.py
--rw-r--r--   0 meira     (1000) users      (100)     4306 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Fuses.py
--rw-r--r--   0 meira     (1000) users      (100)     7672 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Generators.py
--rw-r--r--   0 meira     (1000) users      (100)     2082 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Isource.py
--rw-r--r--   0 meira     (1000) users      (100)     5241 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineCodes.py
--rw-r--r--   0 meira     (1000) users      (100)     5039 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineGeometries.py
--rw-r--r--   0 meira     (1000) users      (100)     2870 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineSpacings.py
--rw-r--r--   0 meira     (1000) users      (100)     9279 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Lines.py
--rw-r--r--   0 meira     (1000) users      (100)     4751 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LoadShape.py
--rw-r--r--   0 meira     (1000) users      (100)    12260 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Loads.py
--rw-r--r--   0 meira     (1000) users      (100)     9461 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Meters.py
--rw-r--r--   0 meira     (1000) users      (100)     5656 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Monitors.py
--rw-r--r--   0 meira     (1000) users      (100)     8426 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/PDElements.py
--rw-r--r--   0 meira     (1000) users      (100)     7270 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/PVsystems.py
--rw-r--r--   0 meira     (1000) users      (100)     2290 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Parallel.py
--rw-r--r--   0 meira     (1000) users      (100)     4475 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Parser.py
--rw-r--r--   0 meira     (1000) users      (100)      601 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Progress.py
--rw-r--r--   0 meira     (1000) users      (100)     1616 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Properties.py
--rw-r--r--   0 meira     (1000) users      (100)     9553 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Reactors.py
--rw-r--r--   0 meira     (1000) users      (100)     4925 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Reclosers.py
--rw-r--r--   0 meira     (1000) users      (100)     2936 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ReduceCkt.py
--rw-r--r--   0 meira     (1000) users      (100)     8295 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/RegControls.py
--rw-r--r--   0 meira     (1000) users      (100)     2713 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Relays.py
--rw-r--r--   0 meira     (1000) users      (100)     5351 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Sensors.py
--rw-r--r--   0 meira     (1000) users      (100)     7573 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Settings.py
--rw-r--r--   0 meira     (1000) users      (100)    13553 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Solution.py
--rw-r--r--   0 meira     (1000) users      (100)     2271 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Storages.py
--rw-r--r--   0 meira     (1000) users      (100)     3823 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/SwtControls.py
--rw-r--r--   0 meira     (1000) users      (100)     5175 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/TSData.py
--rw-r--r--   0 meira     (1000) users      (100)      569 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Text.py
--rw-r--r--   0 meira     (1000) users      (100)     3816 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Topology.py
--rw-r--r--   0 meira     (1000) users      (100)     8186 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Transformers.py
--rw-r--r--   0 meira     (1000) users      (100)     2555 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Vsources.py
--rw-r--r--   0 meira     (1000) users      (100)     3665 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/WireData.py
--rw-r--r--   0 meira     (1000) users      (100)     4036 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/XYCurves.py
--rw-r--r--   0 meira     (1000) users      (100)     3087 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/YMatrix.py
--rw-r--r--   0 meira     (1000) users      (100)     2570 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ZIP.py
--rw-r--r--   0 meira     (1000) users      (100)      883 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/__init__.py
--rw-r--r--   0 meira     (1000) users      (100)      938 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/_utils.py
--rw-r--r--   0 meira     (1000) users      (100)       46 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/_version.py
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/opendssdirect/dss/
--rw-r--r--   0 meira     (1000) users      (100)     1388 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/dss/__init__.py
--rw-r--r--   0 meira     (1000) users      (100)     8286 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/utils.py
--rw-r--r--   0 meira     (1000) users      (100)       38 2023-04-13 12:26:03.605877 OpenDSSDirect.py-0.8.2/setup.cfg
--rw-r--r--   0 meira     (1000) users      (100)     2658 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/setup.py
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/tests/
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/tests/data/
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/tests/data/13Bus/
--rw-r--r--   0 meira     (1000) users      (100)      243 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Node_BusXY.csv
--rw-r--r--   0 meira     (1000) users      (100)     8205 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Nodeckt.dss
--rw-r--r--   0 meira     (1000) users      (100)    11851 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEELineCodes.dss
--rw-r--r--   0 meira     (1000) users      (100)      455 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/test_evaluate_expression.py
--rw-r--r--   0 meira     (1000) users      (100)   175831 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/test_opendssdirect.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/
+-rw-r--r--   0 meira     (1000) users      (100)     2442 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/LICENSE
+-rw-r--r--   0 meira     (1000) users      (100)      197 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/MANIFEST.in
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.864472 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/
+-rw-r--r--   0 meira     (1000) users      (100)     4055 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/PKG-INFO
+-rw-r--r--   0 meira     (1000) users      (100)     2006 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/SOURCES.txt
+-rw-r--r--   0 meira     (1000) users      (100)        1 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/dependency_links.txt
+-rw-r--r--   0 meira     (1000) users      (100)        1 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/not-zip-safe
+-rw-r--r--   0 meira     (1000) users      (100)      130 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/requires.txt
+-rw-r--r--   0 meira     (1000) users      (100)       14 2023-06-13 04:36:53.000000 OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/top_level.txt
+-rw-r--r--   0 meira     (1000) users      (100)     4055 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/PKG-INFO
+-rw-r--r--   0 meira     (1000) users      (100)     3035 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/README.md
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.864472 OpenDSSDirect.py-0.8.3/docs/
+-rw-r--r--   0 meira     (1000) users      (100)      909 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/docs/Makefile
+-rw-r--r--   0 meira     (1000) users      (100)     5331 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/docs/conf.py
+-rw-r--r--   0 meira     (1000) users      (100)      534 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/docs/index.rst
+-rw-r--r--   0 meira     (1000) users      (100)      819 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/docs/make.bat
+-rw-r--r--   0 meira     (1000) users      (100)     6968 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/docs/opendssdirect.rst
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/opendssdirect/
+-rw-r--r--   0 meira     (1000) users      (100)     2417 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/ActiveClass.py
+-rw-r--r--   0 meira     (1000) users      (100)     7216 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Basic.py
+-rw-r--r--   0 meira     (1000) users      (100)     6752 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Bus.py
+-rw-r--r--   0 meira     (1000) users      (100)     5352 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/CNData.py
+-rw-r--r--   0 meira     (1000) users      (100)     5846 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/CapControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     3527 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Capacitors.py
+-rw-r--r--   0 meira     (1000) users      (100)     8072 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Circuit.py
+-rw-r--r--   0 meira     (1000) users      (100)    11317 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/CktElement.py
+-rw-r--r--   0 meira     (1000) users      (100)     1595 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/CmathLib.py
+-rw-r--r--   0 meira     (1000) users      (100)     2173 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/CtrlQueue.py
+-rw-r--r--   0 meira     (1000) users      (100)       88 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/DSSCore.py
+-rw-r--r--   0 meira     (1000) users      (100)       28 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/DSSEvents.py
+-rw-r--r--   0 meira     (1000) users      (100)      323 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/DSSimComs.py
+-rw-r--r--   0 meira     (1000) users      (100)     1053 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Element.py
+-rw-r--r--   0 meira     (1000) users      (100)     2857 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Error.py
+-rw-r--r--   0 meira     (1000) users      (100)     1209 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Executive.py
+-rw-r--r--   0 meira     (1000) users      (100)     4306 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Fuses.py
+-rw-r--r--   0 meira     (1000) users      (100)     7672 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Generators.py
+-rw-r--r--   0 meira     (1000) users      (100)     2082 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Isource.py
+-rw-r--r--   0 meira     (1000) users      (100)     5241 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/LineCodes.py
+-rw-r--r--   0 meira     (1000) users      (100)     5039 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/LineGeometries.py
+-rw-r--r--   0 meira     (1000) users      (100)     2870 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/LineSpacings.py
+-rw-r--r--   0 meira     (1000) users      (100)     9279 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Lines.py
+-rw-r--r--   0 meira     (1000) users      (100)     4751 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/LoadShape.py
+-rw-r--r--   0 meira     (1000) users      (100)    12260 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Loads.py
+-rw-r--r--   0 meira     (1000) users      (100)     9461 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Meters.py
+-rw-r--r--   0 meira     (1000) users      (100)     5656 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Monitors.py
+-rw-r--r--   0 meira     (1000) users      (100)     8426 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/PDElements.py
+-rw-r--r--   0 meira     (1000) users      (100)     7270 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/PVsystems.py
+-rw-r--r--   0 meira     (1000) users      (100)     2290 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Parallel.py
+-rw-r--r--   0 meira     (1000) users      (100)     4475 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Parser.py
+-rw-r--r--   0 meira     (1000) users      (100)      601 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Progress.py
+-rw-r--r--   0 meira     (1000) users      (100)     1616 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Properties.py
+-rw-r--r--   0 meira     (1000) users      (100)     9553 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Reactors.py
+-rw-r--r--   0 meira     (1000) users      (100)     4925 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Reclosers.py
+-rw-r--r--   0 meira     (1000) users      (100)     2936 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/ReduceCkt.py
+-rw-r--r--   0 meira     (1000) users      (100)     8295 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/RegControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     2713 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Relays.py
+-rw-r--r--   0 meira     (1000) users      (100)     5351 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Sensors.py
+-rw-r--r--   0 meira     (1000) users      (100)     7573 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Settings.py
+-rw-r--r--   0 meira     (1000) users      (100)    13553 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Solution.py
+-rw-r--r--   0 meira     (1000) users      (100)     2271 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Storages.py
+-rw-r--r--   0 meira     (1000) users      (100)     3823 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/SwtControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     5175 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/TSData.py
+-rw-r--r--   0 meira     (1000) users      (100)      569 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Text.py
+-rw-r--r--   0 meira     (1000) users      (100)     3816 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Topology.py
+-rw-r--r--   0 meira     (1000) users      (100)     8843 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Transformers.py
+-rw-r--r--   0 meira     (1000) users      (100)     2555 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/Vsources.py
+-rw-r--r--   0 meira     (1000) users      (100)     3665 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/WireData.py
+-rw-r--r--   0 meira     (1000) users      (100)     4036 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/XYCurves.py
+-rw-r--r--   0 meira     (1000) users      (100)     3087 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/YMatrix.py
+-rw-r--r--   0 meira     (1000) users      (100)     2570 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/ZIP.py
+-rw-r--r--   0 meira     (1000) users      (100)      883 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/__init__.py
+-rw-r--r--   0 meira     (1000) users      (100)      918 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/_utils.py
+-rw-r--r--   0 meira     (1000) users      (100)       46 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/_version.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/opendssdirect/dss/
+-rw-r--r--   0 meira     (1000) users      (100)     1388 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/dss/__init__.py
+-rw-r--r--   0 meira     (1000) users      (100)     8286 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/opendssdirect/utils.py
+-rw-r--r--   0 meira     (1000) users      (100)       38 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/setup.cfg
+-rw-r--r--   0 meira     (1000) users      (100)     2697 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/setup.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/tests/
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.860472 OpenDSSDirect.py-0.8.3/tests/data/
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-06-13 04:36:53.872472 OpenDSSDirect.py-0.8.3/tests/data/13Bus/
+-rw-r--r--   0 meira     (1000) users      (100)      243 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/tests/data/13Bus/IEEE13Node_BusXY.csv
+-rw-r--r--   0 meira     (1000) users      (100)     8205 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/tests/data/13Bus/IEEE13Nodeckt.dss
+-rw-r--r--   0 meira     (1000) users      (100)    11851 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/tests/data/13Bus/IEEELineCodes.dss
+-rw-r--r--   0 meira     (1000) users      (100)      455 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/tests/test_evaluate_expression.py
+-rw-r--r--   0 meira     (1000) users      (100)   176569 2023-06-13 04:36:37.000000 OpenDSSDirect.py-0.8.3/tests/test_opendssdirect.py
```

### Comparing `OpenDSSDirect.py-0.8.2/LICENSE` & `OpenDSSDirect.py-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/PKG-INFO` & `OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: OpenDSSDirect.py
-Version: 0.8.2
-Summary: Python direct-mode interface to OpenDSS
+Version: 0.8.3
+Summary: Python direct-mode interface to an alternative implementation of OpenDSS
 Home-page: https://github.com/dss-extensions/OpenDSSDirect.py
 Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: BSD-compatible
 Keywords: OpenDSS,cffi
 Classifier: Development Status :: 4 - Beta
@@ -62,8 +62,8 @@
 If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
 
 ### Thanks
 
 Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
 
 See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
-[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
+[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS-Extensions.
```

### Comparing `OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/SOURCES.txt` & `OpenDSSDirect.py-0.8.3/OpenDSSDirect.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/PKG-INFO` & `OpenDSSDirect.py-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: OpenDSSDirect.py
-Version: 0.8.2
-Summary: Python direct-mode interface to OpenDSS
+Version: 0.8.3
+Summary: Python direct-mode interface to an alternative implementation of OpenDSS
 Home-page: https://github.com/dss-extensions/OpenDSSDirect.py
 Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: BSD-compatible
 Keywords: OpenDSS,cffi
 Classifier: Development Status :: 4 - Beta
@@ -62,8 +62,8 @@
 If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
 
 ### Thanks
 
 Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
 
 See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
-[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
+[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS-Extensions.
```

### Comparing `OpenDSSDirect.py-0.8.2/README.md` & `OpenDSSDirect.py-0.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
 
 ### Thanks
 
 Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
 
 See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
-[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
+[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS-Extensions.
```

### Comparing `OpenDSSDirect.py-0.8.2/docs/Makefile` & `OpenDSSDirect.py-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/docs/conf.py` & `OpenDSSDirect.py-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/docs/index.rst` & `OpenDSSDirect.py-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/docs/make.bat` & `OpenDSSDirect.py-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/docs/opendssdirect.rst` & `OpenDSSDirect.py-0.8.3/docs/opendssdirect.rst`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/ActiveClass.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/ActiveClass.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Basic.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,22 +164,25 @@
 
     **THESE FLAGS ARE GLOBAL, affecting all DSS engines in the process.**
 
     The current bit flags are:
 
     - 0x1 (bit 0): If enabled, don't check for NaNs in the inner solution loop. This can lead to various errors.
         This flag is useful for legacy applications that don't handle OpenDSS API errors properly. Through the 
-        development of DSS Extensions, we noticed this is actually a quite common issue.
+        development of DSS-Extensions, we noticed this is actually a quite common issue.
     - 0x2 (bit 1): Toggle worse precision for certain aspects of the engine. For example, the sequence-to-phase 
         (`As2p`) and sequence-to-phase (`Ap2s`) transform matrices. On DSS C-API, we fill the matrix explicitly
         using higher precision, while numerical inversion of an initially worse precision matrix is used in the 
         official OpenDSS. We will introduce better precision for other aspects of the engine in the future, 
         so this flag can be used to toggle the old/bad values where feasible.
     - 0x4 (bit 2): Toggle some InvControl behavior introduced in OpenDSS 9.6.1.1. It could be a regression 
         but needs further investigation, so we added this flag in the time being.
+    - 0x8 (bit 3): When using "save circuit", the official OpenDSS always includes the "CalcVoltageBases" command
+        in the saved script. We found that it is not always a good idea, so we removed the command (leaving it 
+        commented). Use this flag to enable the command in the saved script.
 
     These flags may change for each version of DSS C-API, but the same value will not be reused. That is,
     when we remove a compatibility flag, it will have no effect but will also not affect anything else
     besides raising an error if the user tries to toggle a flag that was available in a previous version.
 
     We expect to keep a very limited number of flags. Since the flags are more transient than the other
     options/flags, it was preferred to add this generic function instead of a separate function per
```

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Bus.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Bus.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/CNData.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/CNData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/CapControls.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/CapControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Capacitors.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Capacitors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Circuit.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Circuit.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/CktElement.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/CktElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,26 @@
 
 def AllPropertyNames():
     """(read-only) Array containing all property names of the active device."""
     return CheckForError(get_string_array(lib.CktElement_Get_AllPropertyNames))
 
 
 def AllVariableNames():
-    """(read-only) Array of strings listing all the published variable names, if a PCElement. Otherwise, null string."""
+    """
+    Array of strings listing all the published state variable names.
+    Valid only for PCElements.
+    """
     return CheckForError(get_string_array(lib.CktElement_Get_AllVariableNames))
 
 
 def AllVariableValues():
-    """(read-only) Array of doubles. Values of state variables of active element if PC element."""
+    """
+    Array of doubles. Values of state variables of active element if PC element.
+    Valid only for PCElements.
+    """
     return CheckForError(get_float64_array(lib.CktElement_Get_AllVariableValues))
 
 
 def BusNames(*args):
     """
     Array of strings. Get  Bus definitions to which each terminal is connected. 0-based array.
     """
```

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/CmathLib.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/CmathLib.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/CtrlQueue.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/CtrlQueue.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Element.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Element.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Executive.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Executive.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Fuses.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Fuses.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Generators.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Generators.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Isource.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Isource.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/LineCodes.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/LineCodes.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/LineGeometries.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/LineGeometries.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/LineSpacings.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/LineSpacings.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Lines.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Lines.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/LoadShape.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/LoadShape.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Loads.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Loads.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Meters.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Meters.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Monitors.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Monitors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/PDElements.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/PDElements.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/PVsystems.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/PVsystems.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Parallel.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Parallel.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Parser.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Parser.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Progress.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Progress.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Properties.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Properties.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Reactors.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Reactors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Reclosers.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Reclosers.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/ReduceCkt.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/ReduceCkt.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/RegControls.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/RegControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Relays.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Relays.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Sensors.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Sensors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Settings.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Settings.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Solution.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Solution.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Storages.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Storages.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/SwtControls.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/SwtControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/TSData.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/TSData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Text.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Text.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Topology.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Topology.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Transformers.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Transformers.py`

 * *Files 18% similar despite different names*

```diff
@@ -231,25 +231,40 @@
 
     # Setter
     Value, = args
     CheckForError(lib.Transformers_Set_idx(Value))
 
 
 def WdgVoltages():
-    """(read-only) Complex array of voltages for active winding"""
+    """
+    (read-only) Complex array of voltages for active winding
+
+    WARNING: If the transformer has open terminal(s), results may be wrong, i.e. avoid using this
+    in those situations. For more information, see https://github.com/dss-extensions/dss-extensions/issues/24
+    """
     return get_float64_array(lib.Transformers_Get_WdgVoltages)
 
 
 def WdgCurrents():
-    """(read-only) All Winding currents (ph1, wdg1, wdg2,... ph2, wdg1, wdg2 ...)"""
+    """
+    (read-only) All Winding currents (ph1, wdg1, wdg2,... ph2, wdg1, wdg2 ...)
+
+    WARNING: If the transformer has open terminal(s), results may be wrong, i.e. avoid using this
+    in those situations. For more information, see https://github.com/dss-extensions/dss-extensions/issues/24
+    """
     return get_float64_array(lib.Transformers_Get_WdgCurrents)
 
 
 def strWdgCurrents():
-    """(read-only) All winding currents in CSV string form like the WdgCurrents property"""
+    """
+    (read-only) All winding currents in CSV string form like the WdgCurrents property
+
+    WARNING: If the transformer has open terminal(s), results may be wrong, i.e. avoid using this
+    in those situations. For more information, see https://github.com/dss-extensions/dss-extensions/issues/24
+    """
     return get_string(CheckForError(lib.Transformers_Get_strWdgCurrents()))
 
 
 def CoreType(*args):
     """Transformer Core Type: 0=shell;1 = 1-phase; 3= 3-leg; 5= 5-leg"""
     # Getter
     if len(args) == 0:
```

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/Vsources.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/Vsources.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/WireData.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/WireData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/XYCurves.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/XYCurves.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/YMatrix.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/YMatrix.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/ZIP.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/ZIP.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/__init__.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/_utils.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Import dss_python
 import dss as dss_py
 import numpy as np
 import warnings
 
-# Bind to the FFI module instance. This should be refined in a future version,
-# especially after DSS C-API 0.11 is fully released.
+# Bind to the FFI module instance. This should be refined in a future version
 lib = dss_py.prime_api_util.lib
 ffi = dss_py.prime_api_util.ffi
 api_util = dss_py.prime_api_util
 codec = api_util.codec
 CheckForError = dss_py.DSS_GR.CheckForError
 DSSException = dss_py._cffi_api_util.DSSException
+Base = dss_py._cffi_api_util.Base
 
 # Currently, we prefer the functions that return lists (suffix 2)
 # to keep higher compatibility with previous versions of OpenDSSDirect.py.
 
 get_string = api_util.get_string
 get_float64_array = api_util.get_float64_array2
 get_int32_array = api_util.get_int32_array2
```

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/dss/__init__.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/dss/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/opendssdirect/utils.py` & `OpenDSSDirect.py-0.8.3/opendssdirect/utils.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/setup.py` & `OpenDSSDirect.py-0.8.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,25 +32,25 @@
             logger.warning("Unable to run 'pre-commit install'")
         develop.run(self)
 
 
 setup(
     name="OpenDSSDirect.py",
     version=version,
-    description="Python direct-mode interface to OpenDSS",
+    description="Python direct-mode interface to an alternative implementation of OpenDSS",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/dss-extensions/OpenDSSDirect.py",
     download_url="https://github.com/dss-extensions/OpenDSSDirect.py",
     # Author details
     author="Dheepak Krishnamurthy",
     author_email="me@kdheepak.com",
     license="BSD-compatible",
     packages=find_packages(),
-    install_requires=["dss_python==0.14.*"],
+    install_requires=["dss_python>=0.14.3,<0.15"],
     extras_require={
         "extras": ["pandas", "matplotlib", "networkx"],
         "dev": [
             "pytest",
             "pytest-cov",
             "sphinx-rtd-theme",
             "nbsphinx",
```

### Comparing `OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Nodeckt.dss` & `OpenDSSDirect.py-0.8.3/tests/data/13Bus/IEEE13Nodeckt.dss`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEELineCodes.dss` & `OpenDSSDirect.py-0.8.3/tests/data/13Bus/IEEELineCodes.dss`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.2/tests/test_opendssdirect.py` & `OpenDSSDirect.py-0.8.3/tests/test_opendssdirect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
 import pytest as pt
 import os
 import pandas as pd
-from pandas.util.testing import assert_dict_equal
+try:
+    from pandas._testing import assert_dict_equal #TODO: migrate to something else, this is bad
+except:
+    from pandas.util.testing import assert_dict_equal
+
 import numpy as np
 
 current_directory = os.path.dirname(os.path.realpath(__file__))
 PATH_TO_DSS = os.path.abspath(
     os.path.join(current_directory, "./data/13Bus/IEEE13Nodeckt.dss")
 )
 
@@ -4809,14 +4813,16 @@
             "DynOut": {"Storage.631": []},
             "DynamicEq": {"Storage.631": ""},
             "Kp": {"Storage.631": "0.01"},
             "PITol": {"Storage.631": "0"},
             "SafeMode": {"Storage.631": "No"},
             "SafeVoltage": {"Storage.631": "80"},
             "kVDC": {"Storage.631": "8"},
+            "AmpLimit": {"Storage.631": "-1"},
+            "AmpLimitGain": {"Storage.631": "0.8"},
         }
     ).to_dict()
 
     actual_dict = dss.utils.class_to_dataframe("Storage").to_dict()
 
     assert_dict_equal(actual_dict, expected_dict)
 
@@ -5332,7 +5338,24 @@
 
     # Check if the loaded version is correct
     expects_debug = os.environ.get("DSS_EXTENSIONS_DEBUG") == "1"
     if expects_debug:
         assert "DEBUG" in opendssdirect.Basic.Version()
     else:
         assert "DEBUG" not in opendssdirect.Basic.Version()
+
+
+def test_exception_control(dss):
+    # Default behavior
+    assert dss.Error.UseExceptions()
+    with pt.raises(dss.DSSException):
+        dss.Text.Command('this_is_an_invalid_command1')
+
+    # Behavior without exceptions
+    dss.Error.UseExceptions(False)
+    assert not dss.Error.UseExceptions()
+    dss.Text.Command('this_is_an_invalid_command2')
+    # There should be an error code waiting for us...
+    assert dss.Error.Number() != 0
+    # ...but it should be gone after we read it
+    assert dss.Error.Number() == 0
+
```

