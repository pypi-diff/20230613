# Comparing `tmp/oracle_ads-2.8.5.tar.gz` & `tmp/oracle_ads-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracle_ads-2.8.5.tar", last modified: Wed May 17 18:39:08 2023, max compression
+gzip compressed data, was "oracle_ads-2.8.6.tar", last modified: Tue Jun 13 19:39:48 2023, max compression
```

## Comparing `oracle_ads-2.8.5.tar` & `oracle_ads-2.8.6.tar`

### file list

```diff
@@ -1,533 +1,532 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/THIRD_PARTY_LICENSES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/ads
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/ads_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/automl/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/bds/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/bds/big_data_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.134277 oracle_ads-2.8.5/ads/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/catalog/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/artifact/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35972 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/card_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/argument_to_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/runtime_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/decorator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/dsc_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/extended_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/common/function/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/fn_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/function/func_conf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_artifact_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_export_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/object_storage_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_datascience.py
--rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/oci_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    46073 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/common/word_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/data_labeling_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/loader/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/mixin/data_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/dls_record_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/export_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/parser/export_record_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/dls_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/export_record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/jsonl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/metadata_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/reader/record_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/data_labeling/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/data_labeling/visualizer/text_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.138278 oracle_ads-2.8.5/ads/database/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/database/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65402 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataflow/dataflowsummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/correlation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dask_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataframe_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    72309 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/dataset_with_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/feature_engineering_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/forecasting_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/label_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dataset/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/mixin/dataset_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/recommendation_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/regression_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/sampled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dataset/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/dbmixin/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dbmixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/dbmixin/db_pandas_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/environment/ml_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/evaluations/
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/evaluation_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/evaluations/statistical_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.142278 oracle_ads-2.8.5/ads/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/base_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_global_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_local_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/explanations/mlx_whatif_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/dataframe_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/accessor/series_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsimage/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/image_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsimage/interface/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/oci_language/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/oci_language/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/adsstring/string/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/adsstring/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/data_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.146278 oracle_ads-2.8.5/ads/feature_engineering/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/dataset/zip_code_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/oci_language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/creditcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v6.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/lat_long.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type/zip_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/feature_type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/feature_engineering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.150278 oracle_ads-2.8.5/ads/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/ads_search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/search_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/tuner_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/hpo/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_intermediate_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_parallel_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/hpo/visualization/_param_importances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/ads_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35717 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    59213 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/infrastructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/builders/runtimes/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/container_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/builders/runtimes/python_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/env_var_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/infrastructure_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/job_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/runtime_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/schema/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.154278 oracle_ads-2.8.5/ads/jobs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_oci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_python.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/templates/driver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/jobs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/artifact_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/base_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/.model-ignore
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/datascience_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/deployment/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    60718 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/deployment/model_deployment_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.158278 oracle_ads-2.8.5/ads/model/extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/automl_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/huggingface_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/keras_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/lightgbm_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/model_info_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/model_info_extractor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/pytorch_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/sklearn_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/spark_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/tensorflow_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/extractor/xgboost_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/automl_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/huggingface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/lightgbm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/tensorflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/framework/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   131281 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/generic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_metadata_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/env_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/model_deployment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/model_provenance_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/runtime_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/runtime/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/inference_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/model_provenance_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/schemas/training_env_info_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/serde/model_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/service/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21239 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/service/oci_datascience_model_version_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/model/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/model/transformer/onnx_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/mysqldb/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/mysqldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/mysqldb/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/opctl/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.162278 oracle_ads-2.8.5/ads/opctl/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_ml_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/ads_model_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/manifest_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/multipart_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/conda/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/diagnostics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/versioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/check_distributed_job_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/check_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/diagnostics/requirement_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/distributed/common/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_cluster_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_framework_spec_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_provider_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/distributed/common/framework_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.gpu
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job.gpu
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/cuda.repo
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/docker/merge_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/model/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/model/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.166278 oracle_ads-2.8.5/ads/opctl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/spark/cmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/opctl/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/templates/diagnostic_report_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/opctl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/oracledb/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/oracledb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/oracledb/oracle_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/ads_pipeline_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/pipeline/visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/pipeline/visualizer/text_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/big_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/oracledb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/secrets/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/telemetry/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.170279 oracle_ads-2.8.5/ads/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/dataflow_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/dataflow_sparksql.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/func.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score-pkl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_generic.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_huggingface_pipeline.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_lightgbm.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_onnx.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_onnx_new.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_oracle_automl.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_pyspark.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_pytorch.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_scikit-learn.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_tensorflow.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/templates/score_xgboost.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/text_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/udfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/text_dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/type_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/abstract_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/constant_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/continuous_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/credit_card_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/datetime_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/discrete_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/document_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/ip_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/latlon_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/phone_number_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/type_discovery_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/typed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/unknown_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/type_discovery/zipcode_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/ads/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-17 18:39:04.000000 oracle_ads-2.8.5/ads/vault/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/oracle_ads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:39:08.000000 oracle_ads-2.8.5/oracle_ads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 18:39:08.174279 oracle_ads-2.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-17 18:39:05.000000 oracle_ads-2.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50466 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/THIRD_PARTY_LICENSES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.871756 oracle_ads-2.8.6/ads/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/ads_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.875756 oracle_ads-2.8.6/ads/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/automl/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35984 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/automl/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.875756 oracle_ads-2.8.6/ads/bds/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/bds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/bds/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/bds/big_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.875756 oracle_ads-2.8.6/ads/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60039 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/catalog/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/catalog/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/catalog/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/catalog/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/common/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/artifact/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35972 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/card_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20253 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/common/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/decorator/argument_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/decorator/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/decorator/runtime_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/decorator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/dsc_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/extended_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/common/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/function/fn_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/function/func_conf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27269 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72294 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/model_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/model_artifact_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/model_export_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/object_storage_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/oci_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/oci_datascience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42155 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/oci_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37213 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/oci_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/oci_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16565 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46073 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/common/word_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/data_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/data_labeling_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/data_labeling/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/interface/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/interface/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/data_labeling/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/loader/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/data_labeling/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/mixin/data_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.879756 oracle_ads-2.8.6/ads/data_labeling/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/parser/dls_record_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/parser/export_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/parser/export_record_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.883756 oracle_ads-2.8.6/ads/data_labeling/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/dls_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/export_record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/jsonl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/metadata_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/reader/record_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.883756 oracle_ads-2.8.6/ads/data_labeling/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/visualizer/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/data_labeling/visualizer/text_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.883756 oracle_ads-2.8.6/ads/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/database/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17306 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/correlation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/dask_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/dataframe_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72309 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/dataset_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/dataset_with_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37220 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/feature_engineering_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/forecasting_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/label_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/dataset/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/mixin/dataset_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26056 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/recommendation_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/regression_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39503 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/sampled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dataset/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/dbmixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dbmixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/dbmixin/db_pandas_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/environment/ml_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/evaluations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/evaluations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39617 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/evaluations/evaluation_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53173 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/evaluations/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21279 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/evaluations/statistical_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/base_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41704 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/mlx_global_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/mlx_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/mlx_local_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/explanations/mlx_whatif_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.887756 oracle_ads-2.8.6/ads/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/dataframe_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/eda_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/eda_mixin_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/feature_types_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/accessor/series_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/adsimage/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsimage/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsimage/image_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/adsimage/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsimage/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsimage/interface/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsstring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/adsstring/oci_language/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsstring/oci_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/adsstring/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/adsstring/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/data_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.891756 oracle_ads-2.8.6/ads/feature_engineering/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1600358 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/dataset/zip_code_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.895756 oracle_ads-2.8.6/ads/feature_engineering/feature_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.895756 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/oci_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/creditcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/feature_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/feature_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address_v6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type/zip_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/feature_type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/feature_engineering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/ads_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57469 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/search_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16546 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/tuner_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/hpo/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/hpo/visualization/_param_importances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/ads_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.899757 oracle_ads-2.8.6/ads/jobs/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.903756 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59743 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dsc_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40623 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dsc_job_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/infrastructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.903756 oracle_ads-2.8.6/ads/jobs/builders/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/runtimes/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/runtimes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/runtimes/container_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/builders/runtimes/python_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/env_var_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.903756 oracle_ads-2.8.6/ads/jobs/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/schema/infrastructure_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/schema/job_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/schema/runtime_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/schema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.903756 oracle_ads-2.8.6/ads/jobs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/driver_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/driver_oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/driver_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/templates/driver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/jobs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.907756 oracle_ads-2.8.6/ads/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/artifact_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/artifact_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/base_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.907756 oracle_ads-2.8.6/ads/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/common/.model-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37764 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/datascience_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.907756 oracle_ads-2.8.6/ads/model/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.907756 oracle_ads-2.8.6/ads/model/deployment/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/model_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64556 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/model_deployment_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/model_deployment_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26461 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/deployment/model_deployment_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/automl_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/huggingface_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/keras_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/lightgbm_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/model_info_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/model_info_extractor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/pytorch_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/sklearn_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/spark_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/tensorflow_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/extractor/xgboost_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/automl_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/huggingface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/lightgbm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/tensorflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/framework/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131973 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/generic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/artifact_introspection_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/artifact_introspection_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54236 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_metadata_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/env_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/model_deployment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/model_provenance_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/runtime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/runtime/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/schemas/inference_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/schemas/model_provenance_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/schemas/training_env_info_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.911756 oracle_ads-2.8.6/ads/model/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/serde/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18577 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/serde/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43205 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/serde/model_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/model/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/service/oci_datascience_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/service/oci_datascience_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/service/oci_datascience_model_version_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/model/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/model/transformer/onnx_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/mysqldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/mysqldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/mysqldb/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/opctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/opctl/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/ads_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22579 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/ads_ml_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/ads_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/ads_model_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33222 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28311 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.915757 oracle_ads-2.8.6/ads/opctl/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/manifest_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/multipart_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/conda/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/config/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/diagnostics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/config/diagnostics/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/decorator/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/diagnostics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/diagnostics/check_distributed_job_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/diagnostics/check_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/diagnostics/requirement_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/distributed/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/abstract_cluster_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/abstract_framework_spec_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_provider_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/distributed/common/framework_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.919757 oracle_ads-2.8.6/ads/opctl/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.job
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.job.gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/cuda.repo
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/docker/merge_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/opctl/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/model/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/opctl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/spark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/spark/cmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/opctl/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/templates/diagnostic_report_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/opctl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/oracledb/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/oracledb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/oracledb/oracle_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84848 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/ads_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/ads_pipeline_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/ads_pipeline_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/pipeline/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/builders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/pipeline/builders/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/builders/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/builders/infrastructure/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/pipeline/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.923756 oracle_ads-2.8.6/ads/pipeline/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/visualizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/visualizer/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/pipeline/visualizer/text_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.927757 oracle_ads-2.8.6/ads/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15817 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/big_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/oracledb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/secrets/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.927757 oracle_ads-2.8.6/ads/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/telemetry/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.927757 oracle_ads-2.8.6/ads/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/dataflow_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/dataflow_sparksql.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/func.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score-pkl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_generic.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_huggingface_pipeline.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_lightgbm.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_onnx.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_onnx_new.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_oracle_automl.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_pyspark.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_pytorch.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_scikit-learn.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_tensorflow.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/templates/score_xgboost.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.927757 oracle_ads-2.8.6/ads/text_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/udfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/text_dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/ads/type_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/abstract_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/constant_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/continuous_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/credit_card_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/datetime_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/discrete_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/document_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/ip_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/latlon_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/phone_number_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/type_discovery_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/typed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/unknown_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/type_discovery/zipcode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/ads/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/ads/vault/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/oracle_ads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 19:39:48.000000 oracle_ads-2.8.6/oracle_ads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 19:39:48.931757 oracle_ads-2.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-13 19:39:45.000000 oracle_ads-2.8.6/setup.py
```

### Comparing `oracle_ads-2.8.5/LICENSE.txt` & `oracle_ads-2.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/MANIFEST.in` & `oracle_ads-2.8.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/PKG-INFO` & `oracle_ads-2.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracle_ads
-Version: 2.8.5
+Version: 2.8.6
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.5/README.md` & `oracle_ads-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/THIRD_PARTY_LICENSES.txt` & `oracle_ads-2.8.6/THIRD_PARTY_LICENSES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,142 +1,19 @@
 Advanced Data Science and Data Services toolkit for Python Third Party License File
 
 ------------------------ Third Party Components ------------------------
 ------------------------------- Licenses -------------------------------
-- MIT License
 - Apache License 2.0
 - BSD 3-Clause "New" or "Revised" License
+- Google Protobuf License
+- ISC License (ISCL) (ISC)
+- Matplotlib License
+- MIT License
 - Mozilla Public License 2.0 (MPL 2.0)
 - Universal Permissive License (UPL)
-- Matplotlib License
--------------------------------- Notices -------------------------------
-=== NOTICE file corresponding to the section 4 d of the Apache License, ===
-=== Version 2.0, in this case for fdk-python code. ========================
-
-                                Fn Project
-                               ============
-
-    Copyright (c) 2019, 2020 Oracle and/or its affiliates. All rights reserved.
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-            http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
-
-    ==========================================================================
-    Third Party Dependencies
-    ==========================================================================
-
-    This project includes or depends on code from third party projects.
-    Attributions are contained in THIRD_PARTY_LICENSES.txt
-
-
-=== NOTICE file corresponding to the section 4 d of the Apache License, ===
-=== Version 2.0, in this case for oci code. ===============================
-
-     (c) 2016, 2020, Oracle and/or its affiliates.
-
-
-=== NOTICE file corresponding to the section 4 d of the Apache License, ===
-=== Version 2.0, in this case for pyarrow code. ===========================
-
-
-    Apache Arrow
-    Copyright 2016-2019 The Apache Software Foundation
-
-    This product includes software developed at
-    The Apache Software Foundation (http://www.apache.org/).
-
-    This product includes software from the SFrame project (BSD, 3-clause).
-    * Copyright (C) 2015 Dato, Inc.
-    * Copyright (c) 2009 Carnegie Mellon University.
-
-    This product includes software from the Feather project (Apache 2.0)
-    https://github.com/wesm/feather
-
-    This product includes software from the DyND project (BSD 2-clause)
-    https://github.com/libdynd
-
-    This product includes software from the LLVM project
-    * distributed under the University of Illinois Open Source
-
-    This product includes software from the google-lint project
-    * Copyright (c) 2009 Google Inc. All rights reserved.
-
-    This product includes software from the mman-win32 project
-    * Copyright https://code.google.com/p/mman-win32/
-    * Licensed under the MIT License;
-
-    This product includes software from the LevelDB project
-    * Copyright (c) 2011 The LevelDB Authors. All rights reserved.
-    * Use of this source code is governed by a BSD-style license that can be
-    * Moved from Kudu http://github.com/cloudera/kudu
-
-    This product includes software from the CMake project
-    * Copyright 2001-2009 Kitware, Inc.
-    * Copyright 2012-2014 Continuum Analytics, Inc.
-    * All rights reserved.
-
-    This product includes software from https://github.com/matthew-brett/multibuild (BSD 2-clause)
-    * Copyright (c) 2013-2016, Matt Terry and Matthew Brett; all rights reserved.
-
-    This product includes software from the Ibis project (Apache 2.0)
-    * Copyright (c) 2015 Cloudera, Inc.
-    * https://github.com/cloudera/ibis
-
-    This product includes software from Dremio (Apache 2.0)
-    * Copyright (C) 2017-2018 Dremio Corporation
-    * https://github.com/dremio/dremio-oss
-
-    This product includes software from Google Guava (Apache 2.0)
-    * Copyright (C) 2007 The Guava Authors
-    * https://github.com/google/guava
-
-    This product include software from CMake (BSD 3-Clause)
-    * CMake - Cross Platform Makefile Generator
-    * Copyright 2000-2019 Kitware, Inc. and Contributors
-
-    The web site includes files generated by Jekyll.
-
-    --------------------------------------------------------------------------------
-
-    This product includes code from Apache Kudu, which includes the following in
-    its NOTICE file:
-
-    Apache Kudu
-    Copyright 2016 The Apache Software Foundation
-
-    This product includes software developed at
-    The Apache Software Foundation (http://www.apache.org/).
-
-    Portions of this software were developed at
-    Cloudera, Inc (http://www.cloudera.com/).
-
-    --------------------------------------------------------------------------------
-
-    This product includes code from Apache ORC, which includes the following in
-    its NOTICE file:
-
-    Apache ORC
-    Copyright 2013-2019 The Apache Software Foundation
-
-    This product includes software developed by The Apache Software
-    Foundation (http://www.apache.org/).
-
-    This product includes software developed by Hewlett-Packard:
-    (c) Copyright [2014-2015] Hewlett-Packard Development Company, L.P
-
-------------------------------------------------------------------------
 
 ======================== Third Party Components ========================
 asteval
 * Copyright (c) 2021 Matthew Newville, The University of Chicago
 * License: MIT License
 * Source code: https://github.com/newville/asteval
 * Project home: https://github.com/newville/asteval
@@ -150,43 +27,43 @@
 cerberus
 * Copyright (c) 2012-2016 Nicola Iarocci.
 * License: ISC License (ISCL) (ISC)
 * Source code: https://github.com/pyeve/cerberus
 * Project home: http://docs.python-cerberus.org/
 
 cloudpickle
-* Copyright  (c) 2015, Cloudpickle contributors.
+* Copyright (c) 2015, Cloudpickle contributors.
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/cloudpipe/cloudpickle
 * Project home: https://github.com/cloudpipe/cloudpickle
 
+conda-pack
+* Copyright (c) 2017, Jim Crist and contributors
+* License: BSD-3-Clause license
+* Source code: https://github.com/conda/conda-pack
+* Project home: https://conda.github.io/conda-pack/
+
 datefinder
 * Copyright (c) 2015 Alec Koumjian
 * License: MIT License
 * Source code: https://github.com/akoumjian/datefinder
 * Project home: https://github.com/akoumjian/datefinder
 
+docker
+* Copyright 2016 Docker, Inc.
+* License: Apache-2.0 license
+* Source code: https://github.com/docker
+* Project home: https://www.docker.com/
+
 fastavro
 * Copyright (c) 2011 Miki Tebeka
 * License: MIT License
 * Source code: https://github.com/fastavro/fastavro
 * Project home: https://github.com/fastavro/fastavro
 
-fastparquet
-* Copyright
-* License: Apache License 2.0
-* Source code: https://github.com/dask/fastparquet/
-* Project home: https://github.com/dask/fastparquet/
-
-fdk-python
-* Copyright: see notices section above
-* License: Apache License 2.0
-* Source code: https://github.com/fnproject/fdk-python
-* Project home: https://fnproject.io/
-
 folium
 * Copyright (C) 2013, Rob Story
 * License: MIT License
 * Source code: https://github.com/python-visualization/folium
 * Project home: https://github.com/python-visualization/folium
 
 fsspec
@@ -209,20 +86,39 @@
 
 graphviz
 * Copyright (c) 2013-2021 Sebastian Bank
 * License: MIT License
 * Source code: https://github.com/xflr6/graphviz
 * Project home: https://github.com/xflr6/graphviz
 
+hdfs
+* Copyright (c) 2013, Matthieu Monsch.
+* License: MIT License
+* Source code: https://github.com/mtth/hdfs
+* Project home: https://hdfscli.readthedocs.io/en/latest/
+
 htmllistparse
 * Copyright (c) 2016-2017 Dingyuan Wang
 * License: MIT License
 * Source code: https://github.com/gumblex/htmllisting-parser
 * Project home: https://github.com/gumblex/htmllisting-parser
 
+ibisframework
+
+* Copyright 2015 Cloudera Inc.
+* License: Apache-2.0 license
+* Source code: https://github.com/ibis-project/ibis
+* Project home: https://ibis-project.org/
+
+inflection
+* Copyright (C) 2012-2020 Janne Vanhala
+* License: MIT license
+* Source code: https://github.com/jpvanhal/inflection
+* Project home: https://github.com/jpvanhal/inflection
+
 ipython
 * Copyright (c) 2008-Present, IPython Development Team
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/ipython/ipython
 * Project home: https://ipython.org/
 
 ipywidgets
@@ -233,52 +129,70 @@
 
 jinja2
 * Copyright 2007 Pallets
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/pallets/jinja/
 * Project home: https://palletsprojects.com/p/jinja/
 
+lightgbm
+* Copyright (c) 2023 Microsoft Corporation
+* License: MIT license
+* Source code: https://github.com/microsoft/LightGBM
+* Project home: https://github.com/microsoft/LightGBM
+
 matplotlib
 * Copyright
 * License: Matplotlib License
 * Source code: https://github.com/matplotlib/matplotlib
 * Project home: https://matplotlib.org/
 
-numexpr
-* Copyright (c) 2011-      See AUTHORS.txt [in the numexpr Source Code]
-* License: MIT License
-* Source code: https://github.com/pydata/numexpr
-* Project home: https://github.com/pydata/numexpr
+nbconvert
+* Copyright (c) 2001-2015, IPython Development Team, Copyright (c) 2015-, Jupyter Development Team
+* License: BSD-3-Clause license
+* Source code: https://github.com/jupyter/nbconvert
+* Project home: https://jupyter.org/
+
+nbformat
+* Copyright (c) 2001-2015, IPython Development Team, Copyright (c) 2015-, Jupyter Development Team
+* License: BSD-3-Clause license
+* Source code: https://github.com/jupyter/nbconvert
+* Project home: https://jupyter.org/
 
 numpy
 * Copyright (c) 2005-2021, NumPy Developers.
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/numpy/numpy
 * Project home: https://www.numpy.org/
 
+oci-cli
+* Copyright (c) 2016, 2021, Oracle and/or its affiliates.  All rights reserved.
+* License: The Universal Permissive License (UPL), Version 1.0
+* Source code: https://github.com/oracle/oci-cli
+* Project home: https://docs.oracle.com/en-us/iaas/Content/API/Concepts/cliconcepts.htm
+
 oci
 * Copyright (c) 2016, 2020, Oracle and/or its affiliates. [see notices section above]
 * License: Apache License 2.0, Universal Permissive License (UPL)
 * Source code: https://github.com/oracle/oci-python-sdk
 * Project home: https://docs.oracle.com/en-us/iaas/tools/python/2.44.0/index.html
 
 ocifs
 * Copyright (c) 2021 Oracle and/or its affiliates.
 * License: Universal Permissive License (UPL)
 * Source code: https://pypi.org/project/ocifs/
 * Project home: https://pypi.org/project/ocifs/
 
 onnx
-* Copyright
+* Copyright (c) 2023 ONNX Project Contributors.
 * License: Apache License 2.0
 * Source code: https://github.com/onnx/onnx/
 * Project home: https://onnxruntime.ai/
 
 onnxmltools
-* Copyright
+* Copyright (c) Microsoft Corporation
 * License: Apache License 2.0
 * Source code: https://github.com/onnx/onnxmltools
 * Project home: https://github.com/onnx/onnxmltools
 
 onnxruntime
 * Copyright (c) Microsoft Corporation
 * License: MIT License
@@ -293,49 +207,67 @@
 
 optuna
 * Copyright (c) 2018 Preferred Networks, Inc.
 * License: MIT License
 * Source code: https://github.com/optuna/optuna
 * Project home: https://optuna.org/
 
+oracledb
+* Copyright (c) 2016, 2022 Oracle and/or its affiliates.
+* License: Apache Software License Version 2.0, Universal Permissive License (UPL) (Apache and/or UPL)
+* Source code: https://github.com/oracle/python-oracledb
+* Project home: https://oracle.github.io/python-oracledb/
+
 pandas
 * Copyright (c) 2011-2021, Open source contributors.
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/pandas-dev/pandas
 * Project home: https://pandas.pydata.org/
 
 pandavro
 * Copyright (c) 2020 pandavro authors
 * License: MIT License
 * Source code: https://github.com/ynqa/pandavro
 * Project home: https://github.com/ynqa/pandavro
 
-py-cpuinfo
-* Copyright (c) 2014-2021 Matthew Brennan Jones <matthew.brennan.jones@gmail.com>
-* License: MIT License
-* Source code: https://github.com/workhorsy/py-cpuinfo
-* Project home: https://github.com/workhorsy/py-cpuinfo
-
-pyarrow
-* Copyright: see notices section above
-* License: Apache License 2.0
-* Source code: https://github.com/apache/arrow
-* Project home: https://arrow.apache.org/
+protobuf
+* Copyright 2008 Google Inc.  All rights reserved.
+* License: Google Protobuf License
+* Source code: https://github.com/protocolbuffers/protobuf
+* Project home: https://protobuf.dev/
+
+psutil
+* Copyright (c) 2009, Jay Loden, Dave Daeschler, Giampaolo Rodola. All rights reserved.
+* License: BSD-3-Clause license
+* Source code: https://github.com/giampaolo/psutil
+* Project home: https://github.com/giampaolo/psutil
+
+pyspark
+* Copyright 2014 and onwards The Apache Software Foundation.
+* License: Apache-2.0 LICENSE
+* Source code: https://github.com/apache/spark/tree/master/python
+* Project home: https://spark.apache.org/
 
 python_jsonschema_objects
 * Copyright (c) 2014 Chris Wacek
 * License: MIT License
 * Source code: https://github.com/cwacek/python-jsonschema-objects
 * Project home: python-jsonschema-objects.readthedocs.org
 
-python-snappy
-* Copyright (c) 2011-2017, Andres Moreira <andres@andresmoreira.com>
-* License: BSD 3-Clause "New" or "Revised" License
-* Source code: https://github.com/andrix/python-snappy
-* Project home: https://github.com/andrix/python-snappy
+PyYAML
+* Copyright (c) 2017-2021 Ingy döt Net, Copyright (c) 2006-2016 Kirill Simonov
+* License: MIT license
+* Source code: https://github.com/yaml/pyyaml/
+* Project home: https://pyyaml.org/
+
+requests
+* Copyright 2023 Kenneth Reitz
+* License: Apache-2.0 license
+* Source code: https://github.com/psf/requests
+* Project home: https://requests.readthedocs.io/en/latest/
 
 scikit-learn
 * Copyright (c) 2007-2021 The scikit-learn developers
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/scikit-learn/scikit-learn
 * Project home: https://scikit-learn.org/
 
@@ -347,64 +279,95 @@
 
 seaborn
 * Copyright (c) 2012-2021, Michael L. Waskom
 * License: BSD 3-Clause "New" or "Revised" License
 * Source code: https://github.com/mwaskom/seaborn
 * Project home: https://seaborn.pydata.org/
 
-six
-* Copyright (c) 2010-2020 Benjamin Peterson
-* License: MIT License
-* Source code: https://github.com/benjaminp/six
-* Project home: six.readthedocs.io/
+skl2onnx
+* Copyright (c) 2018-2022 Microsoft Corporation
+* License: Apache-2.0 license
+* Source code: https://github.com/onnx/sklearn-onnx
+* Project home: https://onnx.ai/sklearn-onnx/
+
+spacy
+* Copyright (C) 2016-2022 ExplosionAI GmbH, 2016 spaCy GmbH, 2015 Matthew Honnibal
+* License: The MIT License
+* Source code: https://github.com/explosion/spaCy
+* Project home: https://spacy.io/
 
 sqlalchemy
 * Copyright 2005-2021 SQLAlchemy authors and contributors.
 * License: MIT License
 * Source code: https://github.com/sqlalchemy/sqlalchemy
 * Project home: https://www.sqlalchemy.org/
 
 tabulate
 * Copyright (c) 2011-2020 Sergey Astanin and contributors
 * License: MIT License
 * Source code: https://github.com/astanin/python-tabulate
 * Project home: https://github.com/astanin/python-tabulate
 
+tensorflow
+* Copyright (c) 2023 Google, Inc.
+* License: Apache-2.0 license
+* Source code: https://github.com/tensorflow/tensorflow
+* Project home: https://www.tensorflow.org/
+
+tf2onnx
+* No listed copyright holder
+* License: Apache-2.0 license
+* Source code: https://github.com/onnx/tensorflow-onnx
+* Project home: https://github.com/onnx/tensorflow-onnx
+
+torch
+* Copyright (c) 2016-     Facebook, Inc            (Adam Paszke)
+* Copyright (c) 2014-     Facebook, Inc            (Soumith Chintala)
+* Copyright (c) 2011-2014 Idiap Research Institute (Ronan Collobert)
+* Copyright (c) 2012-2014 Deepmind Technologies    (Koray Kavukcuoglu)
+* Copyright (c) 2011-2012 NEC Laboratories America (Koray Kavukcuoglu)
+* Copyright (c) 2011-2013 NYU                      (Clement Farabet)
+* Copyright (c) 2006-2010 NEC Laboratories America (Ronan Collobert, Leon Bottou, Iain Melvin, Jason Weston)
+* Copyright (c) 2006      Idiap Research Institute (Samy Bengio)
+* Copyright (c) 2001-2004 Idiap Research Institute (Ronan Collobert, Samy Bengio, Johnny Mariethoz)
+* License: BSD-3
+* Source code: https://github.com/pytorch/pytorch
+* Project home: https://pytorch.org/
+
+torchvision
+* Copyright (c) Soumith Chintala 2016, All rights reserved.
+* License: BSD-3-Clause license
+* Source code: https://github.com/pytorch/vision
+* Project home: https://pytorch.org/vision/stable/index.html
+
 tqdm
 * Copyright (c) 2013 noamraph, 2016 (c) [PR #96] on behalf of Google Inc., 2015-2021 (c) Casper da Costa-Luis
 * License: MIT License, Mozilla Public License 2.0 (MPL 2.0)
 * Source code: https://github.com/tqdm/tqdm
 * Project home: https://tqdm.github.io/
 
+transformers
+* Copyright 2018- The Hugging Face team. All rights reserved.
+* License: Apache-2.0 license
+* Source code: https://github.com/huggingface/transformers
+* Project home: https://huggingface.co/transformers
+
 wordcloud
 * Copyright (c) 2012 Andreas Christian Mueller
 * License: MIT License
 * Source code: https://github.com/amueller/word_cloud
 * Project home: http://amueller.github.io/word_cloud/
 
-=============================== Licenses ===============================
+xgboost
+* Copyright 2022, xgboost developers
+* License: Apache-2.0 license
+* Source code: https://github.com/dmlc/xgboost
+* Project home: https://xgboost.ai/
 
------------------------------- MIT License -----------------------------
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+=============================== Licenses ===============================
 ------------------------------------------------------------------------
 
 -------------------------- Apache License 2.0 --------------------------
 
 
                                 Apache License
                            Version 2.0, January 2004
@@ -605,14 +568,145 @@
 OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT
 SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
 OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
 TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+------------------------------------------------------------------------
+
+--------------------- Google Protobuf License --------------------------
+
+Copyright 2008 Google Inc.  All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+    * Redistributions of source code must retain the above copyright
+notice, this list of conditions and the following disclaimer.
+    * Redistributions in binary form must reproduce the above
+copyright notice, this list of conditions and the following disclaimer
+in the documentation and/or other materials provided with the
+distribution.
+    * Neither the name of Google Inc. nor the names of its
+contributors may be used to endorse or promote products derived from
+this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Code generated by the Protocol Buffer compiler is owned by the owner
+of the input file used when generating it.  This code is not
+standalone and requires a support library to be linked with it.  This
+support library is itself covered by the above license.
+
+------------------------------------------------------------------------
+
+-------------------------- ISC License ---------------------------------
+ISC License
+
+Copyright (c) 2012-2016 Nicola Iarocci.
+
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted, provided that the above
+copyright notice and this permission notice appear in all copies.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
+
+------------------------------------------------------------------------
+
+------------------- Matplotlib License ---------------------------------
+License agreement for matplotlib versions 1.3.0 and later
+=========================================================
+
+1. This LICENSE AGREEMENT is between the Matplotlib Development Team
+("MDT"), and the Individual or Organization ("Licensee") accessing and
+otherwise using matplotlib software in source or binary form and its
+associated documentation.
+
+2. Subject to the terms and conditions of this License Agreement, MDT
+hereby grants Licensee a nonexclusive, royalty-free, world-wide license
+to reproduce, analyze, test, perform and/or display publicly, prepare
+derivative works, distribute, and otherwise use matplotlib
+alone or in any derivative version, provided, however, that MDT's
+License Agreement and MDT's notice of copyright, i.e., "Copyright (c)
+2012- Matplotlib Development Team; All Rights Reserved" are retained in
+matplotlib  alone or in any derivative version prepared by
+Licensee.
+
+3. In the event Licensee prepares a derivative work that is based on or
+incorporates matplotlib or any part thereof, and wants to
+make the derivative work available to others as provided herein, then
+Licensee hereby agrees to include in any such work a brief summary of
+the changes made to matplotlib .
+
+4. MDT is making matplotlib available to Licensee on an "AS
+IS" basis.  MDT MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, MDT MAKES NO AND
+DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF MATPLOTLIB
+WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
+
+5. MDT SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF MATPLOTLIB
+ FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR
+LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING
+MATPLOTLIB , OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF
+THE POSSIBILITY THEREOF.
+
+6. This License Agreement will automatically terminate upon a material
+breach of its terms and conditions.
+
+7. Nothing in this License Agreement shall be deemed to create any
+relationship of agency, partnership, or joint venture between MDT and
+Licensee.  This License Agreement does not grant permission to use MDT
+trademarks or trade name in a trademark sense to endorse or promote
+products or services of Licensee, or any third party.
+
+8. By copying, installing or otherwise using matplotlib ,
+Licensee agrees to be bound by the terms and conditions of this License
+Agreement.
+
+------------------------------------------------------------------------
+
+------------------------------ MIT License -----------------------------
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
+
 ------------------------------------------------------------------------
 
 ----------------------- Mozilla Public License -------------------------
 
 Bundle of CA Root Certificates
 
 Certificate data from Mozilla as of: Thu Nov  3 19:04:19 2011#
@@ -950,61 +1044,7 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
 INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
 PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
 FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
-
-------------------------------------------------------------------------
-
-------------------- Matplotlib License ---------------------------------
-License agreement for matplotlib versions 1.3.0 and later
-=========================================================
-
-1. This LICENSE AGREEMENT is between the Matplotlib Development Team
-("MDT"), and the Individual or Organization ("Licensee") accessing and
-otherwise using matplotlib software in source or binary form and its
-associated documentation.
-
-2. Subject to the terms and conditions of this License Agreement, MDT
-hereby grants Licensee a nonexclusive, royalty-free, world-wide license
-to reproduce, analyze, test, perform and/or display publicly, prepare
-derivative works, distribute, and otherwise use matplotlib
-alone or in any derivative version, provided, however, that MDT's
-License Agreement and MDT's notice of copyright, i.e., "Copyright (c)
-2012- Matplotlib Development Team; All Rights Reserved" are retained in
-matplotlib  alone or in any derivative version prepared by
-Licensee.
-
-3. In the event Licensee prepares a derivative work that is based on or
-incorporates matplotlib or any part thereof, and wants to
-make the derivative work available to others as provided herein, then
-Licensee hereby agrees to include in any such work a brief summary of
-the changes made to matplotlib .
-
-4. MDT is making matplotlib available to Licensee on an "AS
-IS" basis.  MDT MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
-IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, MDT MAKES NO AND
-DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
-FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF MATPLOTLIB
-WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
-
-5. MDT SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF MATPLOTLIB
- FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR
-LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING
-MATPLOTLIB , OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF
-THE POSSIBILITY THEREOF.
-
-6. This License Agreement will automatically terminate upon a material
-breach of its terms and conditions.
-
-7. Nothing in this License Agreement shall be deemed to create any
-relationship of agency, partnership, or joint venture between MDT and
-Licensee.  This License Agreement does not grant permission to use MDT
-trademarks or trade name in a trademark sense to endorse or promote
-products or services of Licensee, or any third party.
-
-8. By copying, installing or otherwise using matplotlib ,
-Licensee agrees to be bound by the terms and conditions of this License
-Agreement.
-------------------------------------------------------------------------
```

### Comparing `oracle_ads-2.8.5/ads/__init__.py` & `oracle_ads-2.8.6/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/automl/driver.py` & `oracle_ads-2.8.6/ads/automl/driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/automl/provider.py` & `oracle_ads-2.8.6/ads/automl/provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/bds/auth.py` & `oracle_ads-2.8.6/ads/bds/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/bds/big_data_service.py` & `oracle_ads-2.8.6/ads/bds/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/catalog/model.py` & `oracle_ads-2.8.6/ads/catalog/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/catalog/notebook.py` & `oracle_ads-2.8.6/ads/catalog/notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/catalog/project.py` & `oracle_ads-2.8.6/ads/catalog/project.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/catalog/summary.py` & `oracle_ads-2.8.6/ads/catalog/summary.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/cli.py` & `oracle_ads-2.8.6/ads/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/analyzer.py` & `oracle_ads-2.8.6/ads/common/analyzer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/artifact/.model-ignore` & `oracle_ads-2.8.6/ads/common/artifact/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/auth.py` & `oracle_ads-2.8.6/ads/common/auth.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/card_identifier.py` & `oracle_ads-2.8.6/ads/common/card_identifier.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/config.py` & `oracle_ads-2.8.6/ads/common/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/data.py` & `oracle_ads-2.8.6/ads/common/data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/decorator/argument_to_case.py` & `oracle_ads-2.8.6/ads/common/decorator/argument_to_case.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/decorator/deprecate.py` & `oracle_ads-2.8.6/ads/common/decorator/deprecate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/decorator/runtime_dependency.py` & `oracle_ads-2.8.6/ads/common/decorator/runtime_dependency.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/decorator/utils.py` & `oracle_ads-2.8.6/ads/common/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/dsc_file_system.py` & `oracle_ads-2.8.6/ads/common/dsc_file_system.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import ads
 import oci
 import ipaddress
 
 from dataclasses import dataclass
 
 FILE_STORAGE_TYPE = "FILE_STORAGE"
+OBJECT_STORAGE_TYPE = "OBJECT_STORAGE"
 
 
 @dataclass
 class DSCFileSystem:
 
     src: str = None
     dest: str = None
@@ -178,17 +179,61 @@
             )
 
         return {
             "src" : f"{dsc_model.mount_target_id}:{dsc_model.export_id}",
             "dest" : dsc_model.destination_directory_name
         }
 
+@dataclass
+class OCIObjectStorage(DSCFileSystem):
+
+    storage_type: str = OBJECT_STORAGE_TYPE
+
+    def update_to_dsc_model(self) -> dict:
+        arguments = {
+            "destinationDirectoryName" : self.dest,
+            "storageType" : self.storage_type
+        }
+        src_list = self.src.split("@")
+        bucket_segment = src_list[0]
+        namespace_segment = src_list[1].strip("/")
+        arguments["bucket"] = bucket_segment[6:]
+        if "/" in namespace_segment:
+            first_slash_index = namespace_segment.index("/")
+            arguments["namespace"] = namespace_segment[:first_slash_index]
+            arguments["prefix"] = namespace_segment[first_slash_index+1:]
+        else:
+            arguments["namespace"] = namespace_segment
+        return arguments
+
+    @classmethod
+    def update_from_dsc_model(cls, dsc_model) -> dict:
+        if not dsc_model.namespace:
+            raise ValueError(
+                "Missing parameter `namespace` from service. Check service log to see the error."
+            )
+        if not dsc_model.bucket:
+            raise ValueError(
+                "Missing parameter `bucket` from service. Check service log to see the error."
+            )
+        if not dsc_model.destination_directory_name:
+            raise ValueError(
+                "Missing parameter `destination_directory_name` from service. Check service log to see the error."
+            )
+
+        return {
+            "src" : f"oci://{dsc_model.bucket}@{dsc_model.namespace}/{dsc_model.prefix or ''}",
+            "dest" : dsc_model.destination_directory_name
+        }
+
 
 class DSCFileSystemManager:
 
+    storage_mount_dest = set()
+
     @classmethod
     def initialize(cls, arguments: dict) -> dict:
         """Initialize and update arguments to dsc model.
 
         Parameters
         ----------
         arguments: dict
@@ -200,14 +245,24 @@
             )
 
         if "dest" not in arguments:
             raise ValueError(
                 "Parameter `dest` is required for mounting file storage system."
             )
 
+        if arguments["dest"] in cls.storage_mount_dest:
+            raise ValueError(
+                "Duplicate `dest` found. Please specify different `dest` for each file system to be mounted."
+            )
+        cls.storage_mount_dest.add(arguments["dest"])
+
+        # case oci://bucket@namespace/prefix
+        if arguments["src"].startswith("oci://") and "@" in arguments["src"]:
+            return OCIObjectStorage(**arguments).update_to_dsc_model()
+
         first_segment = arguments["src"].split(":")[0]
         # case <mount_target_id>:<export_id>
         if first_segment.startswith("ocid"):
             return OCIFileStorage(**arguments).update_to_dsc_model()
 
         # case <ip_address>:<export_path>
         try:
```

### Comparing `oracle_ads-2.8.5/ads/common/error.py` & `oracle_ads-2.8.6/ads/common/error.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/extended_enum.py` & `oracle_ads-2.8.6/ads/common/extended_enum.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/function/fn_util.py` & `oracle_ads-2.8.6/ads/common/function/fn_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/function/func_conf.yaml` & `oracle_ads-2.8.6/ads/common/function/func_conf.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/ipython.py` & `oracle_ads-2.8.6/ads/common/ipython.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/model.py` & `oracle_ads-2.8.6/ads/common/model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/model_artifact.py` & `oracle_ads-2.8.6/ads/common/model_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/model_artifact_schema.json` & `oracle_ads-2.8.6/ads/common/model_artifact_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/model_export_util.py` & `oracle_ads-2.8.6/ads/common/model_export_util.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/model_metadata.py` & `oracle_ads-2.8.6/ads/common/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/object_storage_details.py` & `oracle_ads-2.8.6/ads/common/object_storage_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/oci_client.py` & `oracle_ads-2.8.6/ads/common/oci_client.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/oci_datascience.py` & `oracle_ads-2.8.6/ads/common/oci_datascience.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/oci_logging.py` & `oracle_ads-2.8.6/ads/common/oci_logging.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/oci_mixin.py` & `oracle_ads-2.8.6/ads/common/oci_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/oci_resource.py` & `oracle_ads-2.8.6/ads/common/oci_resource.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/serializer.py` & `oracle_ads-2.8.6/ads/common/serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/utils.py` & `oracle_ads-2.8.6/ads/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/common/word_lists.py` & `oracle_ads-2.8.6/ads/common/word_lists.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/config.py` & `oracle_ads-2.8.6/ads/config.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/__init__.py` & `oracle_ads-2.8.6/ads/data_labeling/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/boundingbox.py` & `oracle_ads-2.8.6/ads/data_labeling/boundingbox.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/constants.py` & `oracle_ads-2.8.6/ads/data_labeling/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/data_labeling_service.py` & `oracle_ads-2.8.6/ads/data_labeling/data_labeling_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/interface/reader.py` & `oracle_ads-2.8.6/ads/data_labeling/interface/reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/loader/file_loader.py` & `oracle_ads-2.8.6/ads/data_labeling/loader/file_loader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/metadata.py` & `oracle_ads-2.8.6/ads/data_labeling/metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/mixin/data_labeling.py` & `oracle_ads-2.8.6/ads/data_labeling/mixin/data_labeling.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/ner.py` & `oracle_ads-2.8.6/ads/data_labeling/ner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/parser/dls_record_parser.py` & `oracle_ads-2.8.6/ads/data_labeling/parser/dls_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/parser/export_metadata_parser.py` & `oracle_ads-2.8.6/ads/data_labeling/parser/export_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/parser/export_record_parser.py` & `oracle_ads-2.8.6/ads/data_labeling/parser/export_record_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/dataset_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/dls_record_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/dls_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/export_record_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/export_record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/jsonl_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/metadata_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/reader/record_reader.py` & `oracle_ads-2.8.6/ads/data_labeling/reader/record_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/record.py` & `oracle_ads-2.8.6/ads/data_labeling/record.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/visualizer/image_visualizer.py` & `oracle_ads-2.8.6/ads/data_labeling/visualizer/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/data_labeling/visualizer/text_visualizer.py` & `oracle_ads-2.8.6/ads/data_labeling/visualizer/text_visualizer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/database/connection.py` & `oracle_ads-2.8.6/ads/database/connection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataflow/dataflow.py` & `oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dsc_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1892 +1,1766 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
-# Copyright (c) 2020, 2022 Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
+from __future__ import annotations
 
+import datetime
+import logging
+import oci
 import os
-from datetime import datetime
-from types import MethodType
 import time
-import pathlib
-import json
-import re
+import traceback
 import uuid
-from urllib.parse import urlparse
-from pathlib import Path
-from pandas import DataFrame
-from ast import literal_eval
-
-from jinja2 import Environment, PackageLoader
-
-from ads.common import oci_client, auth, logger
-from ads.common.utils import FileOverwriteError
-from ads.common.decorator.runtime_dependency import (
-    runtime_dependency,
-    OptionalDependency,
-)
-from ads.common.decorator.deprecate import deprecated
-
-from oci.data_flow.models import (
-    CreateApplicationDetails,
-    Application,
-    ApplicationParameter,
-    ApplicationSummary,
-    UpdateApplicationDetails,
-    CreateRunDetails,
-    Run,
-    UpdateRunDetails,
-    RunSummary,
-)
+from io import DEFAULT_BUFFER_SIZE
+from string import Template
+from typing import Any, Dict, List, Optional, Union
+
+import fsspec
+import oci.data_science
+import oci.util as oci_util
+import yaml
+from oci.data_science.models import JobInfrastructureConfigurationDetails
 from oci.exceptions import ServiceError
-
 from ads.common import utils
-from ads.dataflow.dataflowsummary import SummaryList
-from ads.config import NB_SESSION_COMPARTMENT_OCID, TENANCY_OCID, OCI_REGION_METADATA
+from ads.common.oci_datascience import DSCNotebookSession, OCIDataScienceMixin
+from ads.common.oci_logging import OCILog
+from ads.common.oci_resource import ResourceNotFoundError
+from ads.jobs.builders.infrastructure.base import Infrastructure, RunInstance
+from ads.jobs.builders.infrastructure.dsc_job_runtime import (
+    DataScienceJobRuntimeManager,
+)
+from ads.jobs.builders.infrastructure.utils import get_value
+from ads.jobs.builders.runtimes.artifact import Artifact
+from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
+from ads.jobs.builders.runtimes.python_runtime import GitPythonRuntime
 
-env = Environment(loader=PackageLoader("ads", "templates"))
+from ads.common.dsc_file_system import OCIFileStorage, DSCFileSystemManager, OCIObjectStorage
 
-create_application_details_attributes = CreateApplicationDetails().swagger_types.keys()
-update_application_details_attributes = UpdateApplicationDetails().swagger_types.keys()
-application_attributes = list(Application().swagger_types.keys())
+logger = logging.getLogger(__name__)
 
-create_run_details_attributes = CreateRunDetails().swagger_types.keys()
-update_run_details_attributes = UpdateRunDetails().swagger_types.keys()
-run_attributes = list(Run().swagger_types.keys())
+SLEEP_INTERVAL = 3
+WAIT_SECONDS_AFTER_FINISHED = 90
+MAXIMUM_MOUNT_COUNT = 5
+FILE_STORAGE_TYPE = "FILE_STORAGE"
+OBJECT_STORAGE_TYPE = "OBJECT_STORAGE"
 
 
-class SPARK_VERSION(str):
-    v2_4_4 = "2.4.4"
-    v3_0_2 = "3.0.2"
+class DSCJob(OCIDataScienceMixin, oci.data_science.models.Job):
+    """Represents an OCI Data Science Job
+    This class contains all attributes of the oci.data_science.models.Job.
+    The main purpose of this class is to link the oci.data_science.models.Job model and the related client methods.
+    Mainly, linking the Job model (payload) to Create/Update/Get/List/Delete methods.
 
+    A DSCJob can be initialized by unpacking a the properties stored in a dictionary (payload):
 
-class DataFlow:
-    @deprecated(
-        "2.6.3",
-        details="Use ads.jobs.DataFlow class for creating Data Flow applications and runs. Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/apachespark/dataflow.html#create-run-data-flow-application-using-ads-python-sdk",
-    )
-    def __init__(
-        self,
-        compartment_id=None,
-        dataflow_base_folder="/home/datascience/dataflow",
-        os_auth=None,
-        df_auth=None,
-    ):
-        # create iff not found dataflow_base_folder
-        self.dataflow_base_folder = dataflow_base_folder
-        self.os_auth = os_auth if os_auth else auth.default_signer()
-        self.df_auth = df_auth if df_auth else auth.default_signer()
-        self.compartment_id = (
-            NB_SESSION_COMPARTMENT_OCID if compartment_id is None else compartment_id
-        )
-        if self.compartment_id is None:
-            raise ValueError("compartment_id needs to be specified.")
-        self.display_name = None
-        self.driver_shape = None
-        self.executor_shape = None
-        self.file_uri = None
-        self.archive_uri = None
-        self.language = None
-        self.logs_bucket_uri = None
-        self.num_executors = None
-        self.spark_version = None
-        self.warehouse_bucket_uri = None
-
-        self.object_storage_client = oci_client.OCIClientFactory(
-            **self.os_auth
-        ).object_storage
-        self.df_client = oci_client.OCIClientFactory(**self.df_auth).dataflow
-
-        self.region = (
-            self.df_auth["config"]["region"]
-            if "config" in self.df_auth and "region" in self.df_auth["config"]
-            else (
-                literal_eval(OCI_REGION_METADATA)["regionIdentifier"]
-                if OCI_REGION_METADATA
-                else None
-            )
-        )
-        if not self.region:
-            logger.warning(
-                "Region information not found from oci config file. Set region in the OCI config file"
-            )
-        try:
-            self.namespace = self.object_storage_client.get_namespace().data
-        except ServiceError as se:
-            if se.status == 404:
-                raise ValueError(
-                    f'The compartment_id "{self.compartment_id}" have to be '
-                    f"in same tenancy as current user "
-                ) from se
-            else:
-                raise
+    .. code-block:: python
 
-        self.short_id_index = {}
-        # Currently Data Flow only supports VM.Standard.2 series
-        # VM_shapes dict needs to be updated if any change from Data Flow
-        self.VM_shapes = {
-            "VM.Standard2.1",
-            "VM.Standard2.2",
-            "VM.Standard2.4",
-            "VM.Standard2.8",
-            "VM.Standard2.16",
-            "VM.Standard2.24",  # not available in some tenancy
+        job_properties = {
+            "display_name": "my_job",
+            "job_infrastructure_configuration_details": {"shape_name": "VM.MY_SHAPE"}
         }
+        job = DSCJob(**job_properties)
 
-    def __iter__(self):
-        return self.list_apps().__iter__()
+    The properties can also be OCI REST API payload, in which the keys are in camel format.
 
-    def __len__(self):
-        return len(self.list_apps())
+    .. code-block:: python
 
-    def _decorate_app(self, app):
-        app.swagger_types["short_id"] = "str"
-        app.ocid = app.id
-
-        def to_dataframe(app_self):
-            if "arguments" in application_attributes:
-                application_attributes.remove("arguments")
-            df = DataFrame.from_dict(
-                {
-                    key: getattr(app_self, key)
-                    for key in application_attributes
-                    if hasattr(app_self, key)
+        job_payload = {
+            "projectId": "<project_ocid>",
+            "compartmentId": "<compartment_ocid>",
+            "displayName": "<job_name>",
+            "jobConfigurationDetails": {
+                "jobType": "DEFAULT",
+                "commandLineArguments": "pos_arg1 pos_arg2 --key1 val1 --key2 val2",
+                "environmentVariables": {
+                    "KEY1": "VALUE1",
+                    "KEY2": "VALUE2",
+                    # User specifies conda env via env var
+                    "CONDA_ENV_TYPE" : "service",
+                    "CONDA_ENV_SLUG" : "mlcpuv1"
+                }
+            },
+            "jobInfrastructureConfigurationDetails": {
+                "jobInfrastructureType": "STANDALONE",
+                "shapeName": "VM.Standard.E3.Flex",
+                "jobShapeConfigDetails": {
+                    "memoryInGBs": 16,
+                    "ocpus": 1
                 },
-                orient="index",
-                columns=[""],
-            )
-            return df
+                "blockStorageSizeInGBs": "100",
+                "subnetId": "<subnet_ocid>"
+            }
+        }
+        job = DSCJob(**job_payload)
+    """
 
-        @runtime_dependency(module="IPython", install_from=OptionalDependency.NOTEBOOK)
-        def show_in_notebook(app_self):
-            """
-            Describe the project by showing its properties
-            """
-            from IPython.display import display
+    DEFAULT_INFRA_TYPE = (
+        JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
+    )
 
-            display(app_self)
+    CONST_DEFAULT_BLOCK_STORAGE_SIZE = 50
 
-        def _repr_html_(app_self):
-            return (
-                app_self.to_dataframe()
-                .style.set_properties(**{"margin-left": "0px"})
-                .render()
-            )
+    def __init__(self, artifact: Union[str, Artifact] = None, **kwargs) -> None:
+        """Initialize a DSCJob object.
 
-        app.to_dataframe = MethodType(to_dataframe, app)
-        app.show_in_notebook = MethodType(show_in_notebook, app)
-        app._repr_html_ = MethodType(_repr_html_, app)
+        Parameters
+        ----------
+        artifact: str or Artifact
+            Job artifact, which can be a path or an Artifact object. Defaults to None.
+        kwargs:
+            Same as kwargs in oci.data_science.models.Job.
+            Keyword arguments are passed into OCI Job model to initialize the properties.
 
-        return app
+        """
+        self._artifact = artifact
 
-    def prepare_app(
-        self,
-        display_name: str,
-        script_bucket: str,
-        pyspark_file_path: str,
-        spark_version: str = SPARK_VERSION.v2_4_4,
-        compartment_id: str = None,
-        archive_path: str = None,
-        archive_bucket: str = None,
-        logs_bucket: str = "dataflow-logs",
-        driver_shape: str = "VM.Standard2.4",
-        executor_shape: str = "VM.Standard2.4",
-        num_executors: int = 1,
-        arguments: list = [],
-        script_parameters: dict = [],
-    ) -> dict:
-        """
-        Check if the parameters provided by users to create an application are
-        valid and then prepare app_configuration for creating an app or saving
-        for future reuse.
+        super().__init__(**kwargs)
+        if not self.job_configuration_details:
+            self.job_configuration_details = {
+                "jobType": "DEFAULT",
+            }
+        if not self.job_infrastructure_configuration_details:
+            self.job_infrastructure_configuration_details = {}
 
-        Parameters
-        ----------
-        display_name: str, required
-            A user-friendly name. This name is not necessarily unique.
-        script_bucket: str, required
-            bucket in object storage to upload the pyspark file
-        pyspark_file_path: str, required
-            path to the pyspark file
-        spark_version: str
-            Allowed values are "2.4.4", "3.0.2".
-        compartment_id: str
-            OCID of the compartment to create a dataflow app. If not
-            provided, compartment_id will use the same as the notebook session.
-        archive_path: str, optional
-            path to the archive file
-        archive_bucket: str, optional
-            bucket in object storage to upload the archive file
-        logs_bucket: str, default is 'dataflow-logs'
-            bucket in object storage to put run logs
-        driver_shape: str
-            The value to assign to the driver_shape property of this
-            CreateApplicationDetails.
-            Allowed values for this property are: "VM.Standard2.1",
-            "VM.Standard2.2", "VM.Standard2.4", "VM.Standard2.8",
-            "VM.Standard2.16", "VM.Standard2.24".
-        executor_shape: str
-            The value to assign to the executor_shape property of this
-            CreateApplicationDetails.
-            Allowed values for this property are: "VM.Standard2.1",
-            "VM.Standard2.2", "VM.Standard2.4", "VM.Standard2.8",
-            "VM.Standard2.16", "VM.Standard2.24".
-        num_executors: int
-            The number of executor VMs requested.
-        arguments: list of str
-            The values passed into the command line string to run the application
-        script_parameters: dict
-            The value of the parameters passed to the running application as
-            command line arguments for the pyspark script.
+    @property
+    def artifact(self) -> Union[str, Artifact]:
+        """Job artifact.
 
         Returns
         -------
-        app_configuration: dictionary containing all the validated params for CreateApplicationDetails.
+        str or Artifact
+            When creating a job, this be a path or an Artifact object.
+            When loading the job from OCI, this will be the filename of the job artifact.
         """
-        if not self._check_bucket_exist(script_bucket):
-            raise ValueError(
-                "The bucket {} does not exist in object storage".format(script_bucket)
+        if self.id and self._artifact is None:
+            try:
+                res = self.client.head_job_artifact(self.id)
+                content = res.headers.get("content-disposition")
+                if content and "filename=" in content:
+                    self._artifact = content.split("filename=", 1)[-1]
+            except ServiceError:
+                self._artifact = ""
+        return self._artifact
+
+    @artifact.setter
+    def artifact(self, artifact: Union[str, Artifact]):
+        """Sets the job artifact."""
+        self._artifact = artifact
+
+    def _load_infra_from_notebook(self, nb_config):
+        """Loads the infrastructure configuration from notebook configuration."""
+        infra = self.job_infrastructure_configuration_details
+        nb_shape_config_details = oci_util.to_dict(
+            getattr(nb_config, "notebook_session_shape_config_details", None) or {}
+        )
+        if isinstance(infra, dict):
+            shape_name = infra.get("shapeName", nb_config.shape)
+
+            # Ignore notebook shape config details if shape names do not match.
+            if shape_name != nb_config.shape:
+                nb_shape_config_details = {}
+
+            infra_type = infra.get("jobInfrastructureType")
+            block_storage = infra.get(
+                "blockStorageSizeInGBs", nb_config.block_storage_size_in_gbs
+            )
+            subnet_id = infra.get(
+                "subnetId",
+                nb_config.subnet_id
+                if infra_type
+                != JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
+                else None,
+            )
+            job_shape_config_details = infra.get("jobShapeConfigDetails", {})
+            memory_in_gbs = job_shape_config_details.get(
+                "memoryInGBs", nb_shape_config_details.get("memory_in_gbs")
+            )
+            ocpus = job_shape_config_details.get(
+                "ocpus", nb_shape_config_details.get("ocpus")
             )
         else:
-            self.script_bucket = script_bucket
+            shape_name = (
+                infra.shape_name
+                if getattr(infra, "shape_name", None)
+                else nb_config.shape
+            )
+            # Ignore notebook shape config details if shape names do not match.
+            if shape_name != nb_config.shape:
+                nb_shape_config_details = {}
+
+            infra_type = getattr(infra, "job_infrastructure_type", None)
+
+            block_storage = (
+                infra.block_storage_size_in_gbs
+                if getattr(infra, "block_storage_size_in_gbs", None)
+                else nb_config.block_storage_size_in_gbs
+            )
+            subnet_id = (
+                infra.subnet_id
+                if getattr(infra, "subnet_id", None)
+                else (
+                    nb_config.subnet_id
+                    if infra_type
+                    != JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
+                    else None
+                )
+            )
+            job_shape_config_details = oci_util.to_dict(
+                getattr(infra, "job_shape_config_details", {}) or {}
+            )
+            memory_in_gbs = job_shape_config_details.get(
+                "memory_in_gbs", nb_shape_config_details.get("memory_in_gbs")
+            )
+            ocpus = job_shape_config_details.get(
+                "ocpus", nb_shape_config_details.get("ocpus")
+            )
 
-        if not self._check_bucket_exist(logs_bucket):
-            raise ValueError(
-                "The log bucket {} does not exist in object storage".format(logs_bucket)
+        self.job_infrastructure_configuration_details = {
+            "jobInfrastructureType": infra_type,
+            "shapeName": shape_name,
+            "blockStorageSizeInGBs": block_storage,
+        }
+        # ADS does not provide explicit API for setting infrastructure type.
+        # If subnet is configured, the type will be set to STANDALONE,
+        # otherwise ME_STANDALONE
+        if subnet_id:
+            self.job_infrastructure_configuration_details.update(
+                {
+                    "subnetId": subnet_id,
+                    "jobInfrastructureType": JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE,
+                }
             )
         else:
-            self.logs_bucket_uri = (
-                self.warehouse_bucket_uri
-            ) = f"oci://{logs_bucket}@{self.namespace}"
-
-        # check if local path of script file is valid
-        self._check_valid_path(pyspark_file_path)
-
-        if archive_path:
-            # check if local path of archive file is valid
-            self._check_valid_path(archive_path)
-
-            if archive_bucket is None:
-                # use script bucket by default if archive_bucket not provided
-                archive_bucket = script_bucket
-            else:
-                if not self._check_bucket_exist(archive_bucket):
-                    raise ValueError(
-                        "The bucket {} does not exist in object storage".format(
-                            archive_bucket
-                        )
-                    )
-
-        # check whether the params have valid input type and value
-        self._check_valid_param(
-            display_name, driver_shape, executor_shape, num_executors
-        )
+            self.job_infrastructure_configuration_details.update(
+                {
+                    "jobInfrastructureType": self.DEFAULT_INFRA_TYPE,
+                }
+            )
 
-        # when user try to specify a non-python application, we throw warnings
-        if self.language is not None and self.language != "PYTHON":
-            logger.warning("ADS only supports Python.")
+        # Specify shape config details
+        if memory_in_gbs or ocpus:
+            self.job_infrastructure_configuration_details.update(
+                {
+                    "jobShapeConfigDetails": {
+                        "memoryInGBs": memory_in_gbs,
+                        "ocpus": ocpus,
+                    }
+                }
+            )
 
-        app_compartment_id = (
-            self.compartment_id if compartment_id is None else compartment_id
-        )
+    def load_properties_from_env(self) -> None:
+        """Loads default properties from the environment"""
+        if "NB_SESSION_OCID" in os.environ:
+            try:
+                nb_session = DSCNotebookSession.from_ocid(os.environ["NB_SESSION_OCID"])
+            except Exception:
+                logger.debug("Failed to load config from notebook.")
+                logger.debug(traceback.format_exc())
+                # If there is an error loading the notebook infra configurations.
+                # Ignore it by setting nb_session to None
+                # This will skip loading the default configure.
+                nb_session = None
+            if nb_session:
+                nb_config = getattr(
+                    nb_session,
+                    "notebook_session_config_details",
+                    getattr(nb_session, "notebook_session_configuration_details", None),
+                )
 
-        app_configuration = {
-            "compartment_id": app_compartment_id,
-            "language": "PYTHON",
-            "pyspark_file_path": pyspark_file_path,
-            "script_bucket": self.script_bucket,
-            "archive_path": archive_path,
-            "archive_bucket": archive_bucket,
-            "logs_bucket": logs_bucket,
-            "display_name": self.display_name,
-            "driver_shape": self.driver_shape,
-            "executor_shape": self.executor_shape,
-            "num_executors": self.num_executors,
-            "spark_version": spark_version,
-        }
+                if nb_config:
+                    self._load_infra_from_notebook(nb_config)
+                if self.project_id is None:
+                    self.project_id = nb_session.project_id
+        super().load_properties_from_env()
+
+    def load_defaults(self) -> DSCJob:
+        self.load_properties_from_env()
+        if not self.job_infrastructure_configuration_details:
+            self.job_infrastructure_configuration_details = {}
+        # Convert the dict to JobInfrastructureConfigurationDetails object
+        if isinstance(self.job_infrastructure_configuration_details, dict):
+            # Default networking
+            if not self.job_infrastructure_configuration_details.get(
+                "jobInfrastructureType"
+            ):
+                self.job_infrastructure_configuration_details[
+                    "jobInfrastructureType"
+                ] = self.DEFAULT_INFRA_TYPE
+            self.job_infrastructure_configuration_details = self.deserialize(
+                self.job_infrastructure_configuration_details,
+                JobInfrastructureConfigurationDetails.__name__,
+            )
+
+        # Default block storage size
+        if not self.job_infrastructure_configuration_details.block_storage_size_in_gbs:
+            self.job_infrastructure_configuration_details.block_storage_size_in_gbs = (
+                self.CONST_DEFAULT_BLOCK_STORAGE_SIZE
+            )
+        return self
 
-        # here we handle the case where users specify arguments
-        if arguments:
-            # check if the arguments are valid
-            for arg in arguments:
-                if not isinstance(arg, str):
-                    raise TypeError("Arguments must be a list of str.")
-
-                if re.match("\$\{([^}]+)\}", arg):
-                    arg_name = arg.strip("${}")
-                    if " " in arg_name:
-                        raise ValueError(
-                            f"With {arg} in the format of "
-                            "${var}, space is not allowed in "
-                            f"{arg_name}"
-                        )
-
-                    if arg_name not in script_parameters:
-                        logger.warning(
-                            f"With `{arg}` in the format of "
-                            "`${var}`, "
-                            f"the argument `{arg_name}` will be replaced by the value provided in script parameters when passed in. "
-                            f"While arguments not in this format are passed to the PySpark script verbatim."
-                            f"Therefore, `{arg_name}` must be a valid key in script parameters."
-                        )
-                        raise KeyError(
-                            f"{arg_name} doesn't exist in script parameters, thus {arg} is not valid."
-                        )
-
-            # convert script parameters to be a list of tuples
-            app_configuration["script_parameters"] = [
-                (k, script_parameters[k]) for k in script_parameters
-            ]
-            app_configuration["arguments"] = arguments
+    def _create_with_oci_api(self) -> None:
+        res = self.client.create_job(
+            self.to_oci_model(oci.data_science.models.CreateJobDetails)
+        )
+        self.update_from_oci_model(res.data)
+        if self.lifecycle_state == "ACTIVE":
+            return
+        try:
+            if issubclass(self.artifact.__class__, Artifact):
+                with self.artifact as artifact:
+                    self.upload_artifact(artifact.path)
+            else:
+                self.upload_artifact()
+        except Exception as ex:
+            # Delete the job if upload artifact is failed.
+            self.delete()
+            raise ex
 
-        return app_configuration
+    def create(self) -> DSCJob:
+        """Create the job on OCI Data Science platform
+
+        Returns
+        -------
+        DSCJob
+            The DSCJob instance (self), which allows chaining additional method.
 
-    def template(
-        self,
-        job_type: str = "standard_pyspark",
-        script_str: str = "",
-        file_dir: str = None,
-        file_name: str = None,
-    ) -> str:
         """
-        Populate a prewritten pyspark or sparksql python script with
-        user's choice to write additional lines and save in local directory.
+        if not self.display_name:
+            if self.artifact:
+                timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d-%H:%M.%S")
+                self.display_name = (
+                    os.path.basename(str(self.artifact)).split(".")[0] + f"-{timestamp}"
+                )
+            else:
+                # Set default display_name if not specified - randomly generated easy to remember name generated
+                self.display_name = utils.get_random_name_for_resource()
+        try:
+            self.load_defaults()
+        except Exception:
+            logger.exception("Failed to load default properties.")
+        # Check compartment ID and project ID before calling the OCI API
+        if not self.compartment_id:
+            raise ValueError("Specify compartment ID for data science job.")
+        if not self.project_id:
+            raise ValueError("Specify project ID for data science job.")
+        self._create_with_oci_api()
+        return self
 
-        Parameters
-        ----------
-        job_type: str, default is 'standard_pyspark'
-            Currently supports two types, 'standard_pyspark' or 'sparksql'
-        script_str: str, optional, default is ''
-            code provided by user to write in the python script
-        file_dir: str, optional
-            Directory to save the python script in local directory
-        file_name: str, optional
-            name of the python script to save to the local directory
+    def update(self) -> DSCJob:
+        """Updates the Data Science Job."""
+        raise NotImplementedError("Updating Job is not supported at the moment.")
+
+    def delete(self) -> DSCJob:
+        """Deletes the job and the corresponding job runs.
 
         Returns
         -------
-        script_path: str
-            Path to the template generated python file in local directory
+        DSCJob
+            The DSCJob instance (self), which allows chaining additional method.
+
         """
-        if file_dir is None:
-            file_dir = self.dataflow_base_folder
-            if not os.path.isdir(file_dir):
-                os.mkdir(file_dir)
+        runs = self.run_list()
+        for run in runs:
+            run.delete()
+        self.client.delete_job(self.id)
+        return self
 
-        if file_name is None:
-            creation_time = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
-            file_name = f"{job_type}_{creation_time}.py"
+    def upload_artifact(self, artifact_path: str = None) -> DSCJob:
+        """Uploads the job artifact to OCI
 
-        script_path = os.path.join(file_dir, file_name)
+        Parameters
+        ----------
+        artifact_path : str, optional
+            Local path to the job artifact file to be uploaded, by default None.
+            If artifact_path is None, the path in self.artifact will be used.
 
-        if os.path.exists(script_path):
-            logger.info(f"Overwriting {script_path}.")
+        Returns
+        -------
+        DSCJob
+            The DSCJob instance (self), which allows chaining additional method.
 
-        if job_type == "standard_pyspark":
-            self._get_pyspark_template(script_path, script_str)
-        elif job_type == "sparksql":
-            self._get_sparksql_template(script_path, script_str)
-        else:
-            raise ValueError(
-                "Currently only supports template for two job types, 'standard_pyspark' or 'sparksql'"
+        """
+        if not artifact_path:
+            artifact_path = self.artifact
+        with fsspec.open(artifact_path, "rb") as f:
+            self.client.create_job_artifact(
+                self.id,
+                f,
+                content_disposition=f"attachment; filename={os.path.basename(artifact_path)}",
             )
-        relative_path = os.path.relpath(script_path)
-        # FileLink has to be tested with router to check compatibility. Till then let us comment it (ODSC-8310)
-        # return display(FileLink(relative_path))
-        logger.info(f"Code generated: {script_path}.")
-        return script_path
+        return self
 
-    def _get_pyspark_template(self, script_path, script_str: str = ""):
-        """
-        Create a prewriiten pyspark script
+    def download_artifact(self, artifact_path: str) -> DSCJob:
+        """Downloads the artifact from OCI
 
         Parameters
         ----------
-        script_path: str
-            Path to the template generated python file in local directory
-        script_str: str, optional, default is ''
-            code provided by user to write in the python script
+        artifact_path : str
+            Local path to store the job artifact.
 
         Returns
         -------
-        None
-        """
-        pyspark_template = env.get_template("dataflow_pyspark.jinja2")
+        DSCJob
+            The DSCJob instance (self), which allows chaining additional method.
 
-        with open(script_path, "w") as fp:
-            fp.write(pyspark_template.render(script_str=script_str))
-
-    def _get_sparksql_template(self, script_path, script_str):
         """
-        Create a prewriiten sparksql python script
+        res = self.client.get_job_artifact_content(self.id)
+        with open(artifact_path, "wb") as f:
+            for chunk in res.data.iter_content(chunk_size=DEFAULT_BUFFER_SIZE * 16):
+                f.write(chunk)
+        return self
+
+    def run_list(self, **kwargs) -> list[DataScienceJobRun]:
+        """Lists the runs of this job.
 
         Parameters
         ----------
-        script_path: str
-            Path to the template generated python file in local directory
-        script_str: str, optional, default is ''
-            code provided by user to write in the python script
+        **kwargs :
+            Keyword arguments to te passed into the OCI list_job_runs() for filtering the job runs.
 
         Returns
         -------
-        None
+        list
+            A list of DSCJobRun objects
+
         """
-        pyspark_template = env.get_template("dataflow_sparksql.jinja2")
+        items = oci.pagination.list_call_get_all_results(
+            self.client.list_job_runs, self.compartment_id, job_id=self.id, **kwargs
+        ).data
+        return [DataScienceJobRun.from_oci_model(item) for item in items]
 
-        with open(script_path, "w") as fp:
-            fp.write(pyspark_template.render(script_str=script_str))
+    def run(self, **kwargs) -> DataScienceJobRun:
+        """Runs the job
 
-    def _check_valid_path(self, file_path):
-        """
-        Returns
-        -------
-        valid_path: bool
-            whether the provided file path is valid
-        """
-        file_dir = os.path.dirname(file_path)
-        if len(file_dir) > 0 and not os.path.exists(file_dir):
-            raise ValueError("The directoy of file {} does not exist".format(file_path))
-        elif not os.path.exists(file_path):
-            raise ValueError(
-                " The directoy of the file {} is valid but the file does not exist".format(
-                    file_path
-                )
-            )
-        return True
+        Parameters
+        ----------
+        **kwargs :
+            Keyword arguments for initializing a Data Science Job Run.
+            The keys can be any keys in supported by OCI JobConfigurationDetails and JobRun, including:
+            * hyperparameter_values: dict(str, str)
+            * environment_variables: dict(str, str)
+            * command_line_arguments: str
+            * maximum_runtime_in_minutes: int
+            * display_name: str
+            * freeform_tags: dict(str, str)
+            * defined_tags: dict(str, dict(str, object))
+
+        If display_name is not specified, it will be generated as "<JOB_NAME>-run-<TIMESTAMP>".
 
-    def _check_valid_param(
-        self, display_name, driver_shape, executor_shape, num_executors
-    ):
-        """
         Returns
         -------
-        valid_param: bool
-            whether the params have valid input type and value
+        DSCJobRun
+            An instance of DSCJobRun, which can be used to monitor the job run.
+
         """
-        if not isinstance(display_name, str):
-            raise TypeError("param 'display_name' must be string")
-        else:
-            self.display_name = display_name
+        if not self.id:
+            self.create()
 
-        if not isinstance(driver_shape, str):
-            raise TypeError("param 'driver_shape' must be string")
-        elif driver_shape not in self.VM_shapes:
-            raise ValueError("param 'driver_shape' is not a valid VM shape")
-        else:
-            self.driver_shape = driver_shape
+        swagger_types = (
+            oci.data_science.models.DefaultJobConfigurationDetails().swagger_types.keys()
+        )
+        config_kwargs = {}
+        keys = list(kwargs.keys())
+        for key in keys:
+            if key in swagger_types:
+                config_kwargs[key] = kwargs.pop(key)
 
-        if not isinstance(executor_shape, str):
-            raise TypeError("param 'executor_shape' must be string")
-        elif executor_shape not in self.VM_shapes:
-            raise ValueError("param 'executor_shape' is not a valid VM shape")
-        else:
-            self.executor_shape = executor_shape
+        # remove timestamp from the job name (added in default names, when display_name not specified by user)
+        if self.display_name:
+            try:
+                datetime.datetime.strptime(self.display_name[-19:], "%Y-%m-%d-%H:%M.%S")
+                self.display_name = self.display_name[:-20]
+            except ValueError:
+                pass
+
+        job_attrs = dict(
+            project_id=self.project_id,
+            display_name=self.display_name
+            + "-run-"
+            + datetime.datetime.now().strftime("%Y-%m-%d-%H:%M.%S"),
+            job_id=self.id,
+            compartment_id=self.compartment_id,
+        )
 
-        if not isinstance(num_executors, int):
-            raise TypeError("param 'num_executors' must be an integer")
-        elif num_executors < 1:
-            raise ValueError("param 'num_executors' has a minimum value of 1")
-        else:
-            self.num_executors = num_executors
-        return True
+        for key, val in job_attrs.items():
+            if not kwargs.get(key):
+                kwargs[key] = val
+
+        if config_kwargs:
+            config_kwargs["jobType"] = "DEFAULT"
+            config_override = kwargs.get("job_configuration_override_details", {})
+            config_override.update(config_kwargs)
+            kwargs["job_configuration_override_details"] = config_override
+
+        wait = kwargs.pop("wait", False)
+        run = DataScienceJobRun(**kwargs).create()
+        if wait:
+            return run.watch()
+        return run
+
+    @classmethod
+    def from_ocid(cls, ocid) -> DSCJob:
+        """Gets a job by OCID
+
+        Parameters
+        ----------
+        ocid : str
+            The OCID of the job.
 
-    def _check_bucket_exist(self, bucket_name: str) -> bool:
-        """
         Returns
         -------
-        bucket_exist: bool
-            whether the bucket already exists in the object storage
-        """
-        try:
-            bucket_response = self.object_storage_client.head_bucket(
-                self.namespace, bucket_name
-            )
-        except ServiceError as se:
-            if se.status == 404:
-                raise KeyError(
-                    f"The bucket {bucket_name} does not exist in object storage"
-                ) from se
-            else:
-                raise
-        return True
-
-    def _download(self, bucket_name, script_uri, target_folder):
+        DSCJob
+            An instance of DSCJob.
 
-        remote_pyspark_file_name = urlparse(script_uri).path[1:]
+        """
+        return super().from_ocid(ocid)
 
-        local_pyspark_file_name = remote_pyspark_file_name
-        if "/" in remote_pyspark_file_name:
-            local_pyspark_file_name = remote_pyspark_file_name.replace("/", "_")
-            if local_pyspark_file_name.endswith(".py"):
-                local_pyspark_file_name = (
-                    local_pyspark_file_name.rstrip(".py")
-                    + "_"
-                    + str(uuid.uuid4())[-6:]
-                    + ".py"
-                )
-            else:
-                local_pyspark_file_name += "_" + str(uuid.uuid4())[-6:]
 
-        destination_pyspark_file = f"{target_folder}/{local_pyspark_file_name}"
+class DataScienceJobRun(
+    OCIDataScienceMixin, oci.data_science.models.JobRun, RunInstance
+):
+    """Represents a Data Science Job run"""
 
-        if not os.path.exists(destination_pyspark_file):
+    _DETAILS_LINK = (
+        "https://console.{region}.oraclecloud.com/data-science/job-runs/{id}"
+    )
 
-            with open(destination_pyspark_file, "wb") as f:
+    TERMINAL_STATES = [
+        oci.data_science.models.JobRun.LIFECYCLE_STATE_SUCCEEDED,
+        oci.data_science.models.JobRun.LIFECYCLE_STATE_FAILED,
+        oci.data_science.models.JobRun.LIFECYCLE_STATE_CANCELED,
+        oci.data_science.models.JobRun.LIFECYCLE_STATE_DELETED,
+    ]
+
+    def create(self) -> DataScienceJobRun:
+        """Creates a job run"""
+        self.load_properties_from_env()
+        res = self.client.create_job_run(
+            self.to_oci_model(oci.data_science.models.CreateJobRunDetails)
+        )
+        self.update_from_oci_model(res.data)
+        return self
 
-                f.write(
-                    self.object_storage_client.get_object(
-                        self.namespace, bucket_name, remote_pyspark_file_name
-                    ).data.content
-                )
+    @property
+    def status(self) -> str:
+        """Lifecycle status
 
-            return destination_pyspark_file
+        Returns
+        -------
+        str
+            Status in a string.
+        """
+        return self.lifecycle_state
 
-        else:
-            raise ValueError(
-                f"The app script file ({remote_pyspark_file_name}) already exists in {target_folder}"
-            )
+    @property
+    def log_id(self) -> str:
+        """The log ID from OCI logging service containing the logs from the job run."""
+        if not self.log_details:
+            return None
+        return self.log_details.log_id
 
-    def _create_or_load_app(
-        self,
-        app_config: dict,
-        file_uri: str,
-        archive_uri: str = None,
-        app_dir: str = None,
-    ) -> object:
-
-        with utils.get_progress_bar(2) as progress:
-            progress.update()
-
-            #
-            # common to load & create
-            #
-
-            self.display_name = app_config["display_name"]
-            self.driver_shape = app_config["driver_shape"]
-            self.executor_shape = app_config["executor_shape"]
-            self.num_executors = app_config["num_executors"]
-            self.logs_bucket_uri = (
-                self.warehouse_bucket_uri
-            ) = f"oci://{app_config['logs_bucket']}@{self.namespace}"
-
-            app_details = CreateApplicationDetails(
-                compartment_id=app_config["compartment_id"],
-                language="PYTHON",
-                display_name=self.display_name,
-                driver_shape=self.driver_shape,
-                executor_shape=self.executor_shape,
-                file_uri=file_uri,
-                archive_uri=archive_uri,
-                logs_bucket_uri=self.logs_bucket_uri,
-                num_executors=self.num_executors,
-                spark_version=app_config.get("spark_version", SPARK_VERSION.v2_4_4),
-                warehouse_bucket_uri=self.warehouse_bucket_uri,
-                arguments=app_config.get("arguments", []),
-                parameters=[
-                    ApplicationParameter(name=k, value=str(v))
-                    for (k, v) in app_config.get("script_parameters", [])
-                ],
-            )
-
-            new_app = self.df_client.create_application(app_details)
-            progress.update("Done")
-            # # add app_config to app obj as an attribute
-            # new_app.data.configuration = app_config
-
-            # make app dir
-            if app_dir is None:
-                app_dir = f"{self.dataflow_base_folder}/{self.display_name}_{str(uuid.uuid4())[-6:]}"
-
-            pathlib.Path(app_dir).mkdir(parents=True, exist_ok=True)
-
-            return DataFlowApp(
-                app_config,
-                new_app,
-                app_dir,
-                f"https://console."
-                f"{self.region}.oraclecloud.com/data-flow/apps/details/{new_app.data.id}",
-                os_auth=self.os_auth,
-                df_auth=self.df_auth,
-            )
-
-    def create_app(
-        self, app_config: dict, overwrite_script=False, overwrite_archive=False
-    ) -> object:
-        """
-        Create a new dataflow application with the supplied app config.
-        app_config contains parameters needed to create a new application,
-        according to oci.data_flow.models.CreateApplicationDetails.
-
-        Parameters
-        ----------
-        app_config: dict
-            the config file that contains all necessary parameters used to create a dataflow app
-        overwrite_script: bool
-            whether to overwrite the existing pyscript script on Object Storage
-        overwrite_archive: bool
-            whether to overwrite the existing archive file on Object Storage
-
-        Returns
-        -------
-        df_app: oci.dataflow.models.Application
-            New dataflow application.
-        """
-        #
-        # upload pyspark_file_path to OCI object storage
-        #
-        try:
-            self._upload(
-                app_config["pyspark_file_path"],
-                app_config["script_bucket"],
-                overwrite=overwrite_script,
-            )
-        except FileOverwriteError:
-            raise ValueError(
-                "You have a file with the same key in your bucket on object storage. Rename your file or set overwrite_script option to True."
-            )
-        script_name = os.path.basename(app_config["pyspark_file_path"])
-        file_uri = f'oci://{app_config["script_bucket"]}@{self.namespace}/{script_name}'
+    @property
+    def log_group_id(self) -> str:
+        """The log group ID from OCI logging service containing the logs from the job run."""
+        if not self.log_details:
+            return None
+        return self.log_details.log_group_id
 
-        # upload archive file to object storage if specified
-        if app_config["archive_path"] is None:
-            return self._create_or_load_app(app_config, file_uri)
-        else:
-            try:
-                self._upload(
-                    app_config["archive_path"],
-                    app_config["archive_bucket"],
-                    overwrite=overwrite_archive,
-                )
-            except FileOverwriteError:
-                raise ValueError(
-                    "You have a file with the same key in your bucket on object storage. Rename your file or set overwrite_archive option to True."
-                )
-            archive_name = os.path.basename(app_config["archive_path"])
-            archive_uri = (
-                f'oci://{app_config["archive_bucket"]}@{self.namespace}/{archive_name}'
-            )
-            return self._create_or_load_app(
-                app_config, file_uri, archive_uri=archive_uri
-            )
+    @property
+    def logging(self) -> OCILog:
+        """The OCILog object containing the logs from the job run"""
+        if not self.log_id:
+            raise ValueError("Log OCID is not specified for this job run.")
+        # Specifying log group ID when initializing OCILog can reduce the number of API calls.
+        return OCILog(id=self.log_id, log_group_id=self.log_details.log_group_id)
 
-    def _upload(self, local_path, bucket_name, overwrite=False):
-        """
-        upload local files to object storage
+    @staticmethod
+    def _format_log(message: str, date_time: datetime.datetime) -> dict:
+        """Formats a message as log record with datetime.
+        This is used to add additional logs to show job run status change.
 
         Parameters
         ----------
-        local_path: str
-            the file path
-        bucket_name: str
-            bucket name on object storage to upload the file
-        overwrite: bool
-            whether to overwrite the existing file on Object Storage
+        message : str
+            Log message.
+        date_time : datetime or str
+            Timestamp for the message
 
         Returns
         -------
-        None
+        dict
+            log record as a dictionary, including id, time and message as keys.
         """
-        object_name = os.path.basename(local_path)
-        if self._check_object_exist(object_name, bucket_name):
-            if not overwrite:
-                raise FileOverwriteError()
-            else:
-                logger.warning(
-                    "You have a file with the same key in your bucket on object storage. It will be overwritten per your request."
-                )
-
-        with open(local_path, "rb") as in_file:
-            self.object_storage_client.put_object(
-                self.namespace, bucket_name, object_name, in_file
-            )
-            logger.info(f"Finished uploading `{object_name}`.")
+        if isinstance(date_time, datetime.datetime):
+            date_time = date_time.strftime("%Y-%m-%dT%H:%M:%S.000Z")
+        return {
+            "id": str(uuid.uuid4()),
+            "message": message,
+            "time": date_time,
+        }
 
-    def _check_object_exist(self, object_name: str, bucket_name: str) -> bool:
-        """
+    def logs(self, limit: int = None) -> list:
+        """Gets the logs of the job run.
 
         Parameters
         ----------
-        object_name: str
-            the file name on object storage
-        bucket_name: str
-            bucket name on object storage
+        limit : int, optional
+            Limit the number of logs to be returned.
+            Defaults to None. All logs will be returned.
 
         Returns
         -------
-        bool
-            whether the file already exists in the bucket in object storage
+        list
+            A list of log records. Each log record is a dictionary with the following keys: id, time, message.
         """
-        object_exist = self._check_object_exist_helper(
-            object_name, bucket_name, start=None
-        )
-
-        if object_exist:
-            logger.info(
-                f"The file object `{object_name}` "
-                f"already exists in bucket `{bucket_name}`."
+        if self.time_accepted:
+            log_messages = self.logging.tail(
+                source=self.id, limit=limit, time_start=self.time_accepted
             )
         else:
-            logger.info(
-                f"The file object `{object_name}` "
-                f"does not exist in bucket `{bucket_name}` and will be uploaded."
-            )
-        return object_exist
+            log_messages = []
+        if self.time_started:
+            log_messages.insert(
+                0, self._format_log("Job Run STARTED", self.time_started)
+            )
+        if self.time_accepted:
+            log_messages.insert(
+                0, self._format_log("Job Run ACCEPTED", self.time_accepted)
+            )
+        if self.time_finished:
+            log_messages.append(
+                self._format_log("Job Run FINISHED", self.time_finished)
+            )
+        return log_messages
+
+    def _job_run_status_text(self) -> str:
+        details = f", {self.lifecycle_details}" if self.lifecycle_details else ""
+        return f"Job Run {self.lifecycle_state}" + details
+
+    def _check_and_print_status(self, prev_status) -> str:
+        status = self._job_run_status_text()
+        if status != prev_status:
+            if self.lifecycle_state in self.TERMINAL_STATES and self.time_finished:
+                timestamp = self.time_finished.strftime("%Y-%m-%d %H:%M:%S")
+            else:
+                timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
+            print(f"{timestamp} - {status}")
+        return status
 
-    def _check_object_exist_helper(
-        self, object_name: str, bucket_name: str, start: str = None
-    ) -> bool:
-        """
+    def watch(
+        self,
+        interval: float = SLEEP_INTERVAL,
+        wait: float = WAIT_SECONDS_AFTER_FINISHED,
+    ) -> DataScienceJobRun:
+        """Watches the job run until it finishes.
+        Before the job start running, this method will output the job run status.
+        Once the job start running,
+        the logs will be streamed until the job is success, failed or cancelled.
 
         Parameters
         ----------
-        object_name: str
-            the file name on object storage
-        bucket_name: str
-            bucket name on object storage
-        start: str
-            Object names returned by a list query must be greater or equal to this parameter.
+        interval : float
+            Time interval in seconds between each request to update the logs.
+            Defaults to 3 (seconds).
+        wait : float
+            Time in seconds to keep updating the logs after the job run finished.
+            It may take some time for logs to appear in OCI logging service
+            after the job run is finished.
+            Defaults to 90 (seconds).
 
-        Returns
-        -------
-        bool
-            whether the file already exists in the bucket in object storage
         """
-        object_exist = False
-        list_objects_response = self.object_storage_client.list_objects(
-            self.namespace, bucket_name, start=start
-        )
 
-        objects_list = list_objects_response.data.objects
-        for object_item in objects_list:
-            if object_item.name == object_name:
-                object_exist = True
+        def stop_condition():
+            """Stops the log streaming once the job is in a terminal state."""
+            self.sync()
+            if self.lifecycle_state not in self.TERMINAL_STATES:
+                return False
+            # Stop if time_finished is not available.
+            if not self.time_finished:
+                return True
+            # Stop only if time_finished is over 2 minute ago.
+            # This is for the time delay between job run stopped and the logs appear in oci logging.
+            if (
+                datetime.datetime.now(self.time_finished.tzinfo)
+                - datetime.timedelta(seconds=wait)
+                > self.time_finished
+            ):
+                return True
+            return False
+
+        if not self.log_id and not self.log_group_id:
+            print(
+                "Logging is not configured for the job. Watch() will only show job status."
+            )
+
+        print(f"Job OCID: {self.job.id}")
+        print(f"Job Run OCID: {self.id}")
+
+        status = ""
+        while not stop_condition():
+            status = self._check_and_print_status(status)
+            # Break and stream logs if job has log ID and started.
+            # Otherwise, keep watching the status until job terminates.
+            if self.time_started and self.log_id:
+                break
+            time.sleep(interval)
+
+        if self.log_id and self.time_accepted:
+            count = self.logging.stream(
+                source=self.id,
+                interval=interval,
+                stop_condition=stop_condition,
+                time_start=self.time_accepted,
+            )
+            if not count:
+                print(
+                    "No logs in the last 14 days. Please set time_start to see older logs."
+                )
 
-        next_start_with = list_objects_response.data.next_start_with
+        self._check_and_print_status(status)
 
-        if object_exist or not next_start_with:
-            return object_exist
-        else:
-            return self._check_object_exist_helper(
-                object_name, bucket_name, start=next_start_with
-            )
-
-    def list_apps(
-        self,
-        include_deleted: bool = False,
-        compartment_id: str = None,
-        datetime_format: str = utils.date_format,
-        **kwargs,
-    ) -> object:
-        """
-        List all apps in a given compartment, or in the current notebook session's compartment.
+        return self
 
-        Parameters
-        ----------
-        include_deleted: bool, optional, default=False
-            Whether to include deleted apps in the returned list.
-        compartment_id: str, optional, default: NB_SESSION_COMPARTMENT_OCID
-            The compartment specified to list apps.
-        datetime_format: str, optional, default: '%Y-%m-%d %H:%M:%S'
-            Change format for date time fields.
+    def cancel(self) -> DataScienceJobRun:
+        """Cancels a job run
+        This method will wait for the job run to be canceled before returning.
 
         Returns
         -------
-        dsl: List
-            List of Dataflow applications.
+        self
+            The job run instance.
         """
-        app_compartment_id = (
-            self.compartment_id if compartment_id is None else compartment_id
-        )
-        list_applications_response = self.df_client.list_applications(
-            app_compartment_id, **kwargs
-        ).data
-
-        # handle empty list
-        if list_applications_response is None:
-            logger.warning("No applications found.")
-            return
+        self.client.cancel_job_run(self.id)
+        while self.lifecycle_state != "CANCELED":
+            self.sync()
+            time.sleep(SLEEP_INTERVAL)
+        return self
 
-        application_list_filtered = [
-            self._decorate_app(app)
-            for app in list_applications_response
-            if include_deleted
-            or Application.lifecycle_state != ApplicationSummary.LIFECYCLE_STATE_DELETED
-        ]
+    def __repr__(self) -> str:
+        """Displays the object as YAML."""
+        return self.to_yaml()
 
-        dsl = SummaryList(
-            entity_list=application_list_filtered,
-            datetime_format=datetime_format,
-        )
-        self.short_id_index.update(dsl.short_id_index)
-        return dsl
+    def to_yaml(self) -> str:
+        """Serializes the object into YAML string.
 
-    def get_app(self, app_id: str):
+        Returns
+        -------
+        str
+            YAML stored in a string.
         """
-        Get the Project based on app_id.
+        # Here the job YAML is used as the base for the job run
+        job_dict = self.job.to_dict()
 
-        Parameters
-        ----------
-        app_id: str, required
-            The OCID of the dataflow app to get.
+        # Update infrastructure from job run
+        run_dict = self.to_dict()
+        infra_specs = [
+            run_dict,
+            run_dict.get("jobInfrastructureConfigurationDetails", {}),
+            run_dict.get("logDetails", {}),
+        ]
+        for infra_spec in infra_specs:
+            for key in infra_spec:
+                if key in job_dict["spec"]["infrastructure"]["spec"]:
+                    job_dict["spec"]["infrastructure"]["spec"][key] = infra_spec[key]
+
+        # Update runtime from job run
+        from ads.jobs import Job
+
+        job = Job.from_dict(job_dict)
+        envs = job.runtime.envs
+        run_config_override = run_dict.get("jobConfigurationOverrideDetails", {})
+        envs.update(run_config_override.get("environmentVariables", {}))
+        job.runtime.with_environment_variable(**envs)
+        if run_config_override.get("commandLineArguments"):
+            job.runtime.set_spec(
+                "args",
+                run_config_override.get("commandLineArguments"),
+            )
+
+        # Update kind, id and name
+        run_dict = job.to_dict()
+        run_dict["kind"] = "jobRun"
+        run_dict["spec"]["id"] = self.id
+        run_dict["spec"]["name"] = self.display_name
+        return yaml.safe_dump(run_dict)
+
+    @property
+    def job(self):
+        """The job instance of this run.
 
         Returns
         -------
-        app: oci.dataflow.models.Application
-            The oci.dataflow.models.Application with the matching ID.
+        Job
+            An ADS Job instance
         """
-        if not app_id.startswith("ocid"):
-            app_id = self.short_id_index[app_id]
+        from ads.jobs import Job
 
-        try:
-            get_app_response = self.df_client.get_application(app_id)
-        except ServiceError as se:
-            if se.status == 404:
-                raise KeyError(se.message) from se
-            else:
-                raise
-        return self._decorate_app(get_app_response.data)
+        return Job.from_datascience_job(self.job_id)
 
-    def load_app(
-        self,
-        app_id: str,
-        target_folder: str = None,
-    ) -> object:
-        """
-        Load an existing dataflow application based on application id.
-        The existing dataflow application can be created either from dataflow
-        service or the dataflow integration of ADS.
+    def download(self, to_dir):
+        """Downloads files from job run output URI to local.
 
         Parameters
         ----------
-        app_id: str, required
-            The OCID of the dataflow app to load.
-
-        target_folder: str, optional,
-            the folder to store the local artifacts of this application.
-            If not specified, the target_folder will use the
-            dataflow_base_folder by default.
+        to_dir : str
+            Local directory to which the files will be downloaded to.
 
         Returns
         -------
-        dfa: ads.dataflow.dataflow.DataFlowApp
-            A dataflow application of type ads.dataflow.dataflow.DataFlowApp
+        DataScienceJobRun
+            The job run instance (self)
         """
+        self.job.download(to_dir)
+        return self
 
-        # support short id when loading an application by getting ocid based on
-        # provided short id
-        if not app_id.startswith("ocid"):
-            app_id = self.short_id_index[app_id]
 
-        # get app response that fetched using df client
-        try:
-            get_app_response = self.df_client.get_application(app_id)
-        except ServiceError as se:
-            if se.status == 404:
-                raise KeyError(se.message) from se
-            else:
-                raise
-
-        # if users try to load a non-python application, we throw a warning
-        if get_app_response.data.language != "PYTHON":
-            logger.warning("ADS only supports Python.")
-            return
+# This is for backward compatibility
+DSCJobRun = DataScienceJobRun
 
-        # for apps created with default logs bucket, logs_bucket_uri attribute in app response will be empty string
-        # set default value manually for logs_bucket
-        if get_app_response.data.logs_bucket_uri == "":
-            logger.info(
-                "Using the default logs bucket 'dataflow-logs'. Set the parameter `logs_bucket_uri` to use a different bucket."
-            )
-            logs_bucket = "dataflow-logs"
-        else:
-            logs_bucket = re.split(r"[@/]", get_app_response.data.logs_bucket_uri)[2]
 
-        # reform app config from app response
-        app_config = {
-            "compartment_id": get_app_response.data.compartment_id,
-            "language": get_app_response.data.language,
-            "script_bucket": re.split(r"[@/]", get_app_response.data.file_uri)[2],
-            "logs_bucket": logs_bucket,
-            "archive_path": None,
-            "archive_bucket": None,
-            "display_name": get_app_response.data.display_name,
-            "driver_shape": get_app_response.data.driver_shape,
-            "executor_shape": get_app_response.data.executor_shape,
-            "num_executors": get_app_response.data.num_executors,
-            "spark_version": get_app_response.data.spark_version,
-            "arguments": get_app_response.data.arguments,
-            "script_parameters": [
-                (param.name, param.value) for param in get_app_response.data.parameters
-            ],
-        }
+class DataScienceJob(Infrastructure):
+    """Represents the OCI Data Science Job infrastructure.
 
-        # set the default value to target_folder to dataflow_base_folder
-        if target_folder is None:
-            target_folder = self.dataflow_base_folder
+    To configure the infrastructure for a Data Science Job::
 
-        app_dir = (
-            f"{target_folder}/{app_config['display_name']}_{str(uuid.uuid4())[-6:]}"
+        infrastructure = (
+            DataScienceJob()
+            # Configure logging for getting the job run outputs.
+            .with_log_group_id("<log_group_ocid>")
+            # Log resource will be auto-generated if log ID is not specified.
+            .with_log_id("<log_ocid>")
+            # If you are in an OCI data science notebook session,
+            # the following configurations are not required.
+            # Configurations from the notebook session will be used as defaults.
+            .with_compartment_id("<compartment_ocid>")
+            .with_project_id("<project_ocid>")
+            .with_subnet_id("<subnet_ocid>")
+            .with_shape_name("VM.Standard.E3.Flex")
+            # Shape config details are applicable only for the flexible shapes.
+            .with_shape_config_details(memory_in_gbs=16, ocpus=1)
+            # Minimum/Default block storage size is 50 (GB).
+            .with_block_storage_size(50)
+            # A list of file systems to be mounted
+            .with_storage_mount(
+                {
+                    "src" : "<mount_target_ip_address>:<export_path>",
+                    "dest" : "<destination_directory_name>"
+                }
+            )
+            # Tags
+            .with_freeform_tag(my_tag="my_value")
+            .with_defined_tag(**{"Operations": {"CostCenter": "42"}})
         )
-        pathlib.Path(app_dir).mkdir(parents=True, exist_ok=True)
 
-        app_config["pyspark_file_path"] = self._download(
-            app_config["script_bucket"], get_app_response.data.file_uri, app_dir
-        )
+    """
 
-        if get_app_response.data.archive_uri != "":
-            app_config["archive_bucket"] = re.split(
-                r"[@/]", get_app_response.data.archive_uri
-            )[2]
-            app_config["archive_path"] = self._download(
-                app_config["archive_bucket"], get_app_response.data.archive_uri, app_dir
-            )
+    CONST_PROJECT_ID = "projectId"
+    CONST_COMPARTMENT_ID = "compartmentId"
+    CONST_DISPLAY_NAME = "displayName"
+    CONST_JOB_TYPE = "jobType"
+    CONST_JOB_INFRA = "jobInfrastructureType"
+    CONST_SHAPE_NAME = "shapeName"
+    CONST_BLOCK_STORAGE = "blockStorageSize"
+    CONST_SUBNET_ID = "subnetId"
+    CONST_SHAPE_CONFIG_DETAILS = "shapeConfigDetails"
+    CONST_MEMORY_IN_GBS = "memoryInGBs"
+    CONST_OCPUS = "ocpus"
+    CONST_LOG_ID = "logId"
+    CONST_LOG_GROUP_ID = "logGroupId"
+    CONST_STORAGE_MOUNT = "storageMount"
+    CONST_FREEFORM_TAGS = "freeformTags"
+    CONST_DEFINED_TAGS = "definedTags"
+
+    attribute_map = {
+        CONST_PROJECT_ID: "project_id",
+        CONST_COMPARTMENT_ID: "compartment_id",
+        CONST_DISPLAY_NAME: "display_name",
+        CONST_JOB_TYPE: "job_type",
+        CONST_JOB_INFRA: "job_infrastructure_type",
+        CONST_SHAPE_NAME: "shape_name",
+        CONST_BLOCK_STORAGE: "block_storage_size",
+        CONST_SUBNET_ID: "subnet_id",
+        CONST_SHAPE_CONFIG_DETAILS: "shape_config_details",
+        CONST_LOG_ID: "log_id",
+        CONST_LOG_GROUP_ID: "log_group_id",
+        CONST_STORAGE_MOUNT: "storage_mount",
+        CONST_FREEFORM_TAGS: "freeform_tags",
+        CONST_DEFINED_TAGS: "defined_tags",
+    }
+
+    shape_config_details_attribute_map = {
+        CONST_MEMORY_IN_GBS: "memory_in_gbs",
+        CONST_OCPUS: "ocpus",
+    }
+
+    payload_attribute_map = {
+        CONST_PROJECT_ID: "project_id",
+        CONST_COMPARTMENT_ID: "compartment_id",
+        CONST_DISPLAY_NAME: "display_name",
+        CONST_JOB_TYPE: "job_configuration_details.job_type",
+        CONST_JOB_INFRA: "job_infrastructure_configuration_details.job_infrastructure_type",
+        CONST_SHAPE_NAME: "job_infrastructure_configuration_details.shape_name",
+        CONST_BLOCK_STORAGE: "job_infrastructure_configuration_details.block_storage_size_in_gbs",
+        CONST_SUBNET_ID: "job_infrastructure_configuration_details.subnet_id",
+        CONST_SHAPE_CONFIG_DETAILS: "job_infrastructure_configuration_details.job_shape_config_details",
+        CONST_LOG_ID: "job_log_configuration_details.log_id",
+        CONST_LOG_GROUP_ID: "job_log_configuration_details.log_group_id",
+    }
+
+    snake_to_camel_map = {
+        v.split(".", maxsplit=1)[-1]: k for k, v in payload_attribute_map.items()
+    }
+
+    storage_mount_type_dict = {
+        FILE_STORAGE_TYPE: OCIFileStorage,
+        OBJECT_STORAGE_TYPE: OCIObjectStorage,
+    }
+
+    @staticmethod
+    def standardize_spec(spec):
+        if not spec:
+            return {}
+
+        attribute_map = {
+            **DataScienceJob.attribute_map,
+            **DataScienceJob.shape_config_details_attribute_map,
+        }
+        snake_to_camel_map = {v: k for k, v in attribute_map.items()}
+        snake_to_camel_map = {
+            **{v: k for k, v in attribute_map.items()},
+            **DataScienceJob.snake_to_camel_map,
+        }
 
-        return DataFlowApp(
-            app_config,
-            get_app_response,
-            app_dir,
-            f"https://console.{self.region}.oraclecloud.com/data-flow/apps/details/{get_app_response.data.id}",
-            os_auth=self.os_auth,
-            df_auth=self.df_auth,
-        )
+        for key in list(spec.keys()):
+            if key not in attribute_map and key.lower() in snake_to_camel_map:
+                value = spec.pop(key)
+                if isinstance(value, dict):
+                    spec[
+                        snake_to_camel_map[key.lower()]
+                    ] = DataScienceJob.standardize_spec(value)
+                else:
+                    spec[snake_to_camel_map[key.lower()]] = value
+        return spec
 
+    def __init__(self, spec: Dict = None, **kwargs) -> None:
+        """Initializes a data science job infrastructure
 
-class DataFlowApp(DataFlow):
-    @deprecated("2.6.3")
-    def __init__(self, app_config, app_response, app_dir, oci_link, **kwargs):
-        super().__init__(compartment_id=app_config["compartment_id"], **kwargs)
-        self._config = app_config
-        self.app_response = app_response
-        self.app_dir = app_dir
-        self._oci_link = oci_link
-
-    def __iter__(self):
-        return self.list_runs().__iter__()
-
-    def __len__(self):
-        return len(self.list_runs())
-
-    def __repr__(self):
-        return self._config["display_name"]
-
-    def _decorate_run(self, run):
-        run.swagger_types["short_id"] = "str"
-        run.ocid = run.id
-
-        def to_dataframe(run_self):
-            if "arguments" in run_attributes:
-                run_attributes.remove("arguments")
-            df = DataFrame.from_dict(
-                {
-                    key: getattr(run_self, key)
-                    for key in run_attributes
-                    if hasattr(run_self, key)
-                },
-                orient="index",
-                columns=[""],
-            )
-            return df
+        Parameters
+        ----------
+        spec : dict, optional
+            Object specification, by default None
+        kwargs: dict
+            Specification as keyword arguments.
+            If spec contains the same key as the one in kwargs, the value from kwargs will be used.
+        """
+        self.standardize_spec(spec)
+        self.standardize_spec(kwargs)
+        super().__init__(spec=spec, **kwargs)
+        if not self.job_type:
+            self.with_job_type("DEFAULT")
+        self.dsc_job = DSCJob()
+        self.runtime = None
+        self._name = None
 
-        @runtime_dependency(module="IPython", install_from=OptionalDependency.NOTEBOOK)
-        def show_in_notebook(run_self):
-            """
-            Describe the project by showing it's properties
-            """
-            from IPython.display import display
-
-            display(run_self)
-
-        def _repr_html_(run_self):
-            return (
-                run_self.to_dataframe()
-                .style.set_properties(**{"margin-left": "0px"})
-                .render()
-            )
-
-        run.to_dataframe = MethodType(to_dataframe, run)
-        run.show_in_notebook = MethodType(show_in_notebook, run)
-        run._repr_html_ = MethodType(_repr_html_, run)
+    @property
+    def name(self) -> str:
+        """Display name of the job"""
+        if self.dsc_job:
+            self._name = self.dsc_job.display_name
+        return self._name
 
-        return run
+    @name.setter
+    def name(self, value: str):
+        """Sets the display name of the job
 
-    @property
-    def config(self) -> dict:
+        Parameters
+        ----------
+        value : str
+            The display name of the job
         """
-        Retrieve the app_config file used to create the data flow app
+        self._name = value
+        if self.dsc_job:
+            self.dsc_job.display_name = value
 
-        Returns
-        -------
-        app_config: Dict
-            dictionary containing all the validated params for this DataFlowApp
-        """
-        return self._config
+    @property
+    def job_id(self) -> Optional[str]:
+        """The OCID of the job"""
+        if self.dsc_job:
+            return self.dsc_job.id
+        return None
 
     @property
-    def oci_link(self) -> object:
-        """
-        Retrieve the oci link of the data flow app
+    def status(self) -> Optional[str]:
+        """Status of the job.
 
         Returns
         -------
-        oci_link: str
-            a link to the app page in an oci console.
+        str
+            Status of the job.
         """
-        return self._oci_link
+        if self.dsc_job:
+            return self.dsc_job.lifecycle_state
+        return None
 
-    def prepare_run(
-        self,
-        run_display_name: str,
-        compartment_id: str = None,
-        logs_bucket: str = "",
-        driver_shape: str = "VM.Standard2.4",
-        executor_shape: str = "VM.Standard2.4",
-        num_executors: int = 1,
-        **kwargs,
-    ) -> dict:
-        """
-        Check if the parameters provided by users to create a run are
-        valid and then prepare run_config for creating run details.
+    def with_project_id(self, project_id: str) -> DataScienceJob:
+        """Sets the project OCID
 
         Parameters
         ----------
-        run_display_name: str
-            A user-friendly name. This name is not necessarily unique.
-        compartment_id: str
-            OCID of the compartment to create a dataflow run. If not
-            provided, compartment_id will use the same as the dataflow app.
-        logs_bucket: str
-            bucket in object storage to put run logs, if not provided,
-            will use the same logs_bucket as defined in app_config
-        driver_shape: str
-            The value to assign to the driver_shape property of this
-            CreateApplicationDetails.
-            Allowed values for this property are: "VM.Standard2.1",
-            "VM.Standard2.2", "VM.Standard2.4", "VM.Standard2.8",
-            "VM.Standard2.16", "VM.Standard2.24".
-        executor_shape: str
-            The value to assign to the executor_shape property of this
-            CreateApplicationDetails.
-            Allowed values for this property are: "VM.Standard2.1",
-            "VM.Standard2.2", "VM.Standard2.4", "VM.Standard2.8",
-            "VM.Standard2.16", "VM.Standard2.24".
-        num_executors: int
-            The number of executor VMs requested.
+        project_id : str
+            The project OCID
 
         Returns
         -------
-        run_config: Dict
-            Dictionary containing all the validated params for CreateRunDetails.
-        """
-        # if logs_bucket not provided to prepare run_config, will use the
-        # same logs_bucket as defined in app_config
-        if logs_bucket == "":
-            logs_bucket = self.config["logs_bucket"]
-        if not self._check_bucket_exist(logs_bucket):
-            raise ValueError(
-                "The log bucket {} does not exist in object storage".format(logs_bucket)
-            )
-        else:
-            logs_bucket_uri = f"oci://{logs_bucket}@{self.namespace}"
-
-        if not isinstance(run_display_name, str):
-            raise TypeError("param 'run_display_name' must be string")
-
-        if not isinstance(driver_shape, str):
-            raise TypeError("param 'driver_shape' must be string")
-        elif driver_shape not in self.VM_shapes:
-            raise ValueError("param 'driver_shape' is not a valid VM shape")
-
-        if not isinstance(executor_shape, str):
-            raise TypeError("param 'executor_shape' must be string")
-        elif executor_shape not in self.VM_shapes:
-            raise ValueError("param 'executor_shape' is not a valid VM shape")
-
-        if not isinstance(num_executors, int):
-            raise TypeError("param 'num_executors' must be integer")
-        elif num_executors < 1:
-            raise ValueError("param 'num_executors' has a minimum value of 1")
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-        run_compartment_id = (
-            self.compartment_id if compartment_id is None else compartment_id
-        )
-
-        run_configuration = {
-            "compartment_id": run_compartment_id,
-            "script_bucket": self._config["script_bucket"],
-            "pyspark_file_path": self._config["pyspark_file_path"],
-            "archive_path": self._config["archive_path"],
-            "archive_bucket": self._config["archive_bucket"],
-            "run_display_name": run_display_name,
-            "logs_bucket": logs_bucket,
-            "logs_bucket_uri": logs_bucket_uri,
-            "driver_shape": driver_shape,
-            "executor_shape": executor_shape,
-            "num_executors": num_executors,
-        }
-
-        # get arguments from app config
-        if "arguments" in self._config:
-            run_configuration["arguments"] = list(self._config["arguments"])
-
-        # get script parameters in app config
-        if "script_parameters" in self._config:
-            run_configuration["script_parameters"] = list(
-                self._config["script_parameters"]
-            )
-
-        # update the new value of the argument in the run config when user provides new name value pairs
-        if kwargs:
-            # convert script parameters into dict
-            param_dict = dict(run_configuration["script_parameters"])
-            for param, value in kwargs.items():
-                # overwrite the value
-                if param in param_dict:
-                    param_dict[param] = value
-                else:
-                    raise KeyError(f"{param} is not a valid key in script parameters")
+        """
+        return self.set_spec(self.CONST_PROJECT_ID, project_id)
 
-            # convert param_dict back to list of tuples
-            run_configuration["script_parameters"] = [
-                (k, param_dict[k]) for k in param_dict
-            ]
+    @property
+    def project_id(self) -> Optional[str]:
+        """Project OCID"""
+        return self.get_spec(self.CONST_PROJECT_ID)
 
-        return run_configuration
-
-    def run(
-        self,
-        run_config: dict,
-        save_log_to_local: bool = False,
-        copy_script_to_object_storage: bool = True,
-        copy_archive_to_object_storage: bool = True,
-        pyspark_file_path: str = None,
-        archive_path: str = None,
-        wait: bool = True,
-    ) -> object:
-        """
-        Create a new dataflow run with the supplied run config.
-        run_config contains parameters needed to create a new run, according to oci.data_flow.models.CreateRunDetails.
+    def with_compartment_id(self, compartment_id: str) -> DataScienceJob:
+        """Sets the compartment OCID
 
         Parameters
         ----------
-        run_config: dict, required
-            The config file that contains all necessary parameters used to create a dataflow run
-        save_log_to_local: bool, optional
-            A boolean value that defaults to false. If set to true, it saves the log files to local dir
-        copy_script_to_object_storage: bool, optional
-            A boolean value that defaults to true. Local script will be copied to object storage
-        copy_archive_to_object_storage: bool, optional
-            A boolean value that defaults to true. Local archive file will be copied to object storage
-        pyspark_file_path: str, optional
-            The pyspark file path used for creating the dataflow app.
-            if pyspark_file_path isn't specified then reuse the path that the app was created with.
-        archive_path: str, optional
-            The archive file path used for creating the dataflow app.
-            if archive_path isn't specified then reuse the path that the app was created with.
-        wait: bool, optional
-            A boolean value that defaults to true.
-            When True, the return will be ads.dataflow.dataflow.DataFlowRun in terminal state.
-            When False, the return will be a ads.dataflow.dataflow.RunObserver.
+        compartment_id : str
+            The compartment OCID
 
         Returns
         -------
-        df_run: Variable
-            Either a new Data Flow run or a run observer.
-        """
-
-        if copy_script_to_object_storage:
-            self._sync(pyspark_file_path)
-
-        if run_config["archive_path"] is not None:
-            if copy_archive_to_object_storage:
-                self._sync(archive_path, type="archive")
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-        run_observer = RunObserver(self, run_config, save_log_to_local)
+        """
+        return self.set_spec(self.CONST_COMPARTMENT_ID, compartment_id)
 
-        if wait:
-            return run_observer.wait()  # blocks, returns DataFlowRun
-        else:
-            return run_observer  # unblocks, returns RunObserver
+    @property
+    def compartment_id(self) -> Optional[str]:
+        """The compartment OCID"""
+        return self.get_spec(self.CONST_COMPARTMENT_ID)
 
-    def _sync(self, file_path: str = None, type: str = "script") -> object:
-        """
-        Push to create a new app if the script has been modified.
+    def with_job_type(self, job_type: str) -> DataScienceJob:
+        """Sets the job type
 
         Parameters
         ----------
-        file_path: str
-            The pyspark file path used for creating the dataflow app.
-            if pyspark_file_path isn't specified then reuse the path that the app was created with.
-        type: str, only two types supported here, 'script' or 'archive'
+        job_type : str
+            Job type as string
 
         Returns
         -------
-        Self, a Data Flow app object.
-        """
-
-        # local pyspark file, which may or may not be modified
-        if type == "script":
-            file_path = (
-                self.config["pyspark_file_path"] if file_path is None else file_path
-            )
-
-            # compare byte content of two files
-            # script no diff, return the original app obj
-            if not self._modified(file_path, type="script"):
-                return self
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-            os_bucket = self.config["script_bucket"]
-            os_objectname = self.config["pyspark_file_path"].rsplit("/")[-1]
-
-        elif type == "archive":
-            file_path = self.config["archive_path"] if file_path is None else file_path
-            if not self._modified(file_path, type="archive"):
-                return self
+        """
+        return self.set_spec(self.CONST_JOB_TYPE, job_type)
 
-            os_bucket = self.config["archive_bucket"]
-            os_objectname = self.config["archive_path"].rsplit("/")[-1]
+    @property
+    def job_type(self) -> Optional[str]:
+        """Job type"""
+        return self.get_spec(self.CONST_JOB_TYPE)
 
-        # push file to object storage
-        with open(file_path, "rb") as in_file:
-            try:
-                self.object_storage_client.put_object(
-                    self.namespace,
-                    os_bucket,
-                    os_objectname,
-                    in_file,
-                )
-                logger.info(
-                    f"The existing file `{os_objectname}` in bucket "
-                    f"`{os_bucket}` on object storage has been overwritten by your latest changes of "
-                    f"`{os_objectname}`."
-                )
-            except ServiceError as se:
-                if se.status == 404:
-                    raise KeyError(se.message) from se
-                else:
-                    raise
-        return self
+    def with_job_infrastructure_type(self, infrastructure_type: str) -> DataScienceJob:
+        """Sets the job infrastructure type
 
-    def _modified(
-        self, file_path: str = None, type: str = "script", encoding="utf8"
-    ) -> bool:
-        """
-        Check if any modification in the pyspark script
+        Parameters
+        ----------
+        infrastructure_type : str
+            Job infrastructure type as string
 
         Returns
         -------
-        True or False
+        DataScienceJob
+            The DataScienceJob instance (self)
+
         """
-        # read local python file into bytes
-        if type == "script":
-            bucket_name = self.config["script_bucket"]
-            # remote pyspark file, which was pushed originally while creating this dataflow app
-            remote_file_name = Path(self.config["pyspark_file_path"]).name.lstrip("/")
-        elif type == "archive":
-            bucket_name = self.config["archive_bucket"]
-            remote_file_name = Path(self.config["archive_path"]).name.lstrip("/")
-        local_file = open(file_path, "rb").read()
+        return self.set_spec(self.CONST_JOB_INFRA, infrastructure_type)
 
-        # remote_file_name = Path(self.config["pyspark_file_path"]).name.lstrip('/')
+    @property
+    def job_infrastructure_type(self) -> Optional[str]:
+        """Job infrastructure type"""
+        return self.get_spec(self.CONST_JOB_INFRA)
 
-        try:
-            remote_file = self.object_storage_client.get_object(
-                self.namespace, bucket_name, remote_file_name
-            ).data.content
-        except ServiceError as se:
-            if se.code == "ObjectNotFound":
-                local_filename = os.path.basename(file_path)
-                logger.info(
-                    f"The `{local_filename}` is "
-                    f"not found in your bucket. "
-                    f"The `{local_filename}` will be uploaded"
-                )
+    def with_shape_name(self, shape_name: str) -> DataScienceJob:
+        """Sets the shape name for running the job
 
-                with open(file_path, "rb") as in_file:
-                    self.object_storage_client.put_object(
-                        self.namespace, bucket_name, local_filename, in_file
-                    )
+        Parameters
+        ----------
+        shape_name : str
+            Shape name
 
-                return False
-            else:
-                raise se
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-        if type == "archive":
-            return local_file != remote_file
+        """
+        return self.set_spec(self.CONST_SHAPE_NAME, shape_name)
 
-        elif type == "script":
-            if isinstance(local_file, bytes):
-                local_file = local_file.decode(encoding)
-            if isinstance(remote_file, bytes):
-                remote_file = remote_file.decode(encoding)
-            return local_file != remote_file
+    @property
+    def shape_name(self) -> Optional[str]:
+        """Shape name"""
+        return self.get_spec(self.CONST_SHAPE_NAME)
 
-    def list_runs(
-        self,
-        include_failed: bool = False,
-        datetime_format: str = utils.date_format,
-        **kwargs,
-    ) -> object:
-        """
-        List all run of a dataflow app
+    def with_block_storage_size(self, size_in_gb: int) -> DataScienceJob:
+        """Sets the block storage size in GB
 
         Parameters
         ----------
-        include_failed: bool, optional, default=False
-            Whether to include failed runs in the returned list
-        datetime_format: str, optional, default: '%Y-%m-%d %H:%M:%S'
-            Change format for date time fields
+        size_in_gb : int
+            Block storage size in GB
 
         Returns
         -------
-        df_runs: List
-            List of Data flow runs.
-        """
-
-        list_runs_response = self.df_client.list_runs(
-            self.compartment_id, **kwargs
-        ).data
-
-        # handle empty list
-        if list_runs_response is None:
-            logger.warning("No runs found.")
-            return
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-        run_list_filtered = [
-            self._decorate_run(run)
-            for run in list_runs_response
-            if include_failed
-            or Run.lifecycle_state != RunSummary.LIFECYCLE_STATE_FAILED
-        ]
+        """
+        return self.set_spec(self.CONST_BLOCK_STORAGE, size_in_gb)
 
-        rsl = SummaryList(
-            entity_list=run_list_filtered, datetime_format=datetime_format
-        )
-        self.short_id_index.update(rsl.short_id_index)
-        return rsl
+    @property
+    def block_storage_size(self) -> int:
+        """Block storage size for the job"""
+        return self.get_spec(self.CONST_BLOCK_STORAGE)
 
-    def get_run(self, run_id: str):
-        """
-        Get the Run based on run_id
+    def with_subnet_id(self, subnet_id: str) -> DataScienceJob:
+        """Sets the subnet ID
 
         Parameters
         ----------
-        run_id: str, required
-            The OCID of the dataflow run to get.
+        subnet_id : str
+            Subnet ID
 
         Returns
         -------
-        df_run: oci.dataflow.models.Run
-            The oci.dataflow.models.Run with the matching ID.
-        """
-        if not run_id.startswith("ocid"):
-            run_id = self.short_id_index[run_id]
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-        try:
-            get_run_response = self.df_client.get_run(run_id)
-        except ServiceError as se:
-            if se.status == 404:
-                raise KeyError(se.message) from se
-            else:
-                raise
-        return self._decorate_run(get_run_response.data)
+        """
+        return self.set_spec(self.CONST_SUBNET_ID, subnet_id)
 
+    @property
+    def subnet_id(self) -> str:
+        """Subnet ID"""
+        return self.get_spec(self.CONST_SUBNET_ID)
+
+    def with_shape_config_details(
+        self, memory_in_gbs: float, ocpus: float, **kwargs: Dict[str, Any]
+    ) -> DataScienceJob:
+        """Sets the details for the job run shape configuration.
+        Specify only when a flex shape is selected.
+        For example `VM.Standard.E3.Flex` allows the memory_in_gbs and cpu count to be specified.
 
-class RunObserver:
-    @deprecated("2.6.3")
-    def __init__(self, app, run_config, save_log_to_local):
-        self.app = app
-        self._config = run_config
-        self.save_log_to_local = save_log_to_local
+        Parameters
+        ----------
+        memory_in_gbs: float
+            The size of the memory in GBs.
+        ocpus: float
+            The OCPUs count.
+        kwargs
+            Additional keyword arguments.
 
-        self._local_dir = self._create_run_dir()
-        self._run_details = self._get_run_details()
-        self._new_run = self.app.df_client.create_run(self._run_details)
-        self._oci_link = f"https://console.{self.app.region}.oraclecloud.com/data-flow/runs/details/{self._new_run.data.id}"
-        self._save_log_to_local = save_log_to_local
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        return self.set_spec(
+            self.CONST_SHAPE_CONFIG_DETAILS,
+            {
+                self.CONST_OCPUS: ocpus,
+                self.CONST_MEMORY_IN_GBS: memory_in_gbs,
+                **kwargs,
+            },
+        )
 
-    def __repr__(self):
-        return self._config["run_display_name"] + " " + self.status
+    @property
+    def shape_config_details(self) -> Dict:
+        """The details for the job run shape configuration."""
+        return self.get_spec(self.CONST_SHAPE_CONFIG_DETAILS)
 
-    def wait(self):
-        """
-        Wait and monitor the run creation process.
+    def with_log_id(self, log_id: str) -> DataScienceJob:
+        """Sets the log OCID for the data science job.
+        If log ID is specified, setting the log group ID (with_log_group_id()) is not strictly needed.
+        ADS will look up the log group ID automatically.
+        However, this may require additional permission,
+        and the look up may not be available for newly created log group.
+        Specifying both log ID (with_log_id()) and log group ID (with_log_group_id())
+        can avoid such lookup and speed up the job creation.
 
         Parameters
         ----------
-        None
+        log_id : str
+            Log resource OCID.
 
         Returns
         -------
-        df_run: oci.dataflow.models.Run
-            The oci.dataflow.models.Run after monitoring is done.
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        # monitor the run creation process
-        self._monitor_run()
-        self._create_run_dir()
+        return self.set_spec(self.CONST_LOG_ID, log_id)
 
-        return DataFlowRun(
-            self._config,
-            self._new_run,
-            self.save_log_to_local,
-            self._local_dir,
-            os_auth=self.app.os_auth,
-            df_auth=self.app.df_auth,
-        )
-
-    def _terminal_state(self, status):
-        return status in ["SUCCEEDED", "FAILED", "CANCELED"]
+    @property
+    def log_id(self) -> str:
+        """Log OCID for the data science job.
 
-    # this is a blocking function, it will only complete when dataflow run reaches terminal state
-    def _monitor_run(self):
-        curr_status = self.status
-        if not self._terminal_state(curr_status):
-
-            # when wait is called after the run being submitted, progress bar does not start from the beginning
-            if curr_status == "ACCEPTED":
-                progress_bar_num = 3
-            elif curr_status == "IN_PROGRESS":
-                progress_bar_num = 2
-            elif curr_status == "SUCCEEDED":
-                progress_bar_num = 1
-            else:
-                progress_bar_num = 4
+        Returns
+        -------
+        str
+            Log OCID
+        """
+        return self.get_spec(self.CONST_LOG_ID)
 
-            with utils.get_progress_bar(progress_bar_num) as progress:
-                progress.update()
-                while not self._terminal_state(curr_status):
-                    time.sleep(2)
-                    new_status = self.status
-                    if new_status != curr_status:
-                        progress.update(f"{new_status}")
-                        curr_status = new_status
-                progress.update("Done")
-
-    def _create_run_dir(self):
-
-        creation_time = datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
-        local_dir = (
-            f"{self.app.app_dir}/{self._config['run_display_name']}-{creation_time}"
-        )
-        pathlib.Path(local_dir).mkdir(parents=True, exist_ok=True)
+    def with_log_group_id(self, log_group_id: str) -> DataScienceJob:
+        """Sets the log group OCID for the data science job.
+        If log group ID is specified but log ID is not,
+        a new log resource will be created automatically for each job run to store the logs.
 
-        # add pyspark script for the run in the run dir
-        user_pyspark_file_path = self._config["pyspark_file_path"]
-        filename = os.path.basename(user_pyspark_file_path)
-        run_pyspark_file_path = os.path.join(local_dir, filename)
-
-        # copy content
-        from shutil import copyfile
-
-        copyfile(user_pyspark_file_path, run_pyspark_file_path)
-
-        # add run metadata for the run in the run dir
-        run_config_path = os.path.join(local_dir, "run_metadata.json")
-        with open(run_config_path, "w") as fp:
-            json.dump(self._config, fp)
-
-        return local_dir
-
-    def _get_run_details(self):
-        self.run_display_name = self._config["run_display_name"]
-        self.logs_bucket_uri = self._config["logs_bucket_uri"]
-        self.driver_shape = self._config["driver_shape"]
-        self.executor_shape = self._config["executor_shape"]
-        self.num_executors = self._config["num_executors"]
-
-        run_details = CreateRunDetails(
-            application_id=self.app.app_response.data.id,
-            compartment_id=self._config["compartment_id"],
-            display_name=self.run_display_name,
-            logs_bucket_uri=self.logs_bucket_uri,
-            driver_shape=self.driver_shape,
-            executor_shape=self.executor_shape,
-            num_executors=self.num_executors,
-            arguments=self._config.get("arguments", []),
-            parameters=[
-                ApplicationParameter(name=k, value=str(v))
-                for (k, v) in self._config.get("script_parameters", [])
-            ],
-        )
-        return run_details
+        Parameters
+        ----------
+        log_group_id : str
+            Log Group OCID
 
-    @property
-    def status(self) -> str:
-        """
-        Returns the lifecycle state of the Data Flow run
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        return self.app.df_client.get_run(self._new_run.data.id).data.lifecycle_state
+        return self.set_spec(self.CONST_LOG_GROUP_ID, log_group_id)
 
     @property
-    def config(self) -> dict:
-        """
-        Retrieve the run_config file used to create the data flow run
+    def log_group_id(self) -> str:
+        """Log group OCID of the data science job
 
         Returns
         -------
-        run_config: Dict
-            Dictionary containing all the validated parameters for this Data Flow run
+        str
+            Log group OCID
         """
-        return self._config
+        return self.get_spec(self.CONST_LOG_GROUP_ID)
 
-    def update_config(self, param_dict) -> None:
-        """
-        Modify the run_config file used to create the data flow run
+    def with_storage_mount(self, *storage_mount: List[dict]) -> DataScienceJob:
+        """Sets the file systems to be mounted for the data science job.
+        A maximum number of 5 file systems are allowed to be mounted for a single data science job.
 
         Parameters
         ----------
-        param_dict: Dict
-            dictionary containing the key value pairs of the run_config parameters and
-            the updated values.
+        storage_mount : List[dict]
+            A list of file systems to be mounted.
 
         Returns
         -------
-        None
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        for key, val in param_dict.items():
-            if key in self._config:
-                self._config[key] = val
-            else:
+        storage_mount_list = []
+        for item in storage_mount:
+            if not isinstance(item, dict):
                 raise ValueError(
-                    "The key '{}' does not exist in run_config parameters".format(key)
+                    "Parameter `storage_mount` should be a list of dictionaries."
                 )
+            storage_mount_list.append(item)
+        if len(storage_mount_list) > MAXIMUM_MOUNT_COUNT:
+            raise ValueError(
+                f"A maximum number of {MAXIMUM_MOUNT_COUNT} file systems are allowed to be mounted at this time for a job."
+            )
+        return self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount_list)
 
     @property
-    def local_dir(self) -> str:
-        """
-        Retrieve the local directory of the data flow run
+    def storage_mount(self) -> List[dict]:
+        """Files systems that have been mounted for the data science job
 
         Returns
         -------
-        local_dir: str
-            the local path to the Data Flow run
+        list
+            A list of file systems that have been mounted
         """
-        return self._local_dir
+        return self.get_spec(self.CONST_STORAGE_MOUNT, [])
 
-    @property
-    def oci_link(self) -> object:
-        """
-        Retrieve the oci link of the data flow run
+    def with_freeform_tag(self, **kwargs) -> DataScienceJob:
+        """Sets freeform tags
 
         Returns
         -------
-        oci_link: str
-            link to the run page in an oci console
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        return self._oci_link
+        return self.set_spec(self.CONST_FREEFORM_TAGS, kwargs)
 
+    def with_defined_tag(self, **kwargs) -> DataScienceJob:
+        """Sets defined tags
 
-class DataFlowRun(DataFlow):
-    LOG_OUTPUTS = ["stdout", "stderr"]
-
-    @deprecated("2.6.3")
-    def __init__(
-        self, run_config, run_response, save_log_to_local, local_dir, **kwargs
-    ):
-        super().__init__(compartment_id=run_config["compartment_id"], **kwargs)
-        self._config = run_config
-        self.run_response = run_response
-        self.run_id = self.run_response.data.id
-        self._log_stdout = None
-        self._log_stderr = None
-        self._local_dir = local_dir
-        self._status = self.df_client.get_run(self.run_id).data.lifecycle_state
-        self._oci_link = None
-        if save_log_to_local:
-            for log_type in DataFlowRun.LOG_OUTPUTS:
-                self.fetch_log(log_type).save()
+        Returns
+        -------
+        DataScienceJob
+            The DataScienceJob instance (self)
+        """
+        return self.set_spec(self.CONST_DEFINED_TAGS, kwargs)
 
-    def __repr__(self):
-        return self._config["run_display_name"]
+    @property
+    def freeform_tags(self) -> dict:
+        """Freeform tags"""
+        return self.get_spec(self.CONST_FREEFORM_TAGS, {})
 
     @property
-    def config(self) -> dict:
-        """
-        Retrieve the run_config file used to create the Data Flow run
+    def defined_tags(self) -> dict:
+        """Defined tags"""
+        return self.get_spec(self.CONST_DEFINED_TAGS, {})
+
+    def _prepare_log_config(self) -> dict:
+        if not self.log_group_id and not self.log_id:
+            return None
+        # Look up log group ID if only the log ID is specified
+        if self.log_id and not self.log_group_id:
+            try:
+                log_obj = OCILog.from_ocid(self.log_id)
+            except ResourceNotFoundError as exc:
+                raise ResourceNotFoundError(
+                    f"Unable to determine log group ID for Log ({self.log_id})."
+                    " The log resource may not exist or You may not have the required permission."
+                    " Try to avoid this by specifying the log group ID."
+                ) from exc
+            self.with_log_group_id(log_obj.log_group_id)
 
-        Returns
-        -------
-        run_config: Dict
-            dictionary containing all the validated params for this DataFlowRun
-        """
-        return self._config
+        if self.log_group_id and not self.log_id:
+            enable_auto_log_creation = True
+        else:
+            enable_auto_log_creation = False
 
-    def update_config(self, param_dict) -> None:
-        """
-        Modify the run_config file used to create the data flow run
+        log_config = {
+            "enable_logging": True,
+            "enable_auto_log_creation": enable_auto_log_creation,
+        }
+        if self.log_id:
+            log_config["log_id"] = self.log_id
+
+        if self.log_group_id:
+            log_config["log_group_id"] = self.log_group_id
+        return log_config
+
+    def _update_from_dsc_model(
+        self, dsc_job: oci.data_science.models.Job, overwrite: bool = True
+    ) -> DataScienceJob:
+        """Update the properties from an OCI data science job model.
 
         Parameters
         ----------
-        param_dict: Dict
-            Dictionary containing the key value pairs of the run_config parameters and
-            the updated values.
+        dsc_job: oci.data_science.models.Job
+            An OCI data science job model.
+
+        overwrite: bool
+            Whether to overwrite the existing values.
+            If this is set to False, only the empty/None properties will be updated.
 
         Returns
         -------
-        None
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        for key, val in param_dict.items():
-            if key in self._config:
-                self._config[key] = val
+        sub_level = {
+            self.CONST_SHAPE_CONFIG_DETAILS: self.shape_config_details_attribute_map
+        }
+        self.dsc_job = dsc_job
+
+        for infra_attr, dsc_attr in self.payload_attribute_map.items():
+            value = get_value(dsc_job, dsc_attr)
+            if not value:
+                continue
+            if infra_attr not in sub_level:
+                if overwrite or not self._spec.get(infra_attr):
+                    self._spec[infra_attr] = value
             else:
-                raise ValueError(
-                    "The key '{}' does not exist in run_config parameters".format(key)
-                )
+                sub_spec = self._spec.get(infra_attr, {})
+                self._spec[infra_attr] = {}
+                for sub_infra_attr, sub_dsc_attr in sub_level[infra_attr].items():
+                    sub_value = get_value(value, sub_dsc_attr)
+                    if not sub_value:
+                        continue
+                    if overwrite or not sub_spec.get(sub_infra_attr):
+                        sub_spec[sub_infra_attr] = sub_value
+                if sub_spec:
+                    self._spec[infra_attr] = sub_spec
 
-    @property
-    def status(self) -> str:
-        """
-        Retrieve the status of the data flow run
+        self._update_storage_mount_from_dsc_model(dsc_job, overwrite)
+        return self
 
-        Returns
-        -------
-        status: str
-            String that describes the status of the run
-        """
-        return self._status
+    def _update_storage_mount_from_dsc_model(
+        self, dsc_job: oci.data_science.models.Job, overwrite: bool = True
+    ) -> DataScienceJob:
+        """Update the mount storage properties from an OCI data science job model.
 
-    @property
-    def log_stdout(self) -> object:
-        """
-        Retrieve the stdout of the data flow run
+        Parameters
+        ----------
+        dsc_job: oci.data_science.models.Job
+            An OCI data science job model.
+
+        overwrite: bool
+            Whether to overwrite the existing values.
+            If this is set to False, only the empty/None properties will be updated.
 
         Returns
         -------
-        log_out: ads.dataflow.dataflow.DataFlowLog
-            a clickable link that opens the stdout log in another tab in a JupyterLab notebook environment
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        if self._log_stdout is None:
-            self._log_stdout = self.fetch_log("stdout")
-        return self._log_stdout
+        storage_mount_list = get_value(
+            dsc_job, "job_storage_mount_configuration_details_list"
+        )
+        if storage_mount_list:
+            storage_mount = [
+                self.storage_mount_type_dict[
+                    file_system.storage_type
+                ].update_from_dsc_model(file_system)
+                for file_system in storage_mount_list
+                if file_system.storage_type in self.storage_mount_type_dict
+            ]
+            if overwrite or not self.get_spec(self.CONST_STORAGE_MOUNT):
+                self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount)
+        return self
 
-    @property
-    def log_stderr(self) -> object:
-        """
-        Retrieve the stderr of the data flow run
+    def _update_job_infra(self, dsc_job: DSCJob) -> DataScienceJob:
+        """Updates the job infrastructure from a DSCJob object.
+
+        Parameters
+        ----------
+        dsc_job : DSCJob
+            A DSCJob instance.
 
         Returns
         -------
-        log_error: ads.dataflow.dataflow.DataFlowLog
-            a clickable link that opens the stderror log in another tab in jupyter notebook environment
-        """
-        if self._log_stderr is None:
-            self._log_stderr = self.fetch_log("stderr")
-        return self._log_stderr
+        DataScienceJob
+            The DataScienceJob instance (self)
 
-    @property
-    def local_dir(self) -> str:
         """
-        Retrieve the local directory of the data flow run
+        attr_map = {
+            self.CONST_JOB_INFRA: "jobInfrastructureType",
+            self.CONST_SHAPE_NAME: "shapeName",
+            self.CONST_SUBNET_ID: "subnetId",
+            self.CONST_BLOCK_STORAGE: "blockStorageSizeInGBs",
+            self.CONST_SHAPE_CONFIG_DETAILS: "jobShapeConfigDetails",
+        }
 
-        Returns
-        -------
-        local_dir: str
-            the local path to the Data Flow run
-        """
-        return self._local_dir
+        if not dsc_job.job_infrastructure_configuration_details:
+            dsc_job.job_infrastructure_configuration_details = {}
 
-    @property
-    def oci_link(self) -> object:
-        """
-        Retrieve the oci link of the data flow run
+        for snake_attr, camel_attr in attr_map.items():
+            value = self.get_spec(snake_attr)
+            if value:
+                dsc_job.job_infrastructure_configuration_details[camel_attr] = value
+
+        if (
+            not dsc_job.job_infrastructure_configuration_details.get("shapeName", "").endswith("Flex")
+            and dsc_job.job_infrastructure_configuration_details.get("jobShapeConfigDetails")
+        ):
+            raise ValueError("Shape config is not required for non flex shape from user end.")
+
+        if dsc_job.job_infrastructure_configuration_details.get("subnetId"):
+            dsc_job.job_infrastructure_configuration_details[
+                "jobInfrastructureType"
+            ] = JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE
+
+        if self.storage_mount:
+            if not hasattr(
+                oci.data_science.models, "JobStorageMountConfigurationDetails"
+            ):
+                raise EnvironmentError(
+                    "Storage mount hasn't been supported in the current OCI SDK installed."
+                )
+            dsc_job.job_storage_mount_configuration_details_list = [
+                DSCFileSystemManager.initialize(file_system)
+                for file_system in self.storage_mount
+            ]
+        return self
+
+    def build(self) -> DataScienceJob:
+        self.dsc_job.load_defaults()
+        self._update_from_dsc_model(self.dsc_job, overwrite=False)
+        return self
+
+    def init(self) -> DataScienceJob:
+        """Initializes a starter specification for the DataScienceJob.
 
         Returns
         -------
-        oci_link: str
-            link to the run page in an oci console
+        DataScienceJob
+            The DataScienceJob instance (self)
         """
-        return self._oci_link
+        return (
+            self.build()
+            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
+            .with_project_id(self.project_id or "{Provide a project OCID}")
+            .with_subnet_id(self.subnet_id or "{Provide a subnet OCID or remove this field if you use a default networking}")
+        )
 
-    def fetch_log(self, log_type: str) -> object:
-        """
-        Fetch the log information of a run
+    def create(self, runtime, **kwargs) -> DataScienceJob:
+        """Creates a job with runtime.
 
         Parameters
         ----------
-        log_type: str, have two values, 'stdout' or 'stderr'
+        runtime : Runtime
+            An ADS job runtime.
 
         Returns
         -------
-        dfl: DataFlowLog
-            a Data Flow log object
+        DataScienceJob
+            The DataScienceJob instance (self)
+
         """
-        if log_type not in DataFlowRun.LOG_OUTPUTS:
-            raise ValueError(
-                f"Invalid log type ({log_type}), valid types: {', '.join(DataFlowRun.LOG_OUTPUTS)}"
-            )
+        if not runtime:
+            raise ValueError("Set a valid runtime.")
+        payload = DataScienceJobRuntimeManager(self).translate(runtime)
+        # Add infra properties to payload
+        for attr in ["project_id", "compartment_id"]:
+            if getattr(self, attr):
+                payload[attr] = getattr(self, attr)
 
-        tmp = self.df_client.get_run_log(
-            self.run_id, f"spark_application_{log_type}.log.gz"
-        )
-        text_str = str(tmp.data.text.lstrip("\x00").rstrip("\n"))
+        if self.name:
+            display_name = Template(self.name).safe_substitute(runtime.envs)
+        elif isinstance(runtime, GitPythonRuntime) or isinstance(
+            runtime, ContainerRuntime
+        ):
+            display_name = utils.get_random_name_for_resource()
+        else:
+            display_name = None
 
-        opc_request_id = self.run_response.data.opc_request_id
+        payload["display_name"] = display_name
+        payload["job_log_configuration_details"] = self._prepare_log_config()
+        if not payload.get("freeform_tags"):
+            payload["freeform_tags"] = self.freeform_tags
+        if not payload.get("defined_tags"):
+            payload["defined_tags"] = self.defined_tags
+
+        self.dsc_job = DSCJob(**payload)
+        # Set Job infra to user values after DSCJob initialized the defaults
+        self._update_job_infra(self.dsc_job)
+        self.dsc_job.create()
+        # Update the model from infra after job creation.
+        self._update_from_dsc_model(self.dsc_job)
+        return self
 
-        log_filename = os.path.join(
-            opc_request_id, f"spark_application_{log_type}.log.gz"
-        )
-        object_storage_log_path = os.path.join(
-            self._config["logs_bucket_uri"], log_filename
+    def run(
+        self,
+        name=None,
+        args=None,
+        env_var=None,
+        freeform_tags=None,
+        defined_tags=None,
+        wait=False,
+        **kwargs
+    ) -> DataScienceJobRun:
+        """Runs a job on OCI Data Science job
+
+        Parameters
+        ----------
+        name : str, optional
+            The name of the job run, by default None.
+        args : str, optional
+            Command line arguments for the job run, by default None.
+        env_var : dict, optional
+            Environment variable for the job run, by default None
+        freeform_tags : dict, optional
+            Freeform tags for the job run, by default None
+        defined_tags : dict, optional
+            Defined tags for the job run, by default None
+        wait : bool, optional
+            Indicate if this method should wait for the run to finish before it returns, by default False.
+        kwargs
+            additional keyword arguments
+
+        Returns
+        -------
+        DataScienceJobRun
+            A Data Science Job Run instance.
+
+        """
+        # Runtime in the infrastructure will be None if the job is not created.
+        if not self.runtime:
+            raise RuntimeError(
+                "Job is not created. Call create() to create the job first."
+            )
+
+        if not freeform_tags:
+            freeform_tags = {}
+        runtime_freeform_tags = self.runtime.freeform_tags
+        if runtime_freeform_tags:
+            freeform_tags.update(runtime_freeform_tags)
+
+        if not defined_tags:
+            defined_tags = {}
+        runtime_defined_tags = self.runtime.defined_tags
+        if runtime_defined_tags:
+            defined_tags.update(runtime_defined_tags)
+
+        if name:
+            envs = self.runtime.envs
+            if env_var:
+                envs.update(env_var)
+            name = Template(name).safe_substitute(envs)
+
+        return self.dsc_job.run(
+            display_name=name,
+            command_line_arguments=args,
+            environment_variables=env_var,
+            freeform_tags=freeform_tags,
+            defined_tags=defined_tags,
+            wait=wait,
+            **kwargs
         )
-        log_local_dir = os.path.join(self._local_dir, "logs")
 
-        log_obj = DataFlowLog(text_str, object_storage_log_path, log_local_dir)
-        if log_type == "stdout":
-            self._log_stdout = log_obj
-        elif log_type == "stderr":
-            self._log_stderr = log_obj
-
-        return log_obj
-
-    def _repr_html_(self):
-        if self.status == "FAILED":
-            logger.warning("Run failed. See the logs for details.")
-            logger.info("Printing tail of the stdout log...")
-            self.log_stdout.tail()
-        else:
-            return
+    def delete(self) -> None:
+        """Deletes a job"""
+        self.dsc_job.delete()
 
-
-class DataFlowLog:
-    @deprecated("2.6.3")
-    def __init__(self, text, oci_path, log_local_dir):
-        self.text = str(text)
-        self._oci_path = oci_path
-        self._local_dir = log_local_dir
-        self._local_path = None
-        self.line_list = self.text.split("\n")
-
-    def head(self, n: int = 10):
-        """
-        Show the first n lines of the log as the output of the notebook cell
+    def run_list(self, **kwargs) -> List[DataScienceJobRun]:
+        """Gets a list of job runs.
 
         Parameters
         ----------
-        n: int, default is 10
-            the number of lines from head of the log file
+        **kwargs :
+            Keyword arguments for filtering the job runs.
+            These arguments will be passed to OCI API.
+
 
         Returns
         -------
-        None
-        """
-        for _, v in enumerate(self.line_list[:n]):
-            print(v)
+        List[DSCJobRun]:
+            A list of job runs.
 
-    def tail(self, n: int = 10):
         """
-        Show the last n lines of the log as the output of the notebook cell
+        return self.dsc_job.run_list(**kwargs)
+
+    @classmethod
+    def from_dsc_job(cls, dsc_job: DSCJob) -> DataScienceJob:
+        """Initialize a DataScienceJob instance from a DSCJob
 
         Parameters
         ----------
-        n: int, default is 10
-            the number of lines from tail of the log file
+        dsc_job : DSCJob
+            An instance of DSCJob
 
         Returns
         -------
-        None
-        """
-        for _, v in enumerate(self.line_list[-n:]):
-            print(v)
+        DataScienceJob
+            An instance of DataScienceJob
 
-    def show_all(self):
         """
-        Show all content of the log as the output of the notebook cell
+        instance = cls()
+        instance._update_from_dsc_model(dsc_job)
+        instance.runtime = DataScienceJobRuntimeManager(instance).extract(dsc_job)
+        return instance
 
-        Returns
-        -------
-        None
-        """
-        for _, v in enumerate(self.line_list):
-            print(v)
+    @classmethod
+    def from_id(cls, job_id: str) -> DataScienceJob:
+        """Gets an existing job using Job OCID
 
-    @property
-    def oci_path(self):
-        """
-        Get the path of the log file in object storage
-
-        Returns
-        -------
-        oci_path: str
-            Path of the log file in object storage
-        """
-        return self._oci_path
+        Parameters
+        ----------
+        job_id : str
+            Job OCID
 
-    @property
-    def local_path(self):
-        """
-        Get the path of the log file in local directory
 
         Returns
         -------
-        local_path: str
-            Path of the log file in local directory
+        DataScienceJob
+            An instance of DataScienceJob
+
         """
-        if self._local_path is None:
-            logger.warning(
-                "The log file is not stored in local directory. "
-                "Call the save() method to save the log file to local first.",
-            )
+        return cls.from_dsc_job(DSCJob.from_ocid(job_id))
 
-        return self._local_path
+    @classmethod
+    def list_jobs(cls, compartment_id: str = None, **kwargs) -> List[DataScienceJob]:
+        """Lists all jobs in a compartment.
 
-    @property
-    def local_dir(self):
-        """
-        Get the local directory where the log file is saved.
+        Parameters
+        ----------
+        compartment_id : str, optional
+            The compartment ID for running the jobs, by default None.
+            This is optional in a OCI Data Science notebook session.
+            If this is not specified, the compartment ID of the notebook session will be used.
+        **kwargs :
+            Keyword arguments to be passed into OCI list_jobs API for filtering the jobs.
 
         Returns
         -------
-        local_dir: str
-            Path to the local directory where the log file is saved.
-        """
-        return self._local_dir
+        List[DataScienceJob]
+            A list of DataScienceJob object.
 
-    def save(self, log_dir=None):
         """
-        save the log file to a local directory.
+        return [
+            cls.from_dsc_job(job)
+            for job in DSCJob.list_resource(compartment_id, **kwargs)
+        ]
+
+    @classmethod
+    def instance_shapes(cls, compartment_id: str = None, **kwargs) -> list:
+        """Lists the supported shapes for running jobs in a compartment.
 
         Parameters
         ----------
-        log_dir: str,
-            The path to the local directory to save log file, if not
-        set, log will be saved to the _local_dir by default.
+        compartment_id : str, optional
+            The compartment ID for running the jobs, by default None.
+            This is optional in a OCI Data Science notebook session.
+            If this is not specified, the compartment ID of the notebook session will be used.
 
         Returns
         -------
-        None
-        """
-        if self._local_path is not None:
-            logger.warning(f"The log file is already exists in `{self._local_path}`.")
-            return
-        if log_dir is not None:
-            self._local_dir = log_dir
-
-        if not os.path.isdir(self._local_dir):
-            os.makedirs(self._local_dir)
+        list
+            A list of oci.data_science.models.JobShapeSummary objects
+            containing the information of the supported shapes.
 
-        filename = os.path.basename(self._oci_path)
-        self._local_path = os.path.join(self._local_dir, filename)
+        Examples
+        --------
+        To get a list of shape names::
 
-        with open(self._local_path, "w+") as in_file:
-            in_file.write(self.text)
+            shapes = DataScienceJob.fast_launch_shapes(
+                compartment_id=os.environ["PROJECT_COMPARTMENT_OCID"]
+            )
+            shape_names = [shape.name for shape in shapes]
 
-        logger.info(f"The log file saved to `{self._local_path}`.")
+        """
+        shapes = oci.pagination.list_call_get_all_results(
+            DSCJob.init_client().list_job_shapes,
+            DSCJob.check_compartment_id(compartment_id),
+            **kwargs,
+        ).data
+        return shapes
 
-    def __str__(self):
-        return self.text
+    @classmethod
+    def fast_launch_shapes(cls, compartment_id: str = None, **kwargs) -> list:
+        """Lists the supported fast launch shapes for running jobs in a compartment.
 
-    def _repr_html_(self):
-        """
-        Display the link of the log file to open in another tab of the jupyter
-        environment.
+        Parameters
+        ----------
+        compartment_id : str, optional
+            The compartment ID for running the jobs, by default None.
+            This is optional in a OCI Data Science notebook session.
+            If this is not specified, the compartment ID of the notebook session will be used.
 
         Returns
         -------
-        link of the log file
-        """
-        if self._local_path is None:
-            return
+        list
+            A list of oci.data_science.models.FastLaunchJobConfigSummary objects
+            containing the information of the supported shapes.
+
+        Examples
+        --------
+        To get a list of shape names::
+
+            shapes = DataScienceJob.fast_launch_shapes(
+                compartment_id=os.environ["PROJECT_COMPARTMENT_OCID"]
+            )
+            shape_names = [shape.shape_name for shape in shapes]
 
-        relative_path = os.path.relpath(self._local_path)
-        # FileLink has to be tested with router to check compatibility. Till then let us comment it (ODSC-8310)
-        # return display(FileLink(relative_path))
-        return logger.info(f"Log file saved to {self._local_path}.")
+        """
+        shapes = oci.pagination.list_call_get_all_results(
+            DSCJob.init_client().list_fast_launch_job_configs,
+            DSCJob.check_compartment_id(compartment_id),
+            **kwargs,
+        ).data
+        return shapes
```

### Comparing `oracle_ads-2.8.5/ads/dataset/classification_dataset.py` & `oracle_ads-2.8.6/ads/dataset/classification_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/correlation.py` & `oracle_ads-2.8.6/ads/dataset/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/correlation_plot.py` & `oracle_ads-2.8.6/ads/dataset/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/dask_series.py` & `oracle_ads-2.8.6/ads/dataset/dask_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/dataframe_transformer.py` & `oracle_ads-2.8.6/ads/dataset/dataframe_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/dataset.py` & `oracle_ads-2.8.6/ads/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/dataset_browser.py` & `oracle_ads-2.8.6/ads/dataset/dataset_browser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/dataset_with_target.py` & `oracle_ads-2.8.6/ads/dataset/dataset_with_target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/exception.py` & `oracle_ads-2.8.6/ads/dataset/exception.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/factory.py` & `oracle_ads-2.8.6/ads/dataset/factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/feature_engineering_transformer.py` & `oracle_ads-2.8.6/ads/dataset/feature_engineering_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/feature_selection.py` & `oracle_ads-2.8.6/ads/dataset/feature_selection.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/forecasting_dataset.py` & `oracle_ads-2.8.6/ads/dataset/forecasting_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/helper.py` & `oracle_ads-2.8.6/ads/dataset/helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/label_encoder.py` & `oracle_ads-2.8.6/ads/dataset/label_encoder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/mixin/dataset_accessor.py` & `oracle_ads-2.8.6/ads/dataset/mixin/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/pipeline.py` & `oracle_ads-2.8.6/ads/dataset/pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/plot.py` & `oracle_ads-2.8.6/ads/dataset/plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/progress.py` & `oracle_ads-2.8.6/ads/dataset/progress.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/recommendation.py` & `oracle_ads-2.8.6/ads/dataset/recommendation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/recommendation_transformer.py` & `oracle_ads-2.8.6/ads/dataset/recommendation_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/regression_dataset.py` & `oracle_ads-2.8.6/ads/dataset/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/sampled_dataset.py` & `oracle_ads-2.8.6/ads/dataset/sampled_dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/target.py` & `oracle_ads-2.8.6/ads/dataset/target.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dataset/timeseries.py` & `oracle_ads-2.8.6/ads/dataset/timeseries.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/dbmixin/db_pandas_accessor.py` & `oracle_ads-2.8.6/ads/dbmixin/db_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/environment/ml_runtime.py` & `oracle_ads-2.8.6/ads/environment/ml_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/evaluations/__init__.py` & `oracle_ads-2.8.6/ads/evaluations/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/evaluations/evaluation_plot.py` & `oracle_ads-2.8.6/ads/evaluations/evaluation_plot.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/evaluations/evaluator.py` & `oracle_ads-2.8.6/ads/evaluations/evaluator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/evaluations/statistical_metrics.py` & `oracle_ads-2.8.6/ads/evaluations/statistical_metrics.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/base_explainer.py` & `oracle_ads-2.8.6/ads/explanations/base_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/explainer.py` & `oracle_ads-2.8.6/ads/explanations/explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/mlx_global_explainer.py` & `oracle_ads-2.8.6/ads/explanations/mlx_global_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/mlx_interface.py` & `oracle_ads-2.8.6/ads/explanations/mlx_interface.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/mlx_local_explainer.py` & `oracle_ads-2.8.6/ads/explanations/mlx_local_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/explanations/mlx_whatif_explainer.py` & `oracle_ads-2.8.6/ads/explanations/mlx_whatif_explainer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/__init__.py` & `oracle_ads-2.8.6/ads/feature_engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/dataframe_accessor.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/dataframe_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/correlation.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/correlation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/eda_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/eda_mixin_series.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/eda_mixin_series.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/feature_types_mixin.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/feature_types_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/mixin/utils.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/mixin/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/accessor/series_accessor.py` & `oracle_ads-2.8.6/ads/feature_engineering/accessor/series_accessor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/adsimage/image.py` & `oracle_ads-2.8.6/ads/feature_engineering/adsimage/image.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/adsimage/image_reader.py` & `oracle_ads-2.8.6/ads/feature_engineering/adsimage/image_reader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/data_schema.json` & `oracle_ads-2.8.6/ads/feature_engineering/data_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/dataset/zip_code_data.py` & `oracle_ads-2.8.6/ads/feature_engineering/dataset/zip_code_data.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/exceptions.py` & `oracle_ads-2.8.6/ads/feature_engineering/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/__init__.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/address.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/common_regex_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/oci_language.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/oci_language.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/base.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/nltk_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/parsers/spacy_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/adsstring/string.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/adsstring/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/base.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/boolean.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/boolean.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/category.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/category.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/constant.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/constant.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/continuous.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/continuous.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/creditcard.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/creditcard.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/datetime.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/datetime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/discrete.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/discrete.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/document.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/document.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/gis.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/gis.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_validator.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/feature_validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/feature_warning.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/feature_warning.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/handler/warnings.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/handler/warnings.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/integer.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/integer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v4.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address_v4.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ip_address_v6.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/ip_address_v6.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/lat_long.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/lat_long.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/object.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/object.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/ordinal.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/ordinal.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/phone_number.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/phone_number.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/string.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/string.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/text.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/text.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/unknown.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/unknown.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type/zip_code.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type/zip_code.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/feature_type_manager.py` & `oracle_ads-2.8.6/ads/feature_engineering/feature_type_manager.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/schema.py` & `oracle_ads-2.8.6/ads/feature_engineering/schema.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/feature_engineering/utils.py` & `oracle_ads-2.8.6/ads/feature_engineering/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/_imports.py` & `oracle_ads-2.8.6/ads/hpo/_imports.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/ads_search_space.py` & `oracle_ads-2.8.6/ads/hpo/ads_search_space.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/distributions.py` & `oracle_ads-2.8.6/ads/hpo/distributions.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/objective.py` & `oracle_ads-2.8.6/ads/hpo/objective.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/search_cv.py` & `oracle_ads-2.8.6/ads/hpo/search_cv.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/stopping_criterion.py` & `oracle_ads-2.8.6/ads/hpo/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/tuner_artifact.py` & `oracle_ads-2.8.6/ads/hpo/tuner_artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/utils.py` & `oracle_ads-2.8.6/ads/hpo/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/validation.py` & `oracle_ads-2.8.6/ads/hpo/validation.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_contour.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_contour.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_edf.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_edf.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_intermediate_values.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_optimization_history.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_optimization_history.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_parallel_coordinate.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/hpo/visualization/_param_importances.py` & `oracle_ads-2.8.6/ads/hpo/visualization/_param_importances.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/__init__.py` & `oracle_ads-2.8.6/ads/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/ads_job.py` & `oracle_ads-2.8.6/ads/jobs/ads_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,22 @@
         infra = self.get_spec("infrastructure")
         infra.name = self.name
         self.infrastructure.create(self.runtime, **kwargs)
         self.set_spec("name", self.infrastructure.name)
         return self
 
     def run(
-        self, name=None, args=None, env_var=None, freeform_tags=None, wait=False
+        self,
+        name=None,
+        args=None,
+        env_var=None,
+        freeform_tags=None,
+        defined_tags=None,
+        wait=False,
+        **kwargs
     ) -> Union[DataScienceJobRun, DataFlowRun]:
         """Runs the job.
 
         Parameters
         ----------
         name : str, optional
             Name of the job run, by default None.
@@ -400,43 +407,50 @@
             Command line arguments for the job run, by default None.
             This will override the configurations on the job.
             If this is None, the args from the job configuration will be used.
         env_var : dict, optional
             Additional environment variables for the job run, by default None
         freeform_tags : dict, optional
             Freeform tags for the job run, by default None
+        defined_tags : dict, optional
+            Defined tags for the job run, by default None
         wait : bool, optional
             Indicate if this method call should wait for the job run.
             By default False, this method returns as soon as the job run is created.
             If this is set to True, this method will stream the job logs and wait until it finishes,
             similar to `job.run().watch()`.
+        kwargs
+            additional keyword arguments
 
         Returns
         -------
         Job Run Instance
             A job run instance, depending on the infrastructure.
 
         Examples
         --------
         To run a job and override the configurations::
 
             job_run = job.run(
                 name="<my_job_run_name>",
                 args="new_arg --new_key new_val",
                 env_var={"new_env": "new_val"},
-                freeform_tags={"new_tag": "new_tag_val"}
+                freeform_tags={"new_tag": "new_tag_val"},
+                defined_tags={"Operations": {"CostCenter": "42"}}
             )
 
         """
         return self.infrastructure.run(
             name=name,
             args=args,
             env_var=env_var,
             freeform_tags=freeform_tags,
+            defined_tags=defined_tags,
             wait=wait,
+            **kwargs
         )
 
     def run_list(self, **kwargs) -> list:
         """Gets a list of runs of the job.
 
         Returns
         -------
```

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/base.py` & `oracle_ads-2.8.6/ads/jobs/builders/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/base.py` & `oracle_ads-2.8.6/ads/jobs/builders/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dataflow.py` & `oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dataflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 CONDA_PACK_SUFFIX = "#conda"
 SLEEP_INTERVAL = 3
 
 DEFAULT_LANGUAGE = "PYTHON"
 DEFAULT_SPARK_VERSION = "3.2.1"
 DEFAULT_NUM_EXECUTORS = 1
 DEFAULT_SHAPE = "VM.Standard.E3.Flex"
+DATAFLOW_SHAPE_FAMILY = [
+    "Standard.E3",
+    "Standard.E4",
+    "Standard3",
+    "Standard.A1",
+    "Standard2"
+]
 
 
 def conda_pack_name_to_dataflow_config(conda_uri):
     return {
         "spark.archives": conda_uri + CONDA_PACK_SUFFIX,
         "dataflow.auth": "resource_principal",
     }
@@ -380,14 +387,17 @@
     CONST_WAREHOUSE_BUCKET_URI = "warehouse_bucket_uri"
     CONST_DRIVER_SHAPE_CONFIG = "driver_shape_config"
     CONST_EXECUTOR_SHAPE_CONFIG = "executor_shape_config"
     CONST_MEMORY_IN_GBS = "memory_in_gbs"
     CONST_OCPUS = "ocpus"
     CONST_ID = "id"
     CONST_PRIVATE_ENDPOINT_ID = "private_endpoint_id"
+    CONST_POOL_ID = "pool_id"
+    CONST_FREEFORM_TAGS = "freeform_tags"
+    CONST_DEFINED_TAGS = "defined_tags"
 
     attribute_map = {
         CONST_COMPARTMENT_ID: "compartmentId",
         CONST_CONFIG: CONST_CONFIG,
         CONST_EXECUTE: CONST_EXECUTE,
         CONST_DRIVER_SHAPE: "driverShape",
         CONST_EXECUTOR_SHAPE: "executorShape",
@@ -398,27 +408,34 @@
         CONST_WAREHOUSE_BUCKET_URI: "warehouseBucketUri",
         CONST_DRIVER_SHAPE_CONFIG: "driverShapeConfig",
         CONST_EXECUTOR_SHAPE_CONFIG: "executorShapeConfig",
         CONST_MEMORY_IN_GBS: "memoryInGBs",
         CONST_OCPUS: CONST_OCPUS,
         CONST_ID: CONST_ID,
         CONST_PRIVATE_ENDPOINT_ID: "privateEndpointId",
+        CONST_POOL_ID: "poolId",
+        CONST_FREEFORM_TAGS: "freeformTags",
+        CONST_DEFINED_TAGS: "definedTags",
     }
 
     def __init__(self, spec: dict = None, **kwargs):
         defaults = self._load_default_properties()
         spec = self._standardize_spec(spec)
         kwargs = self._standardize_spec(kwargs)
         if spec is None:
             super(DataFlow, self).__init__(defaults, **kwargs)
         else:
             spec = {
                 k: v
                 for k, v in spec.items()
-                if f"with_{camel_to_snake(k)}" in self.__dir__() and v is not None
+                if (
+                    f"with_{camel_to_snake(k)}" in self.__dir__()
+                    or (k == "defined_tags" or "freeform_tags")
+                )
+                and v is not None
             }
             defaults.update(spec)
             super().__init__(defaults, **kwargs)
 
         self.df_app = DataFlowApp(**self._spec)
         self.runtime = None
         self._name = None
@@ -772,16 +789,62 @@
         Returns
         -------
         DataFlow
             the Data Flow instance itself
         """
         return self.set_spec(self.CONST_PRIVATE_ENDPOINT_ID, private_endpoint_id)
 
+    def with_freeform_tag(self, **kwargs) -> "DataFlow":
+        """Sets freeform tags
+
+        Returns
+        -------
+        DataFlow
+            The DataFlow instance (self)
+        """
+        return self.set_spec(self.CONST_FREEFORM_TAGS, kwargs)
+
+    def with_defined_tag(self, **kwargs) -> "DataFlow":
+        """Sets defined tags
+
+        Returns
+        -------
+        DataFlow
+            The DataFlow instance (self)
+        """
+        return self.set_spec(self.CONST_DEFINED_TAGS, kwargs)
+
+    def with_pool_id(self, pool_id: str) -> "DataFlow":
+        """
+        Set the Data Flow Pool Id for a Data Flow job.
+
+        Parameters
+        ----------
+        pool_id: str
+            The OCID of a Data Flow Pool.
+
+        Returns
+        -------
+        DataFlow
+            the Data Flow instance itself
+        """
+        if not hasattr(CreateApplicationDetails, "pool_id"):
+            raise EnvironmentError(
+                "Data Flow Pool has not been supported in the current OCI SDK installed."
+            )
+        return self.set_spec(self.CONST_POOL_ID, pool_id)
+
     def __getattr__(self, item):
-        if f"with_{item}" in self.__dir__():
+        if item == self.CONST_DEFINED_TAGS or item == self.CONST_FREEFORM_TAGS:
+            return self.get_spec(item)
+        elif (
+            f"with_{item}" in self.__dir__()
+            and item != "defined_tag"
+            and item != "freeform_tag"
+        ):
             return self.get_spec(item)
         raise AttributeError(f"Attribute {item} not found.")
 
     def create(self, runtime: DataFlowRuntime, **kwargs) -> "DataFlow":
         """
         Create a Data Flow job given a runtime.
 
@@ -793,14 +856,19 @@
             additional keyword arguments
 
         Returns
         -------
         DataFlow
             a Data Flow job instance
         """
+        if self.pool_id:
+            if not hasattr(CreateApplicationDetails, "pool_id"):
+                raise EnvironmentError(
+                    "Data Flow Pool has not been supported in the current OCI SDK installed."
+                )
         # Set default display_name if not specified - randomly generated easy to remember name
         if not self.name:
             self.name = utils.get_random_name_for_resource()
         payload = copy.deepcopy(self._spec)
         overwrite = kwargs.pop("overwrite", runtime.overwrite) or False
         runtime.convert(overwrite=overwrite)
         if not runtime.script_uri:
@@ -845,30 +913,59 @@
             runtime_config.update(conda_pack_name_to_dataflow_config(conda_uri))
             runtime.with_configuration(runtime_config)
 
         payload.update(
             {
                 "display_name": self.name,
                 "file_uri": runtime.script_uri,
-                "freeform_tags": runtime.freeform_tags,
+                "freeform_tags": runtime.freeform_tags or self.freeform_tags,
+                "defined_tags": runtime.defined_tags or self.defined_tags,
                 "archive_uri": runtime.archive_uri,
                 "configuration": runtime.configuration,
             }
         )
         if len(runtime.args) > 0:
             payload["arguments"] = runtime.args
         if not payload.get("compartment_id", None):
             raise ValueError(
                 "Compartment id is required. Specify compartment id via 'with_compartment_id()'."
             )
+        self._validate_shapes(payload)
         payload.pop("id", None)
         logger.debug(f"Creating a DataFlow Application with payload {payload}")
         self.df_app = DataFlowApp(**payload).create()
         self.with_id(self.df_app.id)
         return self
+    
+    @staticmethod
+    def _validate_shapes(payload: Dict):
+        if "executor_shape" not in payload:
+            payload["executor_shape"] = DEFAULT_SHAPE
+        if "driver_shape" not in payload:
+            payload["driver_shape"] = DEFAULT_SHAPE
+        executor_shape = payload["executor_shape"]
+        executor_shape_config = payload.get("executor_shape_config", {})
+        driver_shape = payload["driver_shape"]
+        driver_shape_config = payload.get("driver_shape_config", {})
+        same_shape_family = False
+        for shape in DATAFLOW_SHAPE_FAMILY:
+            if shape in executor_shape and shape in driver_shape:
+                same_shape_family = True
+                break
+        if not same_shape_family:
+            raise ValueError(
+                "`executor_shape` and `driver_shape` must be from the same shape family."
+            )
+        if (
+            (not executor_shape.endswith("Flex") and executor_shape_config) 
+            or (not driver_shape.endswith("Flex") and driver_shape_config)
+        ):
+            raise ValueError(
+                "Shape config is not required for non flex shape from user end."
+            )
 
     @staticmethod
     def _upload_file(local_path, bucket, overwrite=False):
         signer = default_signer()
         os_client = OCIClientFactory(**signer).object_storage
         namespace = os_client.get_namespace().data
         parsed = urllib.parse.urlparse(bucket)
@@ -911,14 +1008,15 @@
 
     def run(
         self,
         name: str = None,
         args: List[str] = None,
         env_vars: Dict[str, str] = None,
         freeform_tags: Dict[str, str] = None,
+        defined_tags: Dict[str, Dict[str, object]] = None,
         wait: bool = False,
         **kwargs,
     ) -> DataFlowRun:
         """
         Run a Data Flow job.
 
         Parameters
@@ -928,14 +1026,16 @@
             with timestamp will be generated, like 'strange-spider-2022-08-17-23:55.02'.
         args: List[str], optional
             list of command line arguments
         env_vars: Dict[str, str], optional
             dictionary of environment variables (not used for data flow)
         freeform_tags: Dict[str, str], optional
             freeform tags
+        defined_tags: Dict[str, Dict[str, object]], optional
+            defined tags
         wait: bool, optional
             whether to wait for a run to terminate
         kwargs
             additional keyword arguments
 
         Returns
         -------
@@ -946,15 +1046,16 @@
         if "application_id" not in payload:
             payload["application_id"] = self.id
         if "compartment_id" not in payload:
             payload["compartment_id"] = self.get_spec("compartment_id")
         # Set default display_name if not specified - randomly generated easy to remember name generated
         payload["display_name"] = name if name else utils.get_random_name_for_resource()
         payload["arguments"] = args if args and len(args) > 0 else None
-        payload["freeform_tags"] = freeform_tags
+        payload["freeform_tags"] = freeform_tags or self.freeform_tags
+        payload["defined_tags"] = defined_tags or self.defined_tags
         payload.pop("spark_version", None)
         logger.debug(f"Creating a DataFlow Run with payload {payload}")
         run = DataFlowRun(**payload).create()
         if wait:
             run.wait(kwargs.pop("interval", SLEEP_INTERVAL))
         return run
```

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job.py` & `oracle_ads-2.8.6/ads/model/deployment/model_deployment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1752 +1,1805 @@
 #!/usr/bin/env python
 # -*- coding: utf-8; -*-
 
 # Copyright (c) 2021, 2023 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
-from __future__ import annotations
 
+
+import collections
+import copy
 import datetime
-import logging
 import oci
-import os
+import warnings
 import time
-import traceback
-import uuid
-from io import DEFAULT_BUFFER_SIZE
-from string import Template
-from typing import Any, Dict, List, Optional, Union
-
-import fsspec
-import oci.data_science
-import oci.util as oci_util
-import yaml
-from oci.data_science.models import JobInfrastructureConfigurationDetails
-from oci.exceptions import ServiceError
-from ads.common import utils
-from ads.common.oci_datascience import DSCNotebookSession, OCIDataScienceMixin
-from ads.common.oci_logging import OCILog
-from ads.common.oci_resource import ResourceNotFoundError
-from ads.jobs.builders.infrastructure.base import Infrastructure, RunInstance
-from ads.jobs.builders.infrastructure.dsc_job_runtime import (
-    DataScienceJobRuntimeManager,
+from typing import Dict, List, Union, Any
+
+import oci.loggingsearch
+from ads.common import auth as authutil
+import pandas as pd
+from ads.model.serde.model_input import JsonModelInputSERDE
+from ads.common.oci_logging import (
+    LOG_INTERVAL,
+    LOG_RECORDS_LIMIT,
+    ConsolidatedLog,
+    OCILog,
 )
+from ads.config import COMPARTMENT_OCID, PROJECT_OCID
+from ads.jobs.builders.base import Builder
 from ads.jobs.builders.infrastructure.utils import get_value
-from ads.jobs.builders.runtimes.artifact import Artifact
-from ads.jobs.builders.runtimes.container_runtime import ContainerRuntime
-from ads.jobs.builders.runtimes.python_runtime import GitPythonRuntime
+from ads.model.common.utils import _is_json_serializable
+from ads.model.deployment.common.utils import send_request
+from ads.model.deployment.model_deployment_infrastructure import (
+    MODEL_DEPLOYMENT_INFRASTRUCTURE_TYPE,
+    ModelDeploymentInfrastructure,
+)
+from ads.model.deployment.model_deployment_runtime import (
+    ModelDeploymentCondaRuntime,
+    ModelDeploymentContainerRuntime,
+    ModelDeploymentRuntime,
+    ModelDeploymentRuntimeType,
+    OCIModelDeploymentRuntimeType,
+)
+from ads.model.service.oci_datascience_model_deployment import (
+    OCIDataScienceModelDeployment,
+)
+from ads.common import utils as ads_utils
+from .common import utils
+from .common.utils import State
+from .model_deployment_properties import ModelDeploymentProperties
+from oci.data_science.models import (
+    LogDetails,
+    CreateModelDeploymentDetails,
+    UpdateModelDeploymentDetails,
+)
 
-from ads.common.dsc_file_system import OCIFileStorage, DSCFileSystemManager
+DEFAULT_WAIT_TIME = 1200
+DEFAULT_POLL_INTERVAL = 10
+DEFAULT_WORKFLOW_STEPS = 6
+DELETE_WORKFLOW_STEPS = 2
+DEACTIVATE_WORKFLOW_STEPS = 2
+DEFAULT_RETRYING_REQUEST_ATTEMPTS = 3
+TERMINAL_STATES = [State.ACTIVE, State.FAILED, State.DELETED, State.INACTIVE]
 
-logger = logging.getLogger(__name__)
+MODEL_DEPLOYMENT_KIND = "deployment"
+MODEL_DEPLOYMENT_TYPE = "modelDeployment"
+MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON = "TRITON"
 
-SLEEP_INTERVAL = 3
-WAIT_SECONDS_AFTER_FINISHED = 90
-MAXIMUM_MOUNT_COUNT = 5
-FILE_STORAGE_TYPE = "FILE_STORAGE"
+MODEL_DEPLOYMENT_INSTANCE_SHAPE = "VM.Standard.E4.Flex"
+MODEL_DEPLOYMENT_INSTANCE_OCPUS = 1
+MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS = 16
+MODEL_DEPLOYMENT_INSTANCE_COUNT = 1
+MODEL_DEPLOYMENT_BANDWIDTH_MBPS = 10
 
+MODEL_DEPLOYMENT_RUNTIMES = {
+    ModelDeploymentRuntimeType.CONDA: ModelDeploymentCondaRuntime,
+    ModelDeploymentRuntimeType.CONTAINER: ModelDeploymentContainerRuntime,
+}
 
-class DSCJob(OCIDataScienceMixin, oci.data_science.models.Job):
-    """Represents an OCI Data Science Job
-    This class contains all attributes of the oci.data_science.models.Job.
-    The main purpose of this class is to link the oci.data_science.models.Job model and the related client methods.
-    Mainly, linking the Job model (payload) to Create/Update/Get/List/Delete methods.
 
-    A DSCJob can be initialized by unpacking a the properties stored in a dictionary (payload):
+class ModelDeploymentLogType:
+    PREDICT = "predict"
+    ACCESS = "access"
 
-    .. code-block:: python
 
-        job_properties = {
-            "display_name": "my_job",
-            "job_infrastructure_configuration_details": {"shape_name": "VM.MY_SHAPE"}
-        }
-        job = DSCJob(**job_properties)
+class ModelDeploymentMode:
+    HTTPS = "HTTPS_ONLY"
+    STREAM = "STREAM_ONLY"
 
-    The properties can also be OCI REST API payload, in which the keys are in camel format.
 
-    .. code-block:: python
+class LogNotConfiguredError(Exception):  # pragma: no cover
+    pass
 
-        job_payload = {
-            "projectId": "<project_ocid>",
-            "compartmentId": "<compartment_ocid>",
-            "displayName": "<job_name>",
-            "jobConfigurationDetails": {
-                "jobType": "DEFAULT",
-                "commandLineArguments": "pos_arg1 pos_arg2 --key1 val1 --key2 val2",
-                "environmentVariables": {
-                    "KEY1": "VALUE1",
-                    "KEY2": "VALUE2",
-                    # User specifies conda env via env var
-                    "CONDA_ENV_TYPE" : "service",
-                    "CONDA_ENV_SLUG" : "mlcpuv1"
-                }
-            },
-            "jobInfrastructureConfigurationDetails": {
-                "jobInfrastructureType": "STANDALONE",
-                "shapeName": "VM.Standard.E3.Flex",
-                "jobShapeConfigDetails": {
-                    "memoryInGBs": 16,
-                    "ocpus": 1
-                },
-                "blockStorageSizeInGBs": "100",
-                "subnetId": "<subnet_ocid>"
-            }
-        }
-        job = DSCJob(**job_payload)
+
+class ModelDeploymentFailedError(Exception):  # pragma: no cover
+    pass
+
+
+class ModelDeployment(Builder):
     """
+    A class used to represent a Model Deployment.
 
-    DEFAULT_INFRA_TYPE = (
-        JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
-    )
+    Attributes
+    ----------
+    config: (dict)
+        Deployment configuration parameters
+    properties: (ModelDeploymentProperties)
+        ModelDeploymentProperties object
+    workflow_state_progress: (str)
+        Workflow request id
+    workflow_steps: (int)
+        The number of steps in the workflow
+    dsc_model_deployment: (OCIDataScienceModelDeployment)
+        The OCIDataScienceModelDeployment instance.
+    state: (State)
+        Returns the deployment state of the current Model Deployment object
+    created_by: (str)
+        The user that creates the model deployment
+    lifecycle_state: (str)
+        Model deployment lifecycle state
+    lifecycle_details: (str)
+        Model deployment lifecycle details
+    time_created: (datetime)
+        The time when the model deployment is created
+    display_name: (str)
+        Model deployment display name
+    description: (str)
+        Model deployment description
+    freeform_tags: (dict)
+        Model deployment freeform tags
+    defined_tags: (dict)
+        Model deployment defined tags
+    runtime: (ModelDeploymentRuntime)
+        Model deployment runtime
+    infrastructure: (ModelDeploymentInfrastructure)
+        Model deployment infrastructure
+
+
+    Methods
+    -------
+    deploy(wait_for_completion, **kwargs)
+        Deploy the current Model Deployment object
+    delete(wait_for_completion, **kwargs)
+        Deletes the current Model Deployment object
+    update(wait_for_completion, **kwargs)
+        Updates a model deployment
+    activate(wait_for_completion, max_wait_time, poll_interval)
+        Activates a model deployment
+    deactivate(wait_for_completion, max_wait_time, poll_interval)
+        Deactivates a model deployment
+    list(status, compartment_id, project_id, **kwargs)
+        List model deployment within given compartment and project.
+    with_display_name(display_name)
+        Sets model deployment display name
+    with_description(description)
+        Sets model deployment description
+    with_freeform_tags(freeform_tags)
+        Sets model deployment freeform tags
+    with_defined_tags(defined_tags)
+        Sets model deployment defined tags
+    with_runtime(self, runtime)
+        Sets model deployment runtime
+    with_infrastructure(self, infrastructure)
+        Sets model deployment infrastructure
+    from_dict(obj_dict)
+        Deserializes model deployment instance from dict
+    from_id(id)
+        Loads model deployment instance from ocid
+    sync()
+        Updates the model deployment instance from backend
+
+
+    Examples
+    --------
+    >>> # Build model deployment from builder apis:
+    >>> ds_model_deployment = (ModelDeployment()
+    ...    .with_display_name("TestModelDeployment")
+    ...    .with_description("Testing the test model deployment")
+    ...    .with_freeform_tags(tag1="val1", tag2="val2")
+    ...    .with_infrastructure(
+    ...        (ModelDeploymentInfrastructure()
+    ...        .with_project_id(<project_id>)
+    ...        .with_compartment_id(<compartment_id>)
+    ...        .with_shape_name("VM.Standard.E4.Flex")
+    ...        .with_shape_config_details(
+    ...            ocpus=1,
+    ...            memory_in_gbs=16
+    ...        )
+    ...        .with_replica(1)
+    ...        .with_bandwidth_mbps(10)
+    ...        .with_web_concurrency(10)
+    ...        .with_access_log(
+    ...            log_group_id=<log_group_id>,
+    ...            log_id=<log_id>
+    ...        )
+    ...        .with_predict_log(
+    ...            log_group_id=<log_group_id>,
+    ...            log_id=<log_id>
+    ...        ))
+    ...    )
+    ...    .with_runtime(
+    ...        (ModelDeploymentContainerRuntime()
+    ...        .with_image(<image>)
+    ...        .with_image_digest(<image_digest>)
+    ...        .with_entrypoint(<entrypoint>)
+    ...        .with_server_port(<server_port>)
+    ...        .with_health_check_port(<health_check_port>)
+    ...        .with_env({"key":"value"})
+    ...        .with_deployment_mode("HTTPS_ONLY")
+    ...        .with_model_uri(<model_uri>)
+    ...        .with_bucket_uri(<bucket_uri>)
+    ...        .with_auth(<auth>)
+    ...        .with_timeout(<time_out>))
+    ...    )
+    ... )
+    >>> ds_model_deployment.deploy()
+    >>> ds_model_deployment.status
+    >>> ds_model_deployment.with_display_name("new name").update()
+    >>> ds_model_deployment.deactivate()
+    >>> ds_model_deployment.sync()
+    >>> ds_model_deployment.list(status="ACTIVE")
+    >>> ds_model_deployment.delete()
 
-    CONST_DEFAULT_BLOCK_STORAGE_SIZE = 50
+    >>> # Build model deployment from yaml
+    >>> ds_model_deployment = ModelDeployment.from_yaml(uri=<path_to_yaml>)
+    """
 
-    def __init__(self, artifact: Union[str, Artifact] = None, **kwargs) -> None:
-        """Initialize a DSCJob object.
+    _PREFIX = "datascience_model_deployment"
 
-        Parameters
-        ----------
-        artifact: str or Artifact
-            Job artifact, which can be a path or an Artifact object. Defaults to None.
-        kwargs:
-            Same as kwargs in oci.data_science.models.Job.
-            Keyword arguments are passed into OCI Job model to initialize the properties.
+    CONST_ID = "id"
+    CONST_CREATED_BY = "createdBy"
+    CONST_DISPLAY_NAME = "displayName"
+    CONST_DESCRIPTION = "description"
+    CONST_FREEFORM_TAG = "freeformTags"
+    CONST_DEFINED_TAG = "definedTags"
+    CONST_MODEL_DEPLOYMENT_URL = "modelDeploymentUrl"
+    CONST_INFRASTRUCTURE = "infrastructure"
+    CONST_RUNTIME = "runtime"
+    CONST_LIFECYCLE_STATE = "lifecycleState"
+    CONST_LIFECYCLE_DETAILS = "lifecycleDetails"
+    CONST_TIME_CREATED = "timeCreated"
 
-        """
-        self._artifact = artifact
+    attribute_map = {
+        CONST_ID: "id",
+        CONST_CREATED_BY: "created_by",
+        CONST_DISPLAY_NAME: "display_name",
+        CONST_DESCRIPTION: "description",
+        CONST_FREEFORM_TAG: "freeform_tags",
+        CONST_DEFINED_TAG: "defined_tags",
+        CONST_MODEL_DEPLOYMENT_URL: "model_deployment_url",
+        CONST_INFRASTRUCTURE: "infrastructure",
+        CONST_RUNTIME: "runtime",
+        CONST_LIFECYCLE_STATE: "lifecycle_state",
+        CONST_LIFECYCLE_DETAILS: "lifecycle_details",
+        CONST_TIME_CREATED: "time_created",
+    }
 
-        super().__init__(**kwargs)
-        if not self.job_configuration_details:
-            self.job_configuration_details = {
-                "jobType": "DEFAULT",
-            }
-        if not self.job_infrastructure_configuration_details:
-            self.job_infrastructure_configuration_details = {}
+    initialize_spec_attributes = [
+        "display_name",
+        "description",
+        "freeform_tags",
+        "defined_tags",
+        "infrastructure",
+        "runtime",
+    ]
+    model_input_serializer = JsonModelInputSERDE()
 
-    @property
-    def artifact(self) -> Union[str, Artifact]:
-        """Job artifact.
+    def __init__(
+        self,
+        properties: Union[ModelDeploymentProperties, Dict] = None,
+        config: Dict = None,
+        model_deployment_id: str = None,
+        model_deployment_url: str = "",
+        spec: Dict = None,
+        **kwargs,
+    ):
+        """Initializes a ModelDeployment object.
 
-        Returns
-        -------
-        str or Artifact
-            When creating a job, this be a path or an Artifact object.
-            When loading the job from OCI, this will be the filename of the job artifact.
+        Parameters
+        ----------
+        properties: (Union[ModelDeploymentProperties, Dict], optional). Defaults to None.
+            Object containing deployment properties.
+            The properties can be `None` when `kwargs` are used for specifying properties.
+        config: (Dict, optional). Defaults to None.
+            ADS auth dictionary for OCI authentication.
+            This can be generated by calling `ads.common.auth.api_keys()` or `ads.common.auth.resource_principal()`.
+            If this is `None` then the `ads.common.default_signer(client_kwargs)` will be used.
+        model_deployment_id: (str, optional). Defaults to None.
+            Model deployment OCID.
+        model_deployment_url: (str, optional). Defaults to empty string.
+            Model deployment url.
+        spec: (dict, optional). Defaults to None.
+            Model deployment spec.
+        kwargs:
+            Keyword arguments for initializing `ModelDeploymentProperties` or `ModelDeployment`.
         """
-        if self.id and self._artifact is None:
-            try:
-                res = self.client.head_job_artifact(self.id)
-                content = res.headers.get("content-disposition")
-                if content and "filename=" in content:
-                    self._artifact = content.split("filename=", 1)[-1]
-            except ServiceError:
-                self._artifact = ""
-        return self._artifact
-
-    @artifact.setter
-    def artifact(self, artifact: Union[str, Artifact]):
-        """Sets the job artifact."""
-        self._artifact = artifact
-
-    def _load_infra_from_notebook(self, nb_config):
-        """Loads the infrastructure configuration from notebook configuration."""
-        infra = self.job_infrastructure_configuration_details
-        nb_shape_config_details = oci_util.to_dict(
-            getattr(nb_config, "notebook_session_shape_config_details", None) or {}
-        )
-        if isinstance(infra, dict):
-            shape_name = infra.get("shapeName", nb_config.shape)
-
-            # Ignore notebook shape config details if shape names do not match.
-            if shape_name != nb_config.shape:
-                nb_shape_config_details = {}
-
-            infra_type = infra.get("jobInfrastructureType")
-            block_storage = infra.get(
-                "blockStorageSizeInGBs", nb_config.block_storage_size_in_gbs
-            )
-            subnet_id = infra.get(
-                "subnetId",
-                nb_config.subnet_id
-                if infra_type
-                != JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
-                else None,
-            )
-            job_shape_config_details = infra.get("jobShapeConfigDetails", {})
-            memory_in_gbs = job_shape_config_details.get(
-                "memoryInGBs", nb_shape_config_details.get("memory_in_gbs")
-            )
-            ocpus = job_shape_config_details.get(
-                "ocpus", nb_shape_config_details.get("ocpus")
-            )
-        else:
-            shape_name = (
-                infra.shape_name
-                if getattr(infra, "shape_name", None)
-                else nb_config.shape
-            )
-            # Ignore notebook shape config details if shape names do not match.
-            if shape_name != nb_config.shape:
-                nb_shape_config_details = {}
-
-            infra_type = getattr(infra, "job_infrastructure_type", None)
-
-            block_storage = (
-                infra.block_storage_size_in_gbs
-                if getattr(infra, "block_storage_size_in_gbs", None)
-                else nb_config.block_storage_size_in_gbs
-            )
-            subnet_id = (
-                infra.subnet_id
-                if getattr(infra, "subnet_id", None)
-                else (
-                    nb_config.subnet_id
-                    if infra_type
-                    != JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_ME_STANDALONE
-                    else None
-                )
-            )
-            job_shape_config_details = oci_util.to_dict(
-                getattr(infra, "job_shape_config_details", {}) or {}
-            )
-            memory_in_gbs = job_shape_config_details.get(
-                "memory_in_gbs", nb_shape_config_details.get("memory_in_gbs")
-            )
-            ocpus = job_shape_config_details.get(
-                "ocpus", nb_shape_config_details.get("ocpus")
+
+        if spec and properties:
+            raise ValueError(
+                "You can only pass in either `spec` or `properties` to initialize model deployment instance."
             )
 
-        self.job_infrastructure_configuration_details = {
-            "jobInfrastructureType": infra_type,
-            "shapeName": shape_name,
-            "blockStorageSizeInGBs": block_storage,
-        }
-        # ADS does not provide explicit API for setting infrastructure type.
-        # If subnet is configured, the type will be set to STANDALONE,
-        # otherwise ME_STANDALONE
-        if subnet_id:
-            self.job_infrastructure_configuration_details.update(
-                {
-                    "subnetId": subnet_id,
-                    "jobInfrastructureType": JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE,
-                }
+        if config:
+            warnings.warn(
+                "Parameter `config` was deprecated in 2.8.2 from ModelDeployment constructor and will be removed in 3.0.0. Please use `ads.set_auth()` to config the auth information. "
+                "Check: https://accelerated-data-science.readthedocs.io/en/latest/user_guide/cli/authentication.html"
             )
-        else:
-            self.job_infrastructure_configuration_details.update(
-                {
-                    "jobInfrastructureType": self.DEFAULT_INFRA_TYPE,
-                }
-            )
-
-        # Specify shape config details
-        if memory_in_gbs or ocpus:
-            self.job_infrastructure_configuration_details.update(
-                {
-                    "jobShapeConfigDetails": {
-                        "memoryInGBs": memory_in_gbs,
-                        "ocpus": ocpus,
-                    }
-                }
-            )
-
-    def load_properties_from_env(self) -> None:
-        """Loads default properties from the environment"""
-        if "NB_SESSION_OCID" in os.environ:
-            try:
-                nb_session = DSCNotebookSession.from_ocid(os.environ["NB_SESSION_OCID"])
-            except Exception:
-                logger.debug("Failed to load config from notebook.")
-                logger.debug(traceback.format_exc())
-                # If there is an error loading the notebook infra configurations.
-                # Ignore it by setting nb_session to None
-                # This will skip loading the default configure.
-                nb_session = None
-            if nb_session:
-                nb_config = getattr(
-                    nb_session,
-                    "notebook_session_config_details",
-                    getattr(nb_session, "notebook_session_configuration_details", None),
-                )
 
-                if nb_config:
-                    self._load_infra_from_notebook(nb_config)
-                if self.project_id is None:
-                    self.project_id = nb_session.project_id
-        super().load_properties_from_env()
-
-    def load_defaults(self) -> DSCJob:
-        self.load_properties_from_env()
-        if not self.job_infrastructure_configuration_details:
-            self.job_infrastructure_configuration_details = {}
-        # Convert the dict to JobInfrastructureConfigurationDetails object
-        if isinstance(self.job_infrastructure_configuration_details, dict):
-            # Default networking
-            if not self.job_infrastructure_configuration_details.get(
-                "jobInfrastructureType"
-            ):
-                self.job_infrastructure_configuration_details[
-                    "jobInfrastructureType"
-                ] = self.DEFAULT_INFRA_TYPE
-            self.job_infrastructure_configuration_details = self.deserialize(
-                self.job_infrastructure_configuration_details,
-                JobInfrastructureConfigurationDetails.__name__,
+        if properties:
+            warnings.warn(
+                "Parameter `properties` was deprecated in 2.8.2 from ModelDeployment constructor and will be removed in 3.0.0. Please use `spec` or the builder pattern to initialize model deployment instance. "
+                "Check: https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/quick_start.html"
             )
 
-        # Default block storage size
-        if not self.job_infrastructure_configuration_details.block_storage_size_in_gbs:
-            self.job_infrastructure_configuration_details.block_storage_size_in_gbs = (
-                self.CONST_DEFAULT_BLOCK_STORAGE_SIZE
+        if model_deployment_url or model_deployment_id:
+            warnings.warn(
+                "Parameter `model_deployment_url` and `model_deployment_id` were deprecated in 2.8.2 from ModelDeployment constructor and will be removed in 3.0.0. These two fields will be auto-populated from the service side. "
+                "Check: https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/quick_start.html"
             )
-        return self
 
-    def _create_with_oci_api(self) -> None:
-        res = self.client.create_job(
-            self.to_oci_model(oci.data_science.models.CreateJobDetails)
-        )
-        self.update_from_oci_model(res.data)
-        if self.lifecycle_state == "ACTIVE":
-            return
-        try:
-            if issubclass(self.artifact.__class__, Artifact):
-                with self.artifact as artifact:
-                    self.upload_artifact(artifact.path)
-            else:
-                self.upload_artifact()
-        except Exception as ex:
-            # Delete the job if upload artifact is failed.
-            self.delete()
-            raise ex
+        initialize_spec = {}
+        initialize_spec_kwargs = {}
+        if spec:
+            initialize_spec = spec
+            initialize_spec_kwargs = self._extract_spec_kwargs(**kwargs)
+        elif not properties and not spec:
+            if self.CONST_INFRASTRUCTURE in kwargs or self.CONST_RUNTIME in kwargs:
+                initialize_spec_kwargs = self._extract_spec_kwargs(**kwargs)
 
-    def create(self) -> DSCJob:
-        """Create the job on OCI Data Science platform
+        super().__init__(spec=initialize_spec, **initialize_spec_kwargs)
 
-        Returns
-        -------
-        DSCJob
-            The DSCJob instance (self), which allows chaining additional method.
+        self.properties = (
+            properties
+            if isinstance(properties, ModelDeploymentProperties)
+            else ModelDeploymentProperties(oci_model_deployment=properties, **kwargs)
+        )
 
-        """
-        if not self.display_name:
-            if self.artifact:
-                timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d-%H:%M.%S")
-                self.display_name = (
-                    os.path.basename(str(self.artifact)).split(".")[0] + f"-{timestamp}"
-                )
-            else:
-                # Set default display_name if not specified - randomly generated easy to remember name generated
-                self.display_name = utils.get_random_name_for_resource()
-        try:
-            self.load_defaults()
-        except Exception:
-            logger.exception("Failed to load default properties.")
-        # Check compartment ID and project ID before calling the OCI API
-        if not self.compartment_id:
-            raise ValueError("Specify compartment ID for data science job.")
-        if not self.project_id:
-            raise ValueError("Specify project ID for data science job.")
-        self._create_with_oci_api()
-        return self
+        self.current_state = (
+            State._from_str(self.properties.lifecycle_state)
+            if self.properties.lifecycle_state
+            else State.UNKNOWN
+        )
 
-    def update(self) -> DSCJob:
-        """Updates the Data Science Job."""
-        raise NotImplementedError("Updating Job is not supported at the moment.")
+        self._access_log = None
+        self._predict_log = None
+        self.dsc_model_deployment = OCIDataScienceModelDeployment()
 
-    def delete(self) -> DSCJob:
-        """Deletes the job and the corresponding job runs.
+    @property
+    def kind(self) -> str:
+        """The kind of the object as showing in YAML.
 
         Returns
         -------
-        DSCJob
-            The DSCJob instance (self), which allows chaining additional method.
-
+        str
+            deployment
         """
-        runs = self.run_list()
-        for run in runs:
-            run.delete()
-        self.client.delete_job(self.id)
-        return self
+        return MODEL_DEPLOYMENT_KIND
 
-    def upload_artifact(self, artifact_path: str = None) -> DSCJob:
-        """Uploads the job artifact to OCI
-
-        Parameters
-        ----------
-        artifact_path : str, optional
-            Local path to the job artifact file to be uploaded, by default None.
-            If artifact_path is None, the path in self.artifact will be used.
+    @property
+    def type(self) -> str:
+        """The type of the object as showing in YAML.
 
         Returns
         -------
-        DSCJob
-            The DSCJob instance (self), which allows chaining additional method.
-
+        str
+            deployment
         """
-        if not artifact_path:
-            artifact_path = self.artifact
-        with fsspec.open(artifact_path, "rb") as f:
-            self.client.create_job_artifact(
-                self.id,
-                f,
-                content_disposition=f"attachment; filename={os.path.basename(artifact_path)}",
-            )
-        return self
+        return MODEL_DEPLOYMENT_TYPE
 
-    def download_artifact(self, artifact_path: str) -> DSCJob:
-        """Downloads the artifact from OCI
-
-        Parameters
-        ----------
-        artifact_path : str
-            Local path to store the job artifact.
+    @property
+    def model_deployment_id(self) -> str:
+        """The model deployment ocid.
 
         Returns
         -------
-        DSCJob
-            The DSCJob instance (self), which allows chaining additional method.
-
+        str
+            The model deployment ocid.
         """
-        res = self.client.get_job_artifact_content(self.id)
-        with open(artifact_path, "wb") as f:
-            for chunk in res.data.iter_content(chunk_size=DEFAULT_BUFFER_SIZE * 16):
-                f.write(chunk)
-        return self
-
-    def run_list(self, **kwargs) -> list[DataScienceJobRun]:
-        """Lists the runs of this job.
+        return self.get_spec(self.CONST_ID, None)
 
-        Parameters
-        ----------
-        **kwargs :
-            Keyword arguments to te passed into the OCI list_job_runs() for filtering the job runs.
+    @property
+    def created_by(self) -> str:
+        """The user that creates the model deployment.
 
         Returns
         -------
-        list
-            A list of DSCJobRun objects
-
+        str
+            The user that creates the model deployment.
         """
-        items = oci.pagination.list_call_get_all_results(
-            self.client.list_job_runs, self.compartment_id, job_id=self.id, **kwargs
-        ).data
-        return [DataScienceJobRun.from_oci_model(item) for item in items]
+        return self.get_spec(self.CONST_CREATED_BY, None)
 
-    def run(self, **kwargs) -> DataScienceJobRun:
-        """Runs the job
-
-        Parameters
-        ----------
-        **kwargs :
-            Keyword arguments for initializing a Data Science Job Run.
-            The keys can be any keys in supported by OCI JobConfigurationDetails and JobRun, including:
-            * hyperparameter_values: dict(str, str)
-            * environment_variables: dict(str, str)
-            * command_line_arguments: str
-            * maximum_runtime_in_minutes: int
-            * display_name: str
-            * freeform_tags: dict(str, str)
-            * defined_tags: dict(str, dict(str, object))
-
-        If display_name is not specified, it will be generated as "<JOB_NAME>-run-<TIMESTAMP>".
+    @property
+    def url(self) -> str:
+        """Model deployment url.
 
         Returns
         -------
-        DSCJobRun
-            An instance of DSCJobRun, which can be used to monitor the job run.
-
+        str
+            Model deployment url.
         """
-        if not self.id:
-            self.create()
-
-        swagger_types = (
-            oci.data_science.models.DefaultJobConfigurationDetails().swagger_types.keys()
-        )
-        config_kwargs = {}
-        keys = list(kwargs.keys())
-        for key in keys:
-            if key in swagger_types:
-                config_kwargs[key] = kwargs.pop(key)
+        return self.get_spec(self.CONST_MODEL_DEPLOYMENT_URL, None)
 
-        # remove timestamp from the job name (added in default names, when display_name not specified by user)
-        if self.display_name:
-            try:
-                datetime.datetime.strptime(self.display_name[-19:], "%Y-%m-%d-%H:%M.%S")
-                self.display_name = self.display_name[:-20]
-            except ValueError:
-                pass
-
-        job_attrs = dict(
-            project_id=self.project_id,
-            display_name=self.display_name
-            + "-run-"
-            + datetime.datetime.now().strftime("%Y-%m-%d-%H:%M.%S"),
-            job_id=self.id,
-            compartment_id=self.compartment_id,
-        )
-
-        for key, val in job_attrs.items():
-            if not kwargs.get(key):
-                kwargs[key] = val
-
-        if config_kwargs:
-            config_kwargs["jobType"] = "DEFAULT"
-            config_override = kwargs.get("job_configuration_override_details", {})
-            config_override.update(config_kwargs)
-            kwargs["job_configuration_override_details"] = config_override
-
-        wait = kwargs.pop("wait", False)
-        run = DataScienceJobRun(**kwargs).create()
-        if wait:
-            return run.watch()
-        return run
-
-    @classmethod
-    def from_ocid(cls, ocid) -> DSCJob:
-        """Gets a job by OCID
-
-        Parameters
-        ----------
-        ocid : str
-            The OCID of the job.
+    @property
+    def lifecycle_state(self) -> str:
+        """Model deployment lifecycle state.
 
         Returns
         -------
-        DSCJob
-            An instance of DSCJob.
-
+        str
+            Model deployment lifecycle state.
         """
-        return super().from_ocid(ocid)
-
-
-class DataScienceJobRun(
-    OCIDataScienceMixin, oci.data_science.models.JobRun, RunInstance
-):
-    """Represents a Data Science Job run"""
-
-    _DETAILS_LINK = (
-        "https://console.{region}.oraclecloud.com/data-science/job-runs/{id}"
-    )
-
-    TERMINAL_STATES = [
-        oci.data_science.models.JobRun.LIFECYCLE_STATE_SUCCEEDED,
-        oci.data_science.models.JobRun.LIFECYCLE_STATE_FAILED,
-        oci.data_science.models.JobRun.LIFECYCLE_STATE_CANCELED,
-        oci.data_science.models.JobRun.LIFECYCLE_STATE_DELETED,
-    ]
-
-    def create(self) -> DataScienceJobRun:
-        """Creates a job run"""
-        self.load_properties_from_env()
-        res = self.client.create_job_run(
-            self.to_oci_model(oci.data_science.models.CreateJobRunDetails)
-        )
-        self.update_from_oci_model(res.data)
-        return self
+        return self.get_spec(self.CONST_LIFECYCLE_STATE, None)
 
     @property
-    def status(self) -> str:
-        """Lifecycle status
+    def lifecycle_details(self) -> str:
+        """Model deployment lifecycle details.
 
         Returns
         -------
         str
-            Status in a string.
+            Model deployment lifecycle details.
         """
-        return self.lifecycle_state
+        return self.get_spec(self.CONST_LIFECYCLE_DETAILS, None)
 
     @property
-    def log_id(self) -> str:
-        """The log ID from OCI logging service containing the logs from the job run."""
-        if not self.log_details:
-            return None
-        return self.log_details.log_id
+    def time_created(self) -> datetime:
+        """The time when the model deployment is created.
 
-    @property
-    def log_group_id(self) -> str:
-        """The log group ID from OCI logging service containing the logs from the job run."""
-        if not self.log_details:
-            return None
-        return self.log_details.log_group_id
+        Returns
+        -------
+        datetime
+            The time when the model deployment is created.
+        """
+        return self.get_spec(self.CONST_TIME_CREATED, None)
 
     @property
-    def logging(self) -> OCILog:
-        """The OCILog object containing the logs from the job run"""
-        if not self.log_id:
-            raise ValueError("Log OCID is not specified for this job run.")
-        # Specifying log group ID when initializing OCILog can reduce the number of API calls.
-        return OCILog(id=self.log_id, log_group_id=self.log_details.log_group_id)
-
-    @staticmethod
-    def _format_log(message: str, date_time: datetime.datetime) -> dict:
-        """Formats a message as log record with datetime.
-        This is used to add additional logs to show job run status change.
-
-        Parameters
-        ----------
-        message : str
-            Log message.
-        date_time : datetime or str
-            Timestamp for the message
+    def display_name(self) -> str:
+        """Model deployment display name.
 
         Returns
         -------
-        dict
-            log record as a dictionary, including id, time and message as keys.
+        str
+            Model deployment display name.
         """
-        if isinstance(date_time, datetime.datetime):
-            date_time = date_time.strftime("%Y-%m-%dT%H:%M:%S.000Z")
-        return {
-            "id": str(uuid.uuid4()),
-            "message": message,
-            "time": date_time,
-        }
+        return self.get_spec(self.CONST_DISPLAY_NAME, None)
 
-    def logs(self, limit: int = None) -> list:
-        """Gets the logs of the job run.
+    def with_display_name(self, display_name: str) -> "ModelDeployment":
+        """Sets the name of model deployment.
 
         Parameters
         ----------
-        limit : int, optional
-            Limit the number of logs to be returned.
-            Defaults to None. All logs will be returned.
+        display_name: str
+            The name of model deployment.
 
         Returns
         -------
-        list
-            A list of log records. Each log record is a dictionary with the following keys: id, time, message.
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        if self.time_accepted:
-            log_messages = self.logging.tail(
-                source=self.id, limit=limit, time_start=self.time_accepted
-            )
-        else:
-            log_messages = []
-        if self.time_started:
-            log_messages.insert(
-                0, self._format_log("Job Run STARTED", self.time_started)
-            )
-        if self.time_accepted:
-            log_messages.insert(
-                0, self._format_log("Job Run ACCEPTED", self.time_accepted)
-            )
-        if self.time_finished:
-            log_messages.append(
-                self._format_log("Job Run FINISHED", self.time_finished)
-            )
-        return log_messages
+        return self.set_spec(self.CONST_DISPLAY_NAME, display_name)
 
-    def _job_run_status_text(self) -> str:
-        details = f", {self.lifecycle_details}" if self.lifecycle_details else ""
-        return f"Job Run {self.lifecycle_state}" + details
+    @property
+    def description(self) -> str:
+        """Model deployment description.
 
-    def _check_and_print_status(self, prev_status) -> str:
-        status = self._job_run_status_text()
-        if status != prev_status:
-            if self.lifecycle_state in self.TERMINAL_STATES and self.time_finished:
-                timestamp = self.time_finished.strftime("%Y-%m-%d %H:%M:%S")
-            else:
-                timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
-            print(f"{timestamp} - {status}")
-        return status
+        Returns
+        -------
+        str
+            Model deployment description.
+        """
+        return self.get_spec(self.CONST_DESCRIPTION, None)
 
-    def watch(
-        self,
-        interval: float = SLEEP_INTERVAL,
-        wait: float = WAIT_SECONDS_AFTER_FINISHED,
-    ) -> DataScienceJobRun:
-        """Watches the job run until it finishes.
-        Before the job start running, this method will output the job run status.
-        Once the job start running,
-        the logs will be streamed until the job is success, failed or cancelled.
+    def with_description(self, description: str) -> "ModelDeployment":
+        """Sets the description of model deployment.
 
         Parameters
         ----------
-        interval : float
-            Time interval in seconds between each request to update the logs.
-            Defaults to 3 (seconds).
-        wait : float
-            Time in seconds to keep updating the logs after the job run finished.
-            It may take some time for logs to appear in OCI logging service
-            after the job run is finished.
-            Defaults to 90 (seconds).
+        description: str
+            The description of model deployment.
 
+        Returns
+        -------
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
+        return self.set_spec(self.CONST_DESCRIPTION, description)
 
-        def stop_condition():
-            """Stops the log streaming once the job is in a terminal state."""
-            self.sync()
-            if self.lifecycle_state not in self.TERMINAL_STATES:
-                return False
-            # Stop if time_finished is not available.
-            if not self.time_finished:
-                return True
-            # Stop only if time_finished is over 2 minute ago.
-            # This is for the time delay between job run stopped and the logs appear in oci logging.
-            if (
-                datetime.datetime.now(self.time_finished.tzinfo)
-                - datetime.timedelta(seconds=wait)
-                > self.time_finished
-            ):
-                return True
-            return False
-
-        if not self.log_id and not self.log_group_id:
-            print(
-                "Logging is not configured for the job. Watch() will only show job status."
-            )
-
-        print(f"Job OCID: {self.job.id}")
-        print(f"Job Run OCID: {self.id}")
-
-        status = ""
-        while not stop_condition():
-            status = self._check_and_print_status(status)
-            # Break and stream logs if job has log ID and started.
-            # Otherwise, keep watching the status until job terminates.
-            if self.time_started and self.log_id:
-                break
-            time.sleep(interval)
-
-        if self.log_id and self.time_accepted:
-            count = self.logging.stream(
-                source=self.id,
-                interval=interval,
-                stop_condition=stop_condition,
-                time_start=self.time_accepted,
-            )
-            if not count:
-                print(
-                    "No logs in the last 14 days. Please set time_start to see older logs."
-                )
-
-        self._check_and_print_status(status)
-
-        return self
-
-    def cancel(self) -> DataScienceJobRun:
-        """Cancels a job run
-        This method will wait for the job run to be canceled before returning.
+    @property
+    def freeform_tags(self) -> Dict:
+        """Model deployment freeform tags.
 
         Returns
         -------
-        self
-            The job run instance.
+        Dict
+            Model deployment freeform tags.
         """
-        self.client.cancel_job_run(self.id)
-        while self.lifecycle_state != "CANCELED":
-            self.sync()
-            time.sleep(SLEEP_INTERVAL)
-        return self
+        return self.get_spec(self.CONST_FREEFORM_TAG, {})
 
-    def __repr__(self) -> str:
-        """Displays the object as YAML."""
-        return self.to_yaml()
+    def with_freeform_tags(self, **kwargs) -> "ModelDeployment":
+        """Sets the freeform tags of model deployment.
 
-    def to_yaml(self) -> str:
-        """Serializes the object into YAML string.
+        Parameters
+        ----------
+        kwargs
+            The freeform tags of model deployment.
 
         Returns
         -------
-        str
-            YAML stored in a string.
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        # Here the job YAML is used as the base for the job run
-        job_dict = self.job.to_dict()
-
-        # Update infrastructure from job run
-        run_dict = self.to_dict()
-        infra_specs = [
-            run_dict,
-            run_dict.get("jobInfrastructureConfigurationDetails", {}),
-            run_dict.get("logDetails", {}),
-        ]
-        for infra_spec in infra_specs:
-            for key in infra_spec:
-                if key in job_dict["spec"]["infrastructure"]["spec"]:
-                    job_dict["spec"]["infrastructure"]["spec"][key] = infra_spec[key]
-
-        # Update runtime from job run
-        from ads.jobs import Job
-
-        job = Job.from_dict(job_dict)
-        envs = job.runtime.envs
-        run_config_override = run_dict.get("jobConfigurationOverrideDetails", {})
-        envs.update(run_config_override.get("environmentVariables", {}))
-        job.runtime.with_environment_variable(**envs)
-        if run_config_override.get("commandLineArguments"):
-            job.runtime.set_spec(
-                "args",
-                run_config_override.get("commandLineArguments"),
-            )
-
-        # Update kind, id and name
-        run_dict = job.to_dict()
-        run_dict["kind"] = "jobRun"
-        run_dict["spec"]["id"] = self.id
-        run_dict["spec"]["name"] = self.display_name
-        return yaml.safe_dump(run_dict)
+        return self.set_spec(self.CONST_FREEFORM_TAG, kwargs)
 
     @property
-    def job(self):
-        """The job instance of this run.
+    def defined_tags(self) -> Dict:
+        """Model deployment defined tags.
 
         Returns
         -------
-        Job
-            An ADS Job instance
+        Dict
+            Model deployment defined tags.
         """
-        from ads.jobs import Job
-
-        return Job.from_datascience_job(self.job_id)
+        return self.get_spec(self.CONST_DEFINED_TAG, {})
 
-    def download(self, to_dir):
-        """Downloads files from job run output URI to local.
+    def with_defined_tags(self, **kwargs) -> "ModelDeployment":
+        """Sets the defined tags of model deployment.
 
         Parameters
         ----------
-        to_dir : str
-            Local directory to which the files will be downloaded to.
+        kwargs
+            The defined tags of model deployment.
 
         Returns
         -------
-        DataScienceJobRun
-            The job run instance (self)
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        self.job.download(to_dir)
-        return self
-
-
-# This is for backward compatibility
-DSCJobRun = DataScienceJobRun
-
-
-class DataScienceJob(Infrastructure):
-    """Represents the OCI Data Science Job infrastructure.
-
-    To configure the infrastructure for a Data Science Job::
-
-        infrastructure = (
-            DataScienceJob()
-            # Configure logging for getting the job run outputs.
-            .with_log_group_id("<log_group_ocid>")
-            # Log resource will be auto-generated if log ID is not specified.
-            .with_log_id("<log_ocid>")
-            # If you are in an OCI data science notebook session,
-            # the following configurations are not required.
-            # Configurations from the notebook session will be used as defaults.
-            .with_compartment_id("<compartment_ocid>")
-            .with_project_id("<project_ocid>")
-            .with_subnet_id("<subnet_ocid>")
-            .with_shape_name("VM.Standard.E3.Flex")
-            # Shape config details are applicable only for the flexible shapes.
-            .with_shape_config_details(memory_in_gbs=16, ocpus=1)
-            # Minimum/Default block storage size is 50 (GB).
-            .with_block_storage_size(50)
-            # A list of file systems to be mounted
-            .with_storage_mount(
-                {
-                    "src" : "<mount_target_ip_address>:<export_path>",
-                    "dest" : "<destination_directory_name>"
-                }
-            )
-            # Tags
-            .with_freeform_tag(my_tag="my_value")
-            .with_defined_tag(**{"Operations": {"CostCenter": "42"}})
-        )
-
-    """
-
-    CONST_PROJECT_ID = "projectId"
-    CONST_COMPARTMENT_ID = "compartmentId"
-    CONST_DISPLAY_NAME = "displayName"
-    CONST_JOB_TYPE = "jobType"
-    CONST_JOB_INFRA = "jobInfrastructureType"
-    CONST_SHAPE_NAME = "shapeName"
-    CONST_BLOCK_STORAGE = "blockStorageSize"
-    CONST_SUBNET_ID = "subnetId"
-    CONST_SHAPE_CONFIG_DETAILS = "shapeConfigDetails"
-    CONST_MEMORY_IN_GBS = "memoryInGBs"
-    CONST_OCPUS = "ocpus"
-    CONST_LOG_ID = "logId"
-    CONST_LOG_GROUP_ID = "logGroupId"
-    CONST_STORAGE_MOUNT = "storageMount"
-    CONST_FREEFORM_TAGS = "freeformTags"
-    CONST_DEFINED_TAGS = "definedTags"
-
-    attribute_map = {
-        CONST_PROJECT_ID: "project_id",
-        CONST_COMPARTMENT_ID: "compartment_id",
-        CONST_DISPLAY_NAME: "display_name",
-        CONST_JOB_TYPE: "job_type",
-        CONST_JOB_INFRA: "job_infrastructure_type",
-        CONST_SHAPE_NAME: "shape_name",
-        CONST_BLOCK_STORAGE: "block_storage_size",
-        CONST_SUBNET_ID: "subnet_id",
-        CONST_SHAPE_CONFIG_DETAILS: "shape_config_details",
-        CONST_LOG_ID: "log_id",
-        CONST_LOG_GROUP_ID: "log_group_id",
-        CONST_STORAGE_MOUNT: "storage_mount",
-        CONST_FREEFORM_TAGS: "freeform_tags",
-        CONST_DEFINED_TAGS: "defined_tags",
-    }
-
-    shape_config_details_attribute_map = {
-        CONST_MEMORY_IN_GBS: "memory_in_gbs",
-        CONST_OCPUS: "ocpus",
-    }
-
-    payload_attribute_map = {
-        CONST_PROJECT_ID: "project_id",
-        CONST_COMPARTMENT_ID: "compartment_id",
-        CONST_DISPLAY_NAME: "display_name",
-        CONST_JOB_TYPE: "job_configuration_details.job_type",
-        CONST_JOB_INFRA: "job_infrastructure_configuration_details.job_infrastructure_type",
-        CONST_SHAPE_NAME: "job_infrastructure_configuration_details.shape_name",
-        CONST_BLOCK_STORAGE: "job_infrastructure_configuration_details.block_storage_size_in_gbs",
-        CONST_SUBNET_ID: "job_infrastructure_configuration_details.subnet_id",
-        CONST_SHAPE_CONFIG_DETAILS: "job_infrastructure_configuration_details.job_shape_config_details",
-        CONST_LOG_ID: "job_log_configuration_details.log_id",
-        CONST_LOG_GROUP_ID: "job_log_configuration_details.log_group_id",
-    }
-
-    snake_to_camel_map = {
-        v.split(".", maxsplit=1)[-1]: k for k, v in payload_attribute_map.items()
-    }
-
-    storage_mount_type_dict = {FILE_STORAGE_TYPE: OCIFileStorage}
+        return self.set_spec(self.CONST_DEFINED_TAG, kwargs)
 
-    @staticmethod
-    def standardize_spec(spec):
-        if not spec:
-            return {}
-
-        attribute_map = {
-            **DataScienceJob.attribute_map,
-            **DataScienceJob.shape_config_details_attribute_map,
-        }
-        snake_to_camel_map = {v: k for k, v in attribute_map.items()}
-        snake_to_camel_map = {
-            **{v: k for k, v in attribute_map.items()},
-            **DataScienceJob.snake_to_camel_map,
-        }
+    @property
+    def runtime(self) -> "ModelDeploymentRuntime":
+        """Model deployment runtime.
 
-        for key in list(spec.keys()):
-            if key not in attribute_map and key.lower() in snake_to_camel_map:
-                value = spec.pop(key)
-                if isinstance(value, dict):
-                    spec[
-                        snake_to_camel_map[key.lower()]
-                    ] = DataScienceJob.standardize_spec(value)
-                else:
-                    spec[snake_to_camel_map[key.lower()]] = value
-        return spec
+        Returns
+        -------
+        ModelDeploymentRuntime
+            Model deployment runtime.
+        """
+        return self.get_spec(self.CONST_RUNTIME, None)
 
-    def __init__(self, spec: Dict = None, **kwargs) -> None:
-        """Initializes a data science job infrastructure
+    def with_runtime(self, runtime: ModelDeploymentRuntime) -> "ModelDeployment":
+        """Sets the runtime of model deployment.
 
         Parameters
         ----------
-        spec : dict, optional
-            Object specification, by default None
-        kwargs: dict
-            Specification as keyword arguments.
-            If spec contains the same key as the one in kwargs, the value from kwargs will be used.
-        """
-        self.standardize_spec(spec)
-        self.standardize_spec(kwargs)
-        super().__init__(spec=spec, **kwargs)
-        if not self.job_type:
-            self.with_job_type("DEFAULT")
-        self.dsc_job = DSCJob()
-        self.runtime = None
-        self._name = None
-
-    @property
-    def name(self) -> str:
-        """Display name of the job"""
-        if self.dsc_job:
-            self._name = self.dsc_job.display_name
-        return self._name
+        runtime: ModelDeploymentRuntime
+            The runtime of model deployment.
 
-    @name.setter
-    def name(self, value: str):
-        """Sets the display name of the job
-
-        Parameters
-        ----------
-        value : str
-            The display name of the job
+        Returns
+        -------
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        self._name = value
-        if self.dsc_job:
-            self.dsc_job.display_name = value
-
-    @property
-    def job_id(self) -> Optional[str]:
-        """The OCID of the job"""
-        if self.dsc_job:
-            return self.dsc_job.id
-        return None
+        return self.set_spec(self.CONST_RUNTIME, runtime)
 
     @property
-    def status(self) -> Optional[str]:
-        """Status of the job.
+    def infrastructure(self) -> "ModelDeploymentInfrastructure":
+        """Model deployment infrastructure.
 
         Returns
         -------
-        str
-            Status of the job.
+        ModelDeploymentInfrastructure
+            Model deployment infrastructure.
         """
-        if self.dsc_job:
-            return self.dsc_job.lifecycle_state
-        return None
+        return self.get_spec(self.CONST_INFRASTRUCTURE, None)
 
-    def with_project_id(self, project_id: str) -> DataScienceJob:
-        """Sets the project OCID
+    def with_infrastructure(
+        self, infrastructure: ModelDeploymentInfrastructure
+    ) -> "ModelDeployment":
+        """Sets the infrastructure of model deployment.
 
         Parameters
         ----------
-        project_id : str
-            The project OCID
+        infrastructure: ModelDeploymentInfrastructure
+            The infrastructure of model deployment.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        return self.set_spec(self.CONST_PROJECT_ID, project_id)
-
-    @property
-    def project_id(self) -> Optional[str]:
-        """Project OCID"""
-        return self.get_spec(self.CONST_PROJECT_ID)
+        return self.set_spec(self.CONST_INFRASTRUCTURE, infrastructure)
 
-    def with_compartment_id(self, compartment_id: str) -> DataScienceJob:
-        """Sets the compartment OCID
+    def deploy(
+        self,
+        wait_for_completion: bool = True,
+        max_wait_time: int = DEFAULT_WAIT_TIME,
+        poll_interval: int = DEFAULT_POLL_INTERVAL,
+    ):
+        """Deploys the current ModelDeployment object
 
         Parameters
         ----------
-        compartment_id : str
-            The compartment OCID
+        wait_for_completion: bool
+            Flag set for whether to wait for deployment to be deployed before proceeding.
+            Defaults to True.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        ModelDeployment
+           The instance of ModelDeployment.
 
+        Raises
+        ------
+        ModelDeploymentFailedError
+            If model deployment fails to deploy
         """
-        return self.set_spec(self.CONST_COMPARTMENT_ID, compartment_id)
+        create_model_deployment_details = (
+            self._build_model_deployment_details()
+            if self._spec
+            else self.properties.build()
+        )
 
-    @property
-    def compartment_id(self) -> Optional[str]:
-        """The compartment OCID"""
-        return self.get_spec(self.CONST_COMPARTMENT_ID)
+        response = self.dsc_model_deployment.create(
+            create_model_deployment_details=create_model_deployment_details,
+            wait_for_completion=wait_for_completion,
+            max_wait_time=max_wait_time,
+            poll_interval=poll_interval,
+        )
+
+        if response.lifecycle_state == State.FAILED.name:
+            raise ModelDeploymentFailedError(
+                f"Model deployment {response.id} failed to deploy: {response.lifecycle_details}"
+            )
 
-    def with_job_type(self, job_type: str) -> DataScienceJob:
-        """Sets the job type
+        return self._update_from_oci_model(response)
+
+    def delete(
+        self,
+        wait_for_completion: bool = True,
+        max_wait_time: int = DEFAULT_WAIT_TIME,
+        poll_interval: int = DEFAULT_POLL_INTERVAL,
+    ):
+        """Deletes the ModelDeployment
 
         Parameters
         ----------
-        job_type : str
-            Job type as string
+        wait_for_completion: bool
+            Flag set for whether to wait for deployment to be deleted before proceeding.
+            Defaults to True.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The instance of ModelDeployment.
         """
-        return self.set_spec(self.CONST_JOB_TYPE, job_type)
-
-    @property
-    def job_type(self) -> Optional[str]:
-        """Job type"""
-        return self.get_spec(self.CONST_JOB_TYPE)
+        response = self.dsc_model_deployment.delete(
+            wait_for_completion=wait_for_completion,
+            max_wait_time=max_wait_time,
+            poll_interval=poll_interval,
+        )
+        return self._update_from_oci_model(response)
 
-    def with_job_infrastructure_type(self, infrastructure_type: str) -> DataScienceJob:
-        """Sets the job infrastructure type
+    def update(
+        self,
+        properties: Union[ModelDeploymentProperties, dict, None] = None,
+        wait_for_completion: bool = True,
+        max_wait_time: int = DEFAULT_WAIT_TIME,
+        poll_interval: int = DEFAULT_POLL_INTERVAL,
+        **kwargs,
+    ):
+        """Updates a model deployment
+
+        You can update `model_deployment_configuration_details` and change `instance_shape` and `model_id`
+        when the model deployment is in the ACTIVE lifecycle state.
+        The `bandwidth_mbps` or `instance_count` can only be updated while the model deployment is in the `INACTIVE` state.
+        Changes to the `bandwidth_mbps` or `instance_count` will take effect the next time
+        the `ActivateModelDeployment` action is invoked on the model deployment resource.
 
         Parameters
         ----------
-        infrastructure_type : str
-            Job infrastructure type as string
+        properties: ModelDeploymentProperties or dict
+            The properties for updating the deployment.
+        wait_for_completion: bool
+            Flag set for whether to wait for deployment to be updated before proceeding.
+            Defaults to True.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
+        kwargs:
+            dict
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The instance of ModelDeployment.
         """
-        return self.set_spec(self.CONST_JOB_INFRA, infrastructure_type)
+        if properties:
+            warnings.warn(
+                "Parameter `properties` is deprecated from ModelDeployment `update()` in 2.8.6 and will be removed in 3.0.0. Please use the builder pattern or kwargs to update model deployment instance. "
+                "Check: https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/quick_start.html"
+            )
 
-    @property
-    def job_infrastructure_type(self) -> Optional[str]:
-        """Job infrastructure type"""
-        return self.get_spec(self.CONST_JOB_INFRA)
+        updated_properties = properties
+        if not isinstance(properties, ModelDeploymentProperties):
+            updated_properties = ModelDeploymentProperties(
+                oci_model_deployment=properties, **kwargs
+            )
+
+        update_model_deployment_details = (
+            updated_properties.to_update_deployment()
+            if properties or updated_properties.oci_model_deployment or kwargs
+            else self._update_model_deployment_details(**kwargs)
+        )
+
+        response = self.dsc_model_deployment.update(
+            update_model_deployment_details=update_model_deployment_details,
+            wait_for_completion=wait_for_completion,
+            max_wait_time=max_wait_time,
+            poll_interval=poll_interval,
+        )
 
-    def with_shape_name(self, shape_name: str) -> DataScienceJob:
-        """Sets the shape name for running the job
+        return self._update_from_oci_model(response)
+
+    def watch(
+        self,
+        log_type: str = ModelDeploymentLogType.ACCESS,
+        time_start: datetime = None,
+        interval: int = LOG_INTERVAL,
+        log_filter: str = None,
+    ) -> "ModelDeployment":
+        """Streams the access and/or predict logs of model deployment.
 
         Parameters
         ----------
-        shape_name : str
-            Shape name
+        log_type: str, optional
+            The log type. Can be `access`, `predict` or None.
+            Defaults to access.
+        time_start : datetime.datetime, optional
+            Starting time for the log query.
+            Defaults to None.
+        interval : int, optional
+            The time interval between sending each request to pull logs from OCI logging service.
+            Defaults to 3.
+        log_filter : str, optional
+            Expression for filtering the logs. This will be the WHERE clause of the query.
+            Defaults to None.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The instance of ModelDeployment.
         """
-        return self.set_spec(self.CONST_SHAPE_NAME, shape_name)
+        status = ""
+        while not self._stop_condition():
+            status = self._check_and_print_status(status)
+            time.sleep(interval)
 
-    @property
-    def shape_name(self) -> Optional[str]:
-        """Shape name"""
-        return self.get_spec(self.CONST_SHAPE_NAME)
+        time_start = time_start or self.time_created
+        try:
+            count = self.logs(log_type).stream(
+                source=self.model_deployment_id,
+                interval=interval,
+                stop_condition=self._stop_condition,
+                time_start=time_start,
+                log_filter=log_filter,
+            )
+
+            if not count:
+                print(
+                    "No logs in the last 14 days. Please reset time_start to see older logs."
+                )
+            return self.sync()
+        except KeyboardInterrupt:
+            print("Stop watching logs.")
+            pass
+
+    def _stop_condition(self):
+        """Stops the sync once the model deployment is in a terminal state."""
+        return self.state in TERMINAL_STATES
 
-    def with_block_storage_size(self, size_in_gb: int) -> DataScienceJob:
-        """Sets the block storage size in GB
+    def _check_and_print_status(self, prev_status) -> str:
+        """Check and print the next status.
 
         Parameters
         ----------
-        size_in_gb : int
-            Block storage size in GB
+        prev_status: str
+            The previous model deployment status.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        str:
+            The next model deployment status.
+        """
+        status = self._model_deployment_status_text()
+        if status != prev_status:
+            timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
+            print(f"{timestamp} - {status}")
+        return status
+
+    def _model_deployment_status_text(self) -> str:
+        """Formats the status message.
 
+        Returns
+        -------
+        str:
+            The model deployment life status and life cycle details.
         """
-        return self.set_spec(self.CONST_BLOCK_STORAGE, size_in_gb)
+        details = f", {self.lifecycle_details}" if self.lifecycle_details else ""
+        return f"Model Deployment {self.lifecycle_state}" + details
+
+    @property
+    def state(self) -> State:
+        """Returns the deployment state of the current Model Deployment object"""
+        request_attempts = 0
+        while request_attempts < DEFAULT_RETRYING_REQUEST_ATTEMPTS:
+            request_attempts += 1
+            try:
+                self.current_state = State._from_str(self.sync().lifecycle_state)
+                break
+            except:
+                pass
+            time.sleep(1)
+
+        return self.current_state
 
     @property
-    def block_storage_size(self) -> int:
-        """Block storage size for the job"""
-        return self.get_spec(self.CONST_BLOCK_STORAGE)
+    def status(self) -> State:
+        """Returns the deployment state of the current Model Deployment object"""
+        return self.state
 
-    def with_subnet_id(self, subnet_id: str) -> DataScienceJob:
-        """Sets the subnet ID
+    def predict(
+        self,
+        json_input=None,
+        data: Any = None,
+        serializer: "ads.model.ModelInputSerializer" = model_input_serializer,
+        auto_serialize_data: bool = False,
+        model_name: str = None,
+        model_version: str = None,
+        **kwargs,
+    ) -> dict:
+        """Returns prediction of input data run against the model deployment endpoint.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> from ads.model import ModelInputSerializer
+        >>> class MySerializer(ModelInputSerializer):
+        ...     def serialize(self, data):
+        ...         serialized_data = 1
+        ...         return serialized_data
+        >>> model_deployment = ModelDeployment.from_id(<model_deployment_id>)
+        >>> prediction = model_deployment.predict(
+        ...        data=np.array([1, 2, 3]),
+        ...        serializer=MySerializer(),
+        ...        auto_serialize_data=True,
+        ... )['prediction']
 
         Parameters
         ----------
-        subnet_id : str
-            Subnet ID
+        json_input: Json serializable
+            JSON payload for the prediction.
+        data: Any
+            Data for the prediction.
+        serializer: ads.model.ModelInputSerializer
+            Defaults to ads.model.JsonModelInputSerializer.
+        auto_serialize_data: bool
+            Defaults to False. Indicate whether to auto serialize input data using `serializer`.
+            If `auto_serialize_data=False`, `data` required to be bytes or json serializable
+            and `json_input` required to be json serializable. If `auto_serialize_data` set
+            to True, data will be serialized before sending to model deployment endpoint.
+        model_name: str
+            Defaults to None. When the `inference_server="triton"`, the name of the model to invoke.
+        model_version: str
+            Defaults to None. When the `inference_server="triton"`, the version of the model to invoke.
+        kwargs:
+            content_type: str
+                Used to indicate the media type of the resource.
+                By default, it will be `application/octet-stream` for bytes input and `application/json` otherwise.
+                The content-type header will be set to this value when calling the model deployment endpoint.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        dict:
+            Prediction results.
 
         """
-        return self.set_spec(self.CONST_SUBNET_ID, subnet_id)
+        endpoint = f"{self.url}/predict"
+        signer = authutil.default_signer()["signer"]
+        header = {
+            "signer": signer,
+            "content_type": kwargs.get("content_type", None),
+        }
+        header.update(kwargs.pop("headers", {}))
 
-    @property
-    def subnet_id(self) -> str:
-        """Subnet ID"""
-        return self.get_spec(self.CONST_SUBNET_ID)
-
-    def with_shape_config_details(
-        self, memory_in_gbs: float, ocpus: float, **kwargs: Dict[str, Any]
-    ) -> DataScienceJob:
-        """Sets the details for the job run shape configuration.
-        Specify only when a flex shape is selected.
-        For example `VM.Standard.E3.Flex` allows the memory_in_gbs and cpu count to be specified.
+        if data is None and json_input is None:
+            raise AttributeError(
+                "Neither `data` nor `json_input` are provided. You need to provide one of them."
+            )
+        if data is not None and json_input is not None:
+            raise AttributeError(
+                "`data` and `json_input` are both provided. You can only use one of them."
+            )
+
+        if auto_serialize_data:
+            data = data or json_input
+            serialized_data = serializer.serialize(data=data)
+            return send_request(
+                data=serialized_data,
+                endpoint=endpoint,
+                is_json_payload=_is_json_serializable(serialized_data),
+                header=header,
+            )
+
+        if json_input is not None:
+            if not _is_json_serializable(json_input):
+                raise ValueError(
+                    "`json_input` must be json serializable. "
+                    "Set `auto_serialize_data` to True, or serialize the provided input data first,"
+                    "or using `data` to pass binary data."
+                )
+            utils.get_logger().warning(
+                "The `json_input` argument of `predict()` will be deprecated soon. "
+                "Please use `data` argument. "
+            )
+            data = json_input
+
+        is_json_payload = _is_json_serializable(data)
+        if not isinstance(data, bytes) and not is_json_payload:
+            raise TypeError(
+                "`data` is not bytes or json serializable. Set `auto_serialize_data` to `True` to serialize the input data."
+            )
+        if model_name and model_version:
+            header["model-name"] = model_name
+            header["model-version"] = model_version
+        elif bool(model_version) ^ bool(model_name):
+            raise ValueError(
+                "`model_name` and `model_version` have to be provided together."
+            )
+        prediction = send_request(
+            data=data,
+            endpoint=endpoint,
+            is_json_payload=is_json_payload,
+            header=header,
+        )
+        return prediction
+
+    def activate(
+        self,
+        wait_for_completion: bool = True,
+        max_wait_time: int = DEFAULT_WAIT_TIME,
+        poll_interval: int = DEFAULT_POLL_INTERVAL,
+    ) -> "ModelDeployment":
+        """Activates a model deployment
 
         Parameters
         ----------
-        memory_in_gbs: float
-            The size of the memory in GBs.
-        ocpus: float
-            The OCPUs count.
-        kwargs
-            Additional keyword arguments.
+        wait_for_completion: bool
+            Flag set for whether to wait for deployment to be activated before proceeding.
+            Defaults to True.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        ModelDeployment
+            The instance of ModelDeployment.
         """
-        return self.set_spec(
-            self.CONST_SHAPE_CONFIG_DETAILS,
-            {
-                self.CONST_OCPUS: ocpus,
-                self.CONST_MEMORY_IN_GBS: memory_in_gbs,
-                **kwargs,
-            },
+        response = self.dsc_model_deployment.activate(
+            wait_for_completion=wait_for_completion,
+            max_wait_time=max_wait_time,
+            poll_interval=poll_interval,
         )
 
-    @property
-    def shape_config_details(self) -> Dict:
-        """The details for the job run shape configuration."""
-        return self.get_spec(self.CONST_SHAPE_CONFIG_DETAILS)
+        return self._update_from_oci_model(response)
 
-    def with_log_id(self, log_id: str) -> DataScienceJob:
-        """Sets the log OCID for the data science job.
-        If log ID is specified, setting the log group ID (with_log_group_id()) is not strictly needed.
-        ADS will look up the log group ID automatically.
-        However, this may require additional permission,
-        and the look up may not be available for newly created log group.
-        Specifying both log ID (with_log_id()) and log group ID (with_log_group_id())
-        can avoid such lookup and speed up the job creation.
+    def deactivate(
+        self,
+        wait_for_completion: bool = True,
+        max_wait_time: int = DEFAULT_WAIT_TIME,
+        poll_interval: int = DEFAULT_POLL_INTERVAL,
+    ) -> "ModelDeployment":
+        """Deactivates a model deployment
 
         Parameters
         ----------
-        log_id : str
-            Log resource OCID.
+        wait_for_completion: bool
+            Flag set for whether to wait for deployment to be deactivated before proceeding.
+            Defaults to True.
+        max_wait_time: int
+            Maximum amount of time to wait in seconds (Defaults to 1200).
+            Negative implies infinite wait time.
+        poll_interval: int
+            Poll interval in seconds (Defaults to 10).
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        ModelDeployment
+            The instance of ModelDeployment.
         """
-        return self.set_spec(self.CONST_LOG_ID, log_id)
+        response = self.dsc_model_deployment.deactivate(
+            wait_for_completion=wait_for_completion,
+            max_wait_time=max_wait_time,
+            poll_interval=poll_interval,
+        )
 
-    @property
-    def log_id(self) -> str:
-        """Log OCID for the data science job.
+        return self._update_from_oci_model(response)
+
+    def _log_details(self, log_type: str = ModelDeploymentLogType.ACCESS):
+        """Gets log details for the provided `log_type`.
+
+        Properties
+        ----------
+        log_type: (str, optional). Defaults to "access".
+            The log type. Can be "access" or "predict".
 
         Returns
         -------
-        str
-            Log OCID
+        oci.datascience_model.CategoryLogDetails
+            Category log details of the ModelDeployment.
+
+        Raises
+        ------
+        AttributeError
+            Deployment doesn't have requested log configuration.
+
         """
-        return self.get_spec(self.CONST_LOG_ID)
+        if self.properties.category_log_details and getattr(
+            self.properties.category_log_details, log_type
+        ):
+            return getattr(self.properties.category_log_details, log_type)
+        elif self.infrastructure:
+            category_log_details = self._build_category_log_details()
+            log = category_log_details.get(log_type, None)
+            if log and log.get("logId", None) and log.get("logGroupId", None):
+                return LogDetails(
+                    log_id=log.get("logId"), log_group_id=log.get("logGroupId")
+                )
 
-    def with_log_group_id(self, log_group_id: str) -> DataScienceJob:
-        """Sets the log group OCID for the data science job.
-        If log group ID is specified but log ID is not,
-        a new log resource will be created automatically for each job run to store the logs.
+        raise LogNotConfiguredError(
+            f"Deployment `{self.model_deployment_id}` "
+            f"has no `{log_type}` log configuration."
+        )
 
-        Parameters
-        ----------
-        log_group_id : str
-            Log Group OCID
+    @property
+    def predict_log(self) -> OCILog:
+        """Gets the model deployment predict logs object.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        OCILog
+            The OCILog object containing the predict logs.
         """
-        return self.set_spec(self.CONST_LOG_GROUP_ID, log_group_id)
+        if not self._predict_log:
+            log_details = self._log_details(log_type=ModelDeploymentLogType.PREDICT)
+            compartment_id = (
+                self.infrastructure.compartment_id
+                if self.infrastructure
+                else self.properties.compartment_id
+            )
+            self._predict_log = OCILog(
+                compartment_id=compartment_id or COMPARTMENT_OCID,
+                id=log_details.log_id,
+                log_group_id=log_details.log_group_id,
+                source=self.model_deployment_id,
+                annotation=ModelDeploymentLogType.PREDICT,
+            )
+        return self._predict_log
 
     @property
-    def log_group_id(self) -> str:
-        """Log group OCID of the data science job
+    def access_log(self) -> OCILog:
+        """Gets the model deployment access logs object.
 
         Returns
         -------
-        str
-            Log group OCID
+        OCILog
+            The OCILog object containing the access logs.
         """
-        return self.get_spec(self.CONST_LOG_GROUP_ID)
+        if not self._access_log:
+            log_details = self._log_details(log_type=ModelDeploymentLogType.ACCESS)
+            compartment_id = (
+                self.infrastructure.compartment_id
+                if self.infrastructure
+                else self.properties.compartment_id
+            )
+            self._access_log = OCILog(
+                compartment_id=compartment_id or COMPARTMENT_OCID,
+                id=log_details.log_id,
+                log_group_id=log_details.log_group_id,
+                source=self.model_deployment_id,
+                annotation=ModelDeploymentLogType.ACCESS,
+            )
+        return self._access_log
 
-    def with_storage_mount(self, *storage_mount: List[dict]) -> DataScienceJob:
-        """Sets the file systems to be mounted for the data science job.
-        A maximum number of 5 file systems are allowed to be mounted for a single data science job.
+    def logs(self, log_type: str = None) -> ConsolidatedLog:
+        """Gets the access or predict logs.
 
         Parameters
         ----------
-        storage_mount : List[dict]
-            A list of file systems to be mounted.
+        log_type: (str, optional). Defaults to None.
+            The log type. Can be "access", "predict" or None.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        ConsolidatedLog
+            The ConsolidatedLog object containing the logs.
         """
-        storage_mount_list = []
-        for item in storage_mount:
-            if not isinstance(item, dict):
-                raise ValueError(
-                    "Parameter `storage_mount` should be a list of dictionaries."
+        loggers = []
+        if not log_type:
+            try:
+                loggers.append(self.access_log)
+            except LogNotConfiguredError:
+                pass
+
+            try:
+                loggers.append(self.predict_log)
+            except LogNotConfiguredError:
+                pass
+
+            if not loggers:
+                raise LogNotConfiguredError(
+                    "Neither `predict` nor `access` log was configured for the model deployment."
                 )
-            storage_mount_list.append(item)
-        if len(storage_mount_list) > MAXIMUM_MOUNT_COUNT:
+        elif log_type == ModelDeploymentLogType.ACCESS:
+            loggers = [self.access_log]
+        elif log_type == ModelDeploymentLogType.PREDICT:
+            loggers = [self.predict_log]
+        else:
             raise ValueError(
-                f"A maximum number of {MAXIMUM_MOUNT_COUNT} file systems are allowed to be mounted at this time for a job."
+                "Parameter log_type should be either access, predict or None."
             )
-        return self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount_list)
 
-    @property
-    def storage_mount(self) -> List[dict]:
-        """Files systems that have been mounted for the data science job
+        return ConsolidatedLog(*loggers)
 
-        Returns
-        -------
-        list
-            A list of file systems that have been mounted
-        """
-        return self.get_spec(self.CONST_STORAGE_MOUNT, [])
+    def show_logs(
+        self,
+        time_start: datetime.datetime = None,
+        time_end: datetime.datetime = None,
+        limit: int = LOG_RECORDS_LIMIT,
+        log_type: str = None,
+    ):
+        """Shows deployment logs as a pandas dataframe.
 
-    def with_freeform_tag(self, **kwargs) -> DataScienceJob:
-        """Sets freeform tags
+        Parameters
+        ----------
+        time_start: (datetime.datetime, optional). Defaults to None.
+            Starting date and time in RFC3339 format for retrieving logs.
+            Defaults to None. Logs will be retrieved 14 days from now.
+        time_end: (datetime.datetime, optional). Defaults to None.
+            Ending date and time in RFC3339 format for retrieving logs.
+            Defaults to None. Logs will be retrieved until now.
+        limit: (int, optional). Defaults to 100.
+            The maximum number of items to return.
+        log_type: (str, optional). Defaults to None.
+            The log type. Can be "access", "predict" or None.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-        """
-        return self.set_spec(self.CONST_FREEFORM_TAGS, kwargs)
+            A pandas DataFrame containing logs.
+        """
+        logging = self.logs(log_type=log_type)
+
+        def prepare_log_record(log):
+            """Converts a log record to ordered dict"""
+            log_content = log.get("logContent", {})
+            return collections.OrderedDict(
+                [
+                    ("type", log_content.get("type").split(".")[-1]),
+                    ("id", log_content.get("id")),
+                    ("message", log_content.get("data", {}).get("message")),
+                    ("time", log_content.get("time")),
+                ]
+            )
+
+        logs = logging.search(
+            source=self.model_deployment_id,
+            time_start=time_start,
+            time_end=time_end,
+            limit=limit,
+        )
+        return pd.DataFrame([prepare_log_record(log.data) for log in logs])
 
-    def with_defined_tag(self, **kwargs) -> DataScienceJob:
-        """Sets defined tags
+    def sync(self) -> "ModelDeployment":
+        """Updates the model deployment instance from backend.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        return self.set_spec(self.CONST_DEFINED_TAGS, kwargs)
-
-    @property
-    def freeform_tags(self) -> dict:
-        """Freeform tags"""
-        return self.get_spec(self.CONST_FREEFORM_TAGS, {})
-
-    @property
-    def defined_tags(self) -> dict:
-        """Defined tags"""
-        return self.get_spec(self.CONST_DEFINED_TAGS, {})
-
-    def _prepare_log_config(self) -> dict:
-        if not self.log_group_id and not self.log_id:
-            return None
-        # Look up log group ID if only the log ID is specified
-        if self.log_id and not self.log_group_id:
-            try:
-                log_obj = OCILog.from_ocid(self.log_id)
-            except ResourceNotFoundError as exc:
-                raise ResourceNotFoundError(
-                    f"Unable to determine log group ID for Log ({self.log_id})."
-                    " The log resource may not exist or You may not have the required permission."
-                    " Try to avoid this by specifying the log group ID."
-                ) from exc
-            self.with_log_group_id(log_obj.log_group_id)
-
-        if self.log_group_id and not self.log_id:
-            enable_auto_log_creation = True
-        else:
-            enable_auto_log_creation = False
-
-        log_config = {
-            "enable_logging": True,
-            "enable_auto_log_creation": enable_auto_log_creation,
-        }
-        if self.log_id:
-            log_config["log_id"] = self.log_id
-
-        if self.log_group_id:
-            log_config["log_group_id"] = self.log_group_id
-        return log_config
+        return self._update_from_oci_model(
+            OCIDataScienceModelDeployment.from_id(self.model_deployment_id)
+        )
 
-    def _update_from_dsc_model(
-        self, dsc_job: oci.data_science.models.Job, overwrite: bool = True
-    ) -> DataScienceJob:
-        """Update the properties from an OCI data science job model.
+    @classmethod
+    def list(
+        cls,
+        status: str = None,
+        compartment_id: str = None,
+        project_id: str = None,
+        **kwargs,
+    ) -> List["ModelDeployment"]:
+        """Lists the model deployments associated with current compartment id and status
 
         Parameters
         ----------
-        dsc_job: oci.data_science.models.Job
-            An OCI data science job model.
-
-        overwrite: bool
-            Whether to overwrite the existing values.
-            If this is set to False, only the empty/None properties will be updated.
+        status : str
+            Status of deployment. Defaults to None.
+            Allowed values: `ACTIVE`, `CREATING`, `DELETED`, `DELETING`, `FAILED`, `INACTIVE` and `UPDATING`.
+        compartment_id : str
+            Target compartment to list deployments from.
+            Defaults to the compartment set in the environment variable "NB_SESSION_COMPARTMENT_OCID".
+            If "NB_SESSION_COMPARTMENT_OCID" is not set, the root compartment ID will be used.
+            An ValueError will be raised if root compartment ID cannot be determined.
+        project_id : str
+            Target project to list deployments from.
+            Defaults to the project id in the environment variable "PROJECT_OCID".
+        kwargs :
+            The values are passed to oci.data_science.DataScienceClient.list_model_deployments.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        list
+            A list of ModelDeployment objects.
         """
-        sub_level = {
-            self.CONST_SHAPE_CONFIG_DETAILS: self.shape_config_details_attribute_map
-        }
-        self.dsc_job = dsc_job
-
-        for infra_attr, dsc_attr in self.payload_attribute_map.items():
-            value = get_value(dsc_job, dsc_attr)
-            if not value:
-                continue
-            if infra_attr not in sub_level:
-                if overwrite or not self._spec.get(infra_attr):
-                    self._spec[infra_attr] = value
-            else:
-                sub_spec = self._spec.get(infra_attr, {})
-                self._spec[infra_attr] = {}
-                for sub_infra_attr, sub_dsc_attr in sub_level[infra_attr].items():
-                    sub_value = get_value(value, sub_dsc_attr)
-                    if not sub_value:
-                        continue
-                    if overwrite or not sub_spec.get(sub_infra_attr):
-                        sub_spec[sub_infra_attr] = sub_value
-                if sub_spec:
-                    self._spec[infra_attr] = sub_spec
-
-        self._update_storage_mount_from_dsc_model(dsc_job, overwrite)
-        return self
+        deployments = OCIDataScienceModelDeployment.list(
+            status=status,
+            compartment_id=compartment_id,
+            project_id=project_id,
+            **kwargs,
+        )
+        return [cls()._update_from_oci_model(deployment) for deployment in deployments]
 
-    def _update_storage_mount_from_dsc_model(
-        self, dsc_job: oci.data_science.models.Job, overwrite: bool = True
-    ) -> DataScienceJob:
-        """Update the mount storage properties from an OCI data science job model.
+    @classmethod
+    def list_df(
+        cls,
+        status: str = None,
+        compartment_id: str = None,
+        project_id: str = None,
+    ) -> pd.DataFrame:
+        """Returns the model deployments associated with current compartment and status
+            as a Dataframe that can be easily visualized
 
         Parameters
         ----------
-        dsc_job: oci.data_science.models.Job
-            An OCI data science job model.
-
-        overwrite: bool
-            Whether to overwrite the existing values.
-            If this is set to False, only the empty/None properties will be updated.
+        status : str
+            Status of deployment. Defaults to None.
+            Allowed values: `ACTIVE`, `CREATING`, `DELETED`, `DELETING`, `FAILED`, `INACTIVE` and `UPDATING`.
+        compartment_id : str
+            Target compartment to list deployments from.
+            Defaults to the compartment set in the environment variable "NB_SESSION_COMPARTMENT_OCID".
+            If "NB_SESSION_COMPARTMENT_OCID" is not set, the root compartment ID will be used.
+            An ValueError will be raised if root compartment ID cannot be determined.
+        project_id : str
+            Target project to list deployments from.
+            Defaults to the project id in the environment variable "PROJECT_OCID".
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        DataFrame
+            pandas Dataframe containing information about the ModelDeployments
         """
-        storage_mount_list = get_value(
-            dsc_job, "job_storage_mount_configuration_details_list"
+        model_deployments = cls.list(
+            status=status, compartment_id=compartment_id, project_id=project_id
         )
-        if storage_mount_list:
-            storage_mount = [
-                self.storage_mount_type_dict[
-                    file_system.storage_type
-                ].update_from_dsc_model(file_system)
-                for file_system in storage_mount_list
-                if file_system.storage_type in self.storage_mount_type_dict
-            ]
-            if overwrite or not self.get_spec(self.CONST_STORAGE_MOUNT):
-                self.set_spec(self.CONST_STORAGE_MOUNT, storage_mount)
-        return self
+        if isinstance(status, str) or status == None:
+            status = State._from_str(status)
+        display = pd.DataFrame()
+        ids, urls, status_list = [], [], []
+        for model_deployment in model_deployments:
+            state_of_model = State._from_str(model_deployment.lifecycle_state)
+            if status == State.UNKNOWN or status.name == state_of_model.name:
+                ids.append(model_deployment.model_deployment_id)
+                urls.append(model_deployment.url)
+                status_list.append(model_deployment.lifecycle_state)
+        display["deployment_id"] = ids
+        display["deployment_url"] = urls
+        display["current_state"] = status_list
+        return display
 
-    def _update_job_infra(self, dsc_job: DSCJob) -> DataScienceJob:
-        """Updates the job infrastructure from a DSCJob object.
+    @classmethod
+    def from_id(cls, id: str) -> "ModelDeployment":
+        """Loads the model deployment instance from ocid.
 
         Parameters
         ----------
-        dsc_job : DSCJob
-            A DSCJob instance.
+        id: str
+            The ocid of model deployment.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The ModelDeployment instance (self).
         """
-        attr_map = {
-            self.CONST_JOB_INFRA: "jobInfrastructureType",
-            self.CONST_SHAPE_NAME: "shapeName",
-            self.CONST_SUBNET_ID: "subnetId",
-            self.CONST_BLOCK_STORAGE: "blockStorageSizeInGBs",
-            self.CONST_SHAPE_CONFIG_DETAILS: "jobShapeConfigDetails",
-        }
+        return cls()._update_from_oci_model(OCIDataScienceModelDeployment.from_id(id))
 
-        if not dsc_job.job_infrastructure_configuration_details:
-            dsc_job.job_infrastructure_configuration_details = {}
+    @classmethod
+    def from_dict(cls, obj_dict: Dict) -> "ModelDeployment":
+        """Loads model deployment instance from a dictionary of configurations.
 
-        for snake_attr, camel_attr in attr_map.items():
-            value = self.get_spec(snake_attr)
-            if value:
-                dsc_job.job_infrastructure_configuration_details[camel_attr] = value
+        Parameters
+        ----------
+        obj_dict: Dict
+            A dictionary of configurations.
 
-        if dsc_job.job_infrastructure_configuration_details.get("subnetId"):
-            dsc_job.job_infrastructure_configuration_details[
-                "jobInfrastructureType"
-            ] = JobInfrastructureConfigurationDetails.JOB_INFRASTRUCTURE_TYPE_STANDALONE
+        Returns
+        -------
+        ModelDeployment
+            The model deployment instance.
+        """
+        if not isinstance(obj_dict, dict):
+            raise ValueError(
+                "The config data for initializing the model deployment is invalid."
+            )
+        spec = ads_utils.batch_convert_case(
+            copy.deepcopy(obj_dict.get("spec")), "camel"
+        )
 
-        if self.storage_mount:
-            if not hasattr(
-                oci.data_science.models, "JobStorageMountConfigurationDetails"
-            ):
-                raise EnvironmentError(
-                    "Storage mount hasn't been supported in the current OCI SDK installed."
+        mappings = {
+            cls.CONST_INFRASTRUCTURE: {
+                MODEL_DEPLOYMENT_INFRASTRUCTURE_TYPE: ModelDeploymentInfrastructure,
+            },
+            cls.CONST_RUNTIME: {
+                ModelDeploymentRuntimeType.CONDA: ModelDeploymentCondaRuntime,
+                ModelDeploymentRuntimeType.CONTAINER: ModelDeploymentContainerRuntime,
+            },
+        }
+        model_deployment = cls()
+
+        for key, value in spec.items():
+            if key in mappings:
+                mapping = mappings[key]
+                child_config = value
+                if child_config.get("type") not in mapping:
+                    raise NotImplementedError(
+                        f"{key.title()} type: {child_config.get('type')} is not supported."
+                    )
+                model_deployment.set_spec(
+                    key, mapping[child_config.get("type")].from_dict(child_config)
                 )
-            dsc_job.job_storage_mount_configuration_details_list = [
-                DSCFileSystemManager.initialize(file_system)
-                for file_system in self.storage_mount
-            ]
-        return self
+            else:
+                model_deployment.set_spec(key, value)
 
-    def build(self) -> DataScienceJob:
-        self.dsc_job.load_defaults()
-        self._update_from_dsc_model(self.dsc_job, overwrite=False)
-        return self
+        return model_deployment
 
-    def init(self) -> DataScienceJob:
-        """Initializes a starter specification for the DataScienceJob.
+    def to_dict(self, **kwargs) -> Dict:
+        """Serializes model deployment to a dictionary.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
+        dict
+            The model deployment serialized as a dictionary.
         """
-        return (
-            self.build()
-            .with_compartment_id(self.compartment_id or "{Provide a compartment OCID}")
-            .with_project_id(self.project_id or "{Provide a project OCID}")
-            .with_subnet_id(self.subnet_id or "{Provide a subnet OCID or remove this field if you use a default networking}")
-        )
+        spec = copy.deepcopy(self._spec)
+        for key, value in spec.items():
+            if hasattr(value, "to_dict"):
+                value = value.to_dict()
+            spec[key] = value
 
-    def create(self, runtime, **kwargs) -> DataScienceJob:
-        """Creates a job with runtime.
+        return {
+            "kind": self.kind,
+            "type": self.type,
+            "spec": ads_utils.batch_convert_case(spec, "camel"),
+        }
+
+    def _update_from_oci_model(self, oci_model_instance) -> "ModelDeployment":
+        """Updates model deployment instance from OCIDataScienceModelDeployment.
 
         Parameters
         ----------
-        runtime : Runtime
-            An ADS job runtime.
+        oci_model_instance: OCIDataScienceModelDeployment
+            The OCIDataScienceModelDeployment instance.
 
         Returns
         -------
-        DataScienceJob
-            The DataScienceJob instance (self)
-
+        ModelDeployment
+            The model deployment instance.
         """
-        if not runtime:
-            raise ValueError("Set a valid runtime.")
-        payload = DataScienceJobRuntimeManager(self).translate(runtime)
-        # Add infra properties to payload
-        for attr in ["project_id", "compartment_id"]:
-            if getattr(self, attr):
-                payload[attr] = getattr(self, attr)
+        self.dsc_model_deployment = oci_model_instance
+        for key, value in self.attribute_map.items():
+            if hasattr(oci_model_instance, value):
+                self.set_spec(key, getattr(oci_model_instance, value))
 
-        if self.name:
-            display_name = Template(self.name).safe_substitute(runtime.envs)
-        elif isinstance(runtime, GitPythonRuntime) or isinstance(
-            runtime, ContainerRuntime
+        infrastructure = ModelDeploymentInfrastructure()
+        self._extract_from_oci_model(
+            infrastructure, oci_model_instance, infrastructure.sub_level_attribute_maps
+        )
+
+        model_deployment_configuration_details = getattr(
+            oci_model_instance, "model_deployment_configuration_details", None
+        )
+        environment_configuration_details = getattr(
+            model_deployment_configuration_details,
+            "environment_configuration_details",
+            None,
+        )
+        runtime = (
+            ModelDeploymentContainerRuntime()
+            if getattr(
+                environment_configuration_details,
+                "environment_configuration_type",
+                None,
+            )
+            == OCIModelDeploymentRuntimeType.CONTAINER
+            else ModelDeploymentCondaRuntime()
+        )
+
+        self._extract_from_oci_model(runtime, oci_model_instance)
+        infrastructure.set_spec(
+            infrastructure.CONST_WEB_CONCURRENCY,
+            runtime.env.get("WEB_CONCURRENCY", None),
+        )
+        if (
+            runtime.env.get("CONTAINER_TYPE", None)
+            == MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
         ):
-            display_name = utils.get_random_name_for_resource()
-        else:
-            display_name = None
+            runtime.set_spec(
+                runtime.CONST_INFERENCE_SERVER,
+                MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON.lower(),
+            )
+
+        self.set_spec(self.CONST_INFRASTRUCTURE, infrastructure)
+        self.set_spec(self.CONST_RUNTIME, runtime)
 
-        payload["display_name"] = display_name
-        payload["job_log_configuration_details"] = self._prepare_log_config()
-        if not payload.get("freeform_tags"):
-            payload["freeform_tags"] = self.freeform_tags
-        if not payload.get("defined_tags"):
-            payload["defined_tags"] = self.defined_tags
-
-        self.dsc_job = DSCJob(**payload)
-        # Set Job infra to user values after DSCJob initialized the defaults
-        self._update_job_infra(self.dsc_job)
-        self.dsc_job.create()
-        # Update the model from infra after job creation.
-        self._update_from_dsc_model(self.dsc_job)
         return self
 
-    def run(
-        self,
-        name=None,
-        args=None,
-        env_var=None,
-        freeform_tags=None,
-        defined_tags=None,
-        wait=False,
-    ) -> DataScienceJobRun:
-        """Runs a job on OCI Data Science job
+    @staticmethod
+    def _extract_from_oci_model(
+        dsc_instance: Union[ModelDeploymentInfrastructure, ModelDeploymentRuntime],
+        oci_model_instance: OCIDataScienceModelDeployment,
+        sub_level: Dict = {},
+    ) -> Union[ModelDeploymentInfrastructure, ModelDeploymentRuntime]:
+        """Extract attributes from OCIDataScienceModelDeployment.
 
         Parameters
         ----------
-        name : str, optional
-            The name of the job run, by default None.
-        args : str, optional
-            Command line arguments for the job run, by default None.
-        env_var : dict, optional
-            Environment variable for the job run, by default None
-        freeform_tags : dict, optional
-            Freeform tags for the job run, by default None
-        defined_tags : dict, optional
-            Defined tags for the job run, by default None
-        wait : bool, optional
-            Indicate if this method should wait for the run to finish before it returns, by default False.
+        dsc_instance: Union[ModelDeploymentInfrastructure, ModelDeploymentRuntime]
+            The ModelDeploymentInfrastructure or ModelDeploymentRuntime instance.
+        oci_model_instance: OCIDataScienceModelDeployment
+            The OCIDataScienceModelDeployment instance.
+        sub_level: Dict
+            The sub level attribute maps of ModelDeploymentInfrastructure or ModelDeploymentRuntime
 
         Returns
         -------
-        DataScienceJobRun
-            A Data Science Job Run instance.
-
+        Union[ModelDeploymentInfrastructure, ModelDeploymentRuntime]
+            The ModelDeploymentInfrastructure or ModelDeploymentRuntime instance.
         """
-        # Runtime in the infrastructure will be None if the job is not created.
-        if not self.runtime:
-            raise RuntimeError(
-                "Job is not created. Call create() to create the job first."
-            )
+        for infra_attr, dsc_attr in dsc_instance.payload_attribute_map.items():
+            value = get_value(oci_model_instance, dsc_attr)
+            if value:
+                if infra_attr not in sub_level:
+                    dsc_instance._spec[infra_attr] = value
+                else:
+                    dsc_instance._spec[infra_attr] = {}
+                    for sub_infra_attr, sub_dsc_attr in sub_level[infra_attr].items():
+                        sub_value = get_value(value, sub_dsc_attr)
+                        if sub_value:
+                            dsc_instance._spec[infra_attr][sub_infra_attr] = sub_value
+        return dsc_instance
 
-        if not freeform_tags:
-            freeform_tags = {}
-        runtime_freeform_tags = self.runtime.freeform_tags
-        if runtime_freeform_tags:
-            freeform_tags.update(runtime_freeform_tags)
+    def _build_model_deployment_details(self) -> CreateModelDeploymentDetails:
+        """Builds CreateModelDeploymentDetails from model deployment instance.
 
-        if not defined_tags:
-            defined_tags = {}
-        runtime_defined_tags = self.runtime.defined_tags
-        if runtime_defined_tags:
-            defined_tags.update(runtime_defined_tags)
+        Returns
+        -------
+        CreateModelDeploymentDetails
+            The CreateModelDeploymentDetails instance.
+        """
+        if not (self.infrastructure and self.runtime):
+            raise ValueError(
+                "Missing parameter runtime or infrastructure. Try reruning it after parameters are fully configured."
+            )
 
-        if name:
-            envs = self.runtime.envs
-            if env_var:
-                envs.update(env_var)
-            name = Template(name).safe_substitute(envs)
+        create_model_deployment_details = {
+            self.CONST_DISPLAY_NAME: self.display_name or self._random_display_name(),
+            self.CONST_DESCRIPTION: self.description,
+            self.CONST_DEFINED_TAG: self.defined_tags,
+            self.CONST_FREEFORM_TAG: self.freeform_tags,
+            self.runtime.CONST_DEPLOYMENT_MODE: self.runtime.deployment_mode
+            or ModelDeploymentMode.HTTPS,
+            self.infrastructure.CONST_COMPARTMENT_ID: self.infrastructure.compartment_id
+            or COMPARTMENT_OCID,
+            self.infrastructure.CONST_PROJECT_ID: self.infrastructure.project_id
+            or PROJECT_OCID,
+            self.infrastructure.CONST_MODEL_DEPLOYMENT_CONFIG_DETAILS: self._build_model_deployment_configuration_details(),
+            self.infrastructure.CONST_CATEGORY_LOG_DETAILS: self._build_category_log_details(),
+        }
 
-        return self.dsc_job.run(
-            display_name=name,
-            command_line_arguments=args,
-            environment_variables=env_var,
-            freeform_tags=freeform_tags,
-            defined_tags=defined_tags,
-            wait=wait,
-        )
+        return OCIDataScienceModelDeployment(
+            **create_model_deployment_details
+        ).to_oci_model(CreateModelDeploymentDetails)
 
-    def delete(self) -> None:
-        """Deletes a job"""
-        self.dsc_job.delete()
+    def _update_model_deployment_details(self, **kwargs) -> UpdateModelDeploymentDetails:
+        """Builds UpdateModelDeploymentDetails from model deployment instance.
 
-    def run_list(self, **kwargs) -> List[DataScienceJobRun]:
-        """Gets a list of job runs.
+        Returns
+        -------
+        UpdateModelDeploymentDetails
+            The UpdateModelDeploymentDetails instance.
+        """
+        if not (self.infrastructure and self.runtime):
+            raise ValueError(
+                "Missing parameter runtime or infrastructure. Try reruning it after parameters are fully configured."
+            )
+        self._update_spec(**kwargs)
+        update_model_deployment_details = {
+            self.CONST_DISPLAY_NAME: self.display_name,
+            self.CONST_DESCRIPTION: self.description,
+            self.CONST_DEFINED_TAG: self.defined_tags,
+            self.CONST_FREEFORM_TAG: self.freeform_tags,
+            self.infrastructure.CONST_MODEL_DEPLOYMENT_CONFIG_DETAILS: self._build_model_deployment_configuration_details(),
+            self.infrastructure.CONST_CATEGORY_LOG_DETAILS: self._build_category_log_details(),
+        }
+        return OCIDataScienceModelDeployment(
+            **update_model_deployment_details
+        ).to_oci_model(UpdateModelDeploymentDetails)
+    
+    def _update_spec(self, **kwargs) -> "ModelDeployment":
+        """Updates model deployment specs from kwargs.
 
         Parameters
         ----------
-        **kwargs :
-            Keyword arguments for filtering the job runs.
-            These arguments will be passed to OCI API.
-
+        kwargs:
+            display_name: (str)
+                Model deployment display name
+            description: (str)
+                Model deployment description
+            freeform_tags: (dict)
+                Model deployment freeform tags
+            defined_tags: (dict)
+                Model deployment defined tags
+            
+            Additional kwargs arguments.
+            Can be any attribute that `ads.model.deployment.ModelDeploymentCondaRuntime`, `ads.model.deployment.ModelDeploymentContainerRuntime`
+            and `ads.model.deployment.ModelDeploymentInfrastructure` accepts.
 
         Returns
         -------
-        List[DSCJobRun]:
-            A list of job runs.
-
-        """
-        return self.dsc_job.run_list(**kwargs)
+        ModelDeployment
+            The instance of ModelDeployment.
+        """
+        if not kwargs:
+            return self
+
+        converted_specs = ads_utils.batch_convert_case(kwargs, "camel")
+        specs = {
+            "self": self._spec,
+            "runtime": self.runtime._spec,
+            "infrastructure": self.infrastructure._spec
+        }
+        sub_set = {
+            self.infrastructure.CONST_ACCESS_LOG,
+            self.infrastructure.CONST_PREDICT_LOG,
+            self.infrastructure.CONST_SHAPE_CONFIG_DETAILS
+        }
+        for spec_value in specs.values():
+            for key in spec_value:
+                if key in converted_specs:
+                    if key in sub_set:
+                        for sub_key in converted_specs[key]:
+                            converted_sub_key = ads_utils.snake_to_camel(sub_key)
+                            spec_value[key][converted_sub_key] = converted_specs[key][sub_key]
+                    else:
+                        spec_value[key] = copy.deepcopy(converted_specs[key])
+        self = (
+            ModelDeployment(spec=specs["self"])
+            .with_runtime(
+                MODEL_DEPLOYMENT_RUNTIMES[self.runtime.type](spec=specs["runtime"])
+            )
+            .with_infrastructure(
+                ModelDeploymentInfrastructure(spec=specs["infrastructure"])
+            )
+        )
 
-    @classmethod
-    def from_dsc_job(cls, dsc_job: DSCJob) -> DataScienceJob:
-        """Initialize a DataScienceJob instance from a DSCJob
+        return self
 
-        Parameters
-        ----------
-        dsc_job : DSCJob
-            An instance of DSCJob
+    def _build_model_deployment_configuration_details(self) -> Dict:
+        """Builds model deployment configuration details from model deployment instance.
 
         Returns
         -------
-        DataScienceJob
-            An instance of DataScienceJob
-
+        Dict:
+            Dict contains model deployment configuration details.
         """
-        instance = cls()
-        instance._update_from_dsc_model(dsc_job)
-        instance.runtime = DataScienceJobRuntimeManager(instance).extract(dsc_job)
-        return instance
+        infrastructure = self.infrastructure
+        runtime = self.runtime
 
-    @classmethod
-    def from_id(cls, job_id: str) -> DataScienceJob:
-        """Gets an existing job using Job OCID
+        instance_configuration = {
+            infrastructure.CONST_INSTANCE_SHAPE_NAME: infrastructure.shape_name
+            or MODEL_DEPLOYMENT_INSTANCE_SHAPE,
+        }
 
-        Parameters
-        ----------
-        job_id : str
-            Job OCID
+        if instance_configuration[infrastructure.CONST_INSTANCE_SHAPE_NAME].endswith(
+            "Flex"
+        ):
+            instance_configuration[
+                infrastructure.CONST_MODEL_DEPLOYMENT_INSTANCE_SHAPE_CONFIG_DETAILS
+            ] = {
+                infrastructure.CONST_OCPUS: infrastructure.shape_config_details.get(
+                    "ocpus", None
+                )
+                or MODEL_DEPLOYMENT_INSTANCE_OCPUS,
+                infrastructure.CONST_MEMORY_IN_GBS: infrastructure.shape_config_details.get(
+                    "memory_in_gbs", None
+                )
+                or infrastructure.shape_config_details.get(
+                    "memoryInGBs", None
+                )
+                or MODEL_DEPLOYMENT_INSTANCE_MEMORY_IN_GBS,
+            }
 
+        if infrastructure.subnet_id:
+            instance_configuration[infrastructure.CONST_SUBNET_ID] = infrastructure.subnet_id
 
-        Returns
-        -------
-        DataScienceJob
-            An instance of DataScienceJob
+        scaling_policy = {
+            infrastructure.CONST_POLICY_TYPE: "FIXED_SIZE",
+            infrastructure.CONST_INSTANCE_COUNT: infrastructure.replica
+            or MODEL_DEPLOYMENT_INSTANCE_COUNT,
+        }
 
-        """
-        return cls.from_dsc_job(DSCJob.from_ocid(job_id))
+        if not runtime.model_uri:
+            raise ValueError(
+                "Missing parameter model uri. Try reruning it after model uri is configured."
+            )
 
-    @classmethod
-    def list_jobs(cls, compartment_id: str = None, **kwargs) -> List[DataScienceJob]:
-        """Lists all jobs in a compartment.
+        model_id = runtime.model_uri
+        if not model_id.startswith("ocid"):
+            
+            from ads.model.datascience_model import DataScienceModel
+            
+            dsc_model = DataScienceModel(
+                name=self.display_name,
+                compartment_id=self.infrastructure.compartment_id
+                or COMPARTMENT_OCID,
+                project_id=self.infrastructure.project_id or PROJECT_OCID,
+                artifact=runtime.model_uri,
+            ).create(
+                bucket_uri=runtime.bucket_uri,
+                auth=runtime.auth,
+                region=runtime.region,
+                overwrite_existing_artifact=runtime.overwrite_existing_artifact,
+                remove_existing_artifact=runtime.remove_existing_artifact,
+                timeout=runtime.timeout
+            )
+            model_id = dsc_model.id
+
+        model_configuration_details = {
+            infrastructure.CONST_BANDWIDTH_MBPS: infrastructure.bandwidth_mbps
+            or MODEL_DEPLOYMENT_BANDWIDTH_MBPS,
+            infrastructure.CONST_INSTANCE_CONFIG: instance_configuration,
+            runtime.CONST_MODEL_ID: model_id,
+            infrastructure.CONST_SCALING_POLICY: scaling_policy,
+        }
 
-        Parameters
-        ----------
-        compartment_id : str, optional
-            The compartment ID for running the jobs, by default None.
-            This is optional in a OCI Data Science notebook session.
-            If this is not specified, the compartment ID of the notebook session will be used.
-        **kwargs :
-            Keyword arguments to be passed into OCI list_jobs API for filtering the jobs.
+        if runtime.env:
+            if not hasattr(
+                oci.data_science.models,
+                "ModelDeploymentEnvironmentConfigurationDetails",
+            ):
+                raise EnvironmentError(
+                    "Environment variable hasn't been supported in the current OCI SDK installed."
+                )
 
-        Returns
-        -------
-        List[DataScienceJob]
-            A list of DataScienceJob object.
+        environment_variables = runtime.env
+        if infrastructure.web_concurrency:
+            environment_variables["WEB_CONCURRENCY"] = str(
+                infrastructure.web_concurrency
+            )
+            runtime.set_spec(runtime.CONST_ENV, environment_variables)
+        if (
+            hasattr(runtime, "inference_server")
+            and runtime.inference_server
+            and runtime.inference_server.upper()
+            == MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
+        ):
+            environment_variables[
+                "CONTAINER_TYPE"
+            ] = MODEL_DEPLOYMENT_INFERENCE_SERVER_TRITON
+            runtime.set_spec(runtime.CONST_ENV, environment_variables)
+        environment_configuration_details = {
+            runtime.CONST_ENVIRONMENT_CONFIG_TYPE: runtime.environment_config_type,
+            runtime.CONST_ENVIRONMENT_VARIABLES: runtime.env,
+        }
 
-        """
-        return [
-            cls.from_dsc_job(job)
-            for job in DSCJob.list_resource(compartment_id, **kwargs)
-        ]
+        if runtime.environment_config_type == OCIModelDeploymentRuntimeType.CONTAINER:
+            if not hasattr(
+                oci.data_science.models,
+                "OcirModelDeploymentEnvironmentConfigurationDetails",
+            ):
+                raise EnvironmentError(
+                    "Container runtime hasn't been supported in the current OCI SDK installed."
+                )
+            environment_configuration_details["image"] = runtime.image
+            environment_configuration_details["imageDigest"] = runtime.image_digest
+            environment_configuration_details["cmd"] = runtime.cmd
+            environment_configuration_details["entrypoint"] = runtime.entrypoint
+            environment_configuration_details["serverPort"] = runtime.server_port
+            environment_configuration_details[
+                "healthCheckPort"
+            ] = runtime.health_check_port
+
+        model_deployment_configuration_details = {
+            infrastructure.CONST_DEPLOYMENT_TYPE: "SINGLE_MODEL",
+            infrastructure.CONST_MODEL_CONFIG_DETAILS: model_configuration_details,
+            runtime.CONST_ENVIRONMENT_CONFIG_DETAILS: environment_configuration_details,
+        }
 
-    @classmethod
-    def instance_shapes(cls, compartment_id: str = None, **kwargs) -> list:
-        """Lists the supported shapes for running jobs in a compartment.
+        if runtime.deployment_mode == ModelDeploymentMode.STREAM:
+            if not hasattr(oci.data_science.models, "StreamConfigurationDetails"):
+                raise EnvironmentError(
+                    "Model deployment mode hasn't been supported in the current OCI SDK installed."
+                )
+            model_deployment_configuration_details[
+                infrastructure.CONST_STREAM_CONFIG_DETAILS
+            ] = {
+                runtime.CONST_INPUT_STREAM_IDS: runtime.input_stream_ids,
+                runtime.CONST_OUTPUT_STREAM_IDS: runtime.output_stream_ids,
+            }
 
-        Parameters
-        ----------
-        compartment_id : str, optional
-            The compartment ID for running the jobs, by default None.
-            This is optional in a OCI Data Science notebook session.
-            If this is not specified, the compartment ID of the notebook session will be used.
+        return model_deployment_configuration_details
+
+    def _build_category_log_details(self) -> Dict:
+        """Builds category log details from model deployment instance.
 
         Returns
         -------
-        list
-            A list of oci.data_science.models.JobShapeSummary objects
-            containing the information of the supported shapes.
+        Dict:
+            Dict contains category log details.
+        """
+        if self.infrastructure.log_group_id and self.infrastructure.log_id:
+            log_group_details = {
+                self.infrastructure.CONST_LOG_GROUP_ID: self.infrastructure.log_group_id,
+                self.infrastructure.CONST_LOG_ID: self.infrastructure.log_id,
+            }
+            return {
+                self.infrastructure.CONST_ACCESS: log_group_details,
+                self.infrastructure.CONST_PREDICT: log_group_details,
+            }
 
-        Examples
-        --------
-        To get a list of shape names::
+        logs = {}
+        if self.infrastructure.access_log:
+            logs[self.infrastructure.CONST_ACCESS] = {
+                self.infrastructure.CONST_LOG_GROUP_ID: self.infrastructure.access_log.get(
+                    "logGroupId", None
+                ),
+                self.infrastructure.CONST_LOG_ID: self.infrastructure.access_log.get(
+                    "logId", None
+                ),
+            }
+        if self.infrastructure.predict_log:
+            logs[self.infrastructure.CONST_PREDICT] = {
+                self.infrastructure.CONST_LOG_GROUP_ID: self.infrastructure.predict_log.get(
+                    "logGroupId", None
+                ),
+                self.infrastructure.CONST_LOG_ID: self.infrastructure.predict_log.get(
+                    "logId", None
+                ),
+            }
 
-            shapes = DataScienceJob.fast_launch_shapes(
-                compartment_id=os.environ["PROJECT_COMPARTMENT_OCID"]
-            )
-            shape_names = [shape.name for shape in shapes]
+        return logs
 
-        """
-        shapes = oci.pagination.list_call_get_all_results(
-            DSCJob.init_client().list_job_shapes,
-            DSCJob.check_compartment_id(compartment_id),
-            **kwargs,
-        ).data
-        return shapes
+    def _random_display_name(self):
+        """Generates a random display name."""
+        return f"{self._PREFIX}-{ads_utils.get_random_name_for_resource()}"
 
-    @classmethod
-    def fast_launch_shapes(cls, compartment_id: str = None, **kwargs) -> list:
-        """Lists the supported fast launch shapes for running jobs in a compartment.
+    def _extract_spec_kwargs(self, **kwargs) -> Dict:
+        """Extract spec related keyword arguments from kwargs.
 
         Parameters
         ----------
-        compartment_id : str, optional
-            The compartment ID for running the jobs, by default None.
-            This is optional in a OCI Data Science notebook session.
-            If this is not specified, the compartment ID of the notebook session will be used.
+        kwargs
 
         Returns
         -------
-        list
-            A list of oci.data_science.models.FastLaunchJobConfigSummary objects
-            containing the information of the supported shapes.
-
-        Examples
-        --------
-        To get a list of shape names::
-
-            shapes = DataScienceJob.fast_launch_shapes(
-                compartment_id=os.environ["PROJECT_COMPARTMENT_OCID"]
-            )
-            shape_names = [shape.shape_name for shape in shapes]
-
+        Dict:
+            Dict contains model deployment spec related keyword arguments.
         """
-        shapes = oci.pagination.list_call_get_all_results(
-            DSCJob.init_client().list_fast_launch_job_configs,
-            DSCJob.check_compartment_id(compartment_id),
-            **kwargs,
-        ).data
-        return shapes
+        spec_kwargs = {}
+        for attribute in self.initialize_spec_attributes:
+            if attribute in kwargs:
+                spec_kwargs[attribute] = kwargs[attribute]
+        return spec_kwargs
+
+    def build(self) -> "ModelDeployment":
+        """Load default values from the environment for the job infrastructure."""
+        build_method = getattr(self.infrastructure, "build", None)
+        if build_method and callable(build_method):
+            build_method()
+        else:
+            raise NotImplementedError
+        return self
```

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/dsc_job_runtime.py` & `oracle_ads-2.8.6/ads/jobs/builders/infrastructure/dsc_job_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/infrastructure/utils.py` & `oracle_ads-2.8.6/ads/jobs/builders/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/runtimes/artifact.py` & `oracle_ads-2.8.6/ads/jobs/builders/runtimes/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/runtimes/base.py` & `oracle_ads-2.8.6/ads/jobs/builders/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/runtimes/container_runtime.py` & `oracle_ads-2.8.6/ads/jobs/builders/runtimes/container_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/builders/runtimes/python_runtime.py` & `oracle_ads-2.8.6/ads/jobs/builders/runtimes/python_runtime.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/cli.py` & `oracle_ads-2.8.6/ads/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/env_var_parser.py` & `oracle_ads-2.8.6/ads/jobs/env_var_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/extension.py` & `oracle_ads-2.8.6/ads/jobs/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/schema/infrastructure_schema.json` & `oracle_ads-2.8.6/ads/jobs/schema/infrastructure_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/schema/job_schema.json` & `oracle_ads-2.8.6/ads/jobs/schema/job_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/schema/runtime_schema.json` & `oracle_ads-2.8.6/ads/jobs/schema/runtime_schema.json`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/schema/validator.py` & `oracle_ads-2.8.6/ads/jobs/schema/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/serializer.py` & `oracle_ads-2.8.6/ads/jobs/serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/templates/driver_notebook.py` & `oracle_ads-2.8.6/ads/jobs/templates/driver_notebook.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/templates/driver_oci.py` & `oracle_ads-2.8.6/ads/jobs/templates/driver_oci.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/templates/driver_python.py` & `oracle_ads-2.8.6/ads/jobs/templates/driver_python.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/templates/driver_utils.py` & `oracle_ads-2.8.6/ads/jobs/templates/driver_utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/jobs/utils.py` & `oracle_ads-2.8.6/ads/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/__init__.py` & `oracle_ads-2.8.6/ads/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/artifact.py` & `oracle_ads-2.8.6/ads/model/artifact.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/artifact_downloader.py` & `oracle_ads-2.8.6/ads/model/artifact_downloader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/artifact_uploader.py` & `oracle_ads-2.8.6/ads/model/artifact_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/base_properties.py` & `oracle_ads-2.8.6/ads/model/base_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/common/.model-ignore` & `oracle_ads-2.8.6/ads/model/common/.model-ignore`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/common/utils.py` & `oracle_ads-2.8.6/ads/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/datascience_model.py` & `oracle_ads-2.8.6/ads/model/datascience_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/deployment/__init__.py` & `oracle_ads-2.8.6/ads/model/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/deployment/common/utils.py` & `oracle_ads-2.8.6/ads/model/deployment/common/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/deployment/model_deployer.py` & `oracle_ads-2.8.6/ads/model/deployment/model_deployer.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,24 @@
 from oci.data_science import DataScienceClientCompositeOperations
 
 from .common import utils
 from .common.utils import OCIClientManager, State
 from .model_deployment import DEFAULT_POLL_INTERVAL, DEFAULT_WAIT_TIME, ModelDeployment
 from .model_deployment_properties import ModelDeploymentProperties
 
+warnings.warn(
+    (
+        "The `ads.model.deployment.model_deployer` is deprecated in `oracle-ads 2.8.6` and will be removed in `oracle-ads 3.0`."
+        "Use `ModelDeployment` class in `ads.model.deployment` module for initializing and deploying model deployment. "
+        "Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/introduction.html"
+    ),
+    DeprecationWarning,
+    stacklevel=2,
+)
+
 
 class ModelDeployer:
     """ModelDeployer is the class responsible for deploying the ModelDeployment
 
     Attributes
     ----------
     config : dict
```

### Comparing `oracle_ads-2.8.5/ads/model/deployment/model_deployment_infrastructure.py` & `oracle_ads-2.8.6/ads/model/deployment/model_deployment_infrastructure.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/deployment/model_deployment_properties.py` & `oracle_ads-2.8.6/ads/model/deployment/model_deployment_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 
 import oci.data_science.models as data_science_models
 from ads.common import utils
 from ads.common.oci_datascience import OCIDataScienceMixin
 
 from .common.utils import OCIClientManager
 
+import warnings
+
+warnings.warn(
+    (
+        "The `ads.model.deployment.model_deployment_properties` is deprecated in `oracle-ads 2.8.6` and will be removed in `oracle-ads 3.0`."
+        "Use `ModelDeploymentInfrastructure` and `ModelDeploymentRuntime` classes in `ads.model.deployment` module for configuring model deployment. "
+        "Check https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/introduction.html"
+    ),
+    DeprecationWarning,
+    stacklevel=2,
+)
+
 
 class ModelDeploymentProperties(
     OCIDataScienceMixin, data_science_models.ModelDeployment
 ):
     """Represents the details for a model deployment
 
     Attributes
```

### Comparing `oracle_ads-2.8.5/ads/model/deployment/model_deployment_runtime.py` & `oracle_ads-2.8.6/ads/model/deployment/model_deployment_runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,46 +32,82 @@
         The deployment mode of model deployment.
     input_stream_ids: List
         The input stream ids of model deployment.
     output_stream_ids: List
         The output stream ids of model deployment.
     model_uri: str
         The model uri of model deployment.
+    bucket_uri: str
+        The OCI Object Storage URI where large size model artifacts will be copied to.
+    auth: Dict
+        The default authentication is set using `ads.set_auth` API.
+    region: str
+        The destination Object Storage bucket region.
+    overwrite_existing_artifact: bool
+        Whether overwrite existing target bucket artifact or not.
+    remove_existing_artifact: bool
+        Whether artifacts uploaded to object storage bucket need to be removed or not.
+    timeout: int
+        The connection timeout in seconds for the client.
 
     Methods
     -------
     with_env(env)
         Sets the environment variables of model deployment
     with_deployment_mode(deployment_mode)
         Sets the deployment mode of model deployment
     with_input_stream_ids(input_stream_ids)
         Sets the input stream ids of model deployment
     with_output_stream_ids(output_stream_ids)
         Sets the output stream ids of model deployment
     with_model_uri(model_uri)
         Sets the model uri of model deployment
+    with_bucket_uri(bucket_uri)
+        Sets the bucket uri when uploading large size model.
+    with_auth(auth)
+        Sets the default authentication when uploading large size model.
+    with_region(region)
+        Sets the region when uploading large size model.
+    with_overwrite_existing_artifact(overwrite_existing_artifact)
+        Sets whether to overwrite existing artifact when uploading large size model.
+    with_remove_existing_artifact(remove_existing_artifact)
+        Sets whether to remove existing artifact when uploading large size model.
+    with_timeout(timeout)
+        Sets the connection timeout when uploading large size model.
     """
 
     CONST_MODEL_ID = "modelId"
     CONST_MODEL_URI = "modelUri"
     CONST_ENV = "env"
     CONST_ENVIRONMENT_VARIABLES = "environmentVariables"
     CONST_ENVIRONMENT_CONFIG_TYPE = "environmentConfigurationType"
     CONST_DEPLOYMENT_MODE = "deploymentMode"
     CONST_INPUT_STREAM_IDS = "inputStreamIds"
     CONST_OUTPUT_STREAM_IDS = "outputStreamIds"
     CONST_ENVIRONMENT_CONFIG_DETAILS = "environmentConfigurationDetails"
+    CONST_BUCKET_URI = "bucketUri"
+    CONST_AUTH = "auth"
+    CONST_REGION = "region"
+    CONST_OVERWRITE_EXISTING_ARTIFACT = "overwriteExistingArtifact"
+    CONST_REMOVE_EXISTING_ARTIFACT = "removeExistingArtifact"
+    CONST_TIMEOUT = "timeout"
 
     attribute_map = {
         CONST_ENV: "env",
         CONST_ENVIRONMENT_VARIABLES: "environment_variables",
         CONST_INPUT_STREAM_IDS: "input_stream_ids",
         CONST_OUTPUT_STREAM_IDS: "output_stream_ids",
         CONST_DEPLOYMENT_MODE: "deployment_mode",
         CONST_MODEL_URI: "model_uri",
+        CONST_BUCKET_URI: "bucket_uri",
+        CONST_AUTH: "auth",
+        CONST_REGION: "region",
+        CONST_OVERWRITE_EXISTING_ARTIFACT: "overwrite_existing_artifact",
+        CONST_REMOVE_EXISTING_ARTIFACT: "remove_existing_artifact",
+        CONST_TIMEOUT: "timeout"
     }
 
     ENVIRONMENT_CONFIG_DETAILS_PATH = (
         "model_deployment_configuration_details.environment_configuration_details"
     )
     STREAM_CONFIG_DETAILS_PATH = (
         "model_deployment_configuration_details.stream_configuration_details"
@@ -232,15 +268,180 @@
 
         Returns
         -------
         ModelDeploymentRuntime
             The ModelDeploymentRuntime instance (self).
         """
         return self.set_spec(self.CONST_MODEL_URI, model_uri)
+    
+    @property
+    def bucket_uri(self) -> str:
+        """The bucket uri of model.
+
+        Returns
+        -------
+        str
+            The bucket uri of model.
+        """
+        return self.get_spec(self.CONST_BUCKET_URI, None)
 
+    def with_bucket_uri(self, bucket_uri: str) -> "ModelDeploymentRuntime":
+        """Sets the bucket uri of model.
+
+        Parameters
+        ----------
+        bucket_uri: str
+            The bucket uri of model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(self.CONST_BUCKET_URI, bucket_uri)
+    
+    @property
+    def auth(self) -> Dict:
+        """The auth when uploading large-size model.
+
+        Returns
+        -------
+        Dict
+            The auth when uploading large-size model.
+        """
+        return self.get_spec(self.CONST_AUTH, {})
+    
+    def with_auth(self, auth: Dict) -> "ModelDeploymentRuntime":
+        """Sets the auth when uploading large-size model.
+
+        Parameters
+        ----------
+        auth: Dict
+            The auth when uploading large-size model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(self.CONST_AUTH, auth)
+    
+    @property
+    def region(self) -> str:
+        """The region when uploading large-size model.
+
+        Returns
+        -------
+        str
+            The region when uploading large-size model.
+        """
+        return self.get_spec(self.CONST_REGION, None)
+    
+    def with_region(self, region: str) -> "ModelDeploymentRuntime":
+        """Sets the region when uploading large-size model.
+
+        Parameters
+        ----------
+        region: str
+            The region when uploading large-size model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(self.CONST_REGION, region)
+    
+    @property
+    def overwrite_existing_artifact(self) -> bool:
+        """Overwrite existing artifact when uploading large size model.
+
+        Returns
+        -------
+        bool
+            Overwrite existing artifact when uploading large size model.
+        """
+        return self.get_spec(self.CONST_OVERWRITE_EXISTING_ARTIFACT, True)
+    
+    def with_overwrite_existing_artifact(
+        self, 
+        overwrite_existing_artifact: bool
+    ) -> "ModelDeploymentRuntime":
+        """Sets whether to overwrite existing artifact when uploading large size model.
+
+        Parameters
+        ----------
+        overwrite_existing_artifact: bool
+            Overwrite existing artifact when uploading large size model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(
+            self.CONST_OVERWRITE_EXISTING_ARTIFACT,
+            overwrite_existing_artifact
+        )
+    
+    @property
+    def remove_existing_artifact(self) -> bool:
+        """Remove existing artifact when uploading large size model.
+
+        Returns
+        -------
+        bool
+            Remove existing artifact when uploading large size model.
+        """
+        return self.get_spec(self.CONST_REMOVE_EXISTING_ARTIFACT, True)
+    
+    def with_remove_existing_artifact(
+        self,
+        remove_existing_artifact: bool
+    ) -> "ModelDeploymentRuntime":
+        """Sets whether to remove existing artifact when uploading large size model.
+
+        Parameters
+        ----------
+        remove_existing_artifact: bool
+            Remove existing artifact when uploading large size model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(self.CONST_REMOVE_EXISTING_ARTIFACT, remove_existing_artifact)
+    
+    @property
+    def timeout(self) -> int:
+        """The timeout when uploading large-size model.
+
+        Returns
+        -------
+        int
+            The timeout when uploading large-size model.
+        """
+        return self.get_spec(self.CONST_TIMEOUT, None)
+    
+    def with_timeout(self, timeout: int) -> "ModelDeploymentRuntime":
+        """Sets the timeout when uploading large-size model.
+
+        Parameters
+        ----------
+        timeout: int
+            The timeout when uploading large-size model.
+
+        Returns
+        -------
+        ModelDeploymentRuntime
+            The ModelDeploymentRuntime instance (self).
+        """
+        return self.set_spec(self.CONST_TIMEOUT, timeout)
+    
     def init(self) -> "ModelDeploymentRuntime":
         """Initializes a starter specification for the runtime.
 
         Returns
         -------
         Self
             This method returns self to support chaining methods.
```

### Comparing `oracle_ads-2.8.5/ads/model/extractor/automl_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/automl_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/huggingface_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/huggingface_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/keras_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/keras_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/lightgbm_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/lightgbm_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/model_info_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/model_info_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/model_info_extractor_factory.py` & `oracle_ads-2.8.6/ads/model/extractor/model_info_extractor_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/pytorch_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/pytorch_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/sklearn_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/sklearn_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/spark_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/spark_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/tensorflow_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/tensorflow_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/extractor/xgboost_extractor.py` & `oracle_ads-2.8.6/ads/model/extractor/xgboost_extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/automl_model.py` & `oracle_ads-2.8.6/ads/model/framework/automl_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/huggingface_model.py` & `oracle_ads-2.8.6/ads/model/framework/huggingface_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/lightgbm_model.py` & `oracle_ads-2.8.6/ads/model/framework/lightgbm_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/pytorch_model.py` & `oracle_ads-2.8.6/ads/model/framework/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/sklearn_model.py` & `oracle_ads-2.8.6/ads/model/framework/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/spark_model.py` & `oracle_ads-2.8.6/ads/model/framework/spark_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/tensorflow_model.py` & `oracle_ads-2.8.6/ads/model/framework/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/framework/xgboost_model.py` & `oracle_ads-2.8.6/ads/model/framework/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/generic_model.py` & `oracle_ads-2.8.6/ads/model/generic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import inspect
 import os
 import shutil
 import tempfile
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
+import warnings
 
 import numpy as np
 import pandas as pd
 import requests
 import yaml
 from PIL import Image
 
@@ -40,15 +41,14 @@
     fetch_manifest_from_conda_location,
     zip_artifact,
 )
 from ads.model.datascience_model import DataScienceModel
 from ads.model.deployment import (
     DEFAULT_POLL_INTERVAL,
     DEFAULT_WAIT_TIME,
-    ModelDeployer,
     ModelDeployment,
     ModelDeploymentMode,
     ModelDeploymentProperties,
     ModelDeploymentCondaRuntime,
     ModelDeploymentInfrastructure,
     ModelDeploymentContainerRuntime,
 )
@@ -295,20 +295,20 @@
     ...     force_overwrite=True
     ... )
     >>> model.verify(2)
     >>> model.save()
     >>> model.deploy()
     >>> # Update access log id, freeform tags and description for the model deployment
     >>> model.update_deployment(
-    >>>     properties=ModelDeploymentProperties(
-    >>>         access_log_id=<log_ocid>,
-    >>>         description="Description for Custom Model",
-    >>>         freeform_tags={"key": "value"},
-    >>>     )
-    >>> )
+    ...     access_log={
+    ...         log_id=<log_ocid>
+    ...     },
+    ...     description="Description for Custom Model",
+    ...     freeform_tags={"key": "value"},
+    ... )
     >>> model.predict(2)
     >>> # Uncomment the line below to delete the model and the associated model deployment
     >>> # model.delete(delete_associated_model_deployment = True)
     """
 
     _summary_status = None
     _PREFIX = "generic"
@@ -1561,17 +1561,15 @@
             and ObjectStorageDetails.is_oci_path(artifact_dir)
         ):
             raise ValueError(
                 f"Unsupported value of `artifact_dir`: {artifact_dir}. "
                 "Only SparkPipelineModel framework supports object storage path as `artifact_dir`."
             )
 
-        model_deployment = ModelDeployer(config=auth).get_model_deployment(
-            model_deployment_id=model_deployment_id
-        )
+        model_deployment = ModelDeployment.from_id(model_deployment_id)
 
         current_state = model_deployment.state.name.upper()
         if current_state != ModelDeploymentState.ACTIVE.name:
             raise NotActiveDeploymentError(current_state)
 
         model = cls.from_model_catalog(
             model_id=model_deployment.properties.model_id,
@@ -1615,20 +1613,20 @@
         Changes to the `bandwidth_mbps` or `instance_count` will take effect the next time
         the `ActivateModelDeployment` action is invoked on the model deployment resource.
 
         Examples
         --------
         >>> # Update access log id, freeform tags and description for the model deployment
         >>> model.update_deployment(
-        >>>     properties=ModelDeploymentProperties(
-        >>>         access_log_id=<log_ocid>,
-        >>>         description="Description for Custom Model",
-        >>>         freeform_tags={"key": "value"},
-        >>>     )
-        >>> )
+        ...     access_log={
+        ...         log_id=<log_ocid>
+        ...     },
+        ...     description="Description for Custom Model",
+        ...     freeform_tags={"key": "value"},
+        ... )
 
         Parameters
         ----------
         model_deployment_id: str.
             The model deployment OCID. Defaults to None.
             If the method called on instance level, then `self.model_deployment.model_deployment_id` will be used.
         properties: ModelDeploymentProperties or dict
@@ -1643,37 +1641,52 @@
             Poll interval in seconds (Defaults to 10).
         kwargs:
             auth: (Dict, optional). Defaults to `None`.
                 The default authetication is set using `ads.set_auth` API.
                 If you need to override the default, use the `ads.common.auth.api_keys` or
                 `ads.common.auth.resource_principal` to create appropriate authentication signer
                 and kwargs required to instantiate IdentityClient object.
+            display_name: (str)
+                Model deployment display name
+            description: (str)
+                Model deployment description
+            freeform_tags: (dict)
+                Model deployment freeform tags
+            defined_tags: (dict)
+                Model deployment defined tags
+            
+            Additional kwargs arguments.
+            Can be any attribute that `ads.model.deployment.ModelDeploymentCondaRuntime`, `ads.model.deployment.ModelDeploymentContainerRuntime`
+            and `ads.model.deployment.ModelDeploymentInfrastructure` accepts.
 
         Returns
         -------
         ModelDeployment
             An instance of ModelDeployment class.
         """
+        if properties:
+            warnings.warn(
+                "Parameter `properties` is deprecated from GenericModel `update_deployment()` in 2.8.6 and will be removed in 3.0.0. Please use kwargs to update model deployment. "
+                "Check: https://accelerated-data-science.readthedocs.io/en/latest/user_guide/model_registration/introduction.html"
+            )
+
         if not inspect.isclass(cls):
             if cls.model_deployment:
                 return cls.model_deployment.update(
                     properties=properties,
                     wait_for_completion=wait_for_completion,
                     max_wait_time=max_wait_time,
                     poll_interval=poll_interval,
                     **kwargs,
                 )
 
         if not model_deployment_id:
             raise ValueError("Parameter `model_deployment_id` must be provided.")
 
-        auth = kwargs.pop("auth", authutil.default_signer())
-        model_deployment = ModelDeployer(config=auth).get_model_deployment(
-            model_deployment_id=model_deployment_id
-        )
+        model_deployment = ModelDeployment.from_id(model_deployment_id)
         return model_deployment.update(
             properties=properties,
             wait_for_completion=wait_for_completion,
             max_wait_time=max_wait_time,
             poll_interval=poll_interval,
             **kwargs,
         )
```

### Comparing `oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py` & `oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/artifact_introspection_test/model_artifact_validate.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_artifact_boilerplate/score.py` & `oracle_ads-2.8.6/ads/model/model_artifact_boilerplate/score.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_introspect.py` & `oracle_ads-2.8.6/ads/model/model_introspect.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_metadata.py` & `oracle_ads-2.8.6/ads/model/model_metadata.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_metadata_mixin.py` & `oracle_ads-2.8.6/ads/model/model_metadata_mixin.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_properties.py` & `oracle_ads-2.8.6/ads/model/model_properties.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/model_version_set.py` & `oracle_ads-2.8.6/ads/model/model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/env_info.py` & `oracle_ads-2.8.6/ads/model/runtime/env_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/model_deployment_details.py` & `oracle_ads-2.8.6/ads/model/runtime/model_deployment_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/model_provenance_details.py` & `oracle_ads-2.8.6/ads/model/runtime/model_provenance_details.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/runtime_info.py` & `oracle_ads-2.8.6/ads/model/runtime/runtime_info.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/schemas/model_provenance_schema.yaml` & `oracle_ads-2.8.6/ads/model/runtime/schemas/model_provenance_schema.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/runtime/utils.py` & `oracle_ads-2.8.6/ads/model/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/serde/common.py` & `oracle_ads-2.8.6/ads/model/serde/common.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/serde/model_input.py` & `oracle_ads-2.8.6/ads/model/serde/model_input.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/serde/model_serializer.py` & `oracle_ads-2.8.6/ads/model/serde/model_serializer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/service/oci_datascience_model.py` & `oracle_ads-2.8.6/ads/model/service/oci_datascience_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import oci.data_science
 from ads.common import utils
 from ads.common.object_storage_details import ObjectStorageDetails
 from ads.common.oci_datascience import OCIDataScienceMixin
 from ads.common.oci_mixin import OCIWorkRequestMixin
 from ads.common.oci_resource import SEARCH_TYPE, OCIResource
 from ads.common.utils import extract_region
-from ads.model.deployment.model_deployer import ModelDeployer
+from ads.model.deployment import ModelDeployment
 from oci.data_science.models import (
     ArtifactExportDetailsObjectStorage,
     ArtifactImportDetailsObjectStorage,
     CreateModelDetails,
     ExportModelArtifactDetails,
     ImportModelArtifactDetails,
     UpdateModelDetails,
@@ -465,17 +465,15 @@
             logger.info(
                 f"Deleting model deployments associated with the model `{self.id}`."
             )
             for oci_model_deployment in active_deployments:
                 logger.info(
                     f"Deleting model deployment `{oci_model_deployment.identifier}`."
                 )
-                ModelDeployer(ds_client=self.client).delete(
-                    model_deployment_id=oci_model_deployment.identifier
-                )
+                ModelDeployment.from_id(oci_model_deployment.identifier).delete()
 
         logger.info(f"Deleting model `{self.id}`.")
         self.client.delete_model(self.id)
         return self.sync()
 
     @check_for_model_id(
         msg="Model needs to be saved to the Model Catalog before the associated model deployments can be read."
```

### Comparing `oracle_ads-2.8.5/ads/model/service/oci_datascience_model_deployment.py` & `oracle_ads-2.8.6/ads/model/service/oci_datascience_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/service/oci_datascience_model_version_set.py` & `oracle_ads-2.8.6/ads/model/service/oci_datascience_model_version_set.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/model/transformer/onnx_transformer.py` & `oracle_ads-2.8.6/ads/model/transformer/onnx_transformer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/mysqldb/mysql_db.py` & `oracle_ads-2.8.6/ads/mysqldb/mysql_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/ads_dataflow.py` & `oracle_ads-2.8.6/ads/opctl/backend/ads_dataflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import os
 import json
 import shlex
 from typing import Dict, Union
 
 from ads.opctl.backend.base import Backend
+from ads.opctl.decorator.common import print_watch_command
 from ads.common.auth import create_signer, AuthContext
 from ads.common.oci_client import OCIClientFactory
 
 from ads.opctl.backend.base import (
     Backend,
     RuntimeFactory,
 )
@@ -110,29 +111,30 @@
                 uri=uri,
                 overwrite=overwrite,
                 note=note,
                 filter_by_attribute_map=True,
                 **kwargs,
             )
 
-    def apply(self):
+    def apply(self) -> Dict:
         """
         Create DataFlow and DataFlow Run from YAML.
         """
         # TODO add the logic for build dataflow and dataflow run from YAML.
         raise NotImplementedError(f"`apply` hasn't been supported for data flow yet.")
 
-    def run(self) -> None:
+    @print_watch_command
+    def run(self) -> Dict:
         """
         Create DataFlow and DataFlow Run from OCID or cli parameters.
         """
         with AuthContext(auth=self.auth_type, profile=self.profile):
             if self.config["execution"].get("ocid", None):
-                data_flow_id = self.config["execution"]["ocid"]
-                run_id = Job.from_dataflow_job(data_flow_id).run().id
+                job_id = self.config["execution"]["ocid"]
+                run_id = Job.from_dataflow_job(job_id).run().id
             else:
                 infra = self.config.get("infrastructure", {})
                 if any(k not in infra for k in REQUIRED_FIELDS):
                     missing = [k for k in REQUIRED_FIELDS if k not in infra]
                     raise ValueError(
                         f"Following fields are missing but are required for OCI DataFlow Jobs: {missing}. Please run `ads opctl configure`."
                     )
```

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/ads_ml_job.py` & `oracle_ads-2.8.6/ads/opctl/backend/ads_ml_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,18 @@
     GitPythonRuntime,
     Job,
     NotebookRuntime,
     PythonRuntime,
     ScriptRuntime,
 )
 from ads.opctl import logger
-from ads.opctl.backend.base import (
-    Backend,
-    RuntimeFactory,
-)
+from ads.opctl.backend.base import Backend, RuntimeFactory
 from ads.opctl.config.resolver import ConfigResolver
 from ads.opctl.constants import DEFAULT_IMAGE_SCRIPT_DIR
+from ads.opctl.decorator.common import print_watch_command
 from ads.opctl.distributed.common.cluster_config_helper import (
     ClusterConfigToJobSpecConverter,
 )
 
 REQUIRED_FIELDS = [
     "project_id",
     "compartment_id",
@@ -122,26 +120,29 @@
                 uri=uri,
                 overwrite=overwrite,
                 note=note,
                 filter_by_attribute_map=True,
                 **kwargs,
             )
 
-    def apply(self) -> None:
+    @print_watch_command
+    def apply(self) -> Dict:
         """
         Create Job and Job Run from YAML.
         """
         with AuthContext(auth=self.auth_type, profile=self.profile):
             job = Job.from_dict(self.config)
             job.create()
             job_run = job.run()
             print("JOB OCID:", job.id)
             print("JOB RUN OCID:", job_run.id)
+            return {"job_id": job.id, "run_id": job_run.id}
 
-    def run(self) -> None:
+    @print_watch_command
+    def run(self) -> Dict:
         """
         Create Job and Job Run from OCID or cli parameters.
         """
         # TODO Check that this still runs smoothly for distributed
         with AuthContext(auth=self.auth_type, profile=self.profile):
             if self.config["execution"].get("ocid", None):
                 job_id = self.config["execution"]["ocid"]
```

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/ads_ml_pipeline.py` & `oracle_ads-2.8.6/ads/opctl/backend/ads_ml_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl/
 
 from typing import Dict, Union
 from ads.common.auth import create_signer, AuthContext
 from ads.common.oci_client import OCIClientFactory
 from ads.opctl.backend.base import Backend
 from ads.opctl.backend.ads_ml_job import JobRuntimeFactory
+from ads.opctl.decorator.common import print_watch_command
 from ads.pipeline import Pipeline, PipelineRun, PipelineStep, CustomScriptStep
 
 from ads.jobs import PythonRuntime
 
 
 class PipelineBackend(Backend):
     def __init__(self, config: Dict) -> None:
@@ -30,34 +31,39 @@
             config["execution"].get("oci_config", None),
             config["execution"].get("oci_profile", None),
         )
         self.auth_type = config["execution"].get("auth")
         self.profile = config["execution"].get("oci_profile", None)
         self.client = OCIClientFactory(**self.oci_auth).data_science
 
-    def apply(self) -> None:
+    @print_watch_command
+    def apply(self) -> Dict:
         """
         Create Pipeline and Pipeline Run from YAML.
         """
         with AuthContext(auth=self.auth_type, profile=self.profile):
             pipeline = Pipeline.from_dict(self.config)
             pipeline.create()
             pipeline_run = pipeline.run()
             print("PIPELINE OCID:", pipeline.id)
             print("PIPELINE RUN OCID:", pipeline_run.id)
+            return {"job_id": pipeline.id, "run_id": pipeline_run.id}
 
-    def run(self) -> None:
+    @print_watch_command
+    def run(self) -> Dict:
         """
         Create Pipeline and Pipeline Run from OCID.
         """
         pipeline_id = self.config["execution"]["ocid"]
         with AuthContext(auth=self.auth_type, profile=self.profile):
             pipeline = Pipeline.from_ocid(ocid=pipeline_id)
             pipeline_run = pipeline.run()
+            print("PIPELINE OCID:", pipeline.id)
             print("PIPELINE RUN OCID:", pipeline_run.id)
+            return {"job_id": pipeline.id, "run_id": pipeline_run.id}
 
     def delete(self) -> None:
         """
         Delete Pipeline or Pipeline Run from OCID.
         """
         if self.config["execution"].get("id"):
             pipeline_id = self.config["execution"]["id"]
@@ -80,15 +86,15 @@
             print(f"Pipeline run {run_id} has been cancelled.")
 
     def watch(self) -> None:
         """
         Watch Pipeline Run from OCID.
         """
         run_id = self.config["execution"]["run_id"]
-        log_type = self.config["execution"]["log_type"]
+        log_type = self.config["execution"].get("log_type")
         with AuthContext(auth=self.auth_type, profile=self.profile):
             PipelineRun.from_ocid(run_id).watch(log_type=log_type)
 
     def init(
         self,
         uri: Union[str, None] = None,
         overwrite: bool = False,
```

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/ads_model_deployment.py` & `oracle_ads-2.8.6/ads/opctl/backend/ads_model_deployment.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/base.py` & `oracle_ads-2.8.6/ads/opctl/backend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @abstractmethod
     def run(self) -> Dict:
         """
         Initiate a run.
 
         Returns
         -------
-        None
+        Dict
         """
 
     def delete(self) -> None:
         """
         Delete a remote run.
 
         Returns
@@ -58,21 +58,21 @@
         Cancel a remote run.
 
         Returns
         -------
         None
         """
 
-    def apply(self) -> None:
+    def apply(self) -> Dict:
         """
         Initiate Data Science service from YAML.
 
         Returns
         -------
-        None
+        Dict
         """
 
     def activate(self) -> None:
         """
         Activate a remote service.
 
         Returns
```

### Comparing `oracle_ads-2.8.5/ads/opctl/backend/local.py` & `oracle_ads-2.8.6/ads/opctl/backend/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     run_command,
     run_container,
 )
 from ads.pipeline.ads_pipeline import Pipeline, PipelineStep
 from ads.common.oci_client import OCIClientFactory
 from ads.config import NO_CONTAINER
 
+
 class CondaPackNotFound(Exception):  # pragma: no cover
     pass
 
 
 class LocalBackend(Backend):
     def __init__(self, config: Dict) -> None:
         """
@@ -215,15 +216,17 @@
             run_command(command, shell=True)
         else:
             conda_pack_path = os.path.join(
                 os.path.expanduser(self.config["execution"]["conda_pack_folder"]), slug
             )
             if os.path.exists(os.path.join(conda_pack_path, "spark-defaults.conf")):
                 env_vars["SPARK_CONF_DIR"] = os.path.join(DEFAULT_IMAGE_CONDA_DIR, slug)
-            logger.info(f"Running with conda pack in a container with command {command}")
+            logger.info(
+                f"Running with conda pack in a container with command {command}"
+            )
             return self._activate_conda_env_and_run(
                 image, slug, command, bind_volumes, env_vars
             )
 
     def _build_command_for_conda_run(self, extra_cmd: str = "") -> str:
         if ConfigResolver(self.config)._is_ads_operator():
             if is_in_notebook_session():
@@ -415,16 +418,15 @@
             client.api.inspect_image(image)
         except docker.errors.ImageNotFound:
             logger.info(f"Image {image} not found. Attempt building it now....")
             if image == ML_JOB_IMAGE:
                 build_image("job-local", gpu=False)
             else:
                 build_image("job-local", gpu=True)
-
-        with tempfile.TemporaryDirectory() as td:
+        with tempfile.TemporaryDirectory(dir=os.path.expanduser("~")) as td:
             with open(os.path.join(td, "entryscript.sh"), "w") as f:
                 f.write(
                     f"""
 #!/bin/bash
 source {os.path.join(DEFAULT_IMAGE_CONDA_DIR, slug, 'bin/activate')}
 {command}
                         """
@@ -677,19 +679,19 @@
         Conducts local verify.
 
         Returns
         -------
         None
             Nothing.
         """
-        
+
         # model artifact in artifact directory
         artifact_directory = self.config["execution"].get("artifact_directory")
         ocid = self.config["execution"].get("ocid")
-        
+
         model_folder = os.path.expanduser(
             self.config["execution"].get("model_save_folder", DEFAULT_MODEL_FOLDER)
         )
         artifact_directory = artifact_directory or os.path.join(model_folder, str(ocid))
         if ocid and (
             not os.path.exists(artifact_directory)
             or len(os.listdir(artifact_directory)) == 0
@@ -707,71 +709,80 @@
                 ocid=ocid,
                 artifact_directory=artifact_directory,
                 region=region,
                 bucket_uri=bucket_uri,
                 timeout=timeout,
                 force_overwrite=True,
             )
-                
+
         # conda
-        conda_slug, conda_path = self.config["execution"].get("conda_slug"), self.config["execution"].get("conda_path")
+        conda_slug = self.config["execution"].get("conda_slug")
+        conda_path = self.config["execution"].get("conda_path")
         if not conda_slug and not conda_path and ocid:
             conda_slug, conda_path = self._get_conda_info_from_custom_metadata(ocid)
         if not conda_slug and not conda_path:
             conda_slug, conda_path = self._get_conda_info_from_runtime(
                 artifact_dir=artifact_directory
             )
-        if 'conda_slug' not in self.config["execution"]:
-            self.config["execution"]["conda_slug"] = conda_path.split("/")[-1] if conda_path else conda_slug 
+        if "conda_slug" not in self.config["execution"]:
+            self.config["execution"]["conda_slug"] = (
+                conda_path.split("/")[-1] if conda_path else conda_slug
+            )
 
         self.config["execution"]["image"] = ML_JOB_IMAGE
-        
+
         # bind_volumnes
         bind_volumes = {}
         SCRIPT = "script.py"
         dir_path = os.path.dirname(os.path.realpath(__file__))
         if not is_in_notebook_session():
             bind_volumes = {
                 os.path.expanduser(
                     os.path.dirname(self.config["execution"]["oci_config"])
                 ): {"bind": os.path.join(DEFAULT_IMAGE_HOME_DIR, ".oci")}
             }
-            
+
             self.config["execution"]["source_folder"] = os.path.abspath(
                 os.path.join(dir_path, "..")
             )
             self.config["execution"]["entrypoint"] = SCRIPT
             bind_volumes[artifact_directory] = {"bind": DEFAULT_MODEL_DEPLOYMENT_FOLDER}
-        
+
         # extra cmd
         data = self.config["execution"].get("payload")
         extra_cmd = f"--payload '{data}' " + f"--auth {self.auth_type} "
         if self.auth_type != "resource_principal":
             extra_cmd += f"--profile {self.profile}"
-        
+
         if is_in_notebook_session() or NO_CONTAINER:
             # _run_with_conda_pack has code to handle notebook session case,
-            # however, it activate the conda pack and then run the script. 
+            # however, it activate the conda pack and then run the script.
             # For the deployment, we just take the current conda env and run it.
             # Hence we just handle the notebook case directly here.
             script_path = os.path.join(os.path.join(dir_path, ".."), SCRIPT)
-            cmd = f"python {script_path} " + f"--artifact-directory {artifact_directory} " + extra_cmd
+            cmd = (
+                f"python {script_path} "
+                + f"--artifact-directory {artifact_directory} "
+                + extra_cmd
+            )
             logger.info(f"Running in a notebook or NO_CONTAINER with command {cmd}")
             run_command(cmd=cmd, shell=True)
         else:
-            extra_cmd = f"--artifact-directory {DEFAULT_MODEL_DEPLOYMENT_FOLDER} "+ extra_cmd
+            extra_cmd = (
+                f"--artifact-directory {DEFAULT_MODEL_DEPLOYMENT_FOLDER} " + extra_cmd
+            )
             exit_code = self._run_with_conda_pack(
-                    bind_volumes, extra_cmd, install=True, conda_uri=conda_path
-                )
+                bind_volumes, extra_cmd, install=True, conda_uri=conda_path
+            )
             if exit_code != 0:
                 raise RuntimeError(
                     f"`predict` did not complete successfully. Exit code: {exit_code}. "
                     f"Run with the --debug argument to view container logs."
                 )
-                
+
     def _get_conda_info_from_custom_metadata(self, ocid):
         """
         Get conda env info from custom metadata from model catalog.
 
         Returns
         -------
         (str, str)
```

### Comparing `oracle_ads-2.8.5/ads/opctl/cli.py` & `oracle_ads-2.8.6/ads/opctl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 from ads.opctl.cmds import init_operator as init_operator_cmd
 from ads.opctl.cmds import init_vscode as init_vscode_cmd
 from ads.opctl.cmds import predict as predict_cmd
 from ads.opctl.cmds import run as run_cmd
 from ads.opctl.cmds import run_diagnostics as run_diagnostics_cmd
 from ads.opctl.cmds import watch as watch_cmd
 from ads.opctl.config.merger import ConfigMerger
-from ads.opctl.constants import (BACKEND_NAME, DEFAULT_MODEL_FOLDER,
-                                 RESOURCE_TYPE, RUNTIME_TYPE)
+from ads.opctl.constants import (
+    BACKEND_NAME,
+    DEFAULT_MODEL_FOLDER,
+    RESOURCE_TYPE,
+    RUNTIME_TYPE,
+)
 from ads.opctl.utils import build_image as build_image_cmd
 from ads.opctl.utils import publish_image as publish_image_cmd
 from ads.opctl.utils import suppress_traceback
 
 
 @click.group("opctl")
 @click.help_option("--help", "-h")
```

### Comparing `oracle_ads-2.8.5/ads/opctl/cmds.py` & `oracle_ads-2.8.6/ads/opctl/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
                 print(yamlContent)
                 _save_yaml(yamlContent, **kwargs)
             return cluster_run_info
     else:
         if (
             "kind" in p.config
             and p.config["execution"].get("backend", None) != BACKEND_NAME.LOCAL.value
+            and "ocid" not in p.config["execution"]
         ):
             p.config["execution"]["backend"] = p.config["kind"]
             return _BackendFactory(p.config).backend.apply()
 
         if "ocid" in p.config["execution"]:
             resource_to_backend = {
                 DataScienceResource.JOB: BACKEND_NAME.JOB,
```

### Comparing `oracle_ads-2.8.5/ads/opctl/conda/cli.py` & `oracle_ads-2.8.6/ads/opctl/conda/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/conda/cmds.py` & `oracle_ads-2.8.6/ads/opctl/conda/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/conda/config.yaml` & `oracle_ads-2.8.6/ads/opctl/conda/config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/conda/multipart_uploader.py` & `oracle_ads-2.8.6/ads/opctl/conda/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/conda/pack.py` & `oracle_ads-2.8.6/ads/opctl/conda/pack.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/base.py` & `oracle_ads-2.8.6/ads/opctl/config/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml` & `oracle_ads-2.8.6/ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/merger.py` & `oracle_ads-2.8.6/ads/opctl/config/merger.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/resolver.py` & `oracle_ads-2.8.6/ads/opctl/config/resolver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/utils.py` & `oracle_ads-2.8.6/ads/opctl/config/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/validator.py` & `oracle_ads-2.8.6/ads/opctl/config/validator.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/versioner.py` & `oracle_ads-2.8.6/ads/opctl/config/versioner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/base.py` & `oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py` & `oracle_ads-2.8.6/ads/opctl/config/yaml_parsers/distributed/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/constants.py` & `oracle_ads-2.8.6/ads/opctl/constants.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/diagnostics/__main__.py` & `oracle_ads-2.8.6/ads/opctl/diagnostics/__main__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/diagnostics/check_distributed_job_requirements.py` & `oracle_ads-2.8.6/ads/opctl/diagnostics/check_distributed_job_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/diagnostics/check_requirements.py` & `oracle_ads-2.8.6/ads/opctl/diagnostics/check_requirements.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/certificates.py` & `oracle_ads-2.8.6/ads/opctl/distributed/certificates.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/cli.py` & `oracle_ads-2.8.6/ads/opctl/distributed/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/cmds.py` & `oracle_ads-2.8.6/ads/opctl/distributed/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_cluster_provider.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/abstract_cluster_provider.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/abstract_framework_spec_builder.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/abstract_framework_spec_builder.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_config_helper.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_config_helper.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_provider_factory.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_provider_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/cluster_runner.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/cluster_runner.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/distributed/common/framework_factory.py` & `oracle_ads-2.8.6/ads/opctl/distributed/common/framework_factory.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile` & `oracle_ads-2.8.6/ads/opctl/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.gpu` & `oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.gpu`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job` & `oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.job`

 * *Files 4% similar despite different names*

```diff
@@ -58,24 +58,23 @@
 #conda
 # set a default language for localization.  necessary for oci cli
 ARG LANG=en_US.utf8
 ENV LANG=$LANG
 ENV SHELL=/bin/bash
 
 # set /opt folder permissions for $DATASCIENCE_USER. Conda is going to live in this folder.
-ARG MINICONDA_VER=4.8.3
 RUN chown $DATASCIENCE_USER /opt
 
 USER $DATASCIENCE_USER
 WORKDIR /home/datascience
 RUN curl -L https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh >> /home/datascience/miniconda.sh \
     && /bin/bash /home/datascience/miniconda.sh -f -b -p /opt/conda \
     && rm /home/datascience/miniconda.sh \
     && ls  /opt/**/* \
-    && /opt/conda/bin/conda install python=3.7 anaconda \
+    && /opt/conda/bin/conda install python=3.8 anaconda \
     && /opt/conda/bin/conda clean -yaf
 
 WORKDIR /
 USER root
 RUN printf "#!/bin/bash\nsource /opt/conda/bin/activate\n" > /etc/profile.d/enableconda.sh \
     && chmod +x /etc/profile.d/enableconda.sh
 
@@ -87,15 +86,15 @@
 #COPY base-env.yaml /opt/base-env.yaml
 #RUN conda env update -q -n root -f /opt/base-env.yaml && conda clean -yaf && rm -rf /home/datascience/.cache/pip
 
 
 USER $DATASCIENCE_USER
 
 ####### WRAP UP ###############################
-RUN python -c 'import sys; assert(sys.version_info[:2]) == (3, 7), "Python 3.7 is not detected"'
+RUN python -c 'import sys; assert(sys.version_info[:2]) == (3, 8), "Python 3.8 is not detected"'
 WORKDIR /
 
 RUN conda list
 
 USER root
 
 ############# Setup Conda environment tools ###########################
```

### Comparing `oracle_ads-2.8.5/ads/opctl/docker/Dockerfile.job.gpu` & `oracle_ads-2.8.6/ads/opctl/docker/Dockerfile.job.gpu`

 * *Files 1% similar despite different names*

```diff
@@ -103,24 +103,23 @@
 #conda
 # set a default language for localization.  necessary for oci cli
 ARG LANG=en_US.utf8
 ENV LANG=$LANG
 ENV SHELL=/bin/bash
 
 # set /opt folder permissions for $DATASCIENCE_USER. Conda is going to live in this folder.
-ARG MINICONDA_VER=4.8.3
 RUN chown $DATASCIENCE_USER /opt
 
 USER $DATASCIENCE_USER
 WORKDIR /home/datascience
 RUN curl -L https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh >> /home/datascience/miniconda.sh \
     && /bin/bash /home/datascience/miniconda.sh -f -b -p /opt/conda \
     && rm /home/datascience/miniconda.sh \
     && ls  /opt/**/* \
-    && /opt/conda/bin/conda install python=3.7 anaconda \
+    && /opt/conda/bin/conda install python=3.8 anaconda \
     && /opt/conda/bin/conda clean -yaf
 
 WORKDIR /
 USER root
 RUN printf "#!/bin/bash\nsource /opt/conda/bin/activate\n" > /etc/profile.d/enableconda.sh \
     && chmod +x /etc/profile.d/enableconda.sh
 
@@ -132,15 +131,15 @@
 #COPY base-env.yaml /opt/base-env.yaml
 #RUN conda env update -q -n root -f /opt/base-env.yaml && conda clean -yaf && rm -rf /home/datascience/.cache/pip
 
 
 USER $DATASCIENCE_USER
 
 ####### WRAP UP ###############################
-RUN python -c 'import sys; assert(sys.version_info[:2]) == (3, 7), "Python 3.7 is not detected"'
+RUN python -c 'import sys; assert(sys.version_info[:2]) == (3, 8), "Python 3.8 is not detected"'
 WORKDIR /
 
 RUN conda list
 
 USER root
 
 ############# Setup Conda environment tools ###########################
```

### Comparing `oracle_ads-2.8.5/ads/opctl/docker/merge_dependencies.py` & `oracle_ads-2.8.6/ads/opctl/docker/merge_dependencies.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/model/cli.py` & `oracle_ads-2.8.6/ads/opctl/model/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/model/cmds.py` & `oracle_ads-2.8.6/ads/opctl/model/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/script.py` & `oracle_ads-2.8.6/ads/opctl/script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/spark/cli.py` & `oracle_ads-2.8.6/ads/opctl/spark/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/spark/cmds.py` & `oracle_ads-2.8.6/ads/opctl/spark/cmds.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/templates/diagnostic_report_template.jinja2` & `oracle_ads-2.8.6/ads/opctl/templates/diagnostic_report_template.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/opctl/utils.py` & `oracle_ads-2.8.6/ads/opctl/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/oracledb/oracle_db.py` & `oracle_ads-2.8.6/ads/oracledb/oracle_db.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/__init__.py` & `oracle_ads-2.8.6/ads/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/ads_pipeline.py` & `oracle_ads-2.8.6/ads/pipeline/ads_pipeline.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/ads_pipeline_run.py` & `oracle_ads-2.8.6/ads/pipeline/ads_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/ads_pipeline_step.py` & `oracle_ads-2.8.6/ads/pipeline/ads_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/builders/infrastructure/custom_script.py` & `oracle_ads-2.8.6/ads/pipeline/builders/infrastructure/custom_script.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/cli.py` & `oracle_ads-2.8.6/ads/pipeline/cli.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/extension.py` & `oracle_ads-2.8.6/ads/pipeline/extension.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/visualizer/base.py` & `oracle_ads-2.8.6/ads/pipeline/visualizer/base.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/visualizer/graph_renderer.py` & `oracle_ads-2.8.6/ads/pipeline/visualizer/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/pipeline/visualizer/text_renderer.py` & `oracle_ads-2.8.6/ads/pipeline/visualizer/text_renderer.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/adb.py` & `oracle_ads-2.8.6/ads/secrets/adb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/auth_token.py` & `oracle_ads-2.8.6/ads/secrets/auth_token.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/big_data_service.py` & `oracle_ads-2.8.6/ads/secrets/big_data_service.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/mysqldb.py` & `oracle_ads-2.8.6/ads/secrets/mysqldb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/oracledb.py` & `oracle_ads-2.8.6/ads/secrets/oracledb.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/secrets/secrets.py` & `oracle_ads-2.8.6/ads/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/telemetry/telemetry.py` & `oracle_ads-2.8.6/ads/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score-pkl.jinja2` & `oracle_ads-2.8.6/ads/templates/score-pkl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score.jinja2` & `oracle_ads-2.8.6/ads/templates/score.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_generic.jinja2` & `oracle_ads-2.8.6/ads/templates/score_generic.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_huggingface_pipeline.jinja2` & `oracle_ads-2.8.6/ads/templates/score_huggingface_pipeline.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_lightgbm.jinja2` & `oracle_ads-2.8.6/ads/templates/score_lightgbm.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_onnx.jinja2` & `oracle_ads-2.8.6/ads/templates/score_onnx.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_onnx_new.jinja2` & `oracle_ads-2.8.6/ads/templates/score_onnx_new.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_oracle_automl.jinja2` & `oracle_ads-2.8.6/ads/templates/score_oracle_automl.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_pyspark.jinja2` & `oracle_ads-2.8.6/ads/templates/score_pyspark.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_pytorch.jinja2` & `oracle_ads-2.8.6/ads/templates/score_pytorch.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_scikit-learn.jinja2` & `oracle_ads-2.8.6/ads/templates/score_scikit-learn.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_tensorflow.jinja2` & `oracle_ads-2.8.6/ads/templates/score_tensorflow.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/templates/score_xgboost.jinja2` & `oracle_ads-2.8.6/ads/templates/score_xgboost.jinja2`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/backends.py` & `oracle_ads-2.8.6/ads/text_dataset/backends.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/dataset.py` & `oracle_ads-2.8.6/ads/text_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/extractor.py` & `oracle_ads-2.8.6/ads/text_dataset/extractor.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/options.py` & `oracle_ads-2.8.6/ads/text_dataset/options.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/udfs.py` & `oracle_ads-2.8.6/ads/text_dataset/udfs.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/text_dataset/utils.py` & `oracle_ads-2.8.6/ads/text_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/abstract_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/abstract_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/constant_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/constant_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/continuous_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/continuous_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/credit_card_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/credit_card_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/datetime_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/datetime_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/discrete_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/discrete_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/document_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/document_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/ip_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/ip_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/latlon_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/latlon_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/phone_number_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/phone_number_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/type_discovery_driver.py` & `oracle_ads-2.8.6/ads/type_discovery/type_discovery_driver.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/typed_feature.py` & `oracle_ads-2.8.6/ads/type_discovery/typed_feature.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/unknown_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/unknown_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/type_discovery/zipcode_detector.py` & `oracle_ads-2.8.6/ads/type_discovery/zipcode_detector.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/ads/vault/vault.py` & `oracle_ads-2.8.6/ads/vault/vault.py`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/oracle_ads.egg-info/PKG-INFO` & `oracle_ads-2.8.6/oracle_ads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracle-ads
-Version: 2.8.5
+Version: 2.8.6
 Summary: Oracle Accelerated Data Science SDK
 Home-page: https://docs.oracle.com/en-us/iaas/tools/ads-sdk/latest/index.html
 Author: Oracle Data Science
 License: Universal Permissive License 1.0
 Project-URL: Github, https://github.com/oracle/accelerated-data-science
 Project-URL: Documentation, https://accelerated-data-science.readthedocs.io/en/latest/index.html
 Keywords: Oracle Cloud Infrastructure,OCI,Machine Learning,ML,Artificial Intelligence,AI,Data Science,Cloud,Oracle
```

### Comparing `oracle_ads-2.8.5/oracle_ads.egg-info/SOURCES.txt` & `oracle_ads-2.8.6/oracle_ads.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 THIRD_PARTY_LICENSES.txt
 setup.cfg
 setup.py
 ads/__init__.py
-ads/ads
 ads/ads_version.json
 ads/cli.py
 ads/config.py
 ads/automl/__init__.py
 ads/automl/driver.py
 ads/automl/provider.py
 ads/bds/__init__.py
@@ -81,17 +80,14 @@
 ads/data_labeling/reader/metadata_reader.py
 ads/data_labeling/reader/record_reader.py
 ads/data_labeling/visualizer/__init__.py
 ads/data_labeling/visualizer/image_visualizer.py
 ads/data_labeling/visualizer/text_visualizer.py
 ads/database/__init__.py
 ads/database/connection.py
-ads/dataflow/__init__.py
-ads/dataflow/dataflow.py
-ads/dataflow/dataflowsummary.py
 ads/dataset/__init__.py
 ads/dataset/classification_dataset.py
 ads/dataset/correlation.py
 ads/dataset/correlation_plot.py
 ads/dataset/dask_series.py
 ads/dataset/dataframe_transformer.py
 ads/dataset/dataset.py
@@ -339,14 +335,16 @@
 ads/opctl/config/versioner.py
 ads/opctl/config/diagnostics/__init__.py
 ads/opctl/config/diagnostics/distributed/default_requirements_config.yaml
 ads/opctl/config/yaml_parsers/__init__.py
 ads/opctl/config/yaml_parsers/base.py
 ads/opctl/config/yaml_parsers/distributed/__init__.py
 ads/opctl/config/yaml_parsers/distributed/yaml_parser.py
+ads/opctl/decorator/__init__.py
+ads/opctl/decorator/common.py
 ads/opctl/diagnostics/__init__.py
 ads/opctl/diagnostics/__main__.py
 ads/opctl/diagnostics/check_distributed_job_requirements.py
 ads/opctl/diagnostics/check_requirements.py
 ads/opctl/diagnostics/requirement_exception.py
 ads/opctl/distributed/__init__.py
 ads/opctl/distributed/certificates.py
@@ -436,9 +434,10 @@
 ads/type_discovery/unknown_detector.py
 ads/type_discovery/zipcode_detector.py
 ads/vault/__init__.py
 ads/vault/vault.py
 oracle_ads.egg-info/PKG-INFO
 oracle_ads.egg-info/SOURCES.txt
 oracle_ads.egg-info/dependency_links.txt
+oracle_ads.egg-info/entry_points.txt
 oracle_ads.egg-info/requires.txt
 oracle_ads.egg-info/top_level.txt
```

### Comparing `oracle_ads-2.8.5/oracle_ads.egg-info/requires.txt` & `oracle_ads-2.8.6/oracle_ads.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `oracle_ads-2.8.5/setup.py` & `oracle_ads-2.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,9 +166,13 @@
     tests_require=[
         "pytest",
     ],
     project_urls={
         "Github": "https://github.com/oracle/accelerated-data-science",
         "Documentation": "https://accelerated-data-science.readthedocs.io/en/latest/index.html",
     },
-    scripts=["ads/ads"],
+    entry_points={
+        'console_scripts': [
+            'ads=ads.cli:cli'
+        ]
+    },
 )
```

