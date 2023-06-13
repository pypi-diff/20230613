# Comparing `tmp/deeplake-3.6.2.tar.gz` & `tmp/deeplake-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.2.tar", last modified: Fri Jun  9 15:01:52 2023, max compression
+gzip compressed data, was "deeplake-3.6.3.tar", last modified: Tue Jun 13 18:21:09 2023, max compression
```

## Comparing `deeplake-3.6.2.tar` & `deeplake-3.6.3.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-09 15:00:23.000000 deeplake-3.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-09 15:00:23.000000 deeplake-3.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-09 15:01:52.265233 deeplake-3.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25351 2023-06-09 15:00:23.000000 deeplake-3.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96883 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    85180 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    25706 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    18863 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7357 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   113519 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171829 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    15422 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15995 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13705 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50140 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.243567 deeplake-3.6.2/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51556 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24052 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    30075 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11148 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    10090 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     9551 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25897 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22353 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9862 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.254400 deeplake-3.6.2/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16165 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34773 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8435 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25235 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.265233 deeplake-3.6.2/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-09 15:00:23.000000 deeplake-3.6.2/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 15:01:52.232733 deeplake-3.6.2/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26080 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12677 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 15:01:52.000000 deeplake-3.6.2/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-09 15:01:52.265233 deeplake-3.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-09 15:00:23.000000 deeplake-3.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-13 18:19:49.000000 deeplake-3.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-13 18:19:49.000000 deeplake-3.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-13 18:21:09.146204 deeplake-3.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25351 2023-06-13 18:19:49.000000 deeplake-3.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.116204 deeplake-3.6.3/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96883 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    85180 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18863 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7332 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   113519 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171829 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15422 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15995 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.126204 deeplake-3.6.3/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13705 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50140 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51556 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    30234 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11211 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10090 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     9551 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.136204 deeplake-3.6.3/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16165 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34773 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8435 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25235 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.146204 deeplake-3.6.3/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-13 18:19:49.000000 deeplake-3.6.3/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 18:21:09.116204 deeplake-3.6.3/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 18:21:08.000000 deeplake-3.6.3/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-13 18:21:09.146204 deeplake-3.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-13 18:19:49.000000 deeplake-3.6.3/setup.py
```

### Comparing `deeplake-3.6.2/LICENSE` & `deeplake-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/PKG-INFO` & `deeplake-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.2
+Version: 3.6.3
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.3 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.2/README.md` & `deeplake-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/__init__.py` & `deeplake-3.6.3/deeplake/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.2"
+__version__ = "3.6.3"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.6.2/deeplake/api/dataset.py` & `deeplake-3.6.3/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/info.py` & `deeplake-3.6.3/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/link.py` & `deeplake-3.6.3/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/link_tiled.py` & `deeplake-3.6.3/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/read.py` & `deeplake-3.6.3/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.3/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.3/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_api.py` & `deeplake-3.6.3/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.3/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.3/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.3/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.3/deeplake/api/tests/test_connect_datasets.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,19 +58,28 @@
         memory_ds.connect(creds_key="some_creds", dest_path="hub://someorg/somename")
 
     # Connecting a cloud dataset is not permitted as its already avaliable via a Deep Lake path
     with pytest.raises(InvalidSourcePathError):
         hub_cloud_ds.connect(creds_key="some_creds", dest_path="hub://someorg/somename")
 
 
-def test_connect_user_not_in_org(s3_ds_generator):
+def test_connect_user_not_in_org(s3_ds_generator, hub_cloud_dev_token):
     with s3_ds_generator() as ds:
         ds.create_tensor("x")
         ds.x.append(10)
 
     with pytest.raises(TokenPermissionError) as e:
-        ds.connect(creds_key="some_creds", dest_path="hub://bad-org/some-name")
+        ds.connect(
+            creds_key="some_creds",
+            dest_path="hub://bad-org/some-name",
+            token=hub_cloud_dev_token,
+        )
         assert "dataset path" in str(e)
 
     with pytest.raises(TokenPermissionError) as e:
-        ds.connect(creds_key="some_creds", org_id="bad-org", ds_name="some-name")
+        ds.connect(
+            creds_key="some_creds",
+            org_id="bad-org",
+            ds_name="some-name",
+            token=hub_cloud_dev_token,
+        )
         assert "organization id" in str(e)
```

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.3/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.3/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.3/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_events.py` & `deeplake-3.6.3/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.3/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_info.py` & `deeplake-3.6.3/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.3/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_json.py` & `deeplake-3.6.3/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_link.py` & `deeplake-3.6.3/deeplake/api/tests/test_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -659,21 +659,21 @@
     ds.add_creds_key(creds_key)
     ds.populate_creds(creds_key, from_environment=True)
     with ds:
         tensor = ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
         tensor.append(deeplake.link(cat_path, creds_key))
 
     assert tensor[0].creds_key() == creds_key
-    ds.add_creds_key("my_s3_creds", True)
-    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
-    assert ds.get_creds_keys() == {"my_s3_creds", "ENV"}
-    ds.update_creds_key("my_s3_creds", managed=True)
+    ds.add_creds_key("aws_creds", True)
+    assert ds.get_managed_creds_keys() == {"aws_creds"}
+    assert set(ds.get_creds_keys()) == {"aws_creds", "ENV"}
+    ds.update_creds_key("aws_creds", managed=True)
     ds = hub_cloud_ds_generator()
-    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
-    assert ds.get_creds_keys() == {"my_s3_creds", "ENV"}
+    assert ds.get_managed_creds_keys() == {"aws_creds"}
+    assert set(ds.get_creds_keys()) == {"aws_creds", "ENV"}
 
 
 def test_bad_link_no_verify(memory_ds):
     with memory_ds as ds:
         ds.add_creds_key("S3_CREDS")
         ds.populate_creds("S3_CREDS", {})
         ds.create_tensor(
@@ -692,41 +692,41 @@
     ds.add_creds_key(creds_key)
     ds.populate_creds(creds_key, from_environment=True)
 
     with ds:
         tensor = ds.create_tensor("abc", "link[image]", sample_compression="jpeg")
         tensor.append(deeplake.link(cat_path, creds_key))
 
-    ds.add_creds_key("my_s3_creds", managed=True)
+    ds.add_creds_key("aws_creds", managed=True)
 
     with pytest.raises(ValueError):
-        ds.update_creds_key("ENV", "my_s3_creds")
+        ds.update_creds_key("ENV", "aws_creds")
 
     with pytest.raises(ValueError):
-        ds.update_creds_key("my_s3_creds", "ENV")
+        ds.update_creds_key("aws_creds", "ENV")
 
     with pytest.raises(ValueError):
-        ds.update_creds_key("ENV", "my_s3_creds", managed=False)
+        ds.update_creds_key("ENV", "aws_creds", managed=False)
 
     with pytest.raises(ValueError):
-        ds.update_creds_key("my_s3_creds", "ENV", managed=True)
+        ds.update_creds_key("aws_creds", "ENV", managed=True)
 
     with ds:
-        tensor.append(deeplake.link(cat_path, "my_s3_creds"))
+        tensor.append(deeplake.link(cat_path, "aws_creds"))
 
-    ds.update_creds_key("ENV", "my_s3_creds", managed=True)
-    assert ds.get_managed_creds_keys() == {"my_s3_creds"}
-    assert ds.get_creds_keys() == {"my_s3_creds"}
-    assert ds.link_creds.creds_keys == ["my_s3_creds", "my_s3_creds"]
+    ds.update_creds_key("ENV", "aws_creds", managed=True)
+    assert ds.get_managed_creds_keys() == {"aws_creds"}
+    assert ds.get_creds_keys() == {"aws_creds"}
+    assert ds.link_creds.creds_keys == ["aws_creds", "aws_creds"]
 
     encoded_creds = ds.abc.chunk_engine.creds_encoder.get_encoded_creds_key(0)
     creds_key = ds.link_creds.get_creds_key(encoded_creds)
-    assert creds_key == "my_s3_creds"
+    assert creds_key == "aws_creds"
 
-    ds.update_creds_key("my_s3_creds", "ENV", managed=False)
+    ds.update_creds_key("aws_creds", "ENV", managed=False)
     assert ds.get_managed_creds_keys() == set()
     assert ds.get_creds_keys() == {"ENV"}
     assert ds.link_creds.creds_keys == ["ENV", "ENV"]
 
     encoded_creds = ds.abc.chunk_engine.creds_encoder.get_encoded_creds_key(0)
     creds_key = ds.link_creds.get_creds_key(encoded_creds)
     assert creds_key == "ENV"
```

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.3/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_linking.py` & `deeplake-3.6.3/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.3/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_meta.py` & `deeplake-3.6.3/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.3/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_none.py` & `deeplake-3.6.3/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.3/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.3/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.3/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.3/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_pop.py` & `deeplake-3.6.3/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.3/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.3/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_reset.py` & `deeplake-3.6.3/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.3/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_text.py` & `deeplake-3.6.3/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.3/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_video.py` & `deeplake-3.6.3/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tests/test_views.py` & `deeplake-3.6.3/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/api/tiled.py` & `deeplake-3.6.3/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/structured/base.py` & `deeplake-3.6.3/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.3/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.3/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.3/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.3/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.3/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/base.py` & `deeplake-3.6.3/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.3/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.3/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.3/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.3/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.3/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.3/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/util.py` & `deeplake-3.6.3/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.3/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.3/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/cli/auth.py` & `deeplake-3.6.3/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/cli/test_cli.py` & `deeplake-3.6.3/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/client/client.py` & `deeplake-3.6.3/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/client/config.py` & `deeplake-3.6.3/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/client/log.py` & `deeplake-3.6.3/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/client/test_client.py` & `deeplake-3.6.3/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/client/utils.py` & `deeplake-3.6.3/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/compression.py` & `deeplake-3.6.3/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/constants.py` & `deeplake-3.6.3/deeplake/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 ENV_GDRIVE_REFRESH_TOKEN = "GDRIVE_REFRESH_TOKEN"
 
 HUB_CLOUD_DEV_USERNAME = os.getenv(ENV_HUB_DEV_USERNAME)  # type: ignore
 HUB_CLOUD_DEV_PASSWORD = os.getenv(ENV_HUB_DEV_PASSWORD)
 
 # dataset base roots for pytests
 PYTEST_MEMORY_PROVIDER_BASE_ROOT = "mem://hub_pytest"
-PYTEST_LOCAL_PROVIDER_BASE_ROOT = "./hub_pytest/"  # TODO: may fail for windows
-PYTEST_S3_PROVIDER_BASE_ROOT = "s3://hub-2.0-tests/"
-PYTEST_GCS_PROVIDER_BASE_ROOT = "gcs://snark-test/"
+PYTEST_LOCAL_PROVIDER_BASE_ROOT = "./hub_pytest/"
+PYTEST_S3_PROVIDER_BASE_ROOT = "s3://deeplake-tests/"
+PYTEST_GCS_PROVIDER_BASE_ROOT = "gcs://deeplake-tests/"
 PYTEST_AZURE_PROVIDER_BASE_ROOT = "az://activeloopgen2/deeplake-tests/"
 PYTEST_GDRIVE_PROVIDER_BASE_ROOT = "gdrive://hubtest"
 PYTEST_HUB_CLOUD_PROVIDER_BASE_ROOT = (
     None if HUB_CLOUD_DEV_USERNAME is None else f"hub://{HUB_CLOUD_DEV_USERNAME}/"
 )
 
 # pytest options
```

### Comparing `deeplake-3.6.2/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.3/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.3/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.3/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.3/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.3/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.3/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.3/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/chunk_engine.py` & `deeplake-3.6.3/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compression.py` & `deeplake-3.6.3/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compute/process.py` & `deeplake-3.6.3/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compute/provider.py` & `deeplake-3.6.3/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compute/ray.py` & `deeplake-3.6.3/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compute/serial.py` & `deeplake-3.6.3/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/compute/thread.py` & `deeplake-3.6.3/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/__init__.py` & `deeplake-3.6.3/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/dataset.py` & `deeplake-3.6.3/deeplake/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.3/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.3/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.3/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.3/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.3/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/fast_forwarding.py` & `deeplake-3.6.3/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/index/index.py` & `deeplake-3.6.3/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/io.py` & `deeplake-3.6.3/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/ipc.py` & `deeplake-3.6.3/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/link_creds.py` & `deeplake-3.6.3/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.3/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/linked_sample.py` & `deeplake-3.6.3/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.3/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/lock.py` & `deeplake-3.6.3/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.3/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.3/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.3/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.3/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.3/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.3/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.3/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.3/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.3/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.3/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/partial_reader.py` & `deeplake-3.6.3/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/partial_sample.py` & `deeplake-3.6.3/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/polygon.py` & `deeplake-3.6.3/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/query/autocomplete.py` & `deeplake-3.6.3/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/query/filter.py` & `deeplake-3.6.3/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/query/query.py` & `deeplake-3.6.3/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/sample.py` & `deeplake-3.6.3/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/serialize.py` & `deeplake-3.6.3/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/azure.py` & `deeplake-3.6.3/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.3/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/gcs.py` & `deeplake-3.6.3/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/google_drive.py` & `deeplake-3.6.3/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/local.py` & `deeplake-3.6.3/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.3/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/memory.py` & `deeplake-3.6.3/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/provider.py` & `deeplake-3.6.3/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/storage/s3.py` & `deeplake-3.6.3/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tensor.py` & `deeplake-3.6.3/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tensor_link.py` & `deeplake-3.6.3/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/test_serialize.py` & `deeplake-3.6.3/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_compression.py` & `deeplake-3.6.3/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_compute.py` & `deeplake-3.6.3/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.3/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_io.py` & `deeplake-3.6.3/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_locking.py` & `deeplake-3.6.3/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.3/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.3/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.3/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.3/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.3/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/serialize.py` & `deeplake-3.6.3/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.3/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.3/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/transform/test_transform.py` & `deeplake-3.6.3/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/transform/transform.py` & `deeplake-3.6.3/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.3/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.3/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.3/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.3/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,20 +337,21 @@
             query=query,
             filter=filter,
             exec_option=exec_option,
             embedding_tensor=embedding_tensor,
             return_tensors=return_tensors,
         )
 
-        # if embedding_function is not None or embedding is not None:
-        query_emb = dataset_utils.get_embedding(
-            embedding,
-            embedding_data,
-            embedding_function=embedding_function or self.embedding_function,
-        )
+        query_emb: Optional[Union[List[float], np.ndarray[Any, Any]]] = None
+        if query is None:
+            query_emb = dataset_utils.get_embedding(
+                embedding,
+                embedding_data,
+                embedding_function=embedding_function or self.embedding_function,
+            )
 
         if not return_tensors:
             return_tensors = [
                 tensor for tensor in self.dataset.tensors if tensor != embedding_tensor
             ]
 
         return vector_search.search(
```

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,23 +265,22 @@
             return_tensors=["metadata", "id"],
         )
 
     vector_store = DeepLakeVectorStore(
         path="mem://xyz", embedding_function=embedding_fn
     )
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
-    result = vector_store.search(embedding=np.zeros(1, EMBEDDING_DIM))
+    result = vector_store.search(embedding=np.zeros((1, EMBEDDING_DIM)))
     assert len(result) == 4
 
 
 @requires_libdeeplake
 @pytest.mark.parametrize("distance_metric", ["L1", "L2", "COS", "MAX"])
 def test_search_quantitative(distance_metric, hub_cloud_dev_token):
     """Test whether TQL and Python return the same results"""
-
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
         path="hub://testingacc2/vectorstore_test",
         read_only=True,
         token=hub_cloud_dev_token,
     )
 
@@ -329,14 +328,20 @@
         data_ce = vector_store.search(
             query="select * where metadata == {'abcdefg': 28}",
             exec_option="compute_engine",
             distance_metric=distance_metric,
             filter={"metadata": {"abcdefg": 28}},
         )
 
+    data_ce = vector_store.search(
+        query="select * where ids == '0'",
+        exec_option="compute_engine",
+    )
+    assert data_ce["ids"] == ["0"]
+
 
 @requires_libdeeplake
 def test_search_managed(hub_cloud_dev_token):
     """Test whether managed TQL and client-side TQL return the same results"""
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
         path="hub://testingacc2/vectorstore_test_managed",
```

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,19 @@
 
 
 def fetch_embeddings(view, embedding_tensor: str = "embedding"):
     return view[embedding_tensor].numpy()
 
 
 def get_embedding(embedding, embedding_data, embedding_function=None):
-    if embedding is None and embedding_function is not None:
+    if (
+        embedding is None
+        and embedding_function is not None
+        and embedding_data is not None
+    ):
         embedding = embedding_function(embedding_data)  # type: ignore
 
     if embedding is not None and (
         isinstance(embedding, list) or embedding.dtype != "float32"
     ):
         embedding = np.array(embedding, dtype=np.float32)
```

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.3/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Dict, Callable, List, Union
-from deeplake.core.dataset import Dataset as DeepLakeDataset
-
+import logging
+from typing import Dict, Callable, List, Union, Optional
 
 import numpy as np
 
 from deeplake.core import vectorstore
 from deeplake.core.dataset import Dataset as DeepLakeDataset
 from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
 from deeplake.core.vectorstore.vector_search import filter as filter_utils
@@ -14,31 +13,36 @@
     "compute_engine": vectorstore.indra_vector_search,
     "python": vectorstore.python_vector_search,
     "tensor_db": vectorstore.indra_vector_search,
 }
 
 
 def search(
-    query,
-    logger,
-    filter,
-    query_embedding: Union[List[float], np.ndarray],
-    k: int,
+    k: Optional[int],
     distance_metric: str,
     exec_option: str,
     deeplake_dataset: DeepLakeDataset,
     return_tensors: List[str],
+    query: Optional[str] = None,
+    logger: Optional[logging.Logger] = None,
+    filter: Optional[Union[Dict, Callable]] = None,
+    query_embedding: Optional[Union[List[float], np.ndarray]] = None,
     embedding_tensor: str = "embedding",
     return_view: bool = False,
 ) -> Union[Dict, DeepLakeDataset]:
     """Searching function
     Args:
+        query (Optional[str]) - TQL Query string for direct evaluation, without application of additional filters or vector search.
+        logger (Optional[logging.Logger]) - logger that will print all of the warnings.
         query_embedding (Union[List[float], np.ndarray]) - embedding representation of the query
         k (int) - number of samples to return after searching
         distance_metric (str, optional): Type of distance metric to use for sorting the data. Avaliable options are: "L1", "L2", "COS", "MAX".
+        filter (Union[Dict, Callable], optional): Additional filter evaluated prior to the embedding search.
+                - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
+                - ``Function`` - Any function that is compatible with `deeplake.filter`.
         exec_option (str, optional): Type of query execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
             ``python`` - runs on the client and can be used for any data stored anywhere. WARNING: using this option with big datasets is discouraged, because it can lead to some memory issues.
             ``compute_engine`` - runs on the client and can be used for any data stored in or connected to Deep Lake.
             ``tensor_db`` - runs on the Deep Lake Managed Database and can be used for any data stored in the Deep Lake Managed.
         deeplake_dataset (DeepLakeDataset): deeplake dataset object.
         return_tensors (List[str]): List of tensors to return data for.
         embedding_tensor (str): name of the tensor in the dataset with `htype="embedding"`. Defaults to "embedding".
```

### Comparing `deeplake-3.6.2/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.3/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.3/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.3/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.3/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.3/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.3/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.3/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/dataloader.py` & `deeplake-3.6.3/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.3/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.3/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.3/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/test_query.py` & `deeplake-3.6.3/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.3/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/enterprise/util.py` & `deeplake-3.6.3/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/hooks.py` & `deeplake-3.6.3/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/htype.py` & `deeplake-3.6.3/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.3/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.3/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.3/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.3/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.3/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.3/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/tf/common.py` & `deeplake-3.6.3/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.3/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.3/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.3/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/tests/client_fixtures.py` & `deeplake-3.6.3/deeplake/tests/client_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,9 @@
 
 
 @pytest.fixture(scope="session")
 def hub_cloud_dev_managed_creds_key(request):
     if not is_opt_true(request, HUB_CLOUD_OPT):
         pytest.skip()
 
-    creds_key = os.getenv(ENV_HUB_DEV_MANAGED_CREDS_KEY, "deeplake_tests")
+    creds_key = os.getenv(ENV_HUB_DEV_MANAGED_CREDS_KEY, "aws_creds")
     return creds_key
```

### Comparing `deeplake-3.6.2/deeplake/tests/common.py` & `deeplake-3.6.3/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.3/deeplake/tests/dataset_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 @pytest.fixture
 def hub_cloud_gcs_ds_generator(gcs_path, gcs_creds, hub_cloud_dev_token):
     def generate_hub_cloud_gcs_ds(**kwargs):
         ds = deeplake.dataset(gcs_path, creds=gcs_creds, **kwargs)
         ds.connect(
             org_id=HUB_CLOUD_DEV_USERNAME,
             token=hub_cloud_dev_token,
-            creds_key="DEEPLAKE_GCP",
+            creds_key="gcp_creds",
         )
         return ds
 
     return generate_hub_cloud_gcs_ds
 
 
 @pytest.fixture
```

### Comparing `deeplake-3.6.2/deeplake/tests/path_fixtures.py` & `deeplake-3.6.3/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.3/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/access_method.py` & `deeplake-3.6.3/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/agreement.py` & `deeplake-3.6.3/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/array_list.py` & `deeplake-3.6.3/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.3/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/auto.py` & `deeplake-3.6.3/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/bugout_reporter.py` & `deeplake-3.6.3/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/cache_chain.py` & `deeplake-3.6.3/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/casting.py` & `deeplake-3.6.3/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/check_latest_version.py` & `deeplake-3.6.3/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/chunk_engine.py` & `deeplake-3.6.3/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/class_label.py` & `deeplake-3.6.3/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/compute.py` & `deeplake-3.6.3/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/connect_dataset.py` & `deeplake-3.6.3/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/dataset.py` & `deeplake-3.6.3/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/diff.py` & `deeplake-3.6.3/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/downsample.py` & `deeplake-3.6.3/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/encoder.py` & `deeplake-3.6.3/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/exceptions.py` & `deeplake-3.6.3/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/exif.py` & `deeplake-3.6.3/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/from_tfds.py` & `deeplake-3.6.3/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/htype.py` & `deeplake-3.6.3/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/image.py` & `deeplake-3.6.3/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/invalid_view_op.py` & `deeplake-3.6.3/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/iteration_warning.py` & `deeplake-3.6.3/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/json.py` & `deeplake-3.6.3/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/keys.py` & `deeplake-3.6.3/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/link.py` & `deeplake-3.6.3/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/logging.py` & `deeplake-3.6.3/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/merge.py` & `deeplake-3.6.3/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/modified.py` & `deeplake-3.6.3/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/notebook.py` & `deeplake-3.6.3/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.3/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.3/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.3/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.3/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.3/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/path.py` & `deeplake-3.6.3/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/pretty_print.py` & `deeplake-3.6.3/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/remove_cache.py` & `deeplake-3.6.3/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/scheduling.py` & `deeplake-3.6.3/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/shape_interval.py` & `deeplake-3.6.3/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/spinner.py` & `deeplake-3.6.3/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/split.py` & `deeplake-3.6.3/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/storage.py` & `deeplake-3.6.3/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tag.py` & `deeplake-3.6.3/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tensor_db.py` & `deeplake-3.6.3/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/testing.py` & `deeplake-3.6.3/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_auto.py` & `deeplake-3.6.3/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.3/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.3/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_read.py` & `deeplake-3.6.3/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.3/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_split.py` & `deeplake-3.6.3/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.3/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.3/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/transform.py` & `deeplake-3.6.3/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/version_control.py` & `deeplake-3.6.3/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/util/video.py` & `deeplake-3.6.3/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.3/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake/visualizer/visualizer.py` & `deeplake-3.6.3/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.3/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.2
+Version: 3.6.3
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.3 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.2/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.3/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.2/deeplake.egg-info/requires.txt` & `deeplake-3.6.3/deeplake.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 azure-storage-blob
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
-libdeeplake==0.0.58
+libdeeplake==0.0.59
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -47,15 +47,15 @@
 azure-storage-blob
 
 [dicom]
 nibabel
 pydicom
 
 [enterprise]
-libdeeplake==0.0.58
+libdeeplake==0.0.59
 pyjwt
 
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
```

### Comparing `deeplake-3.6.2/setup.py` & `deeplake-3.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.58"
+    libdeeplake = "libdeeplake==0.0.59"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

