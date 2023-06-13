# Comparing `tmp/arize-7.0.3rc0.tar.gz` & `tmp/arize-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.3rc0.tar", last modified: Mon May 15 22:07:52 2023, max compression
+gzip compressed data, was "arize-7.0.4.tar", last modified: Tue Jun 13 00:39:02 2023, max compression
```

## Comparing `arize-7.0.3rc0.tar` & `arize-7.0.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.527830 arize-7.0.3rc0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-04-25 01:01:08.000000 arize-7.0.3rc0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-04-25 01:01:08.000000 arize-7.0.3rc0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-15 22:07:52.528084 arize-7.0.3rc0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-04-25 01:01:08.000000 arize-7.0.3rc0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.418439 arize-7.0.3rc0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    29188 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.430634 arize-7.0.3rc0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.432132 arize-7.0.3rc0/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.463692 arize-7.0.3rc0/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4616 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)      470 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/endpoint.py
--rw-r--r--   0 kiko       (501) staff       (20)     1111 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3956 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/session.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.468454 arize-7.0.3rc0/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)       99 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      552 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.469833 arize-7.0.3rc0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.480971 arize-7.0.3rc0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.482105 arize-7.0.3rc0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.486423 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22990 2023-05-10 19:45:18.000000 arize-7.0.3rc0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.505633 arize-7.0.3rc0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4907 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.509754 arize-7.0.3rc0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    70633 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-05-15 21:55:02.000000 arize-7.0.3rc0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.519537 arize-7.0.3rc0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    22244 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7072 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.422774 arize-7.0.3rc0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      430 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-04-25 01:01:08.000000 arize-7.0.3rc0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1518 2023-05-15 22:07:52.529301 arize-7.0.3rc0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.526852 arize-7.0.3rc0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49432 2023-05-04 18:52:13.000000 arize-7.0.3rc0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-04-25 01:01:08.000000 arize-7.0.3rc0/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.666999 arize-7.0.4/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-12 17:30:40.000000 arize-7.0.4/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-12 17:30:40.000000 arize-7.0.4/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-13 00:39:02.667268 arize-7.0.4/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-12 17:30:40.000000 arize-7.0.4/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.556183 arize-7.0.4/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-13 00:36:59.000000 arize-7.0.4/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    28890 2023-06-12 17:30:40.000000 arize-7.0.4/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-12 17:30:40.000000 arize-7.0.4/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.590385 arize-7.0.4/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-12 17:30:40.000000 arize-7.0.4/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.591889 arize-7.0.4/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.599370 arize-7.0.4/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10306 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)      470 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/endpoint.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1111 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3956 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/core/session.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.606759 arize-7.0.4/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)       99 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      552 2023-06-12 17:30:40.000000 arize-7.0.4/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.608874 arize-7.0.4/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.640738 arize-7.0.4/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.642069 arize-7.0.4/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.645927 arize-7.0.4/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    23005 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.648990 arize-7.0.4/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5058 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.653613 arize-7.0.4/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    69574 2023-06-12 17:30:40.000000 arize-7.0.4/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-12 19:46:43.000000 arize-7.0.4/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.662460 arize-7.0.4/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24227 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-12 17:30:40.000000 arize-7.0.4/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.563788 arize-7.0.4/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12555 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      433 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-13 00:39:02.000000 arize-7.0.4/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-12 17:30:40.000000 arize-7.0.4/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-06-13 00:39:02.669456 arize-7.0.4/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 00:39:02.666134 arize-7.0.4/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49447 2023-06-12 17:30:40.000000 arize-7.0.4/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-12 17:30:40.000000 arize-7.0.4/tests/test_utils.py
```

### Comparing `arize-7.0.3rc0/LICENSE.md` & `arize-7.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/PKG-INFO` & `arize-7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.3rc0
+Version: 7.0.4
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.3rc0/README.md` & `arize-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/api.py` & `arize-7.0.4/arize/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # type: ignore[pb2]
 import concurrent.futures as cf
 import time
 from typing import Dict, Optional, Tuple, Union
 
-import numpy as np
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.constants import (
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
     MIN_PREDICTION_ID_LEN,
@@ -101,17 +100,17 @@
         self._space_key = space_key
         self._timeout = timeout
         self._session = FuturesSession(executor=BoundedExecutor(max_queue_bound, max_workers))
         # Grpc-Metadata prefix is required to pass non-standard md through via grpc-gateway
         self._header = {
             "authorization": api_key,
             "Grpc-Metadata-space": space_key,
-            "Grpc-Metadata-python-version": get_python_version(),
+            "Grpc-Metadata-sdk-language": "python",
+            "Grpc-Metadata-language-version": get_python_version(),
             "Grpc-Metadata-sdk-version": __version__,
-            "Grpc-Metadata-sdk": "py",
         }
         if additional_headers is not None:
             if conflicting_keys := self._header.keys() & additional_headers.keys():
                 raise InvalidAdditionalHeaders(conflicting_keys)
             self._header.update(additional_headers)
 
     def log(
@@ -421,16 +420,14 @@
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
 ):
     if not isinstance(label, (float, int)):
         raise TypeError(
             f"label {label} has type {type(label)}, but must be either float or int for "
             f"ModelTypes.{model_type}"
         )
-    elif label is np.nan:
-        raise ValueError(f"label for ModelTypes.{model_type} cannot be null value")
 
 
 def _validate_categorical_label(
     model_type: ModelTypes,
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
 ):
     is_valid = (
@@ -445,18 +442,14 @@
         )
     )
     if not is_valid:
         raise TypeError(
             f"label {label} has type {type(label)}, but must be str, bool, int, float or Tuple[str, "
             f"float] for ModelTypes.{model_type}"
         )
-    if isinstance(label, tuple) and label[1] is np.nan:
-        raise ValueError(
-            f"Prediction confidence score for ModelTypes.{model_type} cannot be null value"
-        )
 
 
 def _validate_object_detection_label(
     prediction_or_actual: str,
     model_type: ModelTypes,
     label: ObjectDetectionLabel,
     embedding_features: Dict[str, Embedding],
```

### Comparing `arize-7.0.3rc0/arize/bounded_executor.py` & `arize-7.0.4/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/bulk_client.py` & `arize-7.0.4/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/bulk_client_shap.py` & `arize-7.0.4/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/client_shap_values.py` & `arize-7.0.4/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/log_client.py` & `arize-7.0.4/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/log_pandas_dataframe.py` & `arize-7.0.4/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/examples/preproduction_client.py` & `arize-7.0.4/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/exporter/core/query.py` & `arize-7.0.4/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/exporter/core/session.py` & `arize-7.0.4/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/exporter/utils/constants.py` & `arize-7.0.4/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/exporter/utils/schema_parser.py` & `arize-7.0.4/arize/exporter/utils/schema_parser.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/exporter/utils/validation.py` & `arize-7.0.4/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.4/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/base_generators.py` & `arize-7.0.4/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.4/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/errors.py` & `arize-7.0.4/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/models.py` & `arize-7.0.4/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.4/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.4/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.4/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/logger.py` & `arize-7.0.4/arize/pandas/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,17 +463,17 @@
         timeout: Optional[float] = None,
     ) -> requests.Response:
         with open(path, "rb") as f:
             headers = {
                 "authorization": self._api_key,
                 "space": self._space_key,
                 "schema": schema,
-                "python-version": get_python_version(),
+                "sdk-language": "python",
+                "language-version": get_python_version(),
                 "sdk-version": __version__,
-                "sdk": "py",
             }
             headers.update(self._additional_headers)
             if sync:
                 headers["sync"] = "1"
             return requests.post(
                 self._files_uri,
                 timeout=timeout,
```

### Comparing `arize-7.0.3rc0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.4/arize/pandas/surrogate_explainer/mimic.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import string
 from dataclasses import replace
 from typing import Callable, Tuple
 
 import numpy as np
 import pandas as pd
 from arize.pandas.logger import Schema
-from arize.utils.types import CATEGORICAL_MODEL_TYPES, ModelTypes
+from arize.utils.types import CATEGORICAL_MODEL_TYPES, NUMERIC_MODEL_TYPES, ModelTypes
 from interpret_community.mimic.mimic_explainer import LGBMExplainableModel, MimicExplainer
 from sklearn.preprocessing import LabelEncoder
 
 
 class Mimic:
     _testing = False
 
@@ -58,16 +58,18 @@
                     f"prediction scores range from {_min} to {_max}."
                 )
 
             # model func requires 1 positional argument
             def model_func(_):
                 return np.column_stack((1 - y, y))
 
-        elif model_type == ModelTypes.NUMERIC:
+        elif model_type in NUMERIC_MODEL_TYPES:
             y_col_name = schema.prediction_label_column_name
+            if schema.prediction_score_column_name is not None:
+                y_col_name = schema.prediction_score_column_name
             y = df[y_col_name].to_numpy()
 
             _finite_count = np.isfinite(y).sum()
             if len(y) - _finite_count:
                 raise ValueError(
                     f"To calculate surrogate explainability for {model_type}, "
                     f"predictions must not contain NaN or infinite values, but "
```

### Comparing `arize-7.0.3rc0/arize/pandas/validation/errors.py` & `arize-7.0.4/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/pandas/validation/validator.py` & `arize-7.0.4/arize/pandas/validation/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     NUMERIC_MODEL_TYPES,
     EmbeddingColumnNames,
     Environments,
     Metrics,
     ModelTypes,
     Schema,
 )
+from arize.utils.utils import is_delayed_schema
 
 
 class Validator:
     @staticmethod
     def validate_required_checks(
         dataframe: pd.DataFrame,
         model_id: str,
@@ -55,15 +56,15 @@
         metric_families: Optional[List[Metrics]] = None,
         model_version: Optional[str] = None,
         batch_id: Optional[str] = None,
     ) -> List[err.ValidationError]:
         # general checks
         general_checks = chain(
             Validator._check_column_names_for_empty_strings(schema),
-            Validator._check_existence_prediction_id_column_delayed_records(schema),
+            Validator._check_existence_prediction_id_column_delayed_schema(schema),
             Validator._check_invalid_model_id(model_id),
             Validator._check_invalid_model_version(model_version),
             Validator._check_invalid_model_type(model_type),
             Validator._check_invalid_environment(environment),
             Validator._check_invalid_batch_id(batch_id, environment),
             Validator._check_missing_columns(dataframe, schema),
             Validator._check_dataframe_for_duplicate_columns(schema, dataframe),
@@ -331,17 +332,15 @@
                             metric_family.name.lower() for metric_family in metric_families
                         ):
                             # This is a valid combination of model type + metrics.
                             # Now validate that required columns are in the schema.
                             is_valid_combination = True
                             # If no prediction values are present, then delayed actuals are being
                             # logged, and we can't validate required columns.
-                            if (schema.prediction_label_column_name is not None) or (
-                                schema.prediction_score_column_name is not None
-                            ):
+                            if schema.has_prediction_columns():
                                 # This is a list of lists.
                                 # In some cases, either one set of columns OR another set of
                                 # columns is required.
                                 required_columns = (
                                     mapping.get("required_columns").get("arrow").get("required")
                                 )
                                 for column_combination in required_columns:
@@ -356,46 +355,23 @@
                                     else:
                                         break
                 if not is_valid_combination:
                     return False, [], metric_combinations
         return True, missing_columns, []
 
     @staticmethod
-    def _check_existence_prediction_id_column_delayed_records(
+    def _check_existence_prediction_id_column_delayed_schema(
         schema: Schema,
     ) -> List[err.MissingPredictionIdColumnForDelayedRecords]:
         if schema.prediction_id_column_name is not None:
             return []
-        prediction_cols = (
-            schema.prediction_label_column_name,
-            schema.prediction_score_column_name,
-            schema.rank_column_name,
-            schema.prediction_group_id_column_name,
-            schema.object_detection_prediction_column_names,
-        )
-        actual_cols = (
-            schema.actual_label_column_name,
-            schema.actual_score_column_name,
-            schema.relevance_labels_column_name,
-            schema.relevance_score_column_name,
-            schema.object_detection_actual_column_names,
-        )
-        feature_importance_cols = (schema.shap_values_column_names,)
-
-        has_prediction_info = any(col is not None for col in prediction_cols)
-        has_actual_info = any(col is not None for col in actual_cols)
-        has_feature_importance_info = any(col is not None for col in feature_importance_cols)
-
-        is_delayed_record = (
-            has_actual_info or has_feature_importance_info
-        ) and not has_prediction_info
-        if is_delayed_record:
+        if is_delayed_schema(schema):
             return [
                 err.MissingPredictionIdColumnForDelayedRecords(
-                    has_actual_info, has_feature_importance_info
+                    schema.has_actual_columns(), schema.has_feature_importance_columns()
                 )
             ]
         # Warning for when prediction_id is not provided by the user and we generate the default
         # prediction ids
         logger.warning(
             "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
             "if not provided by the user. Please note, you won't be able to send delayed data for "
```

### Comparing `arize-7.0.3rc0/arize/utils/constants.py` & `arize-7.0.4/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/utils/logging.py` & `arize-7.0.4/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/arize/utils/model_mapping.json` & `arize-7.0.4/arize/utils/model_mapping.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'external_model_types'": "{insert: [(3, 'object_detection')]}",*

 * * "'required_columns_map'": "{insert: [(3, OrderedDict([('external_model_type', "*

 * *                           "'object_detection'), ('mappings', [OrderedDict([('metrics', "*

 * *                           "[['classification']]), ('required_columns', OrderedDict([('arrow', "*

 * *                           "OrderedDict([('required', "*

 * *                           "[['object_detection_prediction_column_names']]), ('latent', "*

 * *                           "[['o […]*

```diff
@@ -1,12 +1,13 @@
 {
     "external_model_types": [
         "binary_classification",
         "regression",
-        "ranking"
+        "ranking",
+        "object_detection"
     ],
     "metric_families": [
         "classification",
         "regression",
         "ranking",
         "auc_log_loss",
         "ranking_label"
@@ -388,10 +389,48 @@
                                     "prediction_score"
                                 ]
                             ]
                         }
                     }
                 }
             ]
+        },
+        {
+            "external_model_type": "object_detection",
+            "mappings": [
+                {
+                    "metrics": [
+                        [
+                            "classification"
+                        ]
+                    ],
+                    "required_columns": {
+                        "arrow": {
+                            "latent": [
+                                [
+                                    "object_detection_actual_column_names"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "object_detection_prediction_column_names"
+                                ]
+                            ]
+                        },
+                        "generic": {
+                            "latent": [
+                                [
+                                    "object_detection_actual"
+                                ]
+                            ],
+                            "required": [
+                                [
+                                    "object_detection_prediction"
+                                ]
+                            ]
+                        }
+                    }
+                }
+            ]
         }
     ]
 }
```

### Comparing `arize-7.0.3rc0/arize/utils/types.py` & `arize-7.0.4/arize/utils/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,30 @@
         return any(isinstance(data, t) for t in (list, np.ndarray, pd.Series))
 
 
 class ObjectDetectionColumnNames(NamedTuple):
     bounding_boxes_coordinates_column_name: str
     categories_column_name: str
     scores_column_name: Optional[str] = None
+    """
+    Used to log object detection prediction and actual values that are assigned to the prediction or
+    actual schema parameter.
+
+    Arguments:
+    ----------
+        bounding_boxes_coordinates_column_name (str): Column name containing the coordinates of the
+            rectangular outline that locates an object within an image or video. Pascal VOC format
+            required. The contents of this column must be a List[List[float]].
+        categories_column_name (str): Column name containing the predefined classes or labels used
+            by the model to classify the detected objects. The contents of this column must be List[str].
+        scores_column_names (str, optional): Column name containint the confidence scores that the
+            model assigns to it's predictions, indicating how certain the model is that the predicted
+            class is contained within the bounding box. This argument is only applicable for prediction
+            values. The contents of this column must be List[float].
+    """
 
 
 class ObjectDetectionLabel(NamedTuple):
     bounding_boxes_coordinates: List[List[float]]
     categories: List[str]
     scores: Optional[List[float]] = None  # Actual Object Detection Labels won't have scores
 
@@ -524,13 +540,37 @@
         if self.response_column_names is not None:
             columns_used.add(self.response_column_names.vector_column_name)
             if self.response_column_names.data_column_name is not None:
                 columns_used.add(self.response_column_names.data_column_name)
 
         return columns_used
 
+    def has_prediction_columns(self) -> bool:
+        prediction_cols = (
+            self.prediction_label_column_name,
+            self.prediction_score_column_name,
+            self.rank_column_name,
+            self.prediction_group_id_column_name,
+            self.object_detection_prediction_column_names,
+        )
+        return any(col is not None for col in prediction_cols)
+
+    def has_actual_columns(self) -> bool:
+        actual_cols = (
+            self.actual_label_column_name,
+            self.actual_score_column_name,
+            self.relevance_labels_column_name,
+            self.relevance_score_column_name,
+            self.object_detection_actual_column_names,
+        )
+        return any(col is not None for col in actual_cols)
+
+    def has_feature_importance_columns(self) -> bool:
+        feature_importance_cols = (self.shap_values_column_names,)
+        return any(col is not None for col in feature_importance_cols)
+
 
 T = TypeVar("T", bound=type)
 
 
 def is_list_of(lst: Sequence[object], tp: T) -> bool:
     return isinstance(lst, list) and all(isinstance(x, tp) for x in lst)
```

### Comparing `arize-7.0.3rc0/arize/utils/utils.py` & `arize-7.0.4/arize/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,7 +200,23 @@
             shap_val_col_names = {}
         for k, v in schema2.shap_values_column_names.items():
             shap_val_col_names[k] = v
         # replace embedding column names in schema
         schema = schema.replace(shap_values_column_names=shap_val_col_names)
 
     return schema
+
+
+def is_delayed_schema(schema: Schema) -> bool:
+    """
+    This function checks if the given schema, according to the columns provided by the user,
+    has inherently latent information
+    Args:
+        schema (Schema): The schema to analyze
+
+    Returns:
+        bool: True if the schema is "delayed", i.e., does not possess prediction columns and has actual or
+        feature importance columns.
+    """
+    return (
+        schema.has_actual_columns() or schema.has_feature_importance_columns()
+    ) and not schema.has_prediction_columns()
```

### Comparing `arize-7.0.3rc0/arize.egg-info/PKG-INFO` & `arize-7.0.4/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.3rc0
+Version: 7.0.4
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.3rc0/arize.egg-info/SOURCES.txt` & `arize-7.0.4/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.3rc0/setup.cfg` & `arize-7.0.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	requests_futures==1.0.0
 	googleapis_common_protos~=1.51
-	protobuf~=3.12
+	protobuf>=3.12, <5
 	pandas>=0.25.3,<2
 	pyarrow>=5.0.0
 
 [options.extras_require]
 MimicExplainer = 
 	numpy<1.24.0
 	scikit-learn>=0.12.0,<2
```

### Comparing `arize-7.0.3rc0/tests/test_api.py` & `arize-7.0.4/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1282,17 +1282,17 @@
 def test_instantiating_client_additional_header():
     c = get_stubbed_client({"JWT": "FAKE_VALUE"})
     import arize
 
     expected = {
         "authorization": inputs["api_key"],
         "Grpc-Metadata-space": inputs["space_key"],
+        "Grpc-Metadata-sdk-language": "python",
+        "Grpc-Metadata-language-version": get_python_version(),
         "Grpc-Metadata-sdk-version": arize.__version__,
-        "Grpc-Metadata-python-version": get_python_version(),
-        "Grpc-Metadata-sdk": "py",
         "JWT": "FAKE_VALUE",
     }
     assert c._header == expected
 
 
 if __name__ == "__main__":
     raise SystemExit(pytest.main([__file__]))
```

### Comparing `arize-7.0.3rc0/tests/test_utils.py` & `arize-7.0.4/tests/test_utils.py`

 * *Files identical despite different names*

