# Comparing `tmp/kedro-datasets-1.4.0.tar.gz` & `tmp/kedro-datasets-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.4.0.tar", last modified: Wed May 31 12:03:29 2023, max compression
+gzip compressed data, was "kedro-datasets-1.4.1.tar", last modified: Tue Jun 13 16:50:01 2023, max compression
```

## Comparing `kedro-datasets-1.4.0.tar` & `kedro-datasets-1.4.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.122067 kedro-datasets-1.4.0/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.126067 kedro-datasets-1.4.0/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:03:29.118067 kedro-datasets-1.4.0/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 12:03:29.000000 kedro-datasets-1.4.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:03:29.130067 kedro-datasets-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-31 12:03:17.000000 kedro-datasets-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.935040 kedro-datasets-1.4.1/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16973 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.943040 kedro-datasets-1.4.1/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:01.939040 kedro-datasets-1.4.1/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 16:50:01.000000 kedro-datasets-1.4.1/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:50:01.947040 kedro-datasets-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-13 16:49:50.000000 kedro-datasets-1.4.1/setup.py
```

### Comparing `kedro-datasets-1.4.0/PKG-INFO` & `kedro-datasets-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.4.0
+Version: 1.4.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
@@ -14,14 +14,15 @@
 Provides-Extra: dask
 Provides-Extra: databricks
 Provides-Extra: geopandas
 Provides-Extra: holoviews
 Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
+Provides-Extra: pickle
 Provides-Extra: pillow
 Provides-Extra: plotly
 Provides-Extra: polars
 Provides-Extra: redis
 Provides-Extra: snowflake
 Provides-Extra: spark
 Provides-Extra: svmlight
@@ -44,14 +45,15 @@
 Provides-Extra: pandas.HDFDataSet
 Provides-Extra: pandas.JSONDataSet
 Provides-Extra: pandas.ParquetDataSet
 Provides-Extra: pandas.SQLTableDataSet
 Provides-Extra: pandas.SQLQueryDataSet
 Provides-Extra: pandas.XMLDataSet
 Provides-Extra: pandas.GenericDataSet
+Provides-Extra: pickle.PickleDataSet
 Provides-Extra: pillow.ImageDataSet
 Provides-Extra: plotly.PlotlyDataSet
 Provides-Extra: plotly.JSONDataSet
 Provides-Extra: polars.CSVDataSet
 Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: spark.SparkDataSet
 Provides-Extra: spark.SparkHiveDataSet
```

### Comparing `kedro-datasets-1.4.0/README.md` & `kedro-datasets-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/api/api_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/api/api_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/email/message_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.4.1/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.4.1/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/__init__.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/gbq_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/hdf_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pickle/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/polars/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/redis/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/__init__.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/spark/spark_streaming_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.4.1/kedro_datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-1.4.1/kedro_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 1.4.0
+Version: 1.4.1
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: <3.11,>=3.7
@@ -14,14 +14,15 @@
 Provides-Extra: dask
 Provides-Extra: databricks
 Provides-Extra: geopandas
 Provides-Extra: holoviews
 Provides-Extra: matplotlib
 Provides-Extra: networkx
 Provides-Extra: pandas
+Provides-Extra: pickle
 Provides-Extra: pillow
 Provides-Extra: plotly
 Provides-Extra: polars
 Provides-Extra: redis
 Provides-Extra: snowflake
 Provides-Extra: spark
 Provides-Extra: svmlight
@@ -44,14 +45,15 @@
 Provides-Extra: pandas.HDFDataSet
 Provides-Extra: pandas.JSONDataSet
 Provides-Extra: pandas.ParquetDataSet
 Provides-Extra: pandas.SQLTableDataSet
 Provides-Extra: pandas.SQLQueryDataSet
 Provides-Extra: pandas.XMLDataSet
 Provides-Extra: pandas.GenericDataSet
+Provides-Extra: pickle.PickleDataSet
 Provides-Extra: pillow.ImageDataSet
 Provides-Extra: plotly.PlotlyDataSet
 Provides-Extra: plotly.JSONDataSet
 Provides-Extra: polars.CSVDataSet
 Provides-Extra: snowflake.SnowparkTableDataSet
 Provides-Extra: spark.SparkDataSet
 Provides-Extra: spark.SparkHiveDataSet
```

### Comparing `kedro-datasets-1.4.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.4.1/kedro_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/kedro_datasets.egg-info/requires.txt` & `kedro-datasets-1.4.1/kedro_datasets.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 kedro>=0.16
 
 [all]
 Pillow~=9.0
 PyYAML<7.0,>=4.2
 SQLAlchemy<3.0,>=1.4
 biopython~=1.73
+compress-pickle[lz4]~=2.1.0
 dask[complete]~=2021.10
 delta-spark<3.0,>=1.0
 delta-spark~=1.2.1
 geopandas<1.0,>=0.6.0
 hdfs<3.0,>=2.5.8
 holoviews~=1.13.0
 lxml~=4.6
@@ -173,14 +174,20 @@
 
 [pandas:platform_system != "Windows"]
 tables~=3.6
 
 [pandas:platform_system == "Windows"]
 tables~=3.6.0
 
+[pickle]
+compress-pickle[lz4]~=2.1.0
+
+[pickle.PickleDataSet]
+compress-pickle[lz4]~=2.1.0
+
 [pillow]
 Pillow~=9.0
 
 [pillow.ImageDataSet]
 Pillow~=9.0
 
 [plotly]
```

### Comparing `kedro-datasets-1.4.0/pyproject.toml` & `kedro-datasets-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.0/setup.py` & `kedro-datasets-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 def _collect_requirements(requires):
     return sorted(set(chain.from_iterable(requires.values())))
 
 
 api_require = {"api.APIDataSet": ["requests~=2.20"]}
 biosequence_require = {"biosequence.BioSequenceDataSet": ["biopython~=1.73"]}
-dask_require = {"dask.ParquetDataSet": ["dask[complete]~=2021.10", "triad>=0.6.7, <1.0"]}
-databricks_require = {
-    "databricks.ManagedTableDataSet": [SPARK, PANDAS, DELTA]
+dask_require = {
+    "dask.ParquetDataSet": ["dask[complete]~=2021.10", "triad>=0.6.7, <1.0"]
 }
+databricks_require = {"databricks.ManagedTableDataSet": [SPARK, PANDAS, DELTA]}
 geopandas_require = {
     "geopandas.GeoJSONDataSet": ["geopandas>=0.6.0, <1.0", "pyproj~=3.0"]
 }
 holoviews_require = {"holoviews.HoloviewsWriter": ["holoviews~=1.13.0"]}
 matplotlib_require = {"matplotlib.MatplotlibWriter": ["matplotlib>=3.0.3, <4.0"]}
 networkx_require = {"networkx.NetworkXDataSet": ["networkx~=2.4"]}
 pandas_require = {
@@ -41,22 +41,21 @@
     "pandas.JSONDataSet": [PANDAS],
     "pandas.ParquetDataSet": [PANDAS, "pyarrow>=6.0"],
     "pandas.SQLTableDataSet": [PANDAS, "SQLAlchemy>=1.4, <3.0"],
     "pandas.SQLQueryDataSet": [PANDAS, "SQLAlchemy>=1.4, <3.0", "pyodbc~=4.0"],
     "pandas.XMLDataSet": [PANDAS, "lxml~=4.6"],
     "pandas.GenericDataSet": [PANDAS],
 }
+pickle_require = {"pickle.PickleDataSet": ["compress-pickle[lz4]~=2.1.0"]}
 pillow_require = {"pillow.ImageDataSet": ["Pillow~=9.0"]}
 plotly_require = {
     "plotly.PlotlyDataSet": [PANDAS, "plotly>=4.8.0, <6.0"],
     "plotly.JSONDataSet": ["plotly>=4.8.0, <6.0"],
 }
-polars_require = {
-    "polars.CSVDataSet": [POLARS]
-}
+polars_require = {"polars.CSVDataSet": [POLARS]}
 redis_require = {"redis.PickleDataSet": ["redis~=4.1"]}
 snowflake_require = {
     "snowflake.SnowparkTableDataSet": [
         "snowflake-snowpark-python~=1.0.0",
         "pyarrow~=8.0",
     ]
 }
@@ -85,14 +84,15 @@
     "dask": _collect_requirements(dask_require),
     "databricks": _collect_requirements(databricks_require),
     "geopandas": _collect_requirements(geopandas_require),
     "holoviews": _collect_requirements(holoviews_require),
     "matplotlib": _collect_requirements(matplotlib_require),
     "networkx": _collect_requirements(networkx_require),
     "pandas": _collect_requirements(pandas_require),
+    "pickle": _collect_requirements(pickle_require),
     "pillow": _collect_requirements(pillow_require),
     "plotly": _collect_requirements(plotly_require),
     "polars": _collect_requirements(polars_require),
     "redis": _collect_requirements(redis_require),
     "snowflake": _collect_requirements(snowflake_require),
     "spark": _collect_requirements(spark_require),
     "svmlight": _collect_requirements(svmlight_require),
@@ -104,14 +104,15 @@
     **dask_require,
     **databricks_require,
     **geopandas_require,
     **holoviews_require,
     **matplotlib_require,
     **networkx_require,
     **pandas_require,
+    **pickle_require,
     **pillow_require,
     **plotly_require,
     **polars_require,
     **snowflake_require,
     **spark_require,
     **svmlight_require,
     **tensorflow_require,
```

