# Comparing `tmp/debater_python_api-5.0.2.tar.gz` & `tmp/debater_python_api-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-5.0.2.tar", last modified: Mon Jun 12 07:55:17 2023, max compression
+gzip compressed data, was "debater_python_api-5.0.3.tar", last modified: Tue Jun 13 07:10:00 2023, max compression
```

## Comparing `debater_python_api-5.0.2.tar` & `debater_python_api-5.0.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.404361 debater_python_api-5.0.2/
--rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/LICENSE
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-12 07:55:17.404159 debater_python_api-5.0.2/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/README.md
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.388774 debater_python_api-5.0.2/debater_python_api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.389747 debater_python_api-5.0.2/debater_python_api/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.393774 debater_python_api-5.0.2/debater_python_api/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/
--rw-r--r--   0 lilache    (501) staff       (20)      478 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
--rw-r--r--   0 lilache    (501) staff       (20)    38133 2023-06-11 20:39:30.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsResult.py
--rw-r--r--   0 lilache    (501) staff       (20)    12403 2023-06-11 13:30:46.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/docx_generator.py
--rw-r--r--   0 lilache    (501) staff       (20)    16293 2023-06-11 10:50:55.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/graph_generator.py
--rw-r--r--   0 lilache    (501) staff       (20)     4239 2023-06-08 21:02:49.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/utils.py
--rw-r--r--   0 lilache    (501) staff       (20)     6969 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    39175 2023-06-12 07:51:28.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395440 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3263 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395625 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.396760 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.400656 debater_python_api-5.0.2/debater_python_api/examples/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1204 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401150 debater_python_api-5.0.2/debater_python_api/examples/resources/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401331 debater_python_api-5.0.2/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401759 debater_python_api-5.0.2/debater_python_api/examples/usecases/
--rw-r--r--   0 lilache    (501) staff       (20)     4943 2023-06-12 07:54:01.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401931 debater_python_api-5.0.2/debater_python_api/integration_tests/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.402042 debater_python_api-5.0.2/debater_python_api/integration_tests/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.402939 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)     2708 2023-05-22 15:52:47.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 lilache    (501) staff       (20)    11791 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.403790 debater_python_api-5.0.2/debater_python_api/utils/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/general_utils.py
--rw-r--r--   0 lilache    (501) staff       (20)      604 2023-05-22 16:30:58.000000 debater_python_api-5.0.2/debater_python_api/utils/kp_analysis_conf.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.389473 debater_python_api-5.0.2/debater_python_api.egg-info/
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)     4041 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 lilache    (501) staff       (20)        1 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 lilache    (501) staff       (20)       87 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 lilache    (501) staff       (20)       19 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 lilache    (501) staff       (20)      879 2023-06-12 07:32:46.000000 debater_python_api-5.0.2/pyproject.toml
--rw-r--r--   0 lilache    (501) staff       (20)       38 2023-06-12 07:55:17.404409 debater_python_api-5.0.2/setup.cfg
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.434270 debater_python_api-5.0.3/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/LICENSE
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-13 07:10:00.434076 debater_python_api-5.0.3/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/README.md
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.422852 debater_python_api-5.0.3/debater_python_api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.423724 debater_python_api-5.0.3/debater_python_api/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.425837 debater_python_api-5.0.3/debater_python_api/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426558 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      478 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    37388 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsResult.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    12349 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/docx_generator.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    16293 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/graph_generator.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4239 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6969 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    38464 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426802 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3263 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426950 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.427856 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430252 debater_python_api-5.0.3/debater_python_api/examples/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1204 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430708 debater_python_api-5.0.3/debater_python_api/examples/resources/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430860 debater_python_api-5.0.3/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431260 debater_python_api-5.0.3/debater_python_api/examples/usecases/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431401 debater_python_api-5.0.3/debater_python_api/integration_tests/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431521 debater_python_api-5.0.3/debater_python_api/integration_tests/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.433013 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11791 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.433821 debater_python_api-5.0.3/debater_python_api/utils/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/kp_analysis_conf.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.423497 debater_python_api-5.0.3/debater_python_api.egg-info/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4041 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       96 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      895 2023-06-13 07:07:43.000000 debater_python_api-5.0.3/pyproject.toml
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-06-13 07:10:00.434321 debater_python_api-5.0.3/setup.cfg
```

### Comparing `debater_python_api-5.0.2/LICENSE` & `debater_python_api-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/PKG-INFO` & `debater_python_api-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater_python_api
-Version: 5.0.2
+Version: 5.0.3
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsResult.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsResult.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,81 +220,74 @@
         #can create more conversion methods for future json_result versions...
         raise KpsIllegalInputException(f"Unsupported results version old: {old_version}, new: {new_version}. "
                                        f"Supported: old = 1.0, new = 2.0")
 
     def generate_docx_report(self, output_dir: str, result_name: str,
                              n_matches_in_docx: Optional[int] = 50,
                              include_match_score_in_docx: Optional[bool] = False,
-                             min_n_matches_in_docx: Optional[int] = 5,
                              kp_id_to_hierarchical_data=None):
         """
         creates <output_dir>/<result_name>_hierarchical.docx: This Microsoft Word document shows the key point hierarchy and matching sentences
         as a user-friendly report.
         :param output_dir: path to output directory
         :param result_name: name of the results to appear in the output files.
         :param n_matches_in_docx: number of top matches to write in the textual summary (docx file). Pass None for all matches.
         :param include_match_score_in_docx: when set to true, the match score between the sentence and the key point is added.
-        :param min_n_matches_in_docx: remove key points with less than min_n_matches_in_docx matching sentences.
         :param kp_id_to_hierarchical_data: optional, should be set to None.
         """
         if not kp_id_to_hierarchical_data:
             kp_id_to_hierarchical_data = self.kp_id_to_hierarchical_data
         docx_file = os.path.join(output_dir, f'{result_name}_hierarchical.docx')
         meta_data = self.result_json["job_metadata"]
         save_hierarchical_graph_data_to_docx(full_result_df=self.result_df, kp_id_to_data=kp_id_to_hierarchical_data,
                                              result_filename=docx_file, meta_data=meta_data, n_matches=n_matches_in_docx,
                                              include_match_score=include_match_score_in_docx,
-                                             min_n_matches=min_n_matches_in_docx)
+                                             min_n_matches=0)
 
     def generate_docx_report_using_given_tree(self, full_results,
                                               output_dir, result_name, n_top_matches_in_graph=20,
-                                              n_matches_in_docx=50, include_match_score_in_docx=False,
-                                              min_n_matches_in_docx=5):
+                                              n_matches_in_docx=50, include_match_score_in_docx=False):
         '''
         Create hierarchical result for this result, using a precalculated hierarchical results.
         This is useful when we first create results using the whole data, and then want to calculate the
         hierarchical result of its subset while considering the already existing key points and hierarchy generated over the whole data.
         For example, when we have a large survey, we can first run over the entire data to create a hierarchical
         representation of the full results. Then when we want to evaluate a subset of the survey we can run over a subset of
         the survey using the same key points precomputed in the full survey. Then we create its hierarchical
         representation using the hierarchy of the full survey.
         :param full_results: KpsResult over the full data.
         :param output_dir: path to output directory
         :param result_name: name of the results to appear in the output files.
         :param n_top_matches_in_graph : optional, number of top matches to add to the graph_data file.
         :param n_matches_in_docx: optional, number of top matches to write in the textual summary (docx file). Pass None for all matches.
         :param include_match_score_in_docx: optional, when set to true, the match score between the sentence and the key point is added.
-        :param min_n_matches_in_docx: optional, remove key points with less than min_n_matches_in_docx matching sentences.
         '''
         graph_full_data = create_graph_data(full_results.result_df, full_results._get_number_of_unique_sentences())
         hierarchical_graph_full_data = graph_data_to_hierarchical_graph_data(graph_data=graph_full_data)
 
         new_hierarchical_graph_data = get_hierarchical_graph_from_tree_and_subset_results(
             hierarchical_graph_full_data,
             self.result_df, self.filter_min_relations, n_top_matches_in_graph)
 
         new_kp_id_to_hierarchical_data = get_hierarchical_kps_data(self.result_df, new_hierarchical_graph_data, self.filter_min_relations)
         self.generate_docx_report(output_dir, result_name,
                             n_matches_in_docx=n_matches_in_docx,
                             include_match_score_in_docx=include_match_score_in_docx,
-                            min_n_matches_in_docx=min_n_matches_in_docx,
                             kp_id_to_hierarchical_data = new_kp_id_to_hierarchical_data)
 
     def export_to_all_outputs(self, output_dir: str, result_name: str,
                               n_matches_in_docx: Optional[int] = 50,
                               include_match_score_in_docx: Optional[bool] = False,
-                              min_n_matches_in_docx: Optional[int] = 5,
                               ):
         """
         Generates all the kps available output types.
         :param output_dir: path to output directory
         :param result_name: name of the results to appear in the output files.
         :param n_matches_in_docx: optional, number of top matches to write in the textual summary (docx file). Pass None for all matches.
         :param include_match_score_in_docx: optional, when set to true, the match score between the sentence and the key point is added.
-        :param min_n_matches_in_docx: optional, remove key points with less than min_n_matches_in_docx matching sentences.
         Creates 3 outout files:
              * <ouput_dir>/<result_name>.csv : full results as csv .
              * <ouput_dir>/<result_name>_kps_summary.csv : summary results as csv.
              *  <result_file>_hierarchical.docx: This Microsoft Word document shows the key point hierarchy and matching sentences
             as a user-friendly report.
         """
 
@@ -302,16 +295,15 @@
         write_df_to_file(self.result_df, result_file)
 
         summary_file = result_file.replace(".csv", "_kps_summary.csv")
         write_df_to_file(self.summary_df, summary_file)
 
         self.generate_docx_report(output_dir, result_name,
                                   n_matches_in_docx=n_matches_in_docx,
-                                  include_match_score_in_docx=include_match_score_in_docx,
-                                  min_n_matches_in_docx=min_n_matches_in_docx)
+                                  include_match_score_in_docx=include_match_score_in_docx)
 
     def print_result(self, n_sentences_per_kp: int, title: str, n_top_kps:Optional[int]=None):
         '''
         Prints the key point summarization result to console. For each kp, display the number of matched comments, stance
         and top matching sentences.
         :param n_sentences_per_kp: number of top matched sentences to display for each key point
         :param title: title to print for the summarization
```

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/docx_generator.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/docx_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     dicts_not_none = list(filter(lambda r: r["kp"] != "none", dicts))
     n_matches_comments = len(set([d["comment_id"] for d in dicts_not_none])) # Todo: this includes matches to smaller, filtered kps!
     rate_matched_comments = 100*n_matches_comments / n_total_comments
 
     heading = document.add_heading('Data Statistics', 1)
     set_heading(heading)
     s = f'Analyzed {n_total_comments} comments with {n_total_sentences} sentences.\n' \
-        f'Identified {n_kps} key points with at least {min_n_matches or 1} matching sentences.\n' \
+        f'Identified {n_kps} key points.\n' \
         f'{int(np.round(rate_matched_comments, 0))}% of the comments were matched to at least one key point.\n'
     for stance in ["pro","con"]:
         if stance in stances:
             stance_str = get_stance_to_stance_str(stance).lower()
             n_kps_stance = len(list(filter(lambda kp_id:kp_id_to_data[kp_id].get("kp_stance")==stance, kp_id_to_data)))
             kp_stance_str = f"of {n_kps_stance} {stance_str} key points." if len(stances) > 1 else "key point."
```

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/graph_generator.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/graph_generator.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/utils.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -341,34 +341,26 @@
         if description is not None:
             body['description'] = description
 
         res = self._post(url=self.host + kp_extraction_endpoint, body=body)
         logging.info(f'started a kp summarization job - domain: {domain}, stance: {stance}, run_params: {run_params}, {"" if description is None else f"description: {description}, "}job_id: {res["job_id"]}')
         return KpsJobFuture(self, res['job_id'])
 
-    def get_kps_job_status(self, job_id: str, top_k_kps: Optional[int] = None,
-                                     top_k_sentences_per_kp: Optional[int] = None):
+    def get_kps_job_status(self, job_id: str):
         '''
         Checks for the status of a key point summarization job. It returns a json with a 'status' key that can have one of the following values: PENDING, PROCESSING, DONE, CANCELED, ERROR
         If the status is PROCESSING, it also has a 'progress' key that describes the calculation progress.
         If the status is DONE, it also has a 'result' key that has the result_json, that can be converted into KpsResults using KpsResult.create_from_result_json(result_json)
         If the status is ERROR, it also has a 'error_msg' key that has the description of the error.
         :param job_id: the job_id (can be found in the future returned when the job was started or in the user-report)
         :param top_k_kps: use this parameter to truncate the result json to have only the top K key points.
         :param top_k_sentences_per_kp: use this parameter to truncate the result json to have only the top K matched sentences per key point.
         :return: see description above.
         '''
         params = {'job_id': job_id}
-
-        if top_k_kps is not None:
-            params['top_k_kps'] = top_k_kps
-
-        if top_k_sentences_per_kp is not None:
-            params['top_k_sentences_per_kp'] = top_k_sentences_per_kp
-
         return self._get(self.host + kp_extraction_endpoint, params, timeout=180)
 
     def cancel_kps_job(self, job_id: str):
         '''
         Stops a running key point summarization job.
         :param job_id: the job_id
         :return: the request's response
@@ -604,32 +596,30 @@
 
     def get_job_id(self) -> str:
         '''
         :return: the job_id
         '''
         return self.job_id
 
-    def get_result(self, top_k_kps: Optional[int] = None, top_k_sentences_per_kp: Optional[int] = None,
+    def get_result(self,
                    dont_wait: bool = False, wait_secs: Optional[int] = None, polling_timeout_secs: Optional[int] = None,
                    high_verbosity: bool = True) -> KpsResult:
         '''
         Retreives the job's result. This method polls and waits till the job is done and the result is available.
-        :param top_k_kps: use this parameter to truncate the result json to have only the top K key points.
-        :param top_k_sentences_per_kp: use this parameter to truncate the result json to have only the top K matched sentences per key point.
         :param dont_wait: when True, tries to get the result once and returns it if it's available, otherwise returns None.
         :param wait_secs: limit the waiting time (in seconds).
         :param polling_timeout_secs: sets the time to wait before polling again (in seconds). The default is 30 seconds.
         :param high_verbosity: set to False to reduce the number of messages printed to the logger.
         :return: the KpsResult object or throws an exception if an error occurs or if the job was canceled.
         '''
         start_time = time.time()
 
         do_again = True
         while do_again:
-            result = self.client.get_kps_job_status(self.job_id, top_k_kps=top_k_kps, top_k_sentences_per_kp=top_k_sentences_per_kp)
+            result = self.client.get_kps_job_status(self.job_id)
             if result['status'] == 'PENDING':
                 if high_verbosity:
                     logging.info('job_id %s is pending' % self.job_id)
             elif result['status'] == 'PROCESSING':
                 if high_verbosity:
                     progress = result['progress']
                     logging.info('job_id %s is running, progress: %s' % (self.job_id, progress))
```

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-5.0.3/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/debater_api.py` & `debater_python_api-5.0.3/debater_python_api/api/debater_api.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/clustering_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/embedding_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-5.0.3/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/keypoints_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/keypoints_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/pro_con_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/resources/arguments.py` & `debater_python_api-5.0.3/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-5.0.3/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/run_all_services.py` & `debater_python_api-5.0.3/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-5.0.3/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-5.0.3/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-5.0.3/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/examples/usecases/survey.py` & `debater_python_api-5.0.3/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-5.0.3/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/utils/general_utils.py` & `debater_python_api-5.0.3/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-5.0.3/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-5.0.3/debater_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater-python-api
-Version: 5.0.2
+Version: 5.0.3
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.2/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-5.0.3/debater_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.2/pyproject.toml` & `debater_python_api-5.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "5.0.2"
+version = "5.0.3"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
@@ -20,15 +20,16 @@
     "prettytable",
     "scikit-learn",
     "matplotlib",
     "numpy",
     "pandas",
     "spacy",
     "PyHamcrest",
-    "python-docx"
+    "python-docx",
+    "networkx"
 ]
 requires-python = ">=3.6"
 
 #[project.optional-dependencies]
 #dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 #[project.urls]
```

