# Comparing `tmp/analysetool-0.0.3.tar.gz` & `tmp/analysetool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysetool-0.0.3.tar", last modified: Tue Jun 13 02:35:18 2023, max compression
+gzip compressed data, was "analysetool-0.0.4.tar", last modified: Tue Jun 13 02:36:45 2023, max compression
```

## Comparing `analysetool-0.0.3.tar` & `analysetool-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:18.225740 analysetool-0.0.3/
--rw-rw-rw-   0        0        0       58 2023-06-13 02:35:18.225740 analysetool-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:18.223740 analysetool-0.0.3/analysetool.egg-info/
--rw-rw-rw-   0        0        0       58 2023-06-13 02:35:18.000000 analysetool-0.0.3/analysetool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-13 02:35:18.000000 analysetool-0.0.3/analysetool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 02:35:18.000000 analysetool-0.0.3/analysetool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-13 02:35:18.000000 analysetool-0.0.3/analysetool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 02:35:18.000000 analysetool-0.0.3/analysetool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-06-13 02:35:05.000000 analysetool-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      202 2023-06-13 02:35:18.225740 analysetool-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:18.224740 analysetool-0.0.3/test/
--rw-rw-rw-   0        0        0      303 2023-06-09 01:52:37.000000 analysetool-0.0.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.518129 analysetool-0.0.4/
+-rw-rw-rw-   0        0        0       58 2023-06-13 02:36:45.518129 analysetool-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.501129 analysetool-0.0.4/analysetool.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-06-13 02:36:45.000000 analysetool-0.0.4/analysetool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-13 02:36:45.000000 analysetool-0.0.4/analysetool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 02:36:45.000000 analysetool-0.0.4/analysetool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-13 02:36:45.000000 analysetool-0.0.4/analysetool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 02:36:45.000000 analysetool-0.0.4/analysetool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      278 2023-06-13 02:36:30.000000 analysetool-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      192 2023-06-13 02:36:45.519130 analysetool-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.502129 analysetool-0.0.4/test/
+-rw-rw-rw-   0        0        0      303 2023-06-09 01:52:37.000000 analysetool-0.0.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.503128 analysetool-0.0.4/waterquality/
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.506137 analysetool-0.0.4/waterquality/common/
+-rw-rw-rw-   0        0        0     1825 2023-06-09 01:52:36.000000 analysetool-0.0.4/waterquality/common/DataCleaning.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:52:36.000000 analysetool-0.0.4/waterquality/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.509130 analysetool-0.0.4/waterquality/eemdlstm/
+-rw-rw-rw-   0        0        0     7994 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/eemdlstm/EEMD_LSTM_ZY.py
+-rw-rw-rw-   0        0        0     4199 2023-06-12 11:56:48.000000 analysetool-0.0.4/waterquality/eemdlstm/Predict_ZY.py
+-rw-rw-rw-   0        0        0      113 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/eemdlstm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.511132 analysetool-0.0.4/waterquality/eemdlstm/base/
+-rw-rw-rw-   0        0        0     2646 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/eemdlstm/base/EEMD_LSTM_BASE.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/eemdlstm/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.514130 analysetool-0.0.4/waterquality/loaddata/
+-rw-rw-rw-   0        0        0     2707 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/loaddata/ParserHuiZhouExcelData.py
+-rw-rw-rw-   0        0        0     2659 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/loaddata/Parser_jilonghe_ExcelData.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/loaddata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.516130 analysetool-0.0.4/waterquality/normal/
+-rw-rw-rw-   0        0        0     1233 2023-06-13 02:21:57.000000 analysetool-0.0.4/waterquality/normal/RelativeAnalyse.py
+-rw-rw-rw-   0        0        0       42 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/normal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:36:45.517130 analysetool-0.0.4/waterquality/normal/base/
+-rw-rw-rw-   0        0        0        0 2023-06-09 01:52:37.000000 analysetool-0.0.4/waterquality/normal/base/__init__.py
```

