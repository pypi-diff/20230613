# Comparing `tmp/dkist-processing-common-2.8.0rc1.tar.gz` & `tmp/dkist-processing-common-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.8.0rc1.tar", last modified: Mon Jun  5 16:22:54 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc1.tar", last modified: Tue Jun 13 16:54:16 2023, max compression
```

## Comparing `dkist-processing-common-2.8.0rc1.tar` & `dkist-processing-common-3.0.0rc1.tar`

### file list

```diff
@@ -1,122 +1,133 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/139.feature.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/139.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6382 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/dev_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10709 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     7417 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dev_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     5380 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4489 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-05 16:22:54.128769 dkist-processing-common-2.8.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.693971 dkist-processing-common-3.0.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.693971 dkist-processing-common-3.0.0rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.693971 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.693971 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/bytesio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.697971 dkist-processing-common-3.0.0rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.697971 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.697971 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.701971 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     9049 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7966 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/dev_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.701971 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13164 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.701971 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6745 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)    13095 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_dev_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.693971 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-13 16:54:16.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4896 2023-06-13 16:54:16.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 16:54:16.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-13 16:54:16.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-13 16:54:16.000000 dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-13 16:54:16.705972 dkist-processing-common-3.0.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-13 16:54:08.000000 dkist-processing-common-3.0.0rc1/setup.py
```

### Comparing `dkist-processing-common-2.8.0rc1/.gitignore` & `dkist-processing-common-3.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/PKG-INFO` & `dkist-processing-common-3.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.8.0rc1
+Version: 3.0.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.8.0rc1/README.rst` & `dkist-processing-common-3.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Wrappers for all workflow tasks."""
 import json
 import logging
 from abc import ABC
 from io import BytesIO
 from pathlib import Path
+from typing import Any
 from typing import Generator
 from typing import Iterable
 from typing import Type
 from uuid import uuid4
 
 import pkg_resources
 from dkist_processing_core import TaskBase
 
 from dkist_processing_common._util.config import get_config
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.bytes import bytes_encoder
+from dkist_processing_common.codecs.path import path_decoder
 from dkist_processing_common.models.constants import ConstantsBase
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 
 __all__ = ["WorkflowTaskBase", "tag_type_hint"]
 
 logger = logging.getLogger(__name__)
 
@@ -141,46 +144,73 @@
     def pre_run(self) -> None:
         """Execute any pre-task setup required."""
         super().pre_run()
         if self.record_provenance:
             with self.apm_task_step("Record Provenance"):
                 self._record_provenance()
 
-    def read(self, tags: tag_type_hint) -> Generator[Path, None, None]:
-        """Return a generator of file paths associated with the given tags."""
+    def read(
+        self, tags: tag_type_hint, decoder: callable = path_decoder, **decoder_kwargs
+    ) -> Generator[Any, None, None]:
+        """
+        Return a generator corresponding to the files associated with the given tags.
+
+        The type returned is dependent on the given `decoder`.
+
+        Parameters
+        ----------
+        tags
+            Tags to search for. Only files associated with ALL tags will be found.
+
+        decoder
+            Function to convert raw Paths into something more useful. Must accept `Path` as the input type.
+
+        **decoder_kwargs
+            Additional arguments to pass to the `decoder` function.
+        """
         tags = self._parse_tags(tags)
-        return self.scratch.find_all(tags=tags)
+        return (decoder(p, **decoder_kwargs) for p in self.scratch.find_all(tags=tags))
 
     def write(
         self,
-        file_obj: BytesIO | bytes,
+        data: Any,
         tags: tag_type_hint,
         relative_path: Path | str | None = None,
         overwrite: bool = False,
+        encoder: callable = bytes_encoder,
+        **encoder_kwargs,
     ) -> Path:
         """
-        Write a file and tag it using the given tags.
+        Write data to a file and tag it using the given tags.
 
         Parameters
         ----------
-        file_obj
+        data
             The file to be written
+
         tags
             The tags to be associated with the file
+
         relative_path
             The relative path where the file is to be written
+
         overwrite
             Should the file be overwritten if it already exists?
 
+        encoder
+            Function that converts `data` into `bytes`
+
+        **encoder_kwargs
+            Additional arguments to pass to the `encoder` function.
+
         Returns
         -------
         The path for the written file
         """
-        if isinstance(file_obj, BytesIO):
-            file_obj = file_obj.read()
+        file_obj = encoder(data, **encoder_kwargs)
         tags = self._parse_tags(tags)
         relative_path = relative_path or f"{uuid4().hex}.dat"
         relative_path = Path(relative_path)
         self.scratch.write(
             file_obj=file_obj, relative_path=relative_path, tags=tags, overwrite=overwrite
         )
         return relative_path
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/dev_output_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/dev_output_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,82 +2,59 @@
 import logging
 from abc import ABC
 from abc import abstractmethod
 from functools import cached_property
 from pathlib import Path
 
 from dkist_processing_common.models.tags import Tag
-from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.globus import GlobusMixin
 from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
+from dkist_processing_common.tasks.output_data_base import OutputDataBase
+from dkist_processing_common.tasks.output_data_base import TransferDataBase
 
 logger = logging.getLogger(__name__)
 
 
-class DevDataBase(WorkflowTaskBase):
-    """Subclass of WorkflowTaskBase that defines development destination path support."""
-
-    @cached_property
-    def destination_bucket(self) -> str:
-        """Get the destination bucket."""
-        return self.metadata_store_recipe_run_configuration().get("destination_bucket", "dev")
-
-    def format_object_key(self, path: Path) -> str:
-        """
-        Convert output paths into object store keys.
-
-        Parameters
-        ----------
-        path: the Path to convert
-
-        Returns
-        -------
-        formatted path in the object store
-        """
-        object_key = self.destination_folder / Path(path.name)
-        return str(object_key)
-
-    @property
-    def destination_folder(self) -> Path:
-        """Format the destination folder."""
-        dir_name = self.metadata_store_recipe_run_configuration().get("dev_directory_name") or Path(
-            self.constants.dataset_id
-        )
-        return self.destination_root_folder / dir_name
-
-    @property
-    def destination_root_folder(self) -> Path:
-        """Format the destination root folder."""
-        return Path(self.constants.proposal_id)
-
-
-class TransferDevDataBase(DevDataBase, GlobusMixin, ABC):
+class TransferDevDataBase(TransferDataBase, GlobusMixin, ABC):
     """
     Base class for transferring data to a post-run development location.
 
     Provides the basic framework of locating and transferring data, but the specific files to be transferred must be
     identified by subclasses.
 
     Some helper methods that support common conventions are provided:
 
     o `build_debug_frame_transfer_list` - Transfer all frames tagged with DEBUG
 
     o `build_intermediate_frame_transfer_list` - Transfer subsets of frames tagged with INTERMEDIATE
     """
 
-    def run(self) -> None:
+    def transfer_objects(self) -> None:
         """Collect transfer items and send them to Globus for transfer."""
         with self.apm_task_step("Build transfer list"):
             logger.info("Building transfer list")
             transfer_manifest = self.build_transfer_list()
 
         with self.apm_task_step("Send transfer manifest to globus"):
             logger.info("Sending transfer manifests to globus")
             self.transfer_all_dev_frames(transfer_manifest)
 
+    @cached_property
+    def destination_bucket(self) -> str:
+        """Get the destination bucket with a dev default."""
+        return self.metadata_store_recipe_run_configuration().get("destination_bucket", "dev")
+
+    @property
+    def destination_folder(self) -> Path:
+        """Format the destination folder with a parent that can be set by the recipe run configuration."""
+        dir_name = self.metadata_store_recipe_run_configuration().get("dev_directory_name") or Path(
+            self.constants.dataset_id
+        )
+        return self.destination_root_folder / dir_name
+
     @abstractmethod
     def build_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a list of all items on scratch to transfer to the development location."""
         pass
 
     def build_debug_frame_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a transfer list containing all frames tagged with DEBUG."""
@@ -146,14 +123,73 @@
 
         name_parts.sort()
 
         tag_name = "_".join(name_parts)
 
         return f"INTERMEDIATE_TASK-{task}_" + tag_name + ".dat"
 
+    def build_transfer_list_from_tag_lists(
+        self, tag_lists: list[str] | list[list[str]]
+    ) -> list[GlobusTransferItem]:
+        """
+        Build a transfer list containing all files that are tagged with any of the sets of input tags.
+
+        For example, if `tag_lists` is [list1, list2,... listn] then the resulting transfer list will contain:
+
+        ALL(list1) + ALL(list2) + ... + ALL(listn)
+
+        Parameters
+        ----------
+        tag_lists
+            Each element is a list of tags for a single type of file we want to transfer. A single list for a single
+            type of file is also acceptable.
+        """
+        if len(tag_lists) == 0:
+            return []
+
+        if isinstance(tag_lists[0], str):
+            tag_lists = [tag_lists]
+
+        transfer_items = []
+        for tag_set in tag_lists:
+
+            paths = self.read(tags=tag_set)
+            for p in paths:
+                tags = self.tags(p)
+                output_name = Path(self._construct_generic_name_from_tags(tags))
+                destination_object_key = self.format_object_key(output_name)
+                destination_path = Path(self.destination_bucket, destination_object_key)
+                item = GlobusTransferItem(
+                    source_path=p,
+                    destination_path=destination_path,
+                )
+                transfer_items.append(item)
+
+        return list(set(transfer_items))
+
+    def _construct_generic_name_from_tags(self, tags: list[str]) -> str:
+        """
+        Build a sensible filename from an arbitrary set of tags.
+
+        Unlike `_construct_intermediate_name_from_tags` this method doesn't assign any weighting for readability to the
+        input tags. The result is simply `[{TAG_STEM}-{TAG_VALUE}, ...].dat"`.
+        """
+        name_parts = []
+        for t in tags:
+            if t in [Tag.frame()]:
+                continue
+
+            name_parts.append(t.replace("_", "-"))
+
+        name_parts.sort()
+
+        tag_name = "_".join(name_parts)
+
+        return tag_name + ".dat"
+
     def transfer_all_dev_frames(self, transfer_items: list[GlobusTransferItem]) -> None:
         """Send a list of transfer items to Globus for transfer."""
         logger.info(
             f"Preparing globus transfer {len(transfer_items)} items: "
             f"recipe_run_id={self.recipe_run_id}. "
             f"transfer_items={transfer_items[:3]}..."
         )
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,65 @@
 """Task(s) for the transfer and publishing of L1 data from a production run of a processing pipeline."""
 import logging
-from abc import ABC
-from functools import cached_property
 from pathlib import Path
 from typing import Iterable
 
 from dkist_processing_common.models.message import CatalogFrameMessage
 from dkist_processing_common.models.message import CatalogObjectMessage
 from dkist_processing_common.models.message import CreateQualityReportMessage
 from dkist_processing_common.models.tags import Tag
-from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.globus import GlobusMixin
-from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from dkist_processing_common.tasks.mixin.interservice_bus import InterserviceBusMixin
-from dkist_processing_common.tasks.mixin.object_store import ObjectStoreMixin
 
 
 __all__ = [
     "AddDatasetReceiptAccount",
     "PublishCatalogAndQualityMessages",
     "TransferL1Data",
     "L1OutputDataBase",
     "SubmitQuality",
 ]
 
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
+from dkist_processing_common.tasks.output_data_base import OutputDataBase, TransferDataBase
 
 logger = logging.getLogger(__name__)
 
 
-class L1OutputDataBase(WorkflowTaskBase, QualityMixin, ABC):
-    """Subclass of WorkflowTaskBase which encapsulates common level 1 output data methods."""
-
-    @cached_property
-    def destination_bucket(self) -> str:
-        """Get the destination bucket."""
-        return self.metadata_store_recipe_run_configuration().get("destination_bucket", "data")
-
-    def format_object_key(self, path: Path) -> str:
-        """
-        Convert output paths into object store keys.
-
-        Parameters
-        ----------
-        path: the Path to convert
-
-        Returns
-        -------
-        formatted path in the object store
-        """
-        object_key = self.destination_folder / Path(path.name)
-        return str(object_key)
-
-    @property
-    def destination_folder(self) -> Path:
-        """Format the destination folder."""
-        return self.destination_root_folder / Path(self.constants.dataset_id)
-
-    @property
-    def destination_root_folder(self) -> Path:
-        """Format the destination root folder."""
-        return Path(self.constants.proposal_id)
+class L1OutputDataBase(OutputDataBase, QualityMixin):
+    """Subclass of OutputDataBase which encapsulates common level 1 output data methods."""
 
     @property
     def dataset_has_quality_report(self) -> bool:
         """Return True if a quality report has been submitted to the metadata-store."""
         return self.metadata_store_quality_report_exists(dataset_id=self.constants.dataset_id)
 
 
-class TransferL1Data(L1OutputDataBase, GlobusMixin, ObjectStoreMixin):
+class TransferL1Data(TransferDataBase, GlobusMixin):
     """Task class for transferring Level 1 processed data to the object store."""
 
+    def transfer_objects(self):
+        """Transfer movie and L1 output frames."""
+        with self.apm_task_step("Upload movie"):
+            # Movie needs to be transferred separately as the movie headers need to go with it
+            self.transfer_movie()
+
+        with self.apm_task_step("Upload science frames"):
+            self.transfer_output_frames()
+
     def transfer_output_frames(self):
         """Create a Globus transfer for all output data."""
-        science_frame_paths: list[Path] = list(self.read(tags=[Tag.output(), Tag.frame()]))
-        transfer_items = []
-        for p in science_frame_paths:
-            object_key = self.format_object_key(p)
-            destination_path = Path(self.destination_bucket, object_key)
-            item = GlobusTransferItem(
-                source_path=p,
-                destination_path=destination_path,
-            )
-            transfer_items.append(item)
+        transfer_items = self.build_output_frame_transfer_list()
+
         logger.info(
             f"Preparing globus transfer {len(transfer_items)} items: "
             f"recipe_run_id={self.recipe_run_id}. "
             f"transfer_items={transfer_items[:3]}..."
         )
-        # Send transfer
+
         self.globus_transfer_scratch_to_object_store(
             transfer_items=transfer_items,
             label=f"Transfer science frames for recipe_run_id {self.recipe_run_id}",
         )
 
     def transfer_movie(self):
         """Transfer the movie to the object store."""
@@ -115,33 +82,14 @@
         self.object_store_upload_movie(
             movie=movie,
             bucket=self.destination_bucket,
             object_key=movie_object_key,
             content_type="video/mp4",
         )
 
-    def remove_folder_objects(self):
-        """Remove folder objects that would have been added by the Globus transfer."""
-        removed_object_keys = self.object_store_remove_folder_objects(
-            bucket=self.destination_bucket, path=self.destination_root_folder
-        )
-        logger.info(
-            f"Removed folder objects in {self.destination_bucket} bucket. {removed_object_keys=}"
-        )
-
-    def run(self) -> None:
-        """Transfer the data."""
-        with self.apm_task_step("Upload movie"):
-            # Movie needs to be transferred separately as the movie headers need to go with it
-            self.transfer_movie()
-        with self.apm_task_step("Upload science frames"):
-            self.transfer_output_frames()
-        with self.apm_task_step("Remove folder objects"):
-            self.remove_folder_objects()
-
 
 class PublishCatalogAndQualityMessages(L1OutputDataBase, InterserviceBusMixin):
     """Task class for publishing Catalog and Quality Messages."""
 
     def frame_messages(self, paths: Iterable[Path]) -> list[CatalogFrameMessage]:
         """
         Create the frame messages.
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/debug_frame.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/debug_frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Helper to handling saving debug output frames."""
 import logging
 
 import numpy as np
 from astropy.io import fits
 from astropy.io.fits import Header
 
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.models.tags import Tag
 
 logger = logging.getLogger(__name__)
 
 
 class DebugFrameMixin:
     """
@@ -18,27 +19,22 @@
 
     1. They are tagged with DEBUG and thus easily retrievable by downstream tasks.
 
     2. They have expressive file names. These names can either be specified exactly by the user or automatically generated
        based on the other tags.
     """
 
-    @property
-    def _write_debug_switch(self) -> bool:
-        """Read recipe run configuration to determine if debug frames should be written at all."""
-        return self.metadata_store_recipe_run_configuration().get("write_debug_frames", True)
-
     def debug_frame_write_array(
         self,
         array: np.ndarray,
         header: Header | None = None,
         name: str | None = None,
         raw_name: str | None = None,
         tags: list | None = None,
-        overwrite: bool = False,
+        overwrite: bool = True,
     ) -> None:
         """
         Write a single array to a FITS file and tag it with DEBUG.
 
         A header can also be specified.
 
         The on-disk name of the resulting FITS file can be controlled in a few ways:
@@ -47,17 +43,14 @@
           underscores.
 
         * If `raw_name` is provided then the filename will be exactly the value of `raw_name`. Your milage may vary with
           spaces in `raw_name`.
 
         * Otherwise a default name is built from the remaining tags provided in the `tags` argument.
         """
-        if not self._write_debug_switch:
-            return
-
         if raw_name and name:
             raise ValueError("Cannot specify `name` and `raw_name` together.")
 
         default_tags = [Tag.debug(), Tag.frame()]
         if tags:
             # This is not `+=` because that would modify the input tags in place
             tags = tags + default_tags
@@ -66,16 +59,22 @@
 
         if raw_name:
             file_name = raw_name
         else:
             base_name = name or self._construct_base_name_from_tags(tags=tags)
             file_name = self._finalize_file_name(base_name)
 
-        hdul = fits.HDUList([fits.PrimaryHDU(data=array, header=header)])
-        self.fits_data_write(hdu_list=hdul, tags=tags, relative_path=file_name, overwrite=overwrite)
+        self.write(
+            data=array,
+            header=header,
+            tags=tags,
+            encoder=fits_array_encoder,
+            relative_path=file_name,
+            overwrite=overwrite,
+        )
         logger.info(f"Wrote debug file with {tags = } to {file_name}")
 
     def _construct_base_name_from_tags(self, tags: list) -> str:
         """Turn a list of tags into a useful file name."""
         name_parts = []
         for t in tags:
             if t in [Tag.frame(), Tag.debug()]:
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,56 @@
 """Mixin for a WorkflowDataTaskBase subclass which implements fits data retrieval functionality."""
-from io import BytesIO
 from pathlib import Path
 from typing import Generator
 from typing import Iterable
 from typing import Type
 
 from astropy.io import fits
 
+from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.codecs.fits import fits_hdu_decoder
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 
 tag_type_hint = Iterable[str] | str
 
 
 class FitsDataMixin:
     """Mixin for the WorkflowDataTaskBase to support fits r/w operations."""
 
-    def fits_data_read(
-        self, tags: tag_type_hint
-    ) -> Generator[tuple[Path, fits.HDUList], None, None]:
-        """Return a generator of paths and fits HDU lists for input data matching the given tags."""
-        for path in self.read(tags=tags):
-            yield path, self.fits_data_open(path)
-
     def fits_data_read_hdu(
         self, tags: tag_type_hint
-    ) -> Generator[tuple[Path, fits.PrimaryHDU | fits.CompImageHDU], None, None]:
-        """Return a generator of paths and hdus for the input data matching the given tags."""
-        for path, hdul in self.fits_data_read(tags=tags):
-            yield path, self.fits_data_extract_hdu(hdul=hdul)
+    ) -> Generator[fits.PrimaryHDU | fits.CompImageHDU, None, None]:
+        """
+        Return a generator of paths and hdu lists for the input data matching the given tags.
+
+        This method is useful for reading files that lack the header information needed to ingest them as `FitsAccess`
+        objects.
+        """
+        yield from self.read(tags=tags, decoder=fits_hdu_decoder)
 
     def fits_data_read_fits_access(
         self,
         tags: tag_type_hint,
         cls: Type[FitsAccessBase],
         auto_squeeze: bool = True,
     ) -> Generator[FitsAccessBase, None, None]:
         """Return a generator of fits access objects for the input data matching the given tags."""
-        for path, hdu in self.fits_data_read_hdu(tags=tags):
-            yield cls(hdu=hdu, name=str(path), auto_squeeze=auto_squeeze)
-
-    @staticmethod
-    def fits_data_extract_hdu(hdul: fits.HDUList) -> fits.PrimaryHDU | fits.CompImageHDU:
-        """Return the fits hdu associated with the data in the hdu list."""
-        if hdul[0].data is not None:
-            return hdul[0]
-        return hdul[1]
-
-    @staticmethod
-    def fits_data_open(path: str | Path) -> fits.HDUList:
-        """Return the fits object for the given path."""
-        return fits.open(path)
+        yield from self.read(
+            tags=tags, decoder=fits_access_decoder, fits_access_class=cls, auto_squeeze=auto_squeeze
+        )
 
     def fits_data_write(
         self,
         hdu_list: fits.HDUList,
         tags: tag_type_hint,
         relative_path: Path | str | None = None,
         overwrite: bool = False,
     ) -> Path:
         """Write the fits object to a file with the given path and tag with the given tags."""
-        file_obj = BytesIO()
-        hdu_list.writeto(file_obj, checksum=True)
-        file_obj.seek(0)
         return self.write(
-            file_obj=file_obj, tags=tags, relative_path=relative_path, overwrite=overwrite
+            data=hdu_list,
+            tags=tags,
+            relative_path=relative_path,
+            encoder=fits_hdulist_encoder,
+            overwrite=overwrite,
         )
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 class GlobusTransferItem:
     """Dataclass used to support globus transfers."""
 
     source_path: str | Path
     destination_path: str | Path
     recursive: bool = False  # file
 
+    def __hash__(self) -> int:
+        """Hash so we can do set stuff on these items."""
+        return hash((self.source_path, self.destination_path, self.recursive))
+
 
 class GlobusMixin:
     """Mixin to add methods to a Task to support globus transfers."""
 
     @property
     def globus_transfer_client(self) -> TransferClient:
         """Get the globus transfer client, creating it if it doesn't exist."""
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dkist_processing_common.models.graphql import RecipeRunMutation
 from dkist_processing_common.models.graphql import RecipeRunProvenanceMutation
 from dkist_processing_common.models.graphql import RecipeRunQuery
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.graphql import RecipeRunStatusMutation
 from dkist_processing_common.models.graphql import RecipeRunStatusQuery
 from dkist_processing_common.models.graphql import RecipeRunStatusResponse
-from dkist_processing_common.models.json_encoder import QualityReportEncoder
+from dkist_processing_common.models.quality_json_encoders import QualityReportEncoder
 
 
 logger = logging.getLogger(__name__)
 
 input_dataset_part_document_type_hint = list | dict | str | int | float | None
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 
-from dkist_processing_common.models.json_encoder import QualityValueEncoder
+from dkist_processing_common.codecs.json import json_encoder
 from dkist_processing_common.models.quality import ReportMetric
+from dkist_processing_common.models.quality_json_encoders import QualityValueEncoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.quality._metrics import _PolcalQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _SimplePlotQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _SimpleQualityMixin
 from dkist_processing_common.tasks.mixin.quality._metrics import _TableQualityMixin
 
 
@@ -115,16 +116,17 @@
     @staticmethod
     def _format_warnings(warnings: Union[List[str], None]):
         """If warnings is an empty list, change its value to None."""
         return warnings or None
 
     def _record_values(self, values, tags: Union[Iterable[str], str]):
         """Serialize and store distributed quality report values for."""
-        file_obj = json.dumps(values, allow_nan=False, cls=QualityValueEncoder).encode()
-        self.write(file_obj=file_obj, tags=tags)
+        self.write(
+            data=values, tags=tags, encoder=json_encoder, allow_nan=False, cls=QualityValueEncoder
+        )
 
     @staticmethod
     def avg_noise(data) -> float:
         """Estimate the average noise in the image."""
         if len(data.shape) == 2:  # 2D data
             corner_square_length = int(data.shape[0] * 0.2)  # 1/5th of x dimension of array
             corner_square_height = int(data.shape[1] * 0.2)  # 1/5th of y dimension of array
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_debug_frame.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_debug_frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,22 +121,7 @@
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
         new=debug_switch(True),
     )
     with pytest.raises(ValueError):
         debug_task.debug_frame_write_array(array=np.array([1]), name="foo", raw_name="bar")
-
-
-def test_debug_switch_off(debug_task, random_data, mocker):
-    """
-    Given: A task with the DebugFrameMixin and a recipe run configuration that turns off debug frame writing
-    When: Writing a debug array
-    Then: No array is written
-    """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient",
-        new=debug_switch(False),
-    )
-    debug_task.debug_frame_write_array(array=random_data, raw_name="foo.ext")
-    path_list = list(debug_task.read(tags=[Tag.debug()]))
-    assert len(path_list) == 0
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,47 +60,29 @@
     filename = fits_task.scratch.workflow_base_path / "foo.fits"
     hdul.writeto(filename)
     fits_task.tag(filename, [Tag.task("FOO")])
 
     return fits_task, filename
 
 
-@pytest.mark.parametrize("compressed", [pytest.param(False, id="Uncompressed")])
-def test_fits_data_read(fits_task_with_tagged_fits_file, random_data):
-    """
-    Given: A task with the FitsDataMixin and a FITS file in scratch
-    When: Reading a fits file with fits_data_read
-    Then: The correct file is identified and read by astropy.io.fits
-    """
-    task, filename = fits_task_with_tagged_fits_file
-
-    res_list = list(task.fits_data_read(tags=[Tag.task("FOO")]))
-    assert len(res_list) == 1
-    res = res_list[0]
-    assert str(res[0]) == str(filename)
-    assert isinstance(res[1], fits.HDUList)
-    assert len(res[1]) == 1
-    assert np.array_equal(res[1][0].data, random_data)
-
-
 @pytest.mark.parametrize(
     "compressed", [pytest.param(False, id="Uncompressed"), pytest.param(True, id="Compressed")]
 )
 def test_fits_data_read_hdu(fits_task_with_tagged_fits_file, random_data):
     """
     Given: A task with the FitsDataMixin and a FITS file in scratch
     When: Reading a fits file with fits_data_read_hdu
     Then: The correct HDU (i.e., the one with data) is returned
     """
     task, _ = fits_task_with_tagged_fits_file
 
     res_list = list(task.fits_data_read_hdu(tags=[Tag.task("FOO")]))
     assert len(res_list) == 1
     res = res_list[0]
-    assert np.array_equal(res[1].data, random_data)
+    assert np.array_equal(res.data, random_data)
 
 
 @pytest.mark.parametrize(
     "compressed", [pytest.param(False, id="Uncompressed"), pytest.param(True, id="Compressed")]
 )
 def test_fits_data_read_fits_access(fits_task_with_tagged_fits_file, random_data):
     """
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import json
 
 import numpy as np
 import pandas
 import pytest
 
 from dkist_processing_common._util.scratch import WorkflowFileSystem
-from dkist_processing_common.models.json_encoder import QualityValueEncoder
+from dkist_processing_common.codecs.json import json_encoder
+from dkist_processing_common.models.quality_json_encoders import QualityValueEncoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 
 
 class Task(WorkflowTaskBase, QualityMixin):
     def run(self):
@@ -765,26 +766,30 @@
     label = "Beam 1"
     data = {
         "task_type": label,
         "param_names": ["par1", "par2"],
         "param_vals": [0.1, 1.00003456],
     }
 
-    return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
+    return data, label
 
 
 def test_polcal_build_constant_parameter_values(quality_task, polcal_constant_params_json):
     """
     Given: A task with the PolcalQualityMixin
     When: Building the constant parameter QA metric
     Then: The correct dictionary is returned
     """
     data, label = polcal_constant_params_json
     quality_task.write(
-        data, tags=[Tag.quality("POLCAL_CONSTANT_PAR_VALS"), Tag.quality_task(label)]
+        data,
+        tags=[Tag.quality("POLCAL_CONSTANT_PAR_VALS"), Tag.quality_task(label)],
+        encoder=json_encoder,
+        allow_nan=False,
+        cls=QualityValueEncoder,
     )
     metric = quality_task.quality_build_polcal_constant_parameter_values(label=label)
 
     assert metric["name"] == f"PolCal Constant Values in Calibration Unit Fit"
     metric_table = metric["table_data"]["rows"]
     assert len(metric_table) == 3  # 2 rows + one for header
     assert metric_table[1] == ["par1", f"{0.1: 9.6f}"]
@@ -801,25 +806,31 @@
         "param_init_vals": [0.1, 0.2, 0.3],
         "param_fit_vals": [1, 2.222, 0.33],
         "param_diffs": [4, 1.1, 0.2],
         "param_ratios": [3, 2, "-"],
         "warnings": ["A thing is bad"],
     }
 
-    return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
+    return data, label
 
 
 def test_polcal_build_global_parameter_values(quality_task, polcal_global_params_json):
     """
     Given: A task with the PolcalQualityMixin
     When: Building the global parameter QA metric
     Then: The correct dictionary is returned
     """
     data, label = polcal_global_params_json
-    quality_task.write(data, tags=[Tag.quality("POLCAL_GLOBAL_PAR_VALS"), Tag.quality_task(label)])
+    quality_task.write(
+        data,
+        tags=[Tag.quality("POLCAL_GLOBAL_PAR_VALS"), Tag.quality_task(label)],
+        encoder=json_encoder,
+        allow_nan=False,
+        cls=QualityValueEncoder,
+    )
     metric = quality_task.quality_build_polcal_global_parameter_values(label=label)
 
     assert metric["name"] == f"PolCal Global Calibration Unit Fit - {label}"
     assert metric["warnings"] == ["A thing is bad"]
     metric_table = metric["table_data"]["rows"]
     assert len(metric_table) == 4  # 3 rows + one for header
     assert metric_table[1] == ["par1", True, f"{0.1: 6.2f}", f"{1: 6.2f}", f"{4: .2e}", f"{3: .2e}"]
@@ -847,25 +858,31 @@
         "free_param_dict": {
             "I_sys_CS00_step00": {"fit_values": [1, 2, 3.0], "init_value": 0.3},
             "I_sys_CS00_step01": {"fit_values": [10, 20, 30.0], "init_value": 0.33},
             "param_X": {"fit_values": [5, 6, 7.0], "init_value": 99},
         },
     }
 
-    return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
+    return data, label
 
 
 def test_polcal_build_local_parameter_values(quality_task, polcal_local_params_json):
     """
     Given: A task with the PolcalQualityMixin
     When: Building the local parameter QA metric
     Then: The correct dictionary is returned
     """
     data, label = polcal_local_params_json
-    quality_task.write(data, tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)])
+    quality_task.write(
+        data,
+        tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)],
+        encoder=json_encoder,
+        allow_nan=False,
+        cls=QualityValueEncoder,
+    )
     metric = quality_task.quality_build_polcal_local_parameter_values(label=label)
 
     assert metric["name"] == f"PolCal Local Bin Fits - {label}"
     modmat_data = metric["modmat_data"]
     assert modmat_data["modmat_list"] == [[[1, 2.0], [2.0, 3.0]], [[10.0, 20.0], [20.0, 30.0]]]
     hist_list = metric["histogram_data"]
     assert isinstance(hist_list, list)
@@ -888,25 +905,31 @@
         "bin_1_str": "2 spatial",
         "bin_2_str": "3 radical",
         "total_bins": 6,
         "residual_json": json.dumps("Just some garbage"),
         "red_chi_list": [1.0, 2.0, 3.0],
     }
 
-    return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
+    return data, label
 
 
 def test_polcal_build_fit_residuals(quality_task, polcal_fit_residuals_json):
     """
     Given: A task with the PolcalQualityMixin
     When: Building the fit residual QA metric
     Then: The correct dictionary is returned
     """
     data, label = polcal_fit_residuals_json
-    quality_task.write(data, tags=[Tag.quality("POLCAL_FIT_RESIDUALS"), Tag.quality_task(label)])
+    quality_task.write(
+        data,
+        tags=[Tag.quality("POLCAL_FIT_RESIDUALS"), Tag.quality_task(label)],
+        encoder=json_encoder,
+        allow_nan=False,
+        cls=QualityValueEncoder,
+    )
     metric = quality_task.quality_build_polcal_fit_residuals(label=label)
 
     assert metric["name"] == f"PolCal Fit Residuals - {label}"
 
     chisq_data = metric["histogram_data"]
     assert chisq_data["xlabel"] == "Reduced Chisq"
     assert chisq_data["series_data"] == {"Red chisq": [1.0, 2.0, 3.0]}
@@ -926,23 +949,29 @@
         "bin_1_str": "2 spatial",
         "bin_2_str": "3 radical",
         "total_bins": 6,
         "efficiency_list": [[1.0, 2.0], [2.0, 3.0]],
         "warnings": [],
     }
 
-    return json.dumps(data, allow_nan=False, cls=QualityValueEncoder).encode(), label
+    return data, label
 
 
 def test_polcal_build_efficiency(quality_task, polcal_efficiency_json):
     """
     Given: A task with the PolcalQualityMixin
     When: Building the modulation efficiency QA metric
     Then: The correct dictionary is returned
     """
     data, label = polcal_efficiency_json
-    quality_task.write(data, tags=[Tag.quality("POLCAL_EFFICIENCY"), Tag.quality_task(label)])
+    quality_task.write(
+        data,
+        tags=[Tag.quality("POLCAL_EFFICIENCY"), Tag.quality_task(label)],
+        encoder=json_encoder,
+        allow_nan=False,
+        cls=QualityValueEncoder,
+    )
     metric = quality_task.quality_build_polcal_efficiency(label=label)
 
     assert metric["name"] == f"PolCal Modulation Efficiency - {label}"
     efficiency_data = metric["efficiency_data"]
     assert efficiency_data["efficiency_list"] == [[1.0, 2.0], [2.0, 3.0]]
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,54 +91,37 @@
     tagged_filepaths = list(task.read(tags=tag_object))
     assert len(tagged_filepaths) == number_of_files
     for tagged_filepath in tagged_filepaths:
         assert tagged_filepath.name in filenames
         assert tagged_filepath.exists()
 
 
-def test_valid_write_with_bytes(workflow_data_task):
+def test_valid_write(workflow_data_task):
     """
     Given: a WorkflowDataTask
     When: writing a bytes object to disk
     Then: the file is on disk and correctly tagged
     """
     task, _, _, _, _ = workflow_data_task
     relative_path = "bytes_path"
-    task.write(file_obj=bytes("abcdefg", "utf-8"), tags="BYTES_OBJECT", relative_path=relative_path)
+    task.write(data=bytes("abcdefg", "utf-8"), tags="BYTES_OBJECT", relative_path=relative_path)
     assert (task.scratch.workflow_base_path / relative_path).exists()
     assert len(list(task.read(tags="BYTES_OBJECT"))) == 1
 
 
-def test_valid_write_with_bytesio(workflow_data_task):
-    """
-    Given: a WorkflowDataTask
-    When: writing a BytesIO object to disk
-    Then: the file is on disk and correctly tagged
-    """
-    task, _, _, _, _ = workflow_data_task
-    relative_path = "bytesio_path"
-    task.write(
-        file_obj=BytesIO(bytes("abcdefg", "utf-8")),
-        tags="BYTESIO_OBJECT",
-        relative_path=relative_path,
-    )
-    assert (task.scratch.workflow_base_path / relative_path).exists()
-    assert len(list(task.read(tags="BYTESIO_OBJECT"))) == 1
-
-
 def test_write_tags_is_none(workflow_data_task):
     """
     Given: a WorkflowDataTask
     When: writing a file to disk with tags=None
     Then: a ValueError is raised
     """
     task, _, _, _, _ = workflow_data_task
     relative_path = "bytesio_path"
     with pytest.raises(TypeError):
-        task.write(file_obj=bytes("abcdefg", "utf-8"), tags=None, relative_path=relative_path)
+        task.write(data=bytes("abcdefg", "utf-8"), tags=None, relative_path=relative_path)
 
 
 def test_read_nonexistent_tag(workflow_data_task):
     """
     Given: a WorkflowDataTask
     When: reading from a tag that doesn't exist
     Then: an empty generator is returned
@@ -217,17 +200,15 @@
             inputDatasetId=1234,
             isTaskManual=is_task_manual,
             recipeRunId=self.recipe_run_id,
             taskName=self.task_name,
             libraryVersions=library_versions,
             workflowVersion=self.workflow_version,
         )
-        self.write(
-            file_obj=BytesIO(bytes(json.dumps(asdict(params)), "utf-8")), tags=["TEST_PROVENANCE"]
-        )
+        self.write(data=bytes(json.dumps(asdict(params)), "utf-8"), tags=["TEST_PROVENANCE"])
 
 
 @pytest.fixture(scope="function")
 def provenance_task(tmp_path, recipe_run_id):
     with ProvenanceTask(
         recipe_run_id=recipe_run_id,
         workflow_name="workflow_name",
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.8.0rc1
+Version: 3.0.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,47 @@
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
 changelog/139.feature.2.rst
 changelog/139.feature.rst
+changelog/140.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
 dkist_processing_common/_util/__init__.py
 dkist_processing_common/_util/config.py
 dkist_processing_common/_util/constants.py
 dkist_processing_common/_util/dkist_location.py
 dkist_processing_common/_util/graphql.py
 dkist_processing_common/_util/scratch.py
 dkist_processing_common/_util/tags.py
+dkist_processing_common/codecs/__init__.py
+dkist_processing_common/codecs/bytes.py
+dkist_processing_common/codecs/bytesio.py
+dkist_processing_common/codecs/fits.py
+dkist_processing_common/codecs/json.py
+dkist_processing_common/codecs/path.py
+dkist_processing_common/codecs/str.py
 dkist_processing_common/fonts/Lato-Regular.ttf
 dkist_processing_common/fonts/__init__.py
 dkist_processing_common/models/__init__.py
 dkist_processing_common/models/constants.py
 dkist_processing_common/models/fits_access.py
 dkist_processing_common/models/flower_pot.py
 dkist_processing_common/models/graphql.py
-dkist_processing_common/models/json_encoder.py
 dkist_processing_common/models/message.py
 dkist_processing_common/models/parameters.py
 dkist_processing_common/models/quality.py
+dkist_processing_common/models/quality_json_encoders.py
 dkist_processing_common/models/tags.py
 dkist_processing_common/models/wavelength.py
 dkist_processing_common/parsers/__init__.py
 dkist_processing_common/parsers/cs_step.py
 dkist_processing_common/parsers/dsps_repeat.py
 dkist_processing_common/parsers/experiment_id_bud.py
 dkist_processing_common/parsers/id_bud.py
@@ -51,14 +59,15 @@
 dkist_processing_common/parsers/time.py
 dkist_processing_common/parsers/unique_bud.py
 dkist_processing_common/tasks/__init__.py
 dkist_processing_common/tasks/assemble_movie.py
 dkist_processing_common/tasks/base.py
 dkist_processing_common/tasks/dev_output_data.py
 dkist_processing_common/tasks/l1_output_data.py
+dkist_processing_common/tasks/output_data_base.py
 dkist_processing_common/tasks/parse_l0_input_data.py
 dkist_processing_common/tasks/quality_metrics.py
 dkist_processing_common/tasks/teardown.py
 dkist_processing_common/tasks/transfer_input_data.py
 dkist_processing_common/tasks/write_l1.py
 dkist_processing_common/tasks/mixin/__init__.py
 dkist_processing_common/tasks/mixin/debug_frame.py
@@ -71,25 +80,26 @@
 dkist_processing_common/tasks/mixin/quality/__init__.py
 dkist_processing_common/tasks/mixin/quality/_base.py
 dkist_processing_common/tasks/mixin/quality/_metrics.py
 dkist_processing_common/tests/__init__.py
 dkist_processing_common/tests/conftest.py
 dkist_processing_common/tests/test_assemble_movie.py
 dkist_processing_common/tests/test_base.py
+dkist_processing_common/tests/test_codecs.py
 dkist_processing_common/tests/test_constants.py
 dkist_processing_common/tests/test_cs_step.py
 dkist_processing_common/tests/test_debug_frame.py
 dkist_processing_common/tests/test_dev_output_data.py
 dkist_processing_common/tests/test_dkist_location.py
 dkist_processing_common/tests/test_fits.py
 dkist_processing_common/tests/test_fits_access.py
 dkist_processing_common/tests/test_fits_flowers.py
 dkist_processing_common/tests/test_flower_pot.py
 dkist_processing_common/tests/test_input_dataset.py
-dkist_processing_common/tests/test_l1_output_data_base.py
+dkist_processing_common/tests/test_output_data_base.py
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
 dkist_processing_common/tests/test_publish_catalog_messages.py
 dkist_processing_common/tests/test_quality.py
 dkist_processing_common/tests/test_quality_mixin.py
 dkist_processing_common/tests/test_scratch.py
 dkist_processing_common/tests/test_tags.py
```

### Comparing `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/docs/Makefile` & `dkist-processing-common-3.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/docs/conf.py` & `dkist-processing-common-3.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/docs/make.bat` & `dkist-processing-common-3.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/pyproject.toml` & `dkist-processing-common-3.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.8.0rc1/setup.cfg` & `dkist-processing-common-3.0.0rc1/setup.cfg`

 * *Files identical despite different names*

