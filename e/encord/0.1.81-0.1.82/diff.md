# Comparing `tmp/encord-0.1.81.tar.gz` & `tmp/encord-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.81.tar", max compression
+gzip compressed data, was "encord-0.1.82.tar", max compression
```

## Comparing `encord-0.1.81.tar` & `encord-0.1.82.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    11330 2023-06-07 16:04:02.858859 encord-0.1.81/LICENSE
--rw-r--r--   0        0        0     2037 2023-06-07 16:04:02.858859 encord-0.1.81/README.md
--rw-r--r--   0        0        0       84 2023-06-07 16:04:02.858859 encord-0.1.81/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-06-07 16:04:02.878859 encord-0.1.81/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-06-07 16:04:02.878859 encord-0.1.81/encord/_version.py
--rw-r--r--   0        0        0    49810 2023-06-07 16:04:02.878859 encord-0.1.81/encord/client.py
--rw-r--r--   0        0        0    10843 2023-06-07 16:04:02.878859 encord-0.1.81/encord/configs.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-06-07 16:04:02.878859 encord-0.1.81/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-06-07 16:04:02.878859 encord-0.1.81/encord/dataset.py
--rw-r--r--   0        0        0     6351 2023-06-07 16:04:02.878859 encord-0.1.81/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/limits.py
--rw-r--r--   0        0        0     7928 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-06-07 16:04:02.878859 encord-0.1.81/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-06-07 16:04:02.882859 encord-0.1.81/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-06-07 16:04:02.882859 encord-0.1.81/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/classification.py
--rw-r--r--   0        0        0    31614 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/frames.py
--rw-r--r--   0        0        0    21035 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   142513 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/project.py
--rw-r--r--   0        0        0     1289 2023-06-07 16:04:02.882859 encord-0.1.81/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-06-07 16:04:02.882859 encord-0.1.81/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-06-07 16:04:02.882859 encord-0.1.81/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32800 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/ontology.py
--rw-r--r--   0        0        0     8885 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-06-07 16:04:02.886859 encord-0.1.81/encord/orm/workflow.py
--rw-r--r--   0        0        0    39431 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-06-07 16:04:02.886859 encord-0.1.81/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    28768 2023-06-07 16:04:02.886859 encord-0.1.81/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-06-07 16:04:02.886859 encord-0.1.81/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1944 2023-06-07 16:04:02.886859 encord-0.1.81/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.81/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-06-13 15:08:20.190491 encord-0.1.82/LICENSE
+-rw-r--r--   0        0        0     2037 2023-06-13 15:08:20.190491 encord-0.1.82/README.md
+-rw-r--r--   0        0        0       84 2023-06-13 15:08:20.190491 encord-0.1.82/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-13 15:08:20.206491 encord-0.1.82/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-13 15:08:20.206491 encord-0.1.82/encord/_version.py
+-rw-r--r--   0        0        0    49810 2023-06-13 15:08:20.206491 encord-0.1.82/encord/client.py
+-rw-r--r--   0        0        0    10843 2023-06-13 15:08:20.206491 encord-0.1.82/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-06-13 15:08:20.206491 encord-0.1.82/encord/dataset.py
+-rw-r--r--   0        0        0     6351 2023-06-13 15:08:20.206491 encord-0.1.82/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/limits.py
+-rw-r--r--   0        0        0     7928 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/classification.py
+-rw-r--r--   0        0        0    31614 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/frames.py
+-rw-r--r--   0        0        0    21035 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   142839 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/project.py
+-rw-r--r--   0        0        0     1289 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-06-13 15:08:20.206491 encord-0.1.82/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32800 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8885 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/workflow.py
+-rw-r--r--   0        0        0    39431 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    28768 2023-06-13 15:08:20.210491 encord-0.1.82/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1945 2023-06-13 15:08:20.210491 encord-0.1.82/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 encord-0.1.82/PKG-INFO
```

### Comparing `encord-0.1.81/LICENSE` & `encord-0.1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/README.md` & `encord-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/client.py` & `encord-0.1.82/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/configs.py` & `encord-0.1.82/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/constants/enums.py` & `encord-0.1.82/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/constants/model.py` & `encord-0.1.82/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/constants/model_weights.py` & `encord-0.1.82/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/constants/string_constants.py` & `encord-0.1.82/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/constants/test/test_enums.py` & `encord-0.1.82/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/dataset.py` & `encord-0.1.82/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/exceptions.py` & `encord-0.1.82/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/bundle.py` & `encord-0.1.82/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/constants.py` & `encord-0.1.82/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/error_utils.py` & `encord-0.1.82/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/querier.py` & `encord-0.1.82/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/query_methods.py` & `encord-0.1.82/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/request.py` & `encord-0.1.82/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/http/utils.py` & `encord-0.1.82/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/bitmask.py` & `encord-0.1.82/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/common.py` & `encord-0.1.82/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/coordinates.py` & `encord-0.1.82/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/frames.py` & `encord-0.1.82/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/internal_helpers.py` & `encord-0.1.82/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/ontology_labels_impl.py` & `encord-0.1.82/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2805,17 +2805,21 @@
         else:
             track_hash = None
             ranges = None
 
         if isinstance(attribute, TextAttribute):
             self._set_answer_unsafe(answer_dict["answers"], attribute, track_hash, ranges)
         elif isinstance(attribute, RadioAttribute):
-            feature_hash = answer_dict["answers"][0]["featureHash"]
-            option = _get_option_by_hash(feature_hash, attribute.options)
-            self._set_answer_unsafe(option, attribute, track_hash, ranges)
+            if len(answer_dict["answers"]) == 1:
+                # When classification is removed in UI, it keeps the entry about the classification,
+                # but removes the answers.
+                # Thus an empty answers array is equivalent to "no such attribute", and such attribute should be ignored
+                feature_hash = answer_dict["answers"][0]["featureHash"]
+                option = _get_option_by_hash(feature_hash, attribute.options)
+                self._set_answer_unsafe(option, attribute, track_hash, ranges)
         elif isinstance(attribute, ChecklistAttribute):
             options = []
             for answer in answer_dict["answers"]:
                 feature_hash = answer["featureHash"]
                 option = _get_option_by_hash(feature_hash, attribute.options)
                 options.append(option)
             self._set_answer_unsafe(options, attribute, track_hash, ranges)
```

### Comparing `encord-0.1.81/encord/objects/project.py` & `encord-0.1.82/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/objects/utils.py` & `encord-0.1.82/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/ontology.py` & `encord-0.1.82/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/api_key.py` & `encord-0.1.82/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/base_orm.py` & `encord-0.1.82/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/dataset.py` & `encord-0.1.82/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/dataset_with_user_role.py` & `encord-0.1.82/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/label_log.py` & `encord-0.1.82/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/label_row.py` & `encord-0.1.82/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/labeling_algorithm.py` & `encord-0.1.82/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/model.py` & `encord-0.1.82/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/ontology.py` & `encord-0.1.82/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/project.py` & `encord-0.1.82/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/project_api_key.py` & `encord-0.1.82/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/project_with_user_role.py` & `encord-0.1.82/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/orm/test/test_dataset.py` & `encord-0.1.82/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project.py` & `encord-0.1.82/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project_ontology/classification_attribute.py` & `encord-0.1.82/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project_ontology/classification_option.py` & `encord-0.1.82/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project_ontology/ontology.py` & `encord-0.1.82/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project_ontology/ontology_classification.py` & `encord-0.1.82/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/project_ontology/ontology_object.py` & `encord-0.1.82/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/user_client.py` & `encord-0.1.82/encord/user_client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/utilities/client_utilities.py` & `encord-0.1.82/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/utilities/label_utilities.py` & `encord-0.1.82/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/encord/utilities/project_user.py` & `encord-0.1.82/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.81/pyproject.toml` & `encord-0.1.82/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.81"
+version = "0.1.82"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 python-dateutil = "^2.8.2"
 requests = "^2.25.0"
-cryptography = "^3.4.8"
+cryptography = ">=3.4.8"
 tqdm = "^4.32.1"
 importlib_metadata = {version = "^6.1.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 pre-commit = "^2.16.0"
 black = "^23.3.0"
```

### Comparing `encord-0.1.81/PKG-INFO` & `encord-0.1.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.81
+Version: 0.1.82
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=3.4.8,<4.0.0)
+Requires-Dist: cryptography (>=3.4.8)
 Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0) ; python_version < "3.8"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: tqdm (>=4.32.1,<5.0.0)
 Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.81 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.82 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: cryptography (>=3.4.8,<4.0.0) Requires-Dist: importlib_metadata
-(>=6.1.0,<7.0.0) ; python_version < "3.8" Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm
-(>=4.32.1,<5.0.0) Project-URL: Documentation, https://python.docs.encord.com/
-Project-URL: Repository, https://github.com/encord-team/encord-client-python
-Description-Content-Type: text/markdown
+Dist: cryptography (>=3.4.8) Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0)
+; python_version < "3.8" Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm (>=4.32.1,<5.0.0)
+Project-URL: Documentation, https://python.docs.encord.com/ Project-URL:
+Repository, https://github.com/encord-team/encord-client-python Description-
+Content-Type: text/markdown
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
 //opensource.org/licenses/Apache-2.0) # The data engine for computer vision ##
 ð» Features - Minimal low-level Python client that allows you to interact
 with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11` ##
 â¨ Relevant Links * [Encord website](https://encord.com) * [Encord web app]
 (https://app.encord.com) * [Encord documentation](https://docs.encord.com) ##
```

