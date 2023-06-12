# Comparing `tmp/mindsdb_evaluator-0.0.8.tar.gz` & `tmp/mindsdb_evaluator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsdb_evaluator-0.0.8.tar", max compression
+gzip compressed data, was "mindsdb_evaluator-0.0.9.tar", max compression
```

## Comparing `mindsdb_evaluator-0.0.8.tar` & `mindsdb_evaluator-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35103 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/LICENSE
--rw-r--r--   0        0        0       69 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/README.md
--rw-r--r--   0        0        0      186 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/__init__.py
--rw-r--r--   0        0        0      769 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/__init__.py
--rw-r--r--   0        0        0      714 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/classification.py
--rw-r--r--   0        0        0     3512 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/forecasting.py
--rw-r--r--   0        0        0     4210 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/general.py
--rw-r--r--   0        0        0      763 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/regression.py
--rw-r--r--   0        0        0       69 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/calibration/__init__.py
--rw-r--r--   0        0        0      126 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/mindsdb_evaluator/calibration/ece.py
--rw-r--r--   0        0        0      492 2023-04-19 07:17:29.230107 mindsdb_evaluator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35103 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/README.md
+-rw-r--r--   0        0        0      186 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/__init__.py
+-rw-r--r--   0        0        0      769 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/classification.py
+-rw-r--r--   0        0        0     3512 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/forecasting.py
+-rw-r--r--   0        0        0     4210 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/general.py
+-rw-r--r--   0        0        0      763 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/regression.py
+-rw-r--r--   0        0        0       69 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/calibration/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/mindsdb_evaluator/calibration/ece.py
+-rw-r--r--   0        0        0      494 2023-06-12 22:21:09.090291 mindsdb_evaluator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.9/PKG-INFO
```

### Comparing `mindsdb_evaluator-0.0.8/LICENSE` & `mindsdb_evaluator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/__init__.py` & `mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/classification.py` & `mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/classification.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/forecasting.py` & `mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/forecasting.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/general.py` & `mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/general.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/mindsdb_evaluator/accuracy/regression.py` & `mindsdb_evaluator-0.0.9/mindsdb_evaluator/accuracy/regression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.8/PKG-INFO` & `mindsdb_evaluator-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mindsdb-evaluator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Model evaluation for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dataprep-ml (>=0.0.8,<0.0.9)
+Requires-Dist: dataprep-ml (>=0.0.8)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pandas (>=1,<2)
 Requires-Dist: scikit-learn (>=0.24.2)
-Requires-Dist: type-infer (>=0.0.9,<0.0.10)
+Requires-Dist: type-infer (>=0.0.9)
 Description-Content-Type: text/markdown
 
 # mindsdb_evaluator
 
 Model evaluation for Machine Learning pipelines.
```

