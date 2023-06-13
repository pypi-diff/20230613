# Comparing `tmp/credsweeper-1.4.9.tar.gz` & `tmp/credsweeper-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.4.9.tar", last modified: Fri Mar  3 10:05:50 2023, max compression
+gzip compressed data, was "credsweeper-1.5.0.tar", last modified: Tue Jun 13 10:20:00 2023, max compression
```

## Comparing `credsweeper-1.4.9.tar` & `credsweeper-1.5.0.tar`

### file list

```diff
@@ -1,139 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-03 10:05:41.000000 credsweeper-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-03-03 10:05:50.888596 credsweeper-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-03-03 10:05:41.000000 credsweeper-1.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/common/keyword_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.876596 credsweeper-1.4.9/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/deep_scaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.876596 credsweeper-1.4.9/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/cred_card_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/credit_card_number_sequense.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/pem_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_entropy_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.880596 credsweeper-1.4.9/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.884596 credsweeper-1.4.9/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-03 10:05:41.000000 credsweeper-1.4.9/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.872596 credsweeper-1.4.9/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 10:05:50.000000 credsweeper-1.4.9/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-03 10:05:50.888596 credsweeper-1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-03 10:05:41.000000 credsweeper-1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:05:50.888596 credsweeper-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27535 2023-03-03 10:05:41.000000 credsweeper-1.4.9/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    34004 2023-03-03 10:05:41.000000 credsweeper-1.4.9/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-13 10:19:49.000000 credsweeper-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-13 10:20:00.773329 credsweeper-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-13 10:19:49.000000 credsweeper-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.757329 credsweeper-1.5.0/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.761329 credsweeper-1.5.0/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.765329 credsweeper-1.5.0/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/cred_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/structured_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_entropy_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_pem_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_structured_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.769329 credsweeper-1.5.0/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 10:19:49.000000 credsweeper-1.5.0/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.757329 credsweeper-1.5.0/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 10:20:00.000000 credsweeper-1.5.0/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 10:20:00.773329 credsweeper-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 10:19:49.000000 credsweeper-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:20:00.773329 credsweeper-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-13 10:19:49.000000 credsweeper-1.5.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-06-13 10:19:49.000000 credsweeper-1.5.0/tests/test_main.py
```

### Comparing `credsweeper-1.4.9/LICENSE` & `credsweeper-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/PKG-INFO` & `credsweeper-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.4.9
+Version: 1.5.0
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.4.9/README.md` & `credsweeper-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/__init__.py` & `credsweeper-1.5.0/credsweeper/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-
 from credsweeper.app import CredSweeper
 from credsweeper.common.constants import ThresholdPreset
 from credsweeper.file_handler import ContentProvider, ByteContentProvider, DiffContentProvider, StringContentProvider, \
     DataContentProvider, \
     TextContentProvider
 from credsweeper.ml_model.ml_validator import MlValidator
 from credsweeper.validations.apply_validation import ApplyValidation
@@ -15,14 +13,11 @@
     'CredSweeper',  #
     'DataContentProvider',  #
     'DiffContentProvider',  #
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
-    'CREDSWEEPER_DIR',  #
     '__version__'
 ]
 
-CREDSWEEPER_DIR = Path(__file__).resolve().parent
-
-__version__ = "1.4.9"
+__version__ = "1.5.0"
```

### Comparing `credsweeper-1.4.9/credsweeper/__main__.py` & `credsweeper-1.5.0/credsweeper/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import os
 import sys
 import time
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from typing import Any, Union, Optional, Dict
 
-from credsweeper import __version__, CREDSWEEPER_DIR
-from credsweeper.app import CredSweeper
+from credsweeper import __version__
+from credsweeper.app import APP_PATH, CredSweeper
 from credsweeper.common.constants import ThresholdPreset, Severity, RuleType, DiffRowType
 from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.file_handler.patch_provider import PatchProvider
 from credsweeper.file_handler.text_provider import TextProvider
 from credsweeper.logger.logger import Logger
 from credsweeper.utils import Util
 
@@ -60,36 +60,52 @@
         log_level: string with level
 
     Returns True if log_level UPPERCASE is one of keys
     """
     val = log_level.upper()
     if any(val == i for i in Logger.LEVELS.keys()):
         return val
-    raise ArgumentTypeError(f"log level given: {log_level} -- must be one of: {' | '.join(Logger.LEVELS.keys())}")
+    raise ArgumentTypeError(f"Log level provided: {log_level} -- must be one of: {' | '.join(Logger.LEVELS.keys())}")
+
+
+def severity_levels(severity_level: str) -> Severity:
+    """Severity level correctness verification and transformation
+
+    Args:
+        severity_level: string with level
+
+    Returns Severity matched provided string or throws ArgumentTypeError exception
+    """
+
+    if severity := Severity.get(severity_level):
+        return severity
+    raise ArgumentTypeError(
+        f"Severity level provided: {severity_level} -- must be one of: {' | '.join([i.value for i in Severity])}")
 
 
 def check_integrity() -> int:
     """Calculates CRC32 of program files
 
     Returns CRC32 of files in integer
     """
     crc32 = 0
-    for root, dirs, files in os.walk(str(CREDSWEEPER_DIR)):
+    for root, dirs, files in os.walk(APP_PATH):
         for file_path in files:
             if Util.get_extension(file_path) in [".py", ".json", ".txt", ".yaml", ".onnx"]:
                 data = Util.read_data(os.path.join(root, file_path))
                 if data:
                     crc32 ^= binascii.crc32(data)
     return crc32
 
 
 def get_arguments() -> Namespace:
     """All CLI arguments are defined here"""
     parser = ArgumentParser(prog="python -m credsweeper")
-    group = parser.add_mutually_exclusive_group(required=True)
+    single_banner_argument = 2 == len(sys.argv) and "--banner" == sys.argv[1]
+    group = parser.add_mutually_exclusive_group(required=not single_banner_argument)
     group.add_argument("--path", nargs="+", help="file or directory to scan", dest="path", metavar="PATH")
     group.add_argument("--diff_path", nargs="+", help="git diff file to scan", dest="diff_path", metavar="PATH")
     group.add_argument("--export_config",
                        nargs="?",
                        help="exporting default config to file (default: config.json)",
                        const="config.json",
                        dest="export_config",
@@ -104,14 +120,20 @@
                         nargs="?",
                         help="path of rule config file (default: credsweeper/rules/config.yaml). "
                         f"severity:{[i.value for i in Severity]} "
                         f"type:{[i.value for i in RuleType]}",
                         default=None,
                         dest="rule_path",
                         metavar="PATH")
+    parser.add_argument("--severity",
+                        help=f"set minimum level for rules to apply {[i.value for i in Severity]}"
+                        f"(default: '{Severity.INFO}', case insensitive)",
+                        default=Severity.INFO,
+                        dest="severity",
+                        type=severity_levels)
     parser.add_argument("--config",
                         nargs="?",
                         help="use custom config (default: built-in)",
                         default=None,
                         dest="config_path",
                         metavar="PATH")
     parser.add_argument("--log_config",
@@ -122,24 +144,25 @@
                         metavar="PATH")
     parser.add_argument("--denylist",
                         help="path to a plain text file with lines or secrets to ignore",
                         default=None,
                         dest="denylist_path",
                         metavar="PATH")
     parser.add_argument("--find-by-ext",
-                        help="find files by predefined extension.",
+                        help="find files by predefined extension",
                         dest="find_by_ext",
                         action="store_true")
     parser.add_argument("--depth",
-                        help="additional recursive search in data (experimental).",
+                        help="additional recursive search in data (experimental)",
                         type=positive_int,
                         dest="depth",
                         default=0,
                         required=False,
                         metavar="POSITIVE_INT")
+    parser.add_argument("--doc", help="document-specific scanning", dest="doc", action="store_true")
     parser.add_argument("--ml_threshold",
                         help="setup threshold for the ml model. "
                         "The lower the threshold - the more credentials will be reported. "
                         f"Allowed values: float between 0 and 1, or any of {[e.value for e in ThresholdPreset]} "
                         "(default: medium)",
                         type=threshold_or_float,
                         default=ThresholdPreset.medium,
@@ -249,17 +272,20 @@
                                   json_filename=json_filename,
                                   xlsx_filename=xlsx_filename,
                                   pool_count=args.jobs,
                                   ml_batch_size=args.ml_batch_size,
                                   ml_threshold=args.ml_threshold,
                                   find_by_ext=args.find_by_ext,
                                   depth=args.depth,
+                                  doc=args.doc,
+                                  severity=args.severity,
                                   size_limit=args.size_limit,
                                   exclude_lines=denylist,
-                                  exclude_values=denylist)
+                                  exclude_values=denylist,
+                                  log_level=args.log)
         return credsweeper.run(content_provider=content_provider)
     except Exception as exc:
         logger.critical(exc, exc_info=True)
     return -1
 
 
 def main() -> int:
@@ -291,20 +317,23 @@
         content_provider = PatchProvider(args.diff_path, change_type=DiffRowType.DELETED)
         del_credentials_number = scan(args, content_provider, deleted_json_filename, args.xlsx_filename)
         summary["Deleted File Credentials"] = del_credentials_number
         if 0 <= add_credentials_number and 0 <= del_credentials_number:
             result = EXIT_SUCCESS
     elif args.export_config:
         logging.info(f"Exporting default config to file: {args.export_config}")
-        config_dict = Util.json_load(os.path.join(CREDSWEEPER_DIR, "secret", "config.json"))
+        config_dict = Util.json_load(APP_PATH / "secret" / "config.json")
         Util.json_dump(config_dict, args.export_config)
     elif args.export_log_config:
         logging.info(f"Exporting default logger config to file: {args.export_log_config}")
-        config_dict = Util.yaml_load(os.path.join(CREDSWEEPER_DIR, "secret", "log.yaml"))
+        config_dict = Util.yaml_load(APP_PATH / "secret" / "log.yaml")
         Util.yaml_dump(config_dict, args.export_log_config)
+    elif args.banner and 2 == len(sys.argv):
+        # only extend version invocation
+        result = EXIT_SUCCESS
     else:
         logger.error("Not specified 'path' or 'diff_path'")
 
     if EXIT_SUCCESS == result and len(summary):
         for k, v in summary.items():
             print(f"{k}: {v}")
         end_time = time.time()
```

### Comparing `credsweeper-1.4.9/credsweeper/app.py` & `credsweeper-1.5.0/credsweeper/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import itertools
 import logging
 import multiprocessing
-import os
 import signal
 import sys
-from typing import List, Optional, Union
+from pathlib import Path
+from typing import Any, List, Optional, Union, Dict
 
 import pandas as pd
 
-from credsweeper.common.constants import KeyValidationOption, ThresholdPreset, RECURSIVE_SCAN_LIMITATION
+# Directory of credsweeper sources MUST be placed before imports to avoid circular import error
+APP_PATH = Path(__file__).resolve().parent
+
+from credsweeper.common.constants import KeyValidationOption, Severity, ThresholdPreset
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate, CredentialManager
-from credsweeper.deep_scanner.deep_scaner import DeepScanner
+from credsweeper.deep_scanner.deep_scanner import DeepScanner
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
 from credsweeper.file_handler.files_provider import FilesProvider
 from credsweeper.file_handler.text_content_provider import TextContentProvider
 from credsweeper.scanner import Scanner
 from credsweeper.utils import Util
 from credsweeper.validations.apply_validation import ApplyValidation
@@ -35,25 +38,28 @@
 
     """
 
     def __init__(self,
                  rule_path: Optional[str] = None,
                  config_path: Optional[str] = None,
                  api_validation: bool = False,
-                 json_filename: Optional[str] = None,
-                 xlsx_filename: Optional[str] = None,
+                 json_filename: Union[None, str, Path] = None,
+                 xlsx_filename: Union[None, str, Path] = None,
                  use_filters: bool = True,
                  pool_count: int = 1,
                  ml_batch_size: Optional[int] = 16,
                  ml_threshold: Union[float, ThresholdPreset] = ThresholdPreset.medium,
                  find_by_ext: bool = False,
                  depth: int = 0,
+                 doc: bool = False,
+                 severity: Severity = Severity.INFO,
                  size_limit: Optional[str] = None,
                  exclude_lines: Optional[List[str]] = None,
-                 exclude_values: Optional[List[str]] = None) -> None:
+                 exclude_values: Optional[List[str]] = None,
+                 log_level: Optional[str] = None) -> None:
         """Initialize Advanced credential scanner.
 
         Args:
             rule_path: optional str variable, path of rule config file
                 validation was the grained candidate model on machine learning
             config_path: optional str variable, path of CredSweeper config file
                 default built-in config is used if None
@@ -65,46 +71,85 @@
                 to xlsx
             use_filters: boolean variable, specifying the need of rule filters
             pool_count: int value, number of parallel processes to use
             ml_batch_size: int value, size of the batch for model inference
             ml_threshold: float or string value to specify threshold for the ml model
             find_by_ext: boolean - files will be reported by extension
             depth: int - how deep container files will be scanned
+            doc: boolean - document-specific scanning
+            severity: Severity - minimum severity level of rule
             size_limit: optional string integer or human-readable format to skip oversize files
             exclude_lines: lines to omit in scan. Will be added to the lines already in config
             exclude_values: values to omit in scan. Will be added to the values already in config
+            log_level: str - level for pool initializer according logging levels (UPPERCASE)
 
         """
         self.pool_count: int = int(pool_count) if int(pool_count) > 1 else 1
+        config_dict = self._get_config_dict(config_path=config_path,
+                                            api_validation=api_validation,
+                                            use_filters=use_filters,
+                                            find_by_ext=find_by_ext,
+                                            depth=depth,
+                                            doc=doc,
+                                            severity=severity,
+                                            size_limit=size_limit,
+                                            exclude_lines=exclude_lines,
+                                            exclude_values=exclude_values)
+        self.config = Config(config_dict)
+        self.scanner = Scanner(self.config, rule_path)
+        self.doc_scanner = Scanner(self.config, rule_path, ["doc"])
+        self.deep_scanner = DeepScanner(self.config, self.scanner)
+        self.deep_doc_scanner = DeepScanner(self.config, self.doc_scanner)
+        self.credential_manager = CredentialManager()
+        self.json_filename: Union[None, str, Path] = json_filename
+        self.xlsx_filename: Union[None, str, Path] = xlsx_filename
+        self.ml_batch_size = ml_batch_size
+        self.ml_threshold = ml_threshold
+        self.ml_validator = None
+        self.__log_level = log_level
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+    @staticmethod
+    def _get_config_path(config_path: Optional[str]) -> Path:
         if config_path:
-            config_dict = Util.json_load(config_path)
+            return Path(config_path)
         else:
-            dir_path = os.path.dirname(os.path.realpath(__file__))
-            config_dict = Util.json_load(os.path.join(dir_path, "secret", "config.json"))
+            return APP_PATH / "secret" / "config.json"
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
+    def _get_config_dict(
+            self,  #
+            config_path: Optional[str],  #
+            api_validation: bool,  #
+            use_filters: bool,  #
+            find_by_ext: bool,  #
+            depth: int,  #
+            doc: bool,  #
+            severity: Severity,  #
+            size_limit: Optional[str],  #
+            exclude_lines: Optional[List[str]],  #
+            exclude_values: Optional[List[str]]) -> Dict[str, Any]:
+        config_dict = Util.json_load(self._get_config_path(config_path))
         config_dict["validation"] = {}
         config_dict["validation"]["api_validation"] = api_validation
         config_dict["use_filters"] = use_filters
         config_dict["find_by_ext"] = find_by_ext
         config_dict["size_limit"] = size_limit
         config_dict["depth"] = depth
+        config_dict["doc"] = doc
+        config_dict["severity"] = severity.value
+
         if exclude_lines is not None:
             config_dict["exclude"]["lines"] = config_dict["exclude"].get("lines", []) + exclude_lines
         if exclude_values is not None:
             config_dict["exclude"]["values"] = config_dict["exclude"].get("values", []) + exclude_values
 
-        self.config = Config(config_dict)
-        self.credential_manager = CredentialManager()
-        self.scanner = Scanner(self.config, rule_path)
-        self.deep_scanner = DeepScanner(self.config, self.scanner)
-        self.json_filename: Optional[str] = json_filename
-        self.xlsx_filename: Optional[str] = xlsx_filename
-        self.ml_batch_size = ml_batch_size
-        self.ml_threshold = ml_threshold
-        self.ml_validator = None
+        return config_dict  # type: ignore
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def _use_ml_validation(self) -> bool:
         if isinstance(self.ml_threshold, float) and self.ml_threshold <= 0:
             return False
         return True
@@ -131,17 +176,18 @@
     @ml_validator.setter
     def ml_validator(self, _ml_validator: Optional[MlValidator]) -> None:
         """ml_validator setter"""
         self.__ml_validator = _ml_validator
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    @classmethod
-    def pool_initializer(cls) -> None:
+    @staticmethod
+    def pool_initializer(log_kwargs) -> None:
         """Ignore SIGINT in child processes."""
+        logging.basicConfig(**log_kwargs)
         signal.signal(signal.SIGINT, signal.SIG_IGN)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     @property
     def config(self) -> Config:
         """config getter"""
@@ -162,15 +208,15 @@
         Args:
             content_provider: path objects to scan
 
         """
         _empty_list: List[Union[DiffContentProvider, TextContentProvider]] = []
         file_extractors: List[Union[DiffContentProvider, TextContentProvider]] = \
             content_provider.get_scannable_files(self.config) if content_provider else _empty_list
-        logger.info("Start Scanner")
+        logger.info(f"Start Scanner for {len(file_extractors)} providers")
         self.scan(file_extractors)
         self.post_processing()
         self.export_results()
 
         return len(self.credential_manager.get_credentials())
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
@@ -204,15 +250,25 @@
         else:
             self.credential_manager.set_credentials(all_cred)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def __multi_jobs_scan(self, content_providers: List[Union[DiffContentProvider, TextContentProvider]]) -> None:
         """Performs scan with multiple jobs"""
-        with multiprocessing.get_context("spawn").Pool(self.pool_count, initializer=self.pool_initializer) as pool:
+        # use this separation to satisfy YAPF formatter
+        yapfix = "%(asctime)s | %(levelname)s | %(processName)s:%(threadName)s | %(filename)s:%(lineno)s | %(message)s"
+        log_kwargs = {"format": yapfix}
+        if isinstance(self.__log_level, str):
+            # is not None
+            if "SILENCE" == self.__log_level:
+                logging.addLevelName(60, "SILENCE")
+            log_kwargs["level"] = self.__log_level
+        with multiprocessing.get_context("spawn").Pool(processes=self.pool_count,
+                                                       initializer=self.pool_initializer,
+                                                       initargs=(log_kwargs, )) as pool:
             try:
                 # Get list credentials for each file
                 scan_results_per_file = pool.map(self.file_scan, content_providers)
                 # Join all sublist into a single list
                 scan_results = list(itertools.chain(*scan_results_per_file))
                 for cred in scan_results:
                     self.credential_manager.add_credential(cred)
@@ -243,45 +299,50 @@
         if FilePathExtractor.is_find_by_ext_file(self.config, content_provider.file_type):
             # Skip the file scanning and create fake candidate because the extension is suspicious
             dummy_candidate = Candidate.get_dummy_candidate(self.config, content_provider.file_path,
                                                             content_provider.file_type, content_provider.info)
             candidates.append(dummy_candidate)
 
         else:
-            # deep scan with possibly data representation
             if self.config.depth:
-                new_size_limit = self.config.size_limit if self.config.size_limit else RECURSIVE_SCAN_LIMITATION
-                candidates = self.deep_scanner.scan(content_provider, self.config.depth, new_size_limit)
+                # deep scan with possible data representation
+                candidates = self.deep_scanner.scan(content_provider, self.config.depth, self.config.size_limit)
+            elif self.config.doc:
+                # document-specific scanning
+                candidates = self.deep_doc_scanner.scan(content_provider, 0, self.config.size_limit)
             else:
                 if content_provider.file_type not in self.config.exclude_containers:
                     # Regular file scanning
                     analysis_targets = content_provider.get_analysis_target()
                     candidates = self.scanner.scan(analysis_targets)
 
         # finally return result from 'file_scan'
         return candidates
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def post_processing(self) -> None:
         """Machine learning validation for received credential candidates."""
         if self._use_ml_validation():
-            logger.info("Run ML Validation")
+            logger.info(f"Run ML Validation for {len(self.credential_manager.candidates)} candidates")
             new_cred_list = []
             cred_groups = self.credential_manager.group_credentials()
             ml_cred_groups = []
             for group_key, group_candidates in cred_groups.items():
                 # Analyze with ML if all candidates in group require ML
-                if all(candidate.use_ml for candidate in group_candidates):
+                for candidate in group_candidates:
+                    if not candidate.use_ml:
+                        break
+                else:
                     ml_cred_groups.append((group_key.value, group_candidates))
+                    continue
                 # If at least one of credentials in the group do not require ML - automatically report to user
-                else:
-                    for candidate in group_candidates:
-                        candidate.ml_validation = KeyValidationOption.NOT_AVAILABLE
-                    new_cred_list += group_candidates
+                for candidate in group_candidates:
+                    candidate.ml_validation = KeyValidationOption.NOT_AVAILABLE
+                new_cred_list += group_candidates
 
             is_cred, probability = self.ml_validator.validate_groups(ml_cred_groups, self.ml_batch_size)
             for i, (_, group_candidates) in enumerate(ml_cred_groups):
                 if is_cred[i]:
                     for candidate in group_candidates:
                         candidate.ml_validation = KeyValidationOption.VALIDATED_KEY
                         candidate.ml_probability = probability[i]
```

### Comparing `credsweeper-1.4.9/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.5.0/credsweeper/common/keyword_checklist.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 another
 anony
 apache
 appearance
 apple
 application
 apply
+are
 argc
 args
 argv
 argument
 array
 arrow
 article
@@ -85,14 +86,15 @@
 being
 below
 between
 beware
 binary
 binding
 binds
+blah
 black
 blank
 bless
 block
 boost
 bool
 border
@@ -526,14 +528,15 @@
 notes
 nothing
 notice
 notification
 null
 number
 object
+oblique
 observe
 observer
 occurs
 offset
 often
 openssl
 operation
@@ -843,14 +846,15 @@
 terms
 test
 texture
 their
 theme
 there
 these
+thick
 those
 thread
 three
 thrift
 through
 throw
 thrown
```

### Comparing `credsweeper-1.4.9/credsweeper/config/config.py` & `credsweeper-1.5.0/credsweeper/config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-from typing import Dict, List, Optional, Set
+import re
+from typing import Dict, List, Optional, Set, Any
 
 from humanfriendly import parse_size
-from regex import regex
 
+from credsweeper.common.constants import Severity, DEFAULT_PATTERN_LEN, DEFAULT_PEM_PATTERN_LEN
 from credsweeper.utils import Util
 
 
 class Config:
     """Class that contain configs that can be changed by user."""
 
     NOT_ALLOWED_PATH = [
         ".*\\.min\\.js", ".*message.*\\.properties", ".*locale.*\\.properties", ".*makefile.*", ".*package-lock\\.json",
         ".*package\\.json", ".*\\.css", ".*\\.scss"
     ]
 
-    def __init__(self, config: Dict) -> None:
-        self.exclude_patterns: List[regex.Pattern] = [
-            regex.compile(pattern) for pattern in config["exclude"]["pattern"]
-        ]
+    def __init__(self, config: Dict[str, Any]) -> None:
+        self.exclude_patterns: List[re.Pattern] = [re.compile(pattern) for pattern in config["exclude"]["pattern"]]
         self.exclude_paths: List[str] = config["exclude"]["path"]
         self.exclude_containers: List[str] = config["exclude"]["containers"]
         self.exclude_extensions: List[str] = config["exclude"]["extension"]
         self.exclude_lines: Set[str] = set(config["exclude"].get("lines", []))
         self.exclude_values: Set[str] = set(config["exclude"].get("values", []))
         self.source_extensions: List[str] = config["source_ext"]
         self.source_quote_ext: List[str] = config["source_quote_ext"]
         self.find_by_ext_list: List[str] = config["find_by_ext_list"]
         self.check_for_literals: bool = config["check_for_literals"]
-        self.not_allowed_path_pattern = regex.compile(f"{Util.get_regex_combine_or(self.NOT_ALLOWED_PATH)}",
-                                                      flags=regex.IGNORECASE)  # pylint: disable=no-member
+        self.not_allowed_path_pattern = re.compile(f"{Util.get_regex_combine_or(self.NOT_ALLOWED_PATH)}",
+                                                   flags=re.IGNORECASE)
         self.api_validation: bool = config["validation"]["api_validation"]
         self.use_filters: bool = config["use_filters"]
         self.line_data_output: List[str] = config["line_data_output"]
         self.candidate_output: List[str] = config["candidate_output"]
         self.find_by_ext: bool = config["find_by_ext"]
         self.size_limit: Optional[int] = parse_size(config["size_limit"]) if config["size_limit"] is not None else None
         self.depth: int = int(config["depth"])
+        self.doc: bool = config["doc"]
+        self.severity: Severity = Severity.get(config.get("severity"))
 
         self.min_keyword_value_length: int = int(config["min_keyword_value_length"])
         self.min_pattern_value_length: int = int(config["min_pattern_value_length"])
 
         # Trim exclude patterns from space like characters
         self.exclude_lines = set(line.strip() for line in self.exclude_lines)
         self.exclude_values = set(line.strip() for line in self.exclude_values)
+
+        self.pattern_len = config.get("pattern_len", DEFAULT_PATTERN_LEN)
+        self.pem_pattern_len = config.get("pem_pattern_len", DEFAULT_PEM_PATTERN_LEN)
```

### Comparing `credsweeper-1.4.9/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.5.0/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/credentials/candidate.py` & `credsweeper-1.5.0/credsweeper/credentials/candidate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
+import re
 from json.encoder import py_encode_basestring_ascii
-from typing import Any, List, Optional
-
-from regex import regex
+from typing import Any, Dict, List, Optional
 
 from credsweeper.common.constants import KeyValidationOption, Severity
 from credsweeper.config import Config
 from credsweeper.credentials.line_data import LineData
 from credsweeper.validations.validation import Validation
 
 
@@ -23,24 +22,24 @@
         config: user configs
         validations: List of Validation objects that can check this credential using external API
         use_ml: Should ML work on this credential or not. If not prediction based on regular expression and filter only
     """
 
     def __init__(self,
                  line_data_list: List[LineData],
-                 patterns: List[regex.Pattern],
+                 patterns: List[re.Pattern],
                  rule_name: str,
                  severity: Severity,
                  config: Config,
                  validations: List[Validation] = None,
                  use_ml: bool = False) -> None:
         self.api_validation = KeyValidationOption.NOT_AVAILABLE
         self.ml_validation = KeyValidationOption.NOT_AVAILABLE
         self.line_data_list: List[LineData] = line_data_list if line_data_list else []
-        self.patterns: List[regex.Pattern] = patterns if patterns else []
+        self.patterns: List[re.Pattern] = patterns if patterns else []
         self.ml_probability = None
         self.rule_name: str = rule_name
         self.severity: Optional[Severity] = severity
         self.validations: List[Validation] = validations if validations else []
         self.use_ml: bool = use_ml
         self.config = config
 
@@ -71,20 +70,20 @@
 
     @line_data_list.setter
     def line_data_list(self, line_data_list: List[LineData]) -> None:
         """line_data_list setter"""
         self.__line_data_list = line_data_list
 
     @property
-    def patterns(self) -> List[regex.Pattern]:
+    def patterns(self) -> List[re.Pattern]:
         """patterns getter"""
         return self.__patterns
 
     @patterns.setter
-    def patterns(self, patterns: List[regex.Pattern]) -> None:
+    def patterns(self, patterns: List[re.Pattern]) -> None:
         """patterns setter"""
         self.__patterns = patterns
 
     @property
     def rule_name(self) -> str:
         """rule_name getter"""
         return self.__rule_name
@@ -133,15 +132,15 @@
         """
         return len(self.validations) > 0
 
     def __str__(self) -> str:
         return f"rule: {self.rule_name} / severity: {self.severity.value} / line_data_list: {self.line_data_list} " \
                f"/ api_validation: {self.api_validation.name} / ml_validation: {self.ml_validation.name}"
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict:
         """Convert credential candidate object to dictionary.
 
         Return:
             Dictionary object generated from current credential candidate
 
         """
         full_output = {
@@ -179,12 +178,12 @@
             reported_output.append(line_data)
         return reported_output
 
     @classmethod
     def get_dummy_candidate(cls, config: Config, file_path: str, file_type: str, info: str):
         """Create dummy instance to use in searching file by extension"""
         return cls(  #
-            line_data_list=[LineData(config, "dummy line", -1, file_path, file_type, info, regex.compile(".*"))],
-            patterns=[regex.compile(".*")],  #
+            line_data_list=[LineData(config, "dummy line", -1, file_path, file_type, info, re.compile(".*"))],
+            patterns=[re.compile(".*")],  #
             rule_name="Dummy candidate",  #
             severity=Severity.INFO,  #
             config=config)
```

### Comparing `credsweeper-1.4.9/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.5.0/credsweeper/credentials/candidate_group_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Dict, List, Tuple
 
 from credsweeper.credentials.candidate import Candidate
 from credsweeper.credentials.candidate_key import CandidateKey
 
 
 class CandidateGroupGenerator:
+    """CandidateGroupGenerator"""
 
     def __init__(self) -> None:
         self.grouped_candidates: Dict[CandidateKey, List[Candidate]] = {}
 
     @property
     def grouped_candidates(self) -> Dict[CandidateKey, List[Candidate]]:
+        """property getter"""
         return self._grouped_candidates
 
     @grouped_candidates.setter
     def grouped_candidates(self, grouped_candidates: Dict[CandidateKey, List[Candidate]]) -> None:
+        """property setter"""
         self._grouped_candidates = grouped_candidates
 
     def __contains__(self, key: CandidateKey) -> bool:
         return key in self.grouped_candidates
 
     def __getitem__(self, key) -> List[Candidate]:
         return self.grouped_candidates[key]
@@ -26,8 +29,9 @@
     def __setitem__(self, key: CandidateKey, value: List[Candidate]) -> None:
         self.grouped_candidates[key] = value
 
     def __len__(self) -> int:
         return len(self.grouped_candidates)
 
     def items(self) -> List[Tuple[CandidateKey, List[Candidate]]]:
+        """getter"""
         return list(self.grouped_candidates.items())
```

### Comparing `credsweeper-1.4.9/credsweeper/credentials/candidate_key.py` & `credsweeper-1.5.0/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/credentials/credential_manager.py` & `credsweeper-1.5.0/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/credentials/line_data.py` & `credsweeper-1.5.0/credsweeper/credentials/line_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Any, Optional, Tuple
-
-from regex import regex
+import re
+from typing import Any, Dict, Optional, Tuple
 
 from credsweeper.config import Config
 from credsweeper.utils import Util
 
 
 class LineData:
     """Object to treat and store scanned line related data.
@@ -21,33 +20,33 @@
         separator_span: optional tuple variable, separator position
         value: optional string variable, detected value in line
         variable: optional string variable, detected variable in line
 
     """
 
     comment_starts = ["//", "*", "#", "/*", "<!––", "%{", "%", "...", "(*", "--", "--[[", "#="]
-    bash_param_split = regex.compile("\\s+(\\-|\\||\\>|\\w+?\\>|\\&)")
+    bash_param_split = re.compile("\\s+(\\-|\\||\\>|\\w+?\\>|\\&)")
 
     def __init__(
             self,  #
             config: Config,  #
             line: str,  #
             line_num: int,  #
             path: str,  #
             file_type: str,  #
             info: str,  #
-            pattern: regex.Pattern) -> None:
+            pattern: re.Pattern) -> None:
         self.config = config
         self.key: Optional[str] = None
         self.line: str = line
         self.line_num: int = line_num
         self.path: str = path
         self.file_type: str = file_type
         self.info: str = info
-        self.pattern: regex.Pattern = pattern
+        self.pattern: re.Pattern = pattern
         self.separator: Optional[str] = None
         self.separator_span: Optional[Tuple[int, int]] = None
         self.value: Optional[str] = None
         self.variable: Optional[str] = None
         self.value_leftquote: Optional[str] = None
         self.value_rightquote: Optional[str] = None
 
@@ -110,20 +109,20 @@
 
     @info.setter
     def info(self, info: str) -> None:
         """info setter"""
         self.__info = info
 
     @property
-    def pattern(self) -> regex.Pattern:
+    def pattern(self) -> re.Pattern:
         """pattern getter"""
         return self.__pattern
 
     @pattern.setter
-    def pattern(self, pattern: regex.Pattern) -> None:
+    def pattern(self, pattern: re.Pattern) -> None:
         """pattern setter"""
         self.__pattern = pattern
 
     @property
     def separator(self) -> str:
         """separator getter"""
         return self.__separator
@@ -189,21 +188,21 @@
 
     def set_pattern_match_groups(self) -> None:
         """Apply regex to the candidate line and set internal fields based on match."""
         match_obj = self.pattern.search(self.line)
         if match_obj is None:
             return
 
-        def get_group_from_match_obj(match_obj: regex.Match, group: str) -> Any:
+        def get_group_from_match_obj(match_obj: re.Match, group: str) -> Any:
             try:
                 return match_obj.group(group)
             except Exception:
                 return None
 
-        def get_span_from_match_obj(match_obj: regex.Match, group: str) -> Optional[Tuple[int, int]]:
+        def get_span_from_match_obj(match_obj: re.Match, group: str) -> Optional[Tuple[int, int]]:
             try:
                 return match_obj.span(group)
             except Exception:
                 return None
 
         self.key = get_group_from_match_obj(match_obj, "keyword")
         self.separator = get_group_from_match_obj(match_obj, "separator")
@@ -253,16 +252,18 @@
         """Check if line with credential is a comment.
 
         Return:
             True if line is a comment, False otherwise
 
         """
         cleaned_line = self.line.strip()
-        starts_from_comment = any(cleaned_line.startswith(comment_start) for comment_start in self.comment_starts)
-        return starts_from_comment
+        for comment_start in self.comment_starts:
+            if cleaned_line.startswith(comment_start):
+                return True
+        return False
 
     def is_source_file(self) -> bool:
         """Check if file with credential is a source code file or not (data, log, plain text).
 
         Return:
             True if file is source file, False otherwise
 
@@ -286,15 +287,15 @@
             return True
         return False
 
     def __repr__(self) -> str:
         return f"line: '{self.line}' / line_num: {self.line_num} / path: {self.path} " \
                f"/ value: '{self.value}' / entropy_validation: {Util.is_entropy_validate(self.value)}"
 
-    def to_json(self) -> dict:
+    def to_json(self) -> Dict:
         """Convert line data object to dictionary.
 
         Return:
             Dictionary object generated from current line data
 
         """
         full_output = {
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from abc import abstractmethod, ABC, abstractproperty
+from abc import abstractmethod, ABC
 from typing import List
 
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 from credsweeper.file_handler.struct_content_provider import StructContentProvider
 from credsweeper.scanner import Scanner
 
 
 class AbstractScanner(ABC):
     """Base abstract class for all recursive scanners"""
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def config(self) -> Config:
         """Abstract property to be defined in DeepScanner"""
         raise NotImplementedError(__name__)
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def scanner(self) -> Scanner:
         """Abstract property to be defined in DeepScanner"""
         raise NotImplementedError(__name__)
 
     @abstractmethod
     def recursive_scan(
             self,  #
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/byte_scanner.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 from .abstract_scanner import AbstractScanner
 
 logger = logging.getLogger(__name__)
 
 
 class ByteScanner(AbstractScanner, ABC):
-    """Realises plain scanning"""
+    """Implements plain data scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
         """Tries to represent data as plain text with splitting by lines and scan as text lines"""
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
 class Bzip2Scanner(AbstractScanner, ABC):
-    """Realises bzip2 scanning"""
+    """Implements bzip2 scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Extracts data from bzip2 archive and launch data_scan"""
+        """Extracts data from bzip2 archive and launches data_scan"""
         candidates = []
         try:
             new_path = data_provider.file_path if ".bz2" != Util.get_extension(
                 data_provider.file_path) else data_provider.file_path[:-4]
             bzip2_content_provider = DataContentProvider(data=bz2.decompress(data_provider.data),
                                                          file_path=data_provider.file_path,
                                                          file_type=Util.get_extension(new_path),
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/deep_scaner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/deep_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import List, Optional, Any, Tuple, Union
 
+from credsweeper.common.constants import RECURSIVE_SCAN_LIMITATION
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.credentials.augment_candidates import augment_candidates
 from credsweeper.file_handler.byte_content_provider import ByteContentProvider
 from credsweeper.file_handler.content_provider import ContentProvider
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 from credsweeper.file_handler.diff_content_provider import DiffContentProvider
@@ -27,15 +28,15 @@
 from ..file_handler.struct_content_provider import StructContentProvider
 
 logger = logging.getLogger(__name__)
 
 
 class DeepScanner(ByteScanner, Bzip2Scanner, EncoderScanner, GzipScanner, HtmlScanner, LangScanner, PdfScanner,
                   TarScanner, XmlScanner, ZipScanner):
-    """Advanced scanner with recursive exploring data"""
+    """Advanced scanner with recursive exploring of data"""
 
     def __init__(self, config: Config, scanner: Scanner) -> None:
         """Initialize Advanced credential scanner.
 
         Args:
             scanner: CredSweeper scanner object
             config: dictionary variable, stores analyzer features
@@ -69,22 +70,27 @@
             deep_scanners.append(PdfScanner)
         else:
             deep_scanners = [ByteScanner, EncoderScanner, HtmlScanner, XmlScanner, LangScanner]
         return deep_scanners
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def scan(self, content_provider: ContentProvider, depth: int, recursive_limit_size: int) -> List[Candidate]:
+    def scan(self,
+             content_provider: ContentProvider,
+             depth: int,
+             recursive_limit_size: Optional[int] = None) -> List[Candidate]:
         """Initial scan method to launch recursive scan. Skips ByteScanner to prevent extra scan
 
             Args:
                 content_provider: ContentProvider that might contain raw data
                 depth: maximal level of recursion
                 recursive_limit_size: maximal bytes of opened files to prevent recursive zip-bomb attack
         """
+        recursive_limit_size = recursive_limit_size if isinstance(recursive_limit_size,
+                                                                  int) else RECURSIVE_SCAN_LIMITATION
         candidates: List[Candidate] = []
         data: Optional[bytes] = None
         if isinstance(content_provider, TextContentProvider) or isinstance(content_provider, ByteContentProvider):
             # Feature to scan files which might be containers
             data = content_provider.data
         elif isinstance(content_provider, DiffContentProvider) and content_provider.diff:
             analysis_targets = content_provider.get_analysis_target()
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from credsweeper.deep_scanner.abstract_scanner import AbstractScanner
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 
 logger = logging.getLogger(__name__)
 
 
 class EncoderScanner(AbstractScanner, ABC):
-    """Realises recursive iteration when data might be encoded"""
+    """Implements recursive iteration when data might be encoded"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
         """Tries to decode data from base64 encode to bytes and scan as bytes again"""
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """Realises gzip scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Extracts data from gzip archive and launch data_scan"""
+        """Extracts data from gzip archive and launches data_scan"""
         candidates = []
         try:
             with gzip.open(io.BytesIO(data_provider.data)) as f:
                 new_path = data_provider.file_path if ".gz" != Util.get_extension(
                     data_provider.file_path) else data_provider.file_path[:-3]
                 gzip_content_provider = DataContentProvider(data=f.read(),
                                                             file_path=data_provider.file_path,
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/xml_scanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from credsweeper.deep_scanner.abstract_scanner import AbstractScanner
 from credsweeper.file_handler.data_content_provider import DataContentProvider
 from credsweeper.file_handler.string_content_provider import StringContentProvider
 
 logger = logging.getLogger(__name__)
 
 
-class HtmlScanner(AbstractScanner, ABC):
-    """Realises html scanning if possibly"""
+class XmlScanner(AbstractScanner, ABC):
+    """Realises xml scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Tries to represent data as html text and scan as text lines"""
-        if data_provider.represent_as_html():
+        """Tries to represent data as xml text and scan as text lines"""
+        if data_provider.represent_as_xml():
             string_data_provider = StringContentProvider(lines=data_provider.lines,
                                                          line_numbers=data_provider.line_numbers,
                                                          file_path=data_provider.file_path,
-                                                         file_type=".xml",
-                                                         info=f"{data_provider.info}|HTML")
+                                                         file_type=data_provider.file_type,
+                                                         info=f"{data_provider.info}|XML")
             analysis_targets = string_data_provider.get_analysis_target()
             return self.scanner.scan(analysis_targets)
         return []
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/html_scanner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import logging
 from abc import ABC
 from typing import List
 
 from credsweeper.credentials import Candidate
 from credsweeper.deep_scanner.abstract_scanner import AbstractScanner
 from credsweeper.file_handler.data_content_provider import DataContentProvider
-from credsweeper.file_handler.struct_content_provider import StructContentProvider
+from credsweeper.file_handler.string_content_provider import StringContentProvider
 
 logger = logging.getLogger(__name__)
 
 
-class LangScanner(AbstractScanner, ABC):
-    """Realises scanning data if it might be represented as a script"""
+class HtmlScanner(AbstractScanner, ABC):
+    """Implements html scanning if possible"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Tries to represent data as markup language and scan as structure"""
-        if data_provider.represent_as_structure():
-            struct_data_provider = StructContentProvider(struct=data_provider.structure,
+        """Tries to represent data as html text and scan as text lines"""
+        if data_provider.represent_as_html():
+            string_data_provider = StringContentProvider(lines=data_provider.lines,
+                                                         line_numbers=data_provider.line_numbers,
                                                          file_path=data_provider.file_path,
                                                          file_type=data_provider.file_type,
-                                                         info=f"{data_provider.info}|STRUCT")
-            return self.structure_scan(struct_data_provider, depth, recursive_limit_size)
+                                                         info=f"{data_provider.info}|HTML")
+            analysis_targets = string_data_provider.get_analysis_target()
+            return self.scanner.scan(analysis_targets)
         return []
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from credsweeper.file_handler.data_content_provider import DataContentProvider, MIN_DATA_LEN
 from credsweeper.file_handler.string_content_provider import StringContentProvider
 
 logger = logging.getLogger(__name__)
 
 
 class PdfScanner(AbstractScanner, ABC):
-    """Realises pdf scanning"""
+    """Implements pdf scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Extracts text from PDF elements and whole text, then launch data_scan"""
+        """Tries to scan PDF elements recursively and the whole text on page as strings"""
         candidates = []
         # PyPDF2 - https://github.com/py-pdf/pypdf/issues/1328 text in table is merged without spaces
         # pdfminer.six - splits text in table to many lines. Allows to walk through elements
         try:
             pdf_lines = []
             for page in extract_pages(io.BytesIO(data_provider.data), laparams=LAParams()):
                 for element in page:
@@ -48,15 +48,15 @@
                                 pdf_lines.append(element_text)
                     elif isinstance(element, LTItem):
                         pass
                     else:
                         logger.error(f"Unsupported {element}")
             string_data_provider = StringContentProvider(lines=pdf_lines,
                                                          file_path=data_provider.file_path,
-                                                         file_type=".xml",
+                                                         file_type=data_provider.file_type,
                                                          info=f"{data_provider.info}|PDF")
             analysis_targets = string_data_provider.get_analysis_target()
             pdf_candidates = self.scanner.scan(analysis_targets)
             candidates.extend(pdf_candidates)
         except Exception as pdf_exc:
             logger.error(f"{data_provider.file_path}:{pdf_exc}")
         return candidates
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/tar_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
 class TarScanner(AbstractScanner, ABC):
-    """Realises tar scanning"""
+    """Implements tar scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Extracts files one by one from tar archive and launch data_scan"""
+        """Extracts files one by one from tar archive and launches data_scan"""
         candidates = []
         try:
             with TarFile(fileobj=io.BytesIO(data_provider.data)) as tf:
                 for tfi in tf.getmembers():
                     # skip directory
                     if not tfi.isreg():
                         continue
@@ -36,15 +36,15 @@
                                      f" is over limit {recursive_limit_size} depth:{depth}")
                         continue
                     with tf.extractfile(tfi) as f:
                         tar_content_provider = DataContentProvider(data=f.read(),
                                                                    file_path=data_provider.file_path,
                                                                    file_type=Util.get_extension(tfi.name),
                                                                    info=f"{data_provider.info}|TAR|{tfi.name}")
-                        # nevertheless use extracted data size
+                        # Nevertheless, use extracted data size
                         new_limit = recursive_limit_size - len(tar_content_provider.data)
                         tar_candidates = self.recursive_scan(tar_content_provider, depth, new_limit)
                         candidates.extend(tar_candidates)
         except Exception as tar_exc:
             # too many exception types might be produced with broken tar
             logger.error(f"{data_provider.file_path}:{tar_exc}")
         return candidates
```

### Comparing `credsweeper-1.4.9/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.5.0/credsweeper/deep_scanner/zip_scanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from credsweeper.file_handler.file_path_extractor import FilePathExtractor
 from credsweeper.utils import Util
 
 logger = logging.getLogger(__name__)
 
 
 class ZipScanner(AbstractScanner, ABC):
-    """Realises zip scanning"""
+    """Implements zip scanning"""
 
     def data_scan(
             self,  #
             data_provider: DataContentProvider,  #
             depth: int,  #
             recursive_limit_size: int) -> List[Candidate]:
-        """Extracts files one by one from zip archives and launch data_scan"""
+        """Extracts files one by one from zip archives and launches data_scan"""
         candidates = []
         try:
             with ZipFile(io.BytesIO(data_provider.data)) as zf:
                 for zfl in zf.infolist():
                     # skip directory
-                    if "/" == zfl.filename[-1:]:
+                    if zfl.is_dir():
                         continue
                     if FilePathExtractor.check_exclude_file(self.config, zfl.filename):
                         continue
                     if 0 > recursive_limit_size - zfl.file_size:
                         logger.error(f"{zfl.filename}: size {zfl.file_size}"
                                      f" is over limit {recursive_limit_size} depth:{depth}")
                         continue
```

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/__init__.py` & `credsweeper-1.5.0/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/content_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 from typing import List, Optional
 
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.utils import Util
 
 
 class ContentProvider(ABC):
@@ -60,15 +60,16 @@
         return self.__info
 
     @info.setter
     def info(self, _info: str) -> None:
         """info getter"""
         self.__info = _info if _info else ""
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def data(self) -> Optional[bytes]:
         """abstract data getter"""
         raise NotImplementedError(__name__)
 
     @data.setter
     @abstractmethod
     def data(self, data: Optional[bytes]) -> None:
```

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/data_content_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,20 +143,27 @@
 
         Return:
              True if reading was successful
 
         """
         try:
             text = self.data.decode(encoding=DEFAULT_ENCODING)
-            if any(tag in text for tag in ["</html>", "</body>", "</head>", "</div>", "</table>"]):
+            html = None
+            if "</" in text and ">" in text:
                 html = BeautifulSoup(text, features="html.parser")
+            if html:
                 # simple parse as it is displayed to user
-                for line_number, line in enumerate(html.text.splitlines()):
-                    if line and line.strip():
-                        self.line_numbers.append(line_number)
+                # dbg = html.find_all(text=True)
+                for p in html.find_all("p"):
+                    p.append('\n')
+                lines = html.get_text().splitlines()
+                for line_number, doc_line in enumerate(lines):
+                    line = doc_line.strip()
+                    if line:
+                        self.line_numbers.append(line_number + 1)
                         self.lines.append(line)
 
                 # transform table if table cell is assigned to header cell
                 # make from cells a chain like next is assigned to previous
                 for table in html.find_all('table'):
                     table_header = None
                     for tr in table.find_all('tr'):
```

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.5.0/credsweeper/file_handler/file_path_extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 
 class FilePathExtractor:
     """Util class to browse files in directories"""
 
     located_repos: Dict[Path, Repo] = {}
 
-    @classmethod
-    def apply_gitignore(cls, detected_files: List[str]) -> List[str]:
+    @staticmethod
+    def apply_gitignore(detected_files: List[str]) -> List[str]:
         """Apply gitignore rules for each file.
 
         Args:
             detected_files: list of files to be checked
 
         Return:
             List of files with all files ignored by git removed
 
         """
         filtered_files = [file_path for file_path in detected_files if FilePathExtractor.is_valid_path(file_path)]
 
         return filtered_files
 
-    @classmethod
-    def get_file_paths(cls, config: Config, path: Union[str, Path]) -> List[str]:
+    @staticmethod
+    def get_file_paths(config: Config, path: Union[str, Path]) -> List[str]:
         """Get all files in the directory. Automatically exclude files non-code or data files (such as .jpg).
 
         Args:
             config: credsweeper configuration
             path: path to the file or directory to be scanned
 
         Return:
@@ -45,26 +45,29 @@
 
         """
         path = os.path.expanduser(path)  # Replace ~ character with a full path to the home directory
         if not os.path.exists(path):
             logger.warning(f"'{path}' does not exist")
         file_paths = []
         if os.path.isfile(path):
+            # suppose, the file is located outside and should be scanned
             if not FilePathExtractor.check_exclude_file(config, path):
                 file_paths.append(path)
-            return file_paths
-
-        for dirpath, _, filenames in os.walk(path):
-            for filename in filenames:
-                file_path = os.path.join(f"{dirpath}", f"{filename}")
-                if FilePathExtractor.check_exclude_file(config, file_path) or FilePathExtractor.check_file_size(
-                        config, file_path):
-                    continue
-                if os.path.isfile(file_path) and 0 < os.path.getsize(file_path):
-                    file_paths.append(file_path)
+        elif os.path.isdir(path):
+            for dirpath, _, filenames in os.walk(path):
+                for filename in filenames:
+                    file_path = os.path.join(f"{dirpath}", f"{filename}")
+                    if FilePathExtractor.check_exclude_file(config, file_path) \
+                            or os.path.islink(file_path) \
+                            or FilePathExtractor.check_file_size(config, file_path):
+                        continue
+                    if os.path.isfile(file_path) and 0 < os.path.getsize(file_path):
+                        file_paths.append(file_path)
+        else:
+            pass  # symbolic links and so on
         return file_paths
 
     @classmethod
     def is_valid_path(cls, path: str) -> bool:
         """Locate nearest .git directory to the path and check if path is ignored.
 
         Args:
@@ -108,47 +111,47 @@
             extension: str - may be only file name with extension
 
         Return:
             True when the feature is configured and the file extension matches
         """
         return config.find_by_ext and extension in config.find_by_ext_list
 
-    @classmethod
-    def check_exclude_file(cls, config: Config, path: str) -> bool:
+    @staticmethod
+    def check_exclude_file(config: Config, path: str) -> bool:
         """
         Checks whether file should be excluded
 
         Args:
             config: Config
             path: str - full path preferred
 
         Return:
             True when the file full path should be excluded according config
         """
         path = path.replace('\\', '/').lower()
         if config.not_allowed_path_pattern.match(path):
             return True
-        if any(exclude_pattern.match(path) for exclude_pattern in config.exclude_patterns):
-            return True
-        if any(exclude_path in path for exclude_path in config.exclude_paths):
-            return True
+        for exclude_pattern in config.exclude_patterns:
+            if exclude_pattern.match(path):
+                return True
+        for exclude_path in config.exclude_paths:
+            if exclude_path in path:
+                return True
         file_extension = Util.get_extension(path, lower=False)
         if file_extension in config.exclude_extensions:
             return True
         if not config.depth and file_extension in config.exclude_containers:
             return True
         return False
 
-    @classmethod
-    def check_file_size(
-            cls,  #
-            config: Config,  #
-            reference: Union[str, Path, io.BytesIO, Tuple[Union[str, Path], io.BytesIO]]) -> bool:
+    @staticmethod
+    def check_file_size(config: Config, reference: Union[str, Path, io.BytesIO, Tuple[Union[str, Path],
+                                                                                      io.BytesIO]]) -> bool:
         """
-        Checks whether the file is oversize limit
+        Checks whether the file is over the size limit from configuration
 
         Args:
             config: Config
             reference: various types of a file reference
 
         Return:
             True when the file is oversize
```

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/files_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/patch_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/file_handler/text_provider.py` & `credsweeper-1.5.0/credsweeper/file_handler/text_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/filters/__init__.py` & `credsweeper-1.5.0/credsweeper/filters/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 from credsweeper.filters.filter import Filter  # isort:skip
 
+from credsweeper.filters.cred_card_number_check import CreditCardNumberCheck
 from credsweeper.filters.line_specific_key_check import LineSpecificKeyCheck
 from credsweeper.filters.separator_unusual_check import SeparatorUnusualCheck
 from credsweeper.filters.value_allowlist_check import ValueAllowlistCheck
 from credsweeper.filters.value_array_dictionary_check import ValueArrayDictionaryCheck
+from credsweeper.filters.value_base32_data_check import ValueBase32DataCheck
 from credsweeper.filters.value_blocklist_check import ValueBlocklistCheck
 from credsweeper.filters.value_camel_case_check import ValueCamelCaseCheck
+from credsweeper.filters.value_couple_keyword_check import ValueCoupleKeywordCheck
 from credsweeper.filters.value_dictionary_keyword_check import ValueDictionaryKeywordCheck
 from credsweeper.filters.value_dictionary_value_length_check import ValueDictionaryValueLengthCheck
+from credsweeper.filters.value_entropy_base32_check import ValueEntropyBase32Check
+from credsweeper.filters.value_entropy_base36_check import ValueEntropyBase36Check
 from credsweeper.filters.value_entropy_check import ValueEntropyCheck
 from credsweeper.filters.value_file_path_check import ValueFilePathCheck
 from credsweeper.filters.value_first_word_check import ValueFirstWordCheck
+from credsweeper.filters.value_grafana_check import ValueGrafanaCheck
+from credsweeper.filters.value_json_web_token_check import ValueJsonWebTokenCheck
 from credsweeper.filters.value_last_word_check import ValueLastWordCheck
 from credsweeper.filters.value_length_check import ValueLengthCheck
 from credsweeper.filters.value_method_check import ValueMethodCheck
 from credsweeper.filters.value_not_allowed_pattern_check import ValueNotAllowedPatternCheck
+from credsweeper.filters.value_number_check import ValueNumberCheck
 from credsweeper.filters.value_pattern_check import ValuePatternCheck
+from credsweeper.filters.value_pattern_length_check import ValuePatternLengthCheck
+from credsweeper.filters.value_pem_pattern_check import ValuePemPatternCheck
 from credsweeper.filters.value_similarity_check import ValueSimilarityCheck
+from credsweeper.filters.value_split_keyword_check import ValueSplitKeywordCheck
 from credsweeper.filters.value_string_type_check import ValueStringTypeCheck
+from credsweeper.filters.value_structured_token_check import ValueStructuredTokenCheck
+from credsweeper.filters.value_token_base32_check import ValueTokenBase32Check
+from credsweeper.filters.value_token_base36_check import ValueTokenBase36Check
 from credsweeper.filters.value_token_check import ValueTokenCheck
 from credsweeper.filters.value_useless_word_check import ValueUselessWordCheck
 from credsweeper.filters.variable_not_allowed_pattern_check import VariableNotAllowedPatternCheck
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/cred_card_number_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_number_check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,34 @@
+import re
+
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class CreditCardNumberCheck(Filter):
-    """Check that value is a credit card number."""
+class ValueNumberCheck(Filter):
+    """Check value if it a value in hex or decimal representation"""
+
+    HEX_VALUE_REGEX = re.compile("^(0x)?[0-9a-f]+[ul]*$")
+    DEC_VALUE_REGEX = re.compile("^-?[0-9]+[ul]*$")
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
-            False, if the sequence is not card number. True if it is
+            True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None \
-                or 16 != len(line_data.value) \
-                or ("0" == line_data.value[0] and "0" == line_data.value[1]):
+        if not line_data.value:
             return True
-        try:
-            s = 0
-            # https://en.wikipedia.org/wiki/Luhn_algorithm
-            for n in range(0, 16):
-                x = int(line_data.value[n])
-                if 0 == (1 & n):  # Only for odd numbers (with 0 as a start index)
-                    x *= 2
-                    if x > 9:
-                        x -= 9
-                s += x
-
-            if 0 == s % 10:
-                return False
-        except ValueError:
-            pass
-
-        # return False when the sequence is not a credit card number
-        return True
+        value = line_data.value.lower()
+        if 22 > len(value) and ValueNumberCheck.HEX_VALUE_REGEX.match(value):
+            return True
+        if ValueNumberCheck.DEC_VALUE_REGEX.match(value):
+            return True
+        return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/group/group.py` & `credsweeper-1.5.0/credsweeper/filters/group/group.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,50 +3,62 @@
 
 from credsweeper.common.constants import GroupType
 from credsweeper.config import Config
 from credsweeper.filters import (Filter, LineSpecificKeyCheck, SeparatorUnusualCheck, ValueAllowlistCheck,
                                  ValueArrayDictionaryCheck, ValueBlocklistCheck, ValueCamelCaseCheck,
                                  ValueFilePathCheck, ValueFirstWordCheck, ValueLastWordCheck, ValueLengthCheck,
                                  ValueMethodCheck, ValueNotAllowedPatternCheck, ValuePatternCheck, ValueSimilarityCheck,
-                                 ValueStringTypeCheck, ValueTokenCheck, VariableNotAllowedPatternCheck)
+                                 ValueStringTypeCheck, ValueTokenCheck, VariableNotAllowedPatternCheck,
+                                 ValuePatternLengthCheck)
 
 
 class Group(ABC):
+    """Abstract Group class"""
 
-    def __init__(self, config: Config, rule_type: GroupType) -> None:
+    def __init__(self, config: Config, rule_type: GroupType = GroupType.DEFAULT) -> None:
         if rule_type == GroupType.KEYWORD:
             self.filters: List[Filter] = self.get_keyword_base_filters(config)
         elif rule_type == GroupType.PATTERN:
             self.filters: List[Filter] = self.get_pattern_base_filters(config)
         else:
             self.filters: List[Filter] = []
 
     @property
     def filters(self) -> List[Filter]:
+        """property getter"""
         return self.__filters
 
     @filters.setter
     def filters(self, filters: List[Filter]) -> None:
+        """property setter"""
         self.__filters = filters
 
-    def get_keyword_base_filters(self, config: Config) -> List[Filter]:
-        return [
+    @staticmethod
+    def get_keyword_base_filters(config: Config) -> List[Filter]:
+        """returns base filters"""
+        return [  #
             SeparatorUnusualCheck(),
             ValueAllowlistCheck(),
             ValueArrayDictionaryCheck(),
             ValueBlocklistCheck(),
             ValueCamelCaseCheck(),
             ValueFilePathCheck(),
             ValueFirstWordCheck(),
             ValueLastWordCheck(),
-            ValueLengthCheck(config.min_keyword_value_length),
+            ValueLengthCheck(config),
             ValueMethodCheck(),
             ValueNotAllowedPatternCheck(),
             ValueSimilarityCheck(),
             ValueStringTypeCheck(config),
             ValueTokenCheck(),
             VariableNotAllowedPatternCheck(),
-            ValuePatternCheck()
+            ValuePatternCheck(config)
         ]
 
-    def get_pattern_base_filters(self, config: Config) -> List[Filter]:
-        return [LineSpecificKeyCheck(), ValuePatternCheck(), ValueLengthCheck(config.min_pattern_value_length)]
+    @staticmethod
+    def get_pattern_base_filters(config: Config) -> List[Filter]:
+        """return base filters for pattern"""
+        return [  #
+            LineSpecificKeyCheck(),  #
+            ValuePatternCheck(config),  #
+            ValuePatternLengthCheck(config)
+        ]
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.5.0/credsweeper/filters/group/url_credentials_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,32 @@
                                  ValueCamelCaseCheck, ValueDictionaryValueLengthCheck, ValueFilePathCheck,
                                  ValueFirstWordCheck, ValueLastWordCheck, ValueLengthCheck, ValueMethodCheck,
                                  ValueNotAllowedPatternCheck, ValuePatternCheck, ValueStringTypeCheck, ValueTokenCheck)
 from credsweeper.filters.group import Group
 
 
 class UrlCredentialsGroup(Group):
+    """UrlCredentialsGroup"""
 
     def __init__(self, config: Config) -> None:
         """URL credentials group class.
 
         Similar to PasswordKeyword, but exclude all checks dependent on the variable name, as URL credentials have no
         explicitly defined variable
         """
-        super().__init__(config, GroupType.KEYWORD)
+        super().__init__(config, GroupType.DEFAULT)
         self.filters = [
             ValueAllowlistCheck(),
             ValueArrayDictionaryCheck(),
             ValueBlocklistCheck(),
             ValueCamelCaseCheck(),
             ValueFilePathCheck(),
             ValueFirstWordCheck(),
             ValueLastWordCheck(),
-            ValueLengthCheck(config.min_keyword_value_length),
+            ValueLengthCheck(config),
             ValueMethodCheck(),
             ValueStringTypeCheck(config),
             ValueNotAllowedPatternCheck(),
             ValueTokenCheck(),
             ValueDictionaryValueLengthCheck(),
-            ValuePatternCheck()
+            ValuePatternCheck(config)
         ]
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.5.0/credsweeper/filters/line_specific_key_check.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class LineSpecificKeyCheck(Filter):
     """Check that values from list below is not in candidate line."""
 
     NOT_ALLOWED = ["example", "enc\\(", "enc\\[", "true", "false"]
-    NOT_ALLOWED_PATTERN = regex.compile(  #
+    NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
-        flags=regex.IGNORECASE)  # pylint: disable=no-member
+        flags=re.IGNORECASE)
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.5.0/credsweeper/filters/separator_unusual_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
 class SeparatorUnusualCheck(Filter):
     """Check that candidate have no double symbol ops (like ++, --, <<) or comparison ops (like != or ==) as separator.
 
     Example:
         `pwd == 'value'`
         `pwd != 'value'`
         `pwd << value`
 
     """
 
+    def __init__(self, config: Config = None) -> None:
+        pass
+
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.5.0/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
-class ValueAllowlistCheck(Filter):
-    """Check that patterns from the list is not present in the candidate value."""
+class VariableNotAllowedPatternCheck(Filter):
+    """Check if candidate variable is a regex placeholder or ends with match character (like + or >)."""
 
-    ALLOWED = [
-        "ENC\\(.*\\)", "ENC\\[.*\\]", "\\$\\{.*\\}", "#\\{.*\\}", "\\{\\{.+\\}\\}", "(\\w|\\d|\\.|->)+\\(.*\\)",
-        "\\*\\*\\*\\*\\*"
-    ]
-    ALLOWED_PATTERN = regex.compile(  #
-        Util.get_regex_combine_or(ALLOWED),  #
-        flags=regex.IGNORECASE)  # pylint: disable=no-member
+    NOT_ALLOWED = ["^([<]|\\{\\{).*", "(\\@.*)", "[!><+*/^|)](\\s)?$", ".*(public|pubkey)"]
+    NOT_ALLOWED_PATTERN = re.compile(  #
+        Util.get_regex_combine_or(NOT_ALLOWED),  #
+        flags=re.IGNORECASE)
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if line_data.variable is None:
             return True
 
-        if self.ALLOWED_PATTERN.match(line_data.value):
+        if self.NOT_ALLOWED_PATTERN.match(line_data.variable):
             return True
 
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_length_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-from regex import regex
-
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class ValueArrayDictionaryCheck(Filter):
-    """Match call to dictionary or array element.
-
-    This filter checks only calls, not declarations:
-        `token = values[i]` would be filtered
-        `token = {'root'}` would be kept
-    """
+class ValueLengthCheck(Filter):
+    """Check if potential candidate value is not too short (longer or equal to `min_len`)."""
 
-    PATTERN = regex.compile("\\[('|\")?.+('|\")?\\]")
+    def __init__(self, config: Config) -> None:
+        self.min_len = config.min_keyword_value_length
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
-
-        if self.PATTERN.search(line_data.value):
+        if len(line_data.value) < self.min_len:
             return True
-
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_blocklist_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
 class ValueBlocklistCheck(Filter):
     """Check that words from block list is lest that 70% of candidate value length."""
 
@@ -9,25 +10,28 @@
         "true",
         "false",
         "null",
         "bearer",
         "string",
     ]
 
+    def __init__(self, config: Config = None) -> None:
+        pass
+
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
 
         value = line_data.value.lower()
         for not_allowed in self.NOT_ALLOWED:
             if not_allowed in value and len(not_allowed) / len(value) >= 0.7:
                 return True
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_camel_case_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueCamelCaseCheck(Filter):
     """Check that candidate is not written in camel case."""
 
     CAMEL_CASE = ["^([a-z]+([A-Z][a-z]+)+)$", "^([A-Z][a-z]+([A-Z][a-z]+)+)$"]
-    CAMEL_CASE_PATTERN = regex.compile(Util.get_regex_combine_or(CAMEL_CASE))
+    CAMEL_CASE_PATTERN = re.compile(Util.get_regex_combine_or(CAMEL_CASE))
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
 
         if self.CAMEL_CASE_PATTERN.match(line_data.value):
             return True
 
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
 class ValueDictionaryValueLengthCheck(Filter):
     """Check that candidate length is between 5 and 30."""
 
+    def __init__(self, config: Config = None) -> None:
+        pass
+
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
         if len(line_data.value) < 4 or len(line_data.value) > 30:
             return True
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_entropy_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_entropy_base32_check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,42 @@
+import math
+
+from credsweeper.common.constants import Chars
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
-class ValueEntropyCheck(Filter):
-    """Check that candidate have Shanon Entropy > 3 (for HEX_CHARS or BASE36_CHARS) or > 4.5 (for BASE64_CHARS)."""
+class ValueEntropyBase32Check(Filter):
+    """Check that candidate have Shanon Entropy (for [a-z0-9])"""
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
-        return not Util.is_entropy_validate(line_data.value)
+        entropy = Util.get_shannon_entropy(line_data.value, Chars.BASE32_CHARS.value)
+        min_entropy = ValueEntropyBase32Check.get_min_data_entropy(len(line_data.value))
+        return min_entropy > entropy
+
+    @staticmethod
+    def get_min_data_entropy(x: int) -> float:
+        """Returns average entropy for size of random data. Precalculated data is applied for speedup"""
+        if 16 == x:
+            y = 3.46
+        elif 10 <= x:
+            # approximation does not exceed stdev
+            y = 0.64 * math.log2(x) + 0.9
+        else:
+            y = 0
+        return y
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_last_word_check.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+import re
+
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class ValueFilePathCheck(Filter):
-    r"""Check that candidate value is a path or not.
+class ValueLastWordCheck(Filter):
+    """Check that secret is not short value that ends with `:`."""
+
+    NOT_ALLOWED_COLON_PATTERN = re.compile(".*:$", flags=re.IGNORECASE)
 
-    Check if a value contains either '/' or ':\' separators (but not both)
-    and do not have any special characters ( !$`&*()+)
-    """
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
-        contains_unix_separator = '/' in line_data.value
-        contains_windows_separator = ':\\' in line_data.value
-        contains_special_characters = any(c in line_data.value for c in " !$`&*()+")
-        if (contains_unix_separator ^ contains_windows_separator) and not contains_special_characters:
+        if len(line_data.value) < 16 and self.NOT_ALLOWED_COLON_PATTERN.search(line_data.value):
             return True
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_first_word_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueFirstWordCheck(Filter):
     """Check that secret doesn't starts with special character."""
 
     NOT_ALLOWED = [
         "\\=", "\\{", "\\)", "\\<", "\\>", "\\#", "\\:", "\\\\", "\\/\\/", "\\_", "\\\\[u]", "\\/\\*", "\\%[deflspuvxz]"
     ]
-    NOT_ALLOWED_PATTERN = regex.compile(  #
+    NOT_ALLOWED_PATTERN = re.compile(  #
         f"^{Util.get_regex_combine_or(NOT_ALLOWED)}",  #
-        flags=regex.IGNORECASE)  # pylint: disable=no-member
+        flags=re.IGNORECASE)
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
         if self.NOT_ALLOWED_PATTERN.match(line_data.value):
             return True
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_length_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from credsweeper.common import static_keyword_checklist
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class ValueLengthCheck(Filter):
-    """Check if potential candidate value is not too short (longer or equal to `min_len`)."""
+class ValueDictionaryKeywordCheck(Filter):
+    """Check that no word from dictionary present in the candidate value."""
 
-    def __init__(self, min_len) -> None:
-        self.min_len = min_len
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
-            return True
-        if len(line_data.value) < self.min_len:
+        if not line_data.value:
             return True
+        line_data_value_lower = line_data.value.lower()
+        for keyword in static_keyword_checklist.keyword_set:
+            if keyword in line_data_value_lower:
+                return True
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_method_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_array_dictionary_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class ValueMethodCheck(Filter):
-    """Check if potential candidate value is a function.
+class ValueArrayDictionaryCheck(Filter):
+    """Match call to dictionary or array element.
 
-    Check if potential candidate value is a function by looking for '(', ')' or 'function' sub-strings in it
+    This filter checks only calls, not declarations:
+        `token = values[i]` would be filtered
+        `token = {'root'}` would be kept
     """
 
-    PATTERN = regex.compile(".*\\(.*\\).*")
+    PATTERN = re.compile("\\[('|\")?.+('|\")?\\]")
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
-        if "function" in line_data.value or self.PATTERN.search(line_data.value):
+
+        if self.PATTERN.search(line_data.value):
             return True
+
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueNotAllowedPatternCheck(Filter):
     """Check that secret doesn't open or closes brackets or a new line."""
 
     NOT_ALLOWED = ["[,<>{};\\]\\[](\\s)*", "(\\s)+[\\\\]", "(\\\\n)(\\s)*"]
-    NOT_ALLOWED_PATTERN = regex.compile(  #
+    NOT_ALLOWED_PATTERN = re.compile(  #
         f"{Util.get_regex_combine_or(NOT_ALLOWED)}$",  #
-        flags=regex.IGNORECASE)  # pylint: disable=no-member
+        flags=re.IGNORECASE)
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
         if self.NOT_ALLOWED_PATTERN.search(line_data.value):
             return True
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_pattern_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
-DEFAULT_PATTERN_LEN = 4
-
 
 class ValuePatternCheck(Filter):
     """Check if candidate value contain specific pattern.
 
     Similar to linguistic sequences of characters, random strings shouldn't contain math sequences of
     characters. Based on "How Bad Can It Git? Characterizing Secret Leakage in Public GitHub Repositories", details:
     https://www.ndss-symposium.org/ndss-paper/how-bad-can-it-git-characterizing-secret-leakage-in-public-github-repositories/
@@ -17,35 +16,35 @@
     - N or more identical characters in sequence, example: "AAAA", "1111" ...
     - N or more increasing characters sequentially, example: "abcd", "1234" ...
     - N or more decreasing characters sequentially, example: "dcba", "4321" ...
 
     Default pattern LEN is 4
     """
 
-    def __init__(self, pattern_len: int = DEFAULT_PATTERN_LEN):
+    def __init__(self, config: Config):
         """Create ValuePatternCheck with a specific pattern_len to check.
 
         Args:
-            pattern_len: pattern len to use during check. DEFAULT_PATTERN_LEN by default
+            config: pattern len to use during check. DEFAULT_PATTERN_LEN by default
 
         """
-        self.pattern_len = pattern_len
+        self.pattern_len = config.pattern_len
 
     def equal_pattern_check(self, line_data_value: str) -> bool:
         """Check if candidate value contain 4 and more same chars or numbers sequences.
 
         Args:
             line_data_value: string variable, credential candidate value
 
         Return:
             True if contain and False if not
 
         """
         pattern_string = "(.)\\1{" + str(self.pattern_len - 1) + ",}"
-        if regex.findall(pattern_string, line_data_value):
+        if re.findall(pattern_string, line_data_value):
             return True
         return False
 
     def ascending_pattern_check(self, line_data_value: str) -> bool:
         """Check if candidate value contain 4 and more ascending chars or numbers sequences.
 
         Arg:
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_similarity_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
 class ValueSimilarityCheck(Filter):
     """Check if candidate value is at least 70% same as candidate keyword. Like: `secret = "mysecret"`."""
 
+    def __init__(self, config: Config = None) -> None:
+        pass
+
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_grafana_check.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,42 @@
+import base64
+import contextlib
+import json
+
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
-class ValueStringTypeCheck(Filter):
-    r"""Check if line_data is in source code file that require quotes for string declaration.
-
-    If it is, then checks if line_data really have string literal declaration.
-    Comment rows in source files (start with //, /\*, etc) ignored.
-
-    True if:
+class ValueGrafanaCheck(Filter):
+    """Grafana Provisioned API Key and Access Policy Token"""
 
-    - line_data have no value
-    - line_data have no path
-    - line_data is in source code file (.cpp, .py, etc.) and is not comment
-      and contain no quotes (so no string literal declared)
-
-    False otherwise
-    """
-
-    def __init__(self, config: Config) -> None:
-        self.config = config
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
-        """Run filter checks on received credential candidate data 'line_data'.
+        """Run filter checks on received token which might be structured.
 
         Args:
             line_data: credential candidate data
 
         Return:
-            True, if need to filter candidate and False if left
+            True, when need to filter candidate and False if left
 
         """
-        if not self.config.check_for_literals:
-            return False
-
-        if line_data.value is None:
+        if not line_data.value:
             return True
-
-        if line_data.path is None:
-            return True
-
-        not_quoted = not line_data.value_leftquote and not line_data.value_rightquote
-        not_comment = not line_data.is_comment()
-
-        if line_data.is_source_file_with_quotes() and not_comment and not_quoted:
-            return True
-
-        return False
+        with contextlib.suppress(Exception):
+            if line_data.value.startswith("glc_"):
+                # Grafana Access Policy Token
+                decoded = base64.b64decode(line_data.value[4:])
+                keys = ["o", "n", "k", "m"]
+            else:
+                # Grafana Provisioned API Key
+                decoded = base64.b64decode(line_data.value)
+                keys = ["n", "k", "id"]
+            if payload := json.loads(decoded):
+                for key in keys:
+                    if key not in payload:
+                        return True
+                return False
+        return True
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_token_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_token_check.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 
 
 class ValueTokenCheck(Filter):
     """Check if first substring of token is shorter than 5.
 
@@ -13,28 +14,31 @@
         "my password"
         "12);password"
 
     """
 
     SPLIT_PATTERN = " |;|\\)|\\(|{|}|<|>|\\[|\\]|`"
 
+    def __init__(self, config: Config = None) -> None:
+        pass
+
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
 
-        tokens = regex.split(self.SPLIT_PATTERN, line_data.value, maxsplit=1)
+        tokens = re.split(self.SPLIT_PATTERN, line_data.value, maxsplit=1)
         # If tokens have length of 1 - pattern is not present in the value and original value returned from `.split(`
         if len(tokens) < 2:
             return False
 
         token = tokens[0]
         if len(token) < 5:
             return True
```

### Comparing `credsweeper-1.4.9/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.5.0/credsweeper/filters/value_useless_word_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-from regex import regex
+import re
 
+from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.filters import Filter
 from credsweeper.utils import Util
 
 
 class ValueUselessWordCheck(Filter):
     """Check is candidate value contains sub-rows with operators (like ->)."""
 
     NOT_ALLOWED = [
         "((\\{)?(0x)+([0-9a-f]|\\%){1}.*)",  # Check is contain \{0x or 0x
         "(\\-\\>.*)",  # Check if contain ->
         "(xxxx.*)",  # Check if contain xxxxx
         "(\\s).*"  # Check if contain \s
     ]
-    NOT_ALLOWED_PATTERN = regex.compile(  #
+    NOT_ALLOWED_PATTERN = re.compile(  #
         Util.get_regex_combine_or(NOT_ALLOWED),  #
-        flags=regex.IGNORECASE)  # pylint: disable=no-member
+        flags=re.IGNORECASE)
+
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
 
         Return:
             True, if need to filter candidate and False if left
 
         """
-        if line_data.value is None:
+        if not line_data.value:
             return True
 
         if self.NOT_ALLOWED_PATTERN.match(line_data.value):
             return True
 
         return False
```

### Comparing `credsweeper-1.4.9/credsweeper/logger/logger.py` & `credsweeper-1.5.0/credsweeper/logger/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import logging.config
 from pathlib import Path
 from typing import Optional
 
-from credsweeper import CREDSWEEPER_DIR
+from credsweeper.app import APP_PATH
 from credsweeper.utils import Util
 
 
 class Logger:
     """Class that used to configure logging in CredSweeper."""
 
     SILENCE = 60
@@ -37,15 +37,15 @@
         """
         try:
             level = Logger.LEVELS.get(log_level.upper())
             if level is None:
                 raise ValueError(f"log level given: {log_level} -- must be one of: {' | '.join(Logger.LEVELS.keys())}")
             logging_config = Util.yaml_load(file_path) if file_path else None
             if not logging_config:
-                logging_config = Util.yaml_load(str(CREDSWEEPER_DIR / "secret" / "log.yaml"))
+                logging_config = Util.yaml_load(APP_PATH / "secret" / "log.yaml")
             log_dir = Path(logging_config["handlers"]["logfile"]["filename"]).resolve().parent
             log_dir.mkdir(exist_ok=True)
             logging_config["handlers"]["console"]["level"] = level
             logging.config.dictConfig(logging_config)
             for module in logging_config["ignore"]:
                 logging.getLogger(module).setLevel(logging.ERROR)
         except (IOError, OSError):
```

### Comparing `credsweeper-1.4.9/credsweeper/ml_model/features.py` & `credsweeper-1.5.0/credsweeper/ml_model/features.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,95 +10,130 @@
 from credsweeper.common.constants import Base, Chars
 from credsweeper.credentials import Candidate
 
 
 class Feature(ABC):
     """Base class for features."""
 
+    def __init__(self):
+        self.__words: List[str] = []  # type: ignore
+
     def __call__(self, candidates: List[Candidate]) -> List[bool]:
         """Call base class for features.
 
         Args:
             candidates: list of candidates to extract features
 
         """
         return [self.extract(candidate) for candidate in candidates]
 
     @abstractmethod
     def extract(self, candidate: Candidate) -> Any:
         """Abstract method of base class"""
         raise NotImplementedError
 
+    @property
+    def words(self) -> List[str]:
+        """getter"""
+        return self.__words
+
+    @words.setter
+    def words(self, words: List[str]) -> None:
+        """setter - MUST BE IN LOWER CASE"""
+        self.__words = words
+
+    def any_word_in_(self, lower_case_line: str) -> bool:
+        """Returns true if any words in first line"""
+        for i in self.words:
+            if i in lower_case_line:
+                return True
+        return False
+
 
 class WordInSecret(Feature):
     """Feature returns true if candidate value contains at least one word from predefined list."""
 
     def __init__(self, words: List[str]) -> None:
         """Feature is true if candidate value contains at least one predefined word.
 
         Args:
-            words: list of predefined words
+            words: list of predefined words - MUST BE IN LOWER CASE
 
         """
+        super().__init__()
         self.words = words
 
     def extract(self, candidate: Candidate) -> bool:
-        return any(w.lower() in candidate.line_data_list[0].value.lower() for w in self.words)
+        """Returns true if any words in first line"""
+        return self.any_word_in_(candidate.line_data_list[0].value.lower())
 
 
 class WordInLine(Feature):
     """Feature is true if line contains at least one word from predefined list."""
 
     def __init__(self, words: List[str]) -> None:
         """Feature is true if line contains at least one predefined word.
 
         Args:
-            words: list of predefined words
+            words: list of predefined words - MUST BE IN LOWER CASE
 
         """
+        super().__init__()
         self.words = words
 
     def extract(self, candidate: Candidate) -> bool:
-        return any(w.lower() in candidate.line_data_list[0].line.lower() for w in self.words)
+        """Returns true if any words in first line"""
+        return self.any_word_in_(candidate.line_data_list[0].line.lower())
 
 
 class WordInPath(Feature):
     """Feature is true if candidate path contains at least one word from predefined list."""
 
     def __init__(self, words: List[str]) -> None:
         """Feature is true if candidate path contains at least one predefined word.
 
         Args:
-            words: list of predefined words
+            words: list of predefined words - MUST BE IN LOWER CASE
 
         """
+        super().__init__()
         self.words = words
 
     def extract(self, candidate: Candidate) -> bool:
-        return any(c.lower() in candidate.line_data_list[0].path.lower() for c in self.words)
+        """Returns true if any words in first line"""
+        return self.any_word_in_(candidate.line_data_list[0].path.lower())
 
 
 class HasHtmlTag(Feature):
     """Feature is true if line has HTML tags (HTML file)."""
 
     def __init__(self) -> None:
-        self.word_in_line = WordInLine(
-            ['< img', '<img', '< script', '<script', '< p', '<p', '< link', '<link', '< meta', '<meta', '< a', '<a'])
+        super().__init__()
+        self.words = [
+            '< img', '<img', '< script', '<script', '< p', '<p', '< link', '<link', '< meta', '<meta', '< a', '<a'
+        ]
 
     def extract(self, candidate: Candidate) -> bool:
-        tag_closings = ["<", "/>"]
-        return self.word_in_line.extract(candidate) | all(c in candidate.line_data_list[0].line for c in tag_closings)
+        candidate_line_data_list_0_line_lower = candidate.line_data_list[0].line.lower()
+        if self.any_word_in_(candidate_line_data_list_0_line_lower):
+            return True
+        for i in ["<", "/>"]:
+            if i not in candidate_line_data_list_0_line_lower:
+                return False
+        return True
 
 
 class PossibleComment(Feature):
     r"""Feature is true if candidate line starts with #,\*,/\*? (Possible comment)."""
 
     def extract(self, candidate: Candidate) -> bool:
-        comment_symbols = ["#", "*", "/*"]
-        return any(candidate.line_data_list[0].line.startswith(s) for s in comment_symbols)
+        for i in ["#", "*", "/*"]:
+            if candidate.line_data_list[0].line.startswith(i):
+                return True
+        return False
 
 
 class IsSecretNumeric(Feature):
     """Feature is true if candidate value is a numerical value."""
 
     def extract(self, candidate: Candidate) -> bool:
         try:
@@ -132,14 +167,15 @@
 
         Args:
             base: number base type
             alpha: entropy parameter
             norm: set True to normalize output probabilities, default is False
 
         """
+        super().__init__()
         self.base: Base = getattr(Base, base)
         self.alpha = alpha
         self.norm = norm
 
     def extract(self, candidate: Candidate) -> np.ndarray:
         p_x = self.get_probabilities(candidate.line_data_list[0].value)
         return np.array([self.estimate_entropy(p_x)])
@@ -199,14 +235,15 @@
 
     Parameters:
         extensions: extension labels
 
     """
 
     def __init__(self, extensions: List[str]) -> None:
+        super().__init__()
         self.extensions = extensions
 
     def __call__(self, candidates: List[Candidate]) -> csr_matrix:
         enc = LabelBinarizer()
         enc.fit(self.extensions)
         extensions = [candidate.line_data_list[0].file_type for candidate in candidates]
         return enc.transform(extensions)
@@ -220,14 +257,15 @@
 
     Parameters:
         rule_names: rule name labels
 
     """
 
     def __init__(self, rule_names: List[str]) -> None:
+        super().__init__()
         self.rule_names = rule_names
 
     def __call__(self, candidates: List[Candidate]) -> csr_matrix:
         enc = LabelBinarizer()
         enc.fit(self.rule_names)
         rule_names = [candidate.rule_name for candidate in candidates]
         return enc.transform(rule_names)
```

### Comparing `credsweeper-1.4.9/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.5.0/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.5.0/credsweeper/ml_model/ml_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,14 +124,20 @@
 
         common_features = self.extract_common_features(candidates)
         unique_features = self.extract_unique_features(candidates)
         feature_array = np.hstack([common_features, unique_features])
         feature_array = np.array([feature_array])
         return line_input, feature_array
 
+    def _batch_call_model(self, line_inputs, feature_array_list):
+        """auxiliary method to invoke twice"""
+        line_inputs_stack = np.vstack(line_inputs)
+        feature_array_vstack = np.vstack(feature_array_list)
+        return self._call_model(line_inputs_stack, feature_array_vstack)[:, 0]
+
     def validate_groups(self, group_list: List[Tuple[str, List[Candidate]]],
                         batch_size: int) -> Tuple[np.ndarray, np.ndarray]:
         """Use ml model on list of candidate groups.
 
         Args:
             group_list: List of tuples (value, group)
             batch_size: ML model batch
@@ -139,24 +145,27 @@
         Return:
             Boolean numpy array with decision based on the threshold,
             and numpy array with probability predicted by the model
 
         """
         line_input_list = []
         features_list = []
+        probability = np.zeros(len(group_list))
+        head = tail = 0
         for (value, candidates) in group_list:
             line_input, feature_array = self.get_group_features(value, candidates)
             line_input_list.append(line_input)
             features_list.append(feature_array)
-
-        probability = np.zeros(len(features_list))
-        for i in range(0, len(features_list), batch_size):
-            line_inputs = line_input_list[i:i + batch_size]
-            line_inputs_stack = np.vstack(line_inputs)
-            feature_array_list = features_list[i:i + batch_size]
-            feature_array_vstack = np.vstack(feature_array_list)
-            probability[i:i + batch_size] = self._call_model(line_inputs_stack, feature_array_vstack)[:, 0]
+            tail += 1
+            if 0 == tail % batch_size:
+                # use the approach to reduce memory consumption for huge candidates list
+                probability[head:tail] = self._batch_call_model(line_input_list, features_list)
+                head = tail
+                line_input_list.clear()
+                features_list.clear()
+        if head != tail:
+            probability[head:tail] = self._batch_call_model(line_input_list, features_list)
         is_cred = probability > self.threshold
         for i in range(len(is_cred)):
             logger.debug("ML decision: %s with prediction: %s for value: %s", is_cred[i], round(probability[i], 3),
                          group_list[i][0])
         return is_cred, probability
```

### Comparing `credsweeper-1.4.9/credsweeper/ml_model/model_config.json` & `credsweeper-1.5.0/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/rules/rule.py` & `credsweeper-1.5.0/credsweeper/rules/rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,139 @@
-from typing import Dict, List, Optional
+import logging
+import re
+from functools import cached_property
+from typing import Dict, List, Optional, Union
 
-from regex import regex
-
-from credsweeper import validations
-from credsweeper.common.constants import RuleType, Severity
+from credsweeper import validations, filters
+from credsweeper.common.constants import RuleType, Severity, MAX_LINE_LENGTH
 from credsweeper.config import Config
 from credsweeper.filters import Filter, group
+from credsweeper.filters.group import Group
 from credsweeper.utils import Util
 from credsweeper.validations import Validation
 
+logger = logging.getLogger(__name__)
+
 
 class Rule:
     """Regular expression to detect some credential type.
 
     Class contains regular expression to detect some credential type, credential name, assumed severity
         and details on how detection should be processed
 
     Parameters:
         rule_name: Name displayed if rule
         rule_type: RuleType used for this rule
         severity: critical/high/medium/low
-        filters: List of Filter objects that can be used to filters False detections based on rules
+        filters: List of Filter OR _one_ filter Group that can be used to filters False detections based on rules
         patterns: Regular expressions that can be used for detection
         pattern_type: single_pattern/multi_pattern/pem_key_pattern. single_pattern for simple single line credentials
           multi_pattern for credentials span for rew lines. pem_key_pattern for PEM like credentials
         use_ml: Should ML work on this credential or not. If not prediction based on regular expression and filter only
         validations: List of Validation objects that can check this credential using external API
         required_substrings: Optional list of substrings. Scanner would only apply this rule if line contain at least
           one of this substrings
         min_line_len: Optional minimal line length. Scanner would only apply this rule if line is equal or longer
+        usage_list: List of analyze types. There are 2 different analyze type now ("src", "doc")
 
     """
 
     SINGLE_PATTERN = "single_pattern"
     MULTI_PATTERN = "multi_pattern"
     PEM_KEY_PATTERN = "pem_key_pattern"
 
-    def __init__(self, config: Config, rule_template: Dict) -> None:
+    # mandatory fields
+    NAME = "name"
+    SEVERITY = "severity"
+    TYPE = "type"
+    USAGE_LIST = "usage_list"
+    VALUES = "values"
+    FILTER_TYPE = "filter_type"
+
+    # auxiliary fields
+    USE_ML = "use_ml"
+    REQUIRED_SUBSTRINGS = "required_substrings"
+    VALIDATIONS = "validations"
+    MIN_LINE_LEN = "min_line_len"
+
+    def __init__(self, config: Config, rule_dict: Dict) -> None:
         self.config = config
-        self._assert_all_rule_fields(rule_template)
-        self.rule_name: Optional[str] = rule_template["name"]
-        _rule_template_type = rule_template["type"]
-        self.rule_type: Optional[RuleType] = getattr(RuleType, _rule_template_type.upper(), None)
-        if self.rule_type is None:
-            raise ValueError(f"Malformed rule config file. Rule type '{_rule_template_type}' is invalid.")
-        self.severity: Severity = rule_template["severity"]
-        self.filters: List[Filter] = rule_template.get("filter_type")
-        self.patterns: List[regex.Pattern] = Rule._get_patterns(self.rule_type, rule_template["values"])
-        self.pattern_type: str = Rule._get_pattern_type(self.rule_type, len(self.patterns))
-        self.use_ml: bool = rule_template["use_ml"]
-        self.validations: List[Validation] = rule_template.get("validations")
-        self.required_substrings: List[str] = [s.lower() for s in rule_template.get("required_substrings", [""])]
-        self.min_line_len: int = rule_template.get("min_line_len", -1)
+        self._assert_rule_mandatory_fields(rule_dict)
+        # mandatory fields
+        self.__rule_name = str(rule_dict[Rule.NAME])
+        if severity := Severity.get(rule_dict[Rule.SEVERITY]):
+            self.__severity = severity
+        else:
+            self._malformed_rule_error(rule_dict, Rule.SEVERITY)
+        if rule_type := getattr(RuleType, str(rule_dict[Rule.TYPE]).upper(), None):
+            self.__rule_type: RuleType = rule_type
+        else:
+            self._malformed_rule_error(rule_dict, Rule.TYPE)
+        self.__patterns = Rule._get_patterns(self.rule_type, rule_dict[Rule.VALUES])
+        # auxiliary fields
+        self.__filters = self._get_filters(rule_dict.get(Rule.FILTER_TYPE))
+        self.__pattern_type = Rule._get_pattern_type(self.rule_type, len(self.patterns))
+        self.__use_ml = bool(rule_dict.get(Rule.USE_ML))
+        self.__validations = self._get_validations(rule_dict.get(Rule.VALIDATIONS))
+        self.__required_substrings = [i.strip().lower() for i in rule_dict.get(Rule.REQUIRED_SUBSTRINGS, [])]
+        self.__min_line_len = int(rule_dict.get(Rule.MIN_LINE_LEN, MAX_LINE_LENGTH))
+        self.__usage_list: List[str] = rule_dict.get(Rule.USAGE_LIST, [])
+
+    def _malformed_rule_error(self, rule_dict: Dict, field: str):
+        raise ValueError(f"Malformed rule '{self.__rule_name}'."
+                         f" field '{field}' has invalid value"
+                         f" '{rule_dict.get(field)}'")
 
-    @property
+    @cached_property
     def rule_name(self) -> str:
         """rule_name getter"""
         return self.__rule_name
 
-    @rule_name.setter
-    def rule_name(self, rule_name: str) -> None:
-        """rule_name setter"""
-        self.__rule_name = rule_name
-
-    @property
+    @cached_property
     def rule_type(self) -> RuleType:
         """rule_type getter"""
         return self.__rule_type
 
-    @rule_type.setter
-    def rule_type(self, rule_type: RuleType) -> None:
-        """rule_type getter"""
-        self.__rule_type = rule_type
-
-    @property
+    @cached_property
     def severity(self) -> Severity:
         """severity getter"""
         return self.__severity
 
-    @severity.setter
-    def severity(self, severity: str) -> None:
-        """severity setter"""
-        severity_obj: Severity = getattr(Severity, severity.upper(), None)
-        if severity_obj is None:
-            raise ValueError(f'Malformed rule config file. Rule severity "{severity}" is invalid.')
-        self.__severity = severity_obj
-
-    @property
+    @cached_property
     def filters(self) -> List[Filter]:
         """filters getter"""
         return self.__filters
 
-    @filters.setter
-    def filters(self, filter_type: str) -> None:
-        """filters setter"""
-        if filter_type == "" or filter_type is None:
-            self.__filters = []
-        else:
+    def _get_filters(self, filter_type: Union[None, str, List[str]]) -> List[Filter]:
+        """
+            filter_type: str - applies Group of filter
+                         list - creates specific set of Filters
+        """
+        if isinstance(filter_type, str):
+            # when string passed - (Group) of filters is applied
             filter_group = getattr(group, filter_type, None)
-            if filter_group is None:
-                raise ValueError(f'Malformed rule config file. Rule filter_type "{filter_type}" is invalid.')
-            self.__filters = filter_group(self.config).filters
+            if isinstance(filter_group, type) and issubclass(filter_group, Group):
+                return filter_group(self.config).filters  # type: ignore
+        elif isinstance(filter_type, list):
+            # list type means - list of (Filter)s is applied
+            filter_list = []
+            for i in filter_type:
+                _filter = getattr(filters, i, None)
+                if isinstance(_filter, type) and issubclass(_filter, Filter):
+                    filter_list.append(_filter(self.config))
+                else:
+                    break
+            else:
+                return filter_list
+        raise ValueError(f"Malformed rule '{self.__rule_name}'."
+                         f" field '{Rule.FILTER_TYPE}' has invalid value"
+                         f" '{filter_type}'")
 
     @staticmethod
-    def _get_patterns(_rule_type: RuleType, _values: List[str]) -> List[regex.Pattern]:
+    def _get_patterns(_rule_type: RuleType, _values: List[str]) -> List[re.Pattern]:
         """Get pattern values for rule object.
 
         Set the pattern value attribute of the rule object based on the passed values.
         So, if the received rule type corresponds to the RuleType.KEYWORD type,
         the "patterns" attribute is assigned the value of template keyword regex
         with the corresponding value. Otherwise, if the received rule type corresponds
         to the RuleType.PATTERN or RuleType.PEM_KEY types, the "patterns" attribute is
@@ -120,29 +146,24 @@
         """
         _patterns = []
         if RuleType.KEYWORD == _rule_type:
             for value in _values:
                 _patterns.append(Util.get_keyword_pattern(value))
         elif _rule_type in (RuleType.PATTERN, RuleType.PEM_KEY):
             for value in _values:
-                _patterns.append(regex.compile(value))
+                _patterns.append(re.compile(value))
         else:
             raise ValueError(f"Malformed rule config file. Rule type '{_rule_type}' is invalid.")
         return _patterns
 
-    @property
-    def patterns(self) -> List[regex.Pattern]:
+    @cached_property
+    def patterns(self) -> List[re.Pattern]:
         """patterns getter"""
         return self.__patterns
 
-    @patterns.setter
-    def patterns(self, _patterns: List[regex.Pattern]) -> None:
-        """patterns setter"""
-        self.__patterns = _patterns
-
     @staticmethod
     def _get_pattern_type(_rule_type: RuleType, _values_len: int) -> str:
         """Detect pattern type for rule object.
 
         Set the pattern_type attribute of the rule object based on the passed values.
         So, if the received rule type corresponds to the RuleType.PEM_KEY type,
         the class attribute is assigned the value "pem_key_pattern". Otherwise,
@@ -161,90 +182,82 @@
             _pattern_type = Rule.SINGLE_PATTERN
         elif 1 < _values_len:
             _pattern_type = Rule.MULTI_PATTERN
         else:
             raise ValueError(f"Malformed rule config file. Rule type '{_rule_type}' or '{_values_len}' are invalid.")
         return _pattern_type
 
-    @property
+    @cached_property
     def pattern_type(self) -> str:
         """pattern_type getter"""
         return self.__pattern_type
 
-    @pattern_type.setter
-    def pattern_type(self, _pattern_type: str) -> None:
-        """pattern_type setter"""
-        self.__pattern_type = _pattern_type
-
-    @property
+    @cached_property
     def use_ml(self) -> bool:
         """use_ml getter"""
         return self.__use_ml
 
-    @use_ml.setter
-    def use_ml(self, use_ml: bool) -> None:
-        """use_ml setter"""
-        if not isinstance(use_ml, bool):
-            raise ValueError('Malformed rule config file. Field "use_ml" should have a boolean value.')
-        self.__use_ml = use_ml
-
-    @property
+    @cached_property
     def validations(self) -> List[Validation]:
         """validations getter"""
         return self.__validations
 
-    @validations.setter
-    def validations(self, validation_names: List[str]) -> None:
+    def _get_validations(self, validation_names: Union[None, str, List[str]]) -> List[Validation]:
         """Set api validations to the current rule.
 
         All string in `validation_names` should be class names from `credsweeper.validations`
 
         Args:
             validation_names: validation names
 
         """
-        selected_validations = []
 
-        if validation_names is not None:
+        if not validation_names:
+            # empty string check to avoid exceptions for getattr
+            return []
+        elif isinstance(validation_names, str):
+            # more convenience way in case of single validator - only one line in YAML
+            if validation_template := getattr(validations, validation_names, None):
+                return [validation_template]
+        elif isinstance(validation_names, list):
+            selected_validations = []
             for vn in validation_names:
-                validation_template = getattr(validations, vn, None)
-                if validation_template is None:
-                    raise ValueError(f'Malformed rule config file. Validation "{vn}" is invalid.')
-                selected_validations.append(validation_template())
-
-        self.__validations = selected_validations
+                if validation_template := getattr(validations, vn, None):
+                    selected_validations.append(validation_template())
+                else:
+                    break
+            else:
+                return selected_validations
+        raise ValueError(f"Malformed rule '{self.__rule_name}'."
+                         f" field '{Rule.VALIDATIONS}' has invalid value"
+                         f" '{validation_names}'")
 
     @staticmethod
-    def _assert_all_rule_fields(rule_template: Dict) -> None:
+    def _assert_rule_mandatory_fields(rule_template: Dict) -> None:
         """Assert that rule_template have all required fields.
 
         Args:
             rule_template: dictionary loaded from the config file
 
         Raises:
             ValueError if missing fields is present
 
         """
-        required_fields = ["name", "severity", "type", "values", "use_ml"]
-        missing_fields = [field for field in required_fields if field not in rule_template]
+        mandatory_fields = [Rule.NAME, Rule.SEVERITY, Rule.TYPE, Rule.USAGE_LIST, Rule.VALUES, Rule.FILTER_TYPE]
+        missing_fields = [field for field in mandatory_fields if field not in rule_template]
         if len(missing_fields) > 0:
             raise ValueError(f"Malformed rule config file. Contain rule with missing fields: {missing_fields}.")
 
-    @property
+    @cached_property
     def required_substrings(self) -> List[str]:
         """required_substrings getter"""
         return self.__required_substrings
 
-    @required_substrings.setter
-    def required_substrings(self, required_substrings: List[str]) -> None:
-        """required_substrings setter"""
-        self.__required_substrings = required_substrings
-
-    @property
+    @cached_property
     def min_line_len(self) -> int:
         """min_line_len getter"""
         return self.__min_line_len
 
-    @min_line_len.setter
-    def min_line_len(self, min_line_len: int) -> None:
-        """min_line_len setter"""
-        self.__min_line_len = min_line_len
+    @cached_property
+    def usage_list(self) -> List[str]:
+        """usage_list getter"""
+        return self.__usage_list
```

### Comparing `credsweeper-1.4.9/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.5.0/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from credsweeper.common.constants import MAX_LINE_LENGTH
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.rules import Rule
 from credsweeper.scanner.scan_type import ScanType
 
 
@@ -31,15 +32,15 @@
                 present within MAX_SEARCH_MARGIN from the line. False otherwise
 
         """
         assert rule.pattern_type == rule.MULTI_PATTERN, \
             "Rules provided to MultiPattern.run should have pattern_type equal to MULTI_PATTERN"
 
         candidate = cls._get_candidate(config, rule, target)
-        if not isinstance(candidate, Candidate):
+        if not candidate:
             return None
 
         line_num_margin = 1
 
         while line_num_margin <= cls.MAX_SEARCH_MARGIN:
             if 1 <= candidate.line_data_list[0].line_num - line_num_margin <= len(target.lines):
                 if cls._scan(config, candidate, -line_num_margin, target, rule):
@@ -71,22 +72,18 @@
 
         Return:
             Boolean. True if second part detected. False otherwise
 
         """
         candi_line_num = candidate.line_data_list[0].line_num + line_num_margin
         candi_line = target.lines[candi_line_num - 1]
-
-        line_data = cls.get_line_data(config=config,
-                                      line=candi_line,
-                                      line_num=candi_line_num,
-                                      file_path=target.file_path,
-                                      file_type=target.file_type,
-                                      info=target.info,
-                                      pattern=rule.patterns[1],
-                                      filters=rule.filters)
+        if MAX_LINE_LENGTH < len(candi_line):
+            return False
+        # lines are not necessary - skip them
+        new_target = AnalysisTarget(candi_line, candi_line_num, [], target.file_path, target.file_type, target.info)
+        line_data = cls.get_line_data(config=config, target=new_target, pattern=rule.patterns[1], filters=rule.filters)
 
         if line_data is None:
             return False
 
         candidate.add_line_data(line_data)
         return True
```

### Comparing `credsweeper-1.4.9/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.5.0/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,21 @@
             Candidate object if pattern defined in a rule is present in a line and filters defined in rule do not
             remove current line. None otherwise
 
         """
         assert rule.pattern_type == rule.PEM_KEY_PATTERN, \
             "Rules provided to PemKeyPattern.run should have pattern_type equal to PEM_KEY_PATTERN"
 
-        if cls.is_pem_key(target.lines[target.line_num:]):
+        if cls.is_pem_key(target.lines[target.line_num:], config):
             return cls._get_candidate(config, rule, target)
 
         return None
 
     @classmethod
-    def is_pem_key(cls, lines: List[str]) -> bool:
+    def is_pem_key(cls, lines: List[str], config: Config) -> bool:
         """Check if provided lines is a PEM key.
 
         Args:
             lines: Lines to be checked
 
         Return:
             Boolean. True if PEM key, False otherwise
@@ -61,15 +61,15 @@
         for line_num, line in enumerate(lines):
             if line_num >= 190:
                 return False
             if "-----END" in line:
                 # Check if entropy is high enough
                 removed_by_entropy = not Util.is_entropy_validate(key_data)
                 # Check if have no substring with 5 same consecutive characters (like 'AAAAA')
-                pattern_check = ValuePatternCheck(5)
+                pattern_check = ValuePatternCheck(config)
                 removed_by_filter = pattern_check.equal_pattern_check(key_data)
                 not_removed = not (removed_by_entropy or removed_by_filter)
                 return not_removed
             # PEM key line should not contain spaces or . (and especially not ...)
             elif " " in line or "..." in line:
                 return False
             else:
@@ -121,13 +121,18 @@
         Return:
             List of strings without leading non-key lines
 
         """
         leading_lines = 0
 
         for line in lines:
-            if any(line.startswith(ignore_string) for ignore_string in cls.ignore_starts) or len(line) == 0:
+            if len(line) == 0:
                 leading_lines += 1
             else:
-                break
+                for ignore_string in cls.ignore_starts:
+                    if line.startswith(ignore_string):
+                        leading_lines += 1
+                        break
+                if not leading_lines:
+                    break
 
         return lines[leading_lines:]
```

### Comparing `credsweeper-1.4.9/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.5.0/credsweeper/scanner/scan_type/scan_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
+import re
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
-from regex import regex
-
-from credsweeper.common.constants import MAX_LINE_LENGTH
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate, LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.rules import Rule
 
 logger = logging.getLogger(__name__)
@@ -63,48 +61,42 @@
                 return True
         return False
 
     @classmethod
     def get_line_data(
             cls,  #
             config: Config,  #
-            line: str,  #
-            line_num: int,  #
-            file_path: str,  #
-            file_type: str,  #
-            info: str,  #
-            pattern: regex.Pattern,  #
+            target: AnalysisTarget,  #
+            pattern: re.Pattern,  #
             filters: List[Filter]) -> Optional[LineData]:
         """Check if regex pattern is present in line, and line should not be removed by filters.
 
         Args:
             config: dict of credsweeper configuration
-            line: Line to check
-            line_num: Line number of a current line
-            file_path: Path to the file that contain current line
-            file_type: Type of file in extension '.txt'
-            info: Extended info
+            target: AnalysisTarget with all necessary data
             pattern: Compiled regex object to be searched in line
             filters: Filters to use
 
         Return:
             LineData object if pattern a line and filters do not remove current line. None otherwise
 
         """
-        if not cls.is_valid_line(line, pattern, line_num, file_path):
+        if not cls.is_pattern_detected_line(target.line, pattern):
             return None
-        logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern, file_path, line_num, line)
-        line_data = LineData(config, line, line_num, file_path, file_type, info, pattern)
+        logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern, target.file_path,
+                     target.line_num, target.line)
+        line_data = LineData(config, target.line, target.line_num, target.file_path, target.file_type, target.info,
+                             pattern)
 
         if cls.filtering(config, line_data, filters):
             return None
         return line_data
 
     @classmethod
-    def is_pattern_detected_line(cls, line: str, pattern: regex.Pattern) -> bool:
+    def is_pattern_detected_line(cls, line: str, pattern: re.Pattern) -> bool:
         """Check if pattern present in the line.
 
         Args:
             line: Line to check
             pattern: Compiled regex object
 
         Return:
@@ -112,73 +104,30 @@
 
         """
         if pattern.search(line):
             return True
         return False
 
     @classmethod
-    def is_valid_line(cls, line: str, pattern: regex.Pattern, line_num: int = -1, file_path: str = None) -> bool:
-        """Check if line is not too long and pattern present in the line.
-
-        Args:
-            line: Line to check
-            pattern: Compiled regex object to be searched in line
-            line_num: Number of line in the file
-            file_path: Path to the file
-
-        Return:
-            Boolean. True if pattern is present and line is not too long. False otherwise
-
-        """
-        if cls.is_valid_line_length(line, line_num, file_path) and cls.is_pattern_detected_line(line, pattern):
-            return True
-        return False
-
-    @classmethod
-    def is_valid_line_length(cls, line: str, line_num: int = -1, file_path: str = None) -> bool:
-        """Check if line is not too long for the scanner.
-
-        Args:
-            line: Line to check
-            line_num: Number of line in the file
-            file_path: Path to the file
-
-        Return:
-            Boolean. True if line is not too long. False otherwise
-
-        """
-        if len(line) <= MAX_LINE_LENGTH:
-            return True
-        logger.warning(f"Oversize line in file: {file_path}:{line_num}")
-        return False
-
-    @classmethod
     def _get_candidate(cls, config: Config, rule: Rule, target: AnalysisTarget) -> Optional[Candidate]:
         """Returns Candidate object.
 
         Args:
             config: user configs
             rule: Rule object to check current line
 
         Return:
             Candidate object if pattern defined in a rule is present in a line and filters defined in rule do not
             remove current line. None otherwise
 
         """
-        if len(config.exclude_lines) > 0 and target.line.strip() in config.exclude_lines:
+        if config.exclude_lines and target.line.strip() in config.exclude_lines:
             return None
 
-        line_data = cls.get_line_data(config=config,
-                                      line=target.line,
-                                      line_num=target.line_num,
-                                      file_path=target.file_path,
-                                      file_type=target.file_type,
-                                      info=target.info,
-                                      pattern=rule.patterns[0],
-                                      filters=rule.filters)
+        line_data = cls.get_line_data(config=config, target=target, pattern=rule.patterns[0], filters=rule.filters)
 
         if line_data is None:
             return None
         if len(config.exclude_values) > 0 and line_data.value.strip() in config.exclude_values:
             return None
 
         return Candidate([line_data], rule.patterns, rule.rule_name, rule.severity, config, rule.validations,
```

### Comparing `credsweeper-1.4.9/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.5.0/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/scanner/scanner.py` & `credsweeper-1.5.0/credsweeper/scanner/scanner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
-import os
-from typing import List, Optional, Type, Tuple, Dict
+from pathlib import Path
+from typing import List, Optional, Type, Tuple, Dict, Union
 
+from credsweeper.app import APP_PATH
 from credsweeper.common.constants import RuleType, MIN_VARIABLE_LENGTH, MIN_SEPARATOR_LENGTH, MIN_VALUE_LENGTH, \
     MAX_LINE_LENGTH, Separator
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.rules import Rule
 from credsweeper.scanner.scan_type import MultiPattern, PemKeyPattern, ScanType, SinglePattern
@@ -24,35 +25,46 @@
         min_len: Smallest between min_pattern_len and min_keyword_len
         TargetGroup: Type for List[Tuple[AnalysisTarget, str, int]]
 
     """
 
     TargetGroup = List[Tuple[AnalysisTarget, str, int]]
 
-    def __init__(self, config: Config, rule_path: Optional[str]) -> None:
+    def __init__(self, config: Config, rule_path: Optional[str], usage_list: Optional[List[str]] = None) -> None:
         self.config = config
         self.__scanner_for_rule: Dict[str, Type[ScanType]] = {}
         self.rules: List[Rule] = []
         # init with MAX_LINE_LENGTH before _set_rules
+        self.min_keyword_len = MAX_LINE_LENGTH
         self.min_pattern_len = MAX_LINE_LENGTH
-        self._set_rules(rule_path)
-        self.min_len = min(self.min_pattern_len, MIN_VARIABLE_LENGTH + MIN_SEPARATOR_LENGTH + MIN_VALUE_LENGTH)
+        self.min_pem_key_len = MAX_LINE_LENGTH
+        self._set_rules(rule_path, usage_list if isinstance(usage_list, list) else ["src", "doc"])
+        self.min_len = min(self.min_pattern_len, self.min_keyword_len, self.min_pem_key_len,
+                           MIN_VARIABLE_LENGTH + MIN_SEPARATOR_LENGTH + MIN_VALUE_LENGTH)
 
-    def _set_rules(self, rule_path: Optional[str]) -> None:
+    def _set_rules(self, rule_path: Union[None, str, Path], usage_list: List[str]) -> None:
         """Auxiliary method to fill rules, determine min_pattern_len and set scanners"""
         if rule_path is None:
-            project_dir_path = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-            rule_path = os.path.join(project_dir_path, "rules", "config.yaml")
+            rule_path = APP_PATH / "rules" / "config.yaml"
         rule_templates = Util.yaml_load(rule_path)
         if rule_templates and isinstance(rule_templates, list):
             for rule_template in rule_templates:
                 rule = Rule(self.config, rule_template)
+                if not self._is_available(usage_list, rule):
+                    continue
                 self.rules.append(rule)
-                if rule.rule_type == RuleType.PATTERN:
-                    self.min_pattern_len = min(self.min_pattern_len, rule.min_line_len)
+                if 0 < rule.min_line_len:
+                    if rule.rule_type == RuleType.KEYWORD:
+                        self.min_keyword_len = min(self.min_keyword_len, rule.min_line_len)
+                    elif rule.rule_type == RuleType.PATTERN:
+                        self.min_pattern_len = min(self.min_pattern_len, rule.min_line_len)
+                    elif rule.rule_type == RuleType.PEM_KEY:
+                        self.min_pem_key_len = min(self.min_pem_key_len, rule.min_line_len)
+                    else:
+                        logger.warning(f"Unknown rule type:{rule.rule_type}")
                 self.__scanner_for_rule[rule.rule_name] = self.get_scanner(rule)
         else:
             raise RuntimeError(f"Wrong rules '{rule_templates}' were read from '{rule_path}'")
 
     def _select_and_group_targets(self, targets: List[AnalysisTarget]) -> Tuple[TargetGroup, TargetGroup, TargetGroup]:
         """Group targets into 3 lists based on loaded rules.
 
@@ -65,69 +77,93 @@
         """
         keyword_targets = []
         pattern_targets = []
         pem_targets = []
 
         for target in targets:
             # Ignore target if it's too long
-            if len(target.line) > MAX_LINE_LENGTH:
+            line_len = len(target.line)
+            if line_len > MAX_LINE_LENGTH:
+                logger.warning(f"Skipped oversize({line_len}) line in {target.file_path}:{target.line_num}", )
                 continue
             # Trim string from outer spaces to make future `a in str` checks faster
             target_line_trimmed = target.line.strip()
             target_line_trimmed_len = len(target_line_trimmed)
             # Ignore target if trimmed part is too short
             if target_line_trimmed_len < self.min_len:
                 continue
             target_line_trimmed_lower = target_line_trimmed.lower()
-            # Check if have at least one separator character. Otherwise cannot be matched by a keyword
-            if any(x in target_line_trimmed for x in Separator.common_as_set):
-                keyword_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
+            # check minimal length for keyword rule
+            if target_line_trimmed_len >= self.min_keyword_len:
+                # Check if have at least one separator character. Otherwise cannot be matched by a keyword
+                for x in Separator.common_as_set:
+                    if x in target_line_trimmed:
+                        keyword_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
+                        break
             # Check if have length not smaller than smallest `min_line_len` in all pattern rules
             if target_line_trimmed_len >= self.min_pattern_len:
                 pattern_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
             # Check if have "BEGIN" substring. Cannot otherwise ba matched as a PEM key
-            if "BEGIN" in target_line_trimmed:
+            if target_line_trimmed_len >= self.min_pem_key_len and "BEGIN" in target_line_trimmed:
                 pem_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
 
         return keyword_targets, pattern_targets, pem_targets
 
+    def _is_available(self, usage_list: List[str], rule: Rule) -> bool:
+        """separate the method to reduce complexity"""
+        if rule.severity < self.config.severity:
+            return False
+        for usage in usage_list:
+            if usage in rule.usage_list:
+                return True
+        return False
+
+    @staticmethod
+    def _required_substrings_not_present(required_substrings: List[str], line: str):
+        """ returns True if required substring absent in line """
+        for substring in required_substrings:
+            if substring in line:
+                return False
+        return True
+
     def scan(self, targets: List[AnalysisTarget]) -> List[Candidate]:
         """Run scanning of list of target lines from 'targets' with set of rule from 'self.rules'.
 
         Args:
-            targets: objects with data to analyse: line, line number,
+            targets: objects with data to analyze: line, line number,
               filepath and all lines in file
 
         Return:
-            list of all detected credential candidates in analysed targets
+            list of all detected credential candidates in analyzed targets
 
         """
-        credentials = []
+        credentials: List[Candidate] = []
+        if not targets:
+            # optimization for empty list
+            return credentials
         keyword_targets, pattern_targets, pem_targets = self._select_and_group_targets(targets)
         for rule in self.rules:
             min_line_len = rule.min_line_len
             required_substrings = rule.required_substrings
             scanner = self.__scanner_for_rule[rule.rule_name]
             to_check = self.get_targets_to_check(keyword_targets, pattern_targets, pem_targets, rule)
-            # It is almost two times faster to precompute values related to target_line than to compute them in
+            # It is almost two times faster to pre-compute values related to target_line than to compute them in
             # each iteration
             for target, target_line_trimmed_lower, target_line_trimmed_len in to_check:
-                if target_line_trimmed_len < min_line_len:
-                    continue
-                if not any(substring in target_line_trimmed_lower for substring in required_substrings):
+                if target_line_trimmed_len < min_line_len or required_substrings \
+                        and self._required_substrings_not_present(required_substrings, target_line_trimmed_lower):
                     continue
-                new_credential = scanner.run(self.config, rule, target)
-                if new_credential:
+                if new_credential := scanner.run(self.config, rule, target):
                     logger.debug("Credential for rule: %s in file: %s:%d in line: %s", rule.rule_name, target.file_path,
                                  target.line_num, target.line)
                     credentials.append(new_credential)
         return credentials
 
-    @classmethod
-    def get_scanner(cls, rule: Rule) -> Type[ScanType]:
+    @staticmethod
+    def get_scanner(rule: Rule) -> Type[ScanType]:
         """Choose type of scanner base on rule affiliation.
 
         Args:
             rule: rule object used to scanning
 
         Return:
             depending on the rule type, returns the corresponding scanner class
```

### Comparing `credsweeper-1.4.9/credsweeper/secret/config.json` & `credsweeper-1.5.0/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/secret/log.yaml` & `credsweeper-1.5.0/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/utils/util.py` & `credsweeper-1.5.0/credsweeper/utils/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import ast
 import json
 import logging
 import math
 import os
+import re
 import tarfile
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, List, Tuple, Optional, Any, Union
+from typing import Any, Dict, List, Tuple, Optional, Union
 
 import whatthepatch
 import yaml
 from lxml import etree
-from regex import regex
 from typing_extensions import TypedDict
 
 from credsweeper.common.constants import Chars, DiffRowType, KeywordPattern, Separator, AVAILABLE_ENCODINGS, \
-    DEFAULT_ENCODING
+    DEFAULT_ENCODING, LATIN_1
 
 logger = logging.getLogger(__name__)
 
 DiffDict = TypedDict(
     "DiffDict",
     {
         "old": Optional[int],  #
@@ -37,35 +37,33 @@
     line_numb: int
     line: str
 
 
 class Util:
     """Class that contains different useful methods."""
 
-    default_encodings: Tuple[str, ...] = AVAILABLE_ENCODINGS
-
     @staticmethod
     def get_extension(file_path: str, lower=True) -> str:
         """Return extension of file in lower case by default e.g.: '.txt', '.JPG'"""
         _, extension = os.path.splitext(str(file_path))
         return extension.lower() if lower else extension
 
     @staticmethod
-    def get_keyword_pattern(keyword: str, separator: str = Separator.common) -> regex.Pattern:
+    def get_keyword_pattern(keyword: str, separator: str = Separator.common) -> re.Pattern:
         """Returns compiled regex pattern"""
-        return regex.compile(KeywordPattern.key.format(keyword) + KeywordPattern.separator.format(separator) +
-                             KeywordPattern.value,
-                             flags=regex.IGNORECASE)  # pylint: disable=no-member
+        return re.compile(KeywordPattern.key.format(keyword) + KeywordPattern.separator.format(separator) +
+                          KeywordPattern.value,
+                          flags=re.IGNORECASE)
 
     @staticmethod
-    def get_regex_combine_or(regex_strs: List[str]) -> str:
+    def get_regex_combine_or(re_strs: List[str]) -> str:
         """Routine combination for regex 'or'"""
         result = "(?:"
 
-        for elem in regex_strs:
+        for elem in re_strs:
             result += elem + "|"
 
         if result[-1] == "|":
             result = result[:-1]
         result += ")"
 
         return result
@@ -86,75 +84,163 @@
     @staticmethod
     def get_shannon_entropy(data: str, iterator: str) -> float:
         """Borrowed from http://blog.dkbza.org/2007/05/scanning-data-for-entropy-anomalies.html."""
         if not data:
             return 0
 
         entropy = 0.
+        data_len = len(data)
         for x in iterator:
-            p_x = float(data.count(x)) / len(data)
+            p_x = float(data.count(x)) / data_len
             if p_x > 0:
                 entropy += -p_x * math.log(p_x, 2)
 
         return entropy
 
+    """Precalculated data for speedup"""
+    MIN_DATA_ENTROPY: Dict[int, float] = {
+        16: 1.66973671780348,
+        20: 2.07723544540831,
+        32: 3.25392803184602,
+        40: 3.64853567064867,
+        64: 4.57756933688035,
+    }
+
+    @staticmethod
+    def get_min_data_entropy(x: int) -> float:
+        """Returns minimal entropy for size of random data. Precalculated data is applied for speedup"""
+        if x in Util.MIN_DATA_ENTROPY:
+            y = Util.MIN_DATA_ENTROPY[x]
+        elif 8 < x < 64:
+            # approximated for range 12 - 64
+            _x = x - 8
+            y = ((0.000016617804 * _x - 0.002695077) * _x + 0.170393) * _x + 0.4
+        elif 64 < x:
+            # logarithm base 2 - slow, but precise
+            _x = x - 8
+            y = 1.581026279659 * math.log2(_x) - 1.90156
+        else:
+            # less or equal to 8 bytes might have 0 entropy
+            y = 0
+        return y
+
+    @staticmethod
+    def is_ascii_entropy_validate(data: bytes) -> bool:
+        """
+        Tests small data sequence (<256) for data randomness by testing for ascii and shannon entropy
+        Returns True when data is an ASCII symbols or have small entropy
+        """
+        if not data:
+            return True
+        data_len = len(data)
+        if 9 > data_len:
+            # even random data may have 0 entropy for length of 8 bytes and less
+            return True
+        entropy = 0.
+        cells = [int(0)] * 256
+        ascii_test = True
+        # "basket" sorting approach
+        for x in data:
+            cells[x] += 1
+            if ascii_test and 0b10000000 & x:
+                ascii_test = False
+        if ascii_test:
+            # only ascii symbols found
+            return True
+        left = 0.
+        step = 256.0 / data_len
+        right = left + step
+        while left < 256:
+            cell_sum = 0
+            i = int(left)
+            r = int(right)
+            while i < r and i < 256:
+                cell_sum += cells[i]
+                i += 1
+            p_x = float(cell_sum) / data_len
+            if p_x > 0:
+                entropy += -p_x * math.log2(p_x)
+            left = right
+            right += step
+        min_entropy = Util.get_min_data_entropy(data_len)
+        return entropy < min_entropy
+
     @staticmethod
-    def read_file(path: Union[str, Path], encodings: Tuple[str, ...] = default_encodings) -> List[str]:
+    def is_binary(data: bytes) -> bool:
+        """
+        Returns true if any recognized binary format found
+        or two zeroes sequence is found which never exists in text format (UTF-8, UTF-16)
+        UTF-32 is not supported
+        """
+        if Util.is_zip(data) \
+                or Util.is_gzip(data) \
+                or Util.is_tar(data) \
+                or Util.is_bzip2(data) \
+                or Util.is_pdf(data) \
+                or Util.is_elf(data):
+            return True
+        if b"\0\0" in data:
+            return True
+        return False
+
+    @staticmethod
+    def read_file(path: Union[str, Path], encodings: Optional[List[str]] = None) -> List[str]:
         """Read the file content using different encodings.
 
         Try to read the contents of the file according to the list of encodings "encodings" as soon as reading
         occurs without any exceptions, the data is returned in the current encoding
 
         Args:
             path: path to file
             encodings: supported encodings
 
         Return:
             list of file rows in a suitable encoding from "encodings",
             if none of the encodings match, an empty list will be returned
 
         """
-        file_data = []
-        for encoding in encodings:
-            try:
-                with open(path, "r", encoding=encoding) as file:
-                    file_data = file.read().split("\n")
-                break
-            except UnicodeError:
-                logger.info(f"UnicodeError: Can't read content from \"{path}\" as {encoding}.")
-            except Exception as exc:
-                logger.error(f"Unexpected Error: Can't read \"{path}\" as {encoding}. Error message: {exc}")
-        return file_data
+        data = Util.read_data(path)
+        return Util.decode_bytes(data, encodings)
 
     @staticmethod
-    def decode_bytes(content: bytes, encodings: Tuple[str, ...] = default_encodings) -> List[str]:
+    def decode_bytes(content: bytes, encodings: Optional[List[str]] = None) -> List[str]:
         """Decode content using different encodings.
 
         Try to decode bytes according to the list of encodings "encodings"
         occurs without any exceptions. UTF-16 requires BOM
 
         Args:
             content: raw data that might be text
             encodings: supported encodings
 
         Return:
             list of file rows in a suitable encoding from "encodings",
             if none of the encodings match, an empty list will be returned
+            Also empty list will be returned after last encoding and 0 symbol is present in lines not at end
 
         """
         lines = []
+        binary_suggest = False
+        if encodings is None:
+            encodings = AVAILABLE_ENCODINGS
         for encoding in encodings:
             try:
-                text = content.decode(encoding)
-                if content != text.encode(encoding):
+                if binary_suggest and LATIN_1 == encoding and Util.is_binary(content):
+                    # LATIN_1 may convert data (bytes in range 0x80:0xFF are transformed)
+                    # so skip this encoding when checking binaries
+                    logger.warning("Binary file detected")
+                    return []
+                text = content.decode(encoding, errors="strict")
+                if content != text.encode(encoding, errors="strict"):
                     raise UnicodeError
                 # windows style workaround
                 lines = text.replace('\r\n', '\n').replace('\r', '\n').split("\n")
                 break
             except UnicodeError:
+                binary_suggest = True
                 logger.info(f"UnicodeError: Can't decode content as {encoding}.")
             except Exception as exc:
                 logger.error(f"Unexpected Error: Can't read content as {encoding}. Error message: {exc}")
         return lines
 
     @staticmethod
     def patch2files_diff(raw_patch: List[str], change_type: DiffRowType) -> Dict[str, List[DiffDict]]:
@@ -228,32 +314,40 @@
             rows_data.append(DiffRowData(DiffRowType.DELETED, deleted_line_number, line))
         else:
             rows_data.append(DiffRowData(DiffRowType.ADDED_ACCOMPANY, added_line_number, line))
             rows_data.append(DiffRowData(DiffRowType.DELETED_ACCOMPANY, deleted_line_number, line))
         return rows_data
 
     @staticmethod
+    def wrong_change(change: DiffDict) -> bool:
+        """Returns True if the change is wrong"""
+        for i in ["line", "new", "old"]:
+            if i not in change:
+                logger.error(f"Skipping wrong change {change}")
+                return True
+        return False
+
+    @staticmethod
     def preprocess_file_diff(changes: List[DiffDict]) -> List[DiffRowData]:
         """Generate changed file rows from diff data with changed lines (e.g. marked + or - in diff).
 
         Args:
             changes: git diff by file rows data
 
         Return:
             diff rows data with as list of row change type, line number, row content
 
         """
-        if changes is None:
+        if not changes:
             return []
 
         rows_data = []
         # process diff to restore lines and their positions
         for change in changes:
-            if not all(x in change for x in ["line", "new", "old"]):
-                logger.error(f"Skipping wrong change {change}")
+            if Util.wrong_change(change):
                 continue
             line = change["line"]
             if isinstance(line, str):
                 rows_data.extend(Util.preprocess_diff_rows(change.get("new"), change.get("old"), line))
             elif isinstance(line, bytes):
                 logger.warning("The feature is available with the deep scan option")
             else:
@@ -319,15 +413,25 @@
         """According https://en.wikipedia.org/wiki/List_of_file_signatures - pdf"""
         if isinstance(data, bytes) and 5 <= len(data):
             if data[0] == 0x25 and data[1] == 0x50 and data[2] == 0x44 and data[3] == 0x46 and data[4] == 0x2D:
                 return True
         return False
 
     @staticmethod
-    def read_data(path: str) -> Optional[bytes]:
+    def is_elf(data: Union[bytes, bytearray]) -> bool:
+        """According to https://en.wikipedia.org/wiki/Executable_and_Linkable_Format use only 5 bytes"""
+        if isinstance(data, (bytes, bytearray)) and 127 <= len(data):
+            # minimal is 127 bytes https://github.com/tchajed/minimal-elf
+            if 0x7f == data[0] and 0x45 == data[1] and 0x4c == data[2] and 0x46 == data[3] and (0x01 == data[5]
+                                                                                                or 0x02 == data[5]):
+                return True
+        return False
+
+    @staticmethod
+    def read_data(path: Union[str, Path]) -> Optional[bytes]:
         """Read the file bytes as is.
 
         Try to read the data of the file.
 
         Args:
             path: path to file
 
@@ -384,44 +488,44 @@
         """
         element_attr: Any = getattr(element, attr)
         if element_attr is None or not isinstance(element_attr, str):
             return ""
         return str(element_attr).strip()
 
     @staticmethod
-    def json_load(file_path: str, encoding=DEFAULT_ENCODING) -> Any:
+    def json_load(file_path: Union[str, Path], encoding=DEFAULT_ENCODING) -> Any:
         """Load dictionary from json file"""
         try:
             with open(file_path, "r", encoding=encoding) as f:
                 return json.load(f)
         except Exception as exc:
             logging.error(f"Failed to read: {file_path} {exc}")
         return None
 
     @staticmethod
-    def json_dump(obj: Any, file_path: str, encoding=DEFAULT_ENCODING, indent=4) -> None:
+    def json_dump(obj: Any, file_path: Union[str, Path], encoding=DEFAULT_ENCODING, indent=4) -> None:
         """Write dictionary to json file"""
         try:
             with open(file_path, "w", encoding=encoding) as f:
                 json.dump(obj, f, indent=indent)
         except Exception as exc:
             logging.error(f"Failed to write: {file_path} {exc}")
 
     @staticmethod
-    def yaml_load(file_path: str, encoding=DEFAULT_ENCODING) -> Any:
+    def yaml_load(file_path: Union[str, Path], encoding=DEFAULT_ENCODING) -> Any:
         """Load dictionary from yaml file"""
         try:
             with open(file_path, "r", encoding=encoding) as f:
                 return yaml.load(f, Loader=yaml.FullLoader)
         except Exception as exc:
             logger.error(f"Failed to read {file_path} {exc}")
         return None
 
     @staticmethod
-    def yaml_dump(obj: Any, file_path: str, encoding=DEFAULT_ENCODING) -> None:
+    def yaml_dump(obj: Any, file_path: Union[str, Path], encoding=DEFAULT_ENCODING) -> None:
         """Write dictionary to yaml file"""
         try:
             with open(file_path, "w", encoding=encoding) as f:
                 yaml.dump(obj, f)
         except Exception as exc:
             logging.error(f"Failed to write: {file_path} {exc}")
```

### Comparing `credsweeper-1.4.9/credsweeper/validations/__init__.py` & `credsweeper-1.5.0/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/apply_validation.py` & `credsweeper-1.5.0/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/github_token_validation.py` & `credsweeper-1.5.0/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.5.0/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.5.0/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.5.0/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.5.0/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.5.0/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.5.0/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.5.0/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.4.9/credsweeper/validations/validation.py` & `credsweeper-1.5.0/credsweeper/validations/validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from credsweeper.common.constants import KeyValidationOption
 from credsweeper.credentials.line_data import LineData
 
 
 class Validation(ABC):
     """Abstract class for verify method"""
 
+    @classmethod
     @abstractmethod
-    def verify(self, line_data_list: List[LineData]) -> KeyValidationOption:
+    def verify(cls, line_data_list: List[LineData]) -> KeyValidationOption:
         """Verify line_data_list with external API.
 
         Args:
             line_data_list: List of LineData objects, data in current credential candidate
 
         Return:
             Enum object, returns the validation status for the passed value
```

### Comparing `credsweeper-1.4.9/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.5.0/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.4.9
+Version: 1.5.0
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.4.9/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.5.0/credsweeper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 credsweeper.egg-info/entry_points.txt
 credsweeper.egg-info/requires.txt
 credsweeper.egg-info/top_level.txt
 credsweeper/common/__init__.py
 credsweeper/common/constants.py
 credsweeper/common/keyword_checklist.py
 credsweeper/common/keyword_checklist.txt
+credsweeper/common/morpheme_checklist.txt
 credsweeper/config/__init__.py
 credsweeper/config/config.py
 credsweeper/credentials/__init__.py
 credsweeper/credentials/augment_candidates.py
 credsweeper/credentials/candidate.py
 credsweeper/credentials/candidate_group_generator.py
 credsweeper/credentials/candidate_key.py
 credsweeper/credentials/credential_manager.py
 credsweeper/credentials/line_data.py
 credsweeper/deep_scanner/__init__.py
 credsweeper/deep_scanner/abstract_scanner.py
 credsweeper/deep_scanner/byte_scanner.py
 credsweeper/deep_scanner/bzip2_scanner.py
-credsweeper/deep_scanner/deep_scaner.py
+credsweeper/deep_scanner/deep_scanner.py
 credsweeper/deep_scanner/encoder_scanner.py
 credsweeper/deep_scanner/gzip_scanner.py
 credsweeper/deep_scanner/html_scanner.py
 credsweeper/deep_scanner/lang_scanner.py
 credsweeper/deep_scanner/pdf_scanner.py
 credsweeper/deep_scanner/tar_scanner.py
 credsweeper/deep_scanner/xml_scanner.py
@@ -54,39 +55,53 @@
 credsweeper/filters/__init__.py
 credsweeper/filters/cred_card_number_check.py
 credsweeper/filters/filter.py
 credsweeper/filters/line_specific_key_check.py
 credsweeper/filters/separator_unusual_check.py
 credsweeper/filters/value_allowlist_check.py
 credsweeper/filters/value_array_dictionary_check.py
+credsweeper/filters/value_base32_data_check.py
 credsweeper/filters/value_blocklist_check.py
 credsweeper/filters/value_camel_case_check.py
+credsweeper/filters/value_couple_keyword_check.py
 credsweeper/filters/value_dictionary_keyword_check.py
 credsweeper/filters/value_dictionary_value_length_check.py
+credsweeper/filters/value_entropy_base32_check.py
+credsweeper/filters/value_entropy_base36_check.py
 credsweeper/filters/value_entropy_check.py
 credsweeper/filters/value_file_path_check.py
 credsweeper/filters/value_first_word_check.py
+credsweeper/filters/value_grafana_check.py
+credsweeper/filters/value_json_web_token_check.py
 credsweeper/filters/value_last_word_check.py
 credsweeper/filters/value_length_check.py
 credsweeper/filters/value_method_check.py
 credsweeper/filters/value_not_allowed_pattern_check.py
+credsweeper/filters/value_number_check.py
 credsweeper/filters/value_pattern_check.py
+credsweeper/filters/value_pattern_length_check.py
+credsweeper/filters/value_pem_pattern_check.py
 credsweeper/filters/value_similarity_check.py
+credsweeper/filters/value_split_keyword_check.py
 credsweeper/filters/value_string_type_check.py
+credsweeper/filters/value_structured_token_check.py
+credsweeper/filters/value_token_base32_check.py
+credsweeper/filters/value_token_base36_check.py
 credsweeper/filters/value_token_check.py
 credsweeper/filters/value_useless_word_check.py
 credsweeper/filters/variable_not_allowed_pattern_check.py
 credsweeper/filters/group/__init__.py
-credsweeper/filters/group/credit_card_number_sequense.py
 credsweeper/filters/group/general_keyword.py
 credsweeper/filters/group/general_pattern.py
 credsweeper/filters/group/group.py
 credsweeper/filters/group/password_keyword.py
-credsweeper/filters/group/pem_pattern.py
+credsweeper/filters/group/structured_token.py
+credsweeper/filters/group/token_pattern.py
 credsweeper/filters/group/url_credentials_group.py
+credsweeper/filters/group/weird_base36_token.py
 credsweeper/logger/__init__.py
 credsweeper/logger/logger.py
 credsweeper/ml_model/__init__.py
 credsweeper/ml_model/features.py
 credsweeper/ml_model/ml_model.onnx
 credsweeper/ml_model/ml_validator.py
 credsweeper/ml_model/model_config.json
```

### Comparing `credsweeper-1.4.9/setup.py` & `credsweeper-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-import sys
-
 import setuptools
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 install_requires = [
     "beautifulsoup4",  #
     "GitPython",  #
     "google_auth_oauthlib",  #
     "humanfriendly",  #
     "lxml",  #
     "oauthlib",  #
     "openpyxl",  #
     "pandas",  #
+    "password-strength",  #
     "pdfminer.six",  #
     "PyYAML",  #
-    "regex",  #
     "requests",  #
     "scipy",  #
     "typing_extensions",  #
     "whatthepatch",  #
     "numpy",  #
     "scikit-learn",  #
     "onnxruntime",  #
@@ -32,14 +30,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=("credsweeper*", )),
     package_data={
         "credsweeper": [
             "py.typed",  #
             "common/keyword_checklist.txt",  #
+            "common/morpheme_checklist.txt",  #
             "ml_model/ml_model.onnx",  #
             "ml_model/model_config.json",  #
             "secret/config.json",  #
             "secret/log.yaml",  #
             "rules/config.yaml"  #
         ],
     },
```

### Comparing `credsweeper-1.4.9/tests/test_app.py` & `credsweeper-1.5.0/tests/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,45 @@
 import tempfile
 import time
 from typing import AnyStr, Tuple
 from unittest import TestCase
 
 import pytest
 
-from credsweeper import CREDSWEEPER_DIR
+from credsweeper.app import APP_PATH
 from credsweeper.utils import Util
-from tests import AZ_STRING, SAMPLES_FILTERED_BY_POST_COUNT, SAMPLES_POST_CRED_COUNT, SAMPLES_IN_DEEP_1, \
-    SAMPLES_IN_DEEP_3, SAMPLES_DIR, TESTS_DIR, PROJECT_DIR
+from tests import AZ_STRING, SAMPLES_FILTERED_BY_POST_COUNT, SAMPLES_POST_CRED_COUNT, SAMPLES_IN_DEEP_3, SAMPLES_PATH, \
+    TESTS_PATH, SAMPLES_CRED_COUNT
 
 
 class TestApp(TestCase):
 
     @staticmethod
-    def _m_credsweeper(args) -> Tuple[AnyStr, AnyStr]:
+    def _m_credsweeper(args) -> Tuple[str, str]:
         proc = subprocess.Popen(
             [sys.executable, "-m", "credsweeper", *args],  #
-            cwd=PROJECT_DIR,  #
+            cwd=APP_PATH.parent,  #
             stdout=subprocess.PIPE,  #
             stderr=subprocess.PIPE)  #
-        return proc.communicate()
+        _stdout, _stderr = proc.communicate()
+
+        def transform(x: AnyStr) -> str:
+            if isinstance(x, bytes):
+                return x.decode(errors='replace')
+            elif isinstance(x, str):
+                return x
+            else:
+                raise ValueError(f"Unknown type: {type(x)}")
+
+        return transform(_stdout), transform(_stderr)
 
     def test_it_works_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
+        target_path = str(SAMPLES_PATH / "password.gradle")
         _stdout, _stderr = self._m_credsweeper(["--path", target_path, "--log", "silence"])
-        output = " ".join(_stdout.decode("UTF-8").split()[:-1])
+        output = " ".join(_stdout.split()[:-1])
 
         expected = f"""
                     rule: Password
                     / severity: medium
                     / line_data_list:
                         [line: 'password = \"cackle!\"'
                         / line_num: 1
@@ -44,15 +54,15 @@
                         / entropy_validation: False]
                     / api_validation: NOT_AVAILABLE
                     / ml_validation: VALIDATED_KEY\n
                     Detected Credentials: 1\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
-        assert output == expected
+        self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_huge_diff_p(self) -> None:
         # verifies issue when huge patch is parsed very slow
         # https://github.com/Samsung/CredSweeper/issues/242
         text = """diff --git a/huge.file b/huge.file
@@ -74,42 +84,18 @@
             target_path = os.path.join(tmp_dir, f"{__name__}.diff")
             start_time = time.time()
             _stdout, _stderr = self._m_credsweeper(["--path", target_path, "--ml_threshold", "0", "--log", "silence"])
             self.assertGreater(100, time.time() - start_time)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def test_it_works_without_ml_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
-        _stdout, _stderr = self._m_credsweeper(["--path", target_path, "--ml_threshold", "0", "--log", "silence"])
-        output = " ".join(_stdout.decode("UTF-8").split()[:-1])
-
-        expected = f"""
-                    rule: Password
-                    / severity: medium
-                    / line_data_list:
-                        [line: 'password = \"cackle!\"'
-                        / line_num: 1
-                        / path: {target_path}
-                        / value: 'cackle!'
-                        / entropy_validation: False]
-                    / api_validation: NOT_AVAILABLE
-                    / ml_validation: NOT_AVAILABLE\n
-                    Detected Credentials: 1\n
-                    Time Elapsed:
-                    """
-        expected = " ".join(expected.split())
-        assert output == expected
-
-    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
-
     def test_it_works_with_patch_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password.patch")
+        target_path = str(SAMPLES_PATH / "password.patch")
         _stdout, _stderr = self._m_credsweeper(["--diff_path", target_path, "--log", "silence"])
-        output = " ".join(_stdout.decode("UTF-8").split()[:-1])
+        output = " ".join(_stdout.split()[:-1])
 
         expected = """
                     rule: Password
                     / severity: medium
                     / line_data_list:
                     [line: '  "password": "dkajco1"'
                         / line_num: 3
@@ -119,22 +105,22 @@
                     / api_validation: NOT_AVAILABLE
                     / ml_validation: VALIDATED_KEY\n
                     Added File Credentials: 1\n
                     Deleted File Credentials: 0\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
-        assert output == expected
+        self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_it_works_with_multiline_in_patch_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "multiline.patch")
+        target_path = str(SAMPLES_PATH / "multiline.patch")
         _stdout, _stderr = self._m_credsweeper(["--diff_path", target_path, "--log", "silence"])
-        output = " ".join(_stdout.decode("UTF-8").split()[:-1])
+        output = " ".join(_stdout.split()[:-1])
 
         expected = """
                     rule: AWS Client ID
                         / severity: high
                         / line_data_list:
                             [line: ' clid = "AKIAQWADE5R42RDZ4JEM"'
                             / line_num: 4
@@ -168,25 +154,25 @@
                         / api_validation: NOT_AVAILABLE
                         / ml_validation: VALIDATED_KEY\n
                     Added File Credentials: 3\n
                     Deleted File Credentials: 0\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
-        assert output == expected
+        self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     @pytest.mark.skipif(0 != subprocess.call(["curl", "https://maps.googleapis.com/"]),
                         reason="network is not available")
     def test_it_works_with_api_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "google_api_key")
+        target_path = str(SAMPLES_PATH / "google_api_key.toml")
         _stdout, _stderr = self._m_credsweeper(
             ["--path", target_path, "--ml_threshold", "0", "--api_validation", "--log", "silence"], )
-        output = " ".join(_stdout.decode("UTF-8").split()[:-1])
+        output = " ".join(_stdout.split()[:-1])
 
         expected = f"""
                     rule: Google API Key
                     / severity: high
                     / line_data_list:
                     [line: 'AIzaGiReoGiCrackleCrackle12315618112315'
                         / line_num: 1
@@ -195,36 +181,38 @@
                         / entropy_validation: True]
                     / api_validation: INVALID_KEY
                     / ml_validation: NOT_AVAILABLE\n
                     Detected Credentials: 1\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
-        assert output == expected
+        self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_it_works_n(self) -> None:
         _stdout, _stderr = self._m_credsweeper([])
 
         # Merge more than two whitespaces into one because _stdout and _stderr are changed based on the terminal size
-        output = " ".join(_stderr.decode("UTF-8").split())
+        output = " ".join(_stderr.split())
 
         expected = "usage: python -m credsweeper [-h]" \
                    " (--path PATH [PATH ...]" \
                    " | --diff_path PATH [PATH ...]" \
                    " | --export_config [PATH]" \
                    " | --export_log_config [PATH]" \
                    ")" \
                    " [--rules [PATH]]" \
+                   " [--severity SEVERITY]" \
                    " [--config [PATH]]" \
                    " [--log_config [PATH]]" \
                    " [--denylist PATH]" \
                    " [--find-by-ext]" \
                    " [--depth POSITIVE_INT]" \
+                   " [--doc]" \
                    " [--ml_threshold FLOAT_OR_STR]" \
                    " [--ml_batch_size POSITIVE_INT]" \
                    " [--api_validation]" \
                    " [--jobs POSITIVE_INT]" \
                    " [--skip_ignored]" \
                    " [--save-json [PATH]]" \
                    " [--save-xlsx [PATH]]" \
@@ -235,188 +223,188 @@
                    "python -m credsweeper: error: one of the arguments" \
                    " --path" \
                    " --diff_path" \
                    " --export_config" \
                    " --export_log_config" \
                    " is required "
         expected = " ".join(expected.split())
-        assert output == expected
+        self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_log_p(self) -> None:
-        apk_path = str(SAMPLES_DIR / "pem_key.apk")
+        apk_path = str(SAMPLES_PATH / "pem_key.apk")
         _stdout, _stderr = self._m_credsweeper(
             ["--log", "Debug", "--depth", "7", "--ml_threshold", "0", "--path", apk_path, "not_existed_path"])
-        assert len(_stderr) == 0
-        output = _stdout.decode()
+        self.assertEqual(0, len(_stderr))
 
-        assert "DEBUG" in output, output
-        assert "INFO" in output, output
-        assert "WARNING" in output, output
-        assert "ERROR" in output, output
-        assert not ("CRITICAL" in output), output
+        self.assertIn("DEBUG", _stdout)
+        self.assertIn("INFO", _stdout)
+        self.assertIn("WARNING", _stdout)
+        self.assertIn("ERROR", _stdout)
+        self.assertNotIn("CRITICAL", _stdout)
 
-        for line in output.splitlines():
+        for line in _stdout.splitlines():
             if 5 <= len(line) and "rule:" == line[0:5]:
-                assert re.match(r"rule: \.*", line), line
+                self.assertRegex(line, r"rule: \.*")
             elif 21 <= len(line) and "Detected Credentials:" == line[0:21]:
-                assert re.match(r"Detected Credentials: \d+", line), line
+                self.assertRegex(line, r"Detected Credentials: \d+")
             elif 13 <= len(line) and "Time Elapsed:" == line[0:13]:
-                assert re.match(r"Time Elapsed: \d+\.\d+", line), line
+                self.assertRegex(line, r"Time Elapsed: \d+\.\d+")
             else:
-                self.assertRegex(line,
-                                 r"\d{4}-\d\d-\d\d \d\d:\d\d:\d\d,\d+ \| (DEBUG|INFO|WARNING|ERROR) \| \w+:\d+ \| .*",
-                                 line)
+                self.assertRegex(
+                    line,
+                    r"\d{4}-\d\d-\d\d \d\d:\d\d:\d\d,\d+ \| (DEBUG|INFO|WARNING|ERROR) \| \w+:\d+ \| .*",
+                )
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_log_n(self) -> None:
         _stdout, _stderr = self._m_credsweeper(["--log", "CriTicaL", "--rule", "NOT_EXISTED_PATH", "--path", "."])
-        assert len(_stderr) == 0
-        output = _stdout.decode()
+        self.assertEqual(0, len(_stderr))
 
-        assert not ("DEBUG" in output), output
-        assert not ("INFO" in output), output
-        assert not ("WARNING" in output), output
-        assert not ("ERROR" in output), output
-        assert "CRITICAL" in output, output
-
-        assert any(
-            re.match(r"\d{4}-\d\d-\d\d \d\d:\d\d:\d\d,\d+ \| (CRITICAL) \| \w+:\d+ \| .*", line)
-            for line in output.splitlines()), output
+        self.assertNotIn("DEBUG", _stdout)
+        self.assertNotIn("INFO", _stdout)
+        self.assertNotIn("WARNING", _stdout)
+        self.assertNotIn("ERROR", _stdout)
+        self.assertIn("CRITICAL", _stdout)
+
+        self.assertTrue(
+            any(
+                re.match(r"\d{4}-\d\d-\d\d \d\d:\d\d:\d\d,\d+ \| (CRITICAL) \| \w+:\d+ \| .*", line)
+                for line in _stdout.splitlines()), _stdout)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_help_p(self) -> None:
         _stdout, _stderr = self._m_credsweeper(["--help"])
-        output = " ".join(_stdout.decode("UTF-8").split())
-        help_path = os.path.join(TESTS_DIR, "..", "docs", "source", "guide.rst")
+        output = " ".join(_stdout.split())
+        if 10 > sys.version_info.minor and output.find("options:"):
+            # Legacy support python3.8 - 3.9 to display "optional arguments:" like in python 3.10
+            output = output.replace("options:", "optional arguments:")
+        help_path = os.path.join(TESTS_PATH, "..", "docs", "source", "guide.rst")
         with open(help_path, "r") as f:
             text = ""
             started = False
             for line in f.read().splitlines():
                 if ".. note::" == line:
                     break
                 if ".. code-block:: text" == line:
                     started = True
                     continue
                 if started:
-                    # There is argparse change on python3.10 to display just "options:"
-                    if sys.version_info.minor >= 10 and line.strip() == "optional arguments:":
-                        text += line.replace("optional arguments:", "options:")
+                    if 10 > sys.version_info.minor and line.strip() == "options:":
+                        # Legacy support python3.8 - 3.9 to display "optional arguments:"
+                        text = ' '.join([text, line.replace("options:", "optional arguments:")])
                     else:
-                        text += line
+                        text = ' '.join([text, line])
             expected = " ".join(text.split())
-            assert output == expected
+            self.maxDiff = 65536
+            self.assertEqual(expected, output)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_version_p(self) -> None:
         _stdout, _stderr = self._m_credsweeper(["--version"])
         # Merge more than two whitespaces into one because _stdout and _stderr are changed based on the terminal size
-        output = " ".join(_stdout.decode("UTF-8").split())
+        output = " ".join(_stdout.split())
         self.assertRegex(output, r"CredSweeper \d+\.\d+\.\d+")
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_banner_p(self) -> None:
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            json_filename = os.path.join(tmp_dir, f"{__name__}.json")
-            _stdout, _stderr = self._m_credsweeper(["--banner", "--export_config", json_filename])
-            output = " ".join(_stdout.decode().split())
-            self.assertRegex(output, r"CredSweeper \d+\.\d+\.\d+ crc32:[0-9a-f]{8}")
+        _stdout, _stderr = self._m_credsweeper(["--banner"])
+        output = " ".join(_stdout.split())
+        self.assertRegex(output, r"CredSweeper \d+\.\d+\.\d+ crc32:[0-9a-f]{8}", _stderr or _stdout)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_patch_save_json_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password.patch")
+        target_path = str(SAMPLES_PATH / "password.patch")
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper(
                 ["--diff_path", target_path, "--save-json", json_filename, "--log", "silence"])
-            assert os.path.exists(os.path.join(tmp_dir, f"{__name__}_added.json"))
-            assert os.path.exists(os.path.join(tmp_dir, f"{__name__}_deleted.json"))
+            self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_added.json")))
+            self.assertTrue(os.path.exists(os.path.join(tmp_dir, f"{__name__}_deleted.json")))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_patch_save_json_n(self) -> None:
         start_time = time.time()
-        target_path = str(SAMPLES_DIR / "password.patch")
+        target_path = str(SAMPLES_PATH / "password.patch")
         _stdout, _stderr = self._m_credsweeper(["--diff_path", target_path, "--log", "silence"])
-        for root, dirs, files in os.walk(PROJECT_DIR):
+        for root, dirs, files in os.walk(APP_PATH.parent):
             self.assertIn("credsweeper", dirs)
             for file in files:
                 # check whether the report was created AFTER test launch to avoid failures during development
                 self.assertFalse(file.endswith(".json") and os.stat(os.path.join(root, file)).st_mtime > start_time)
             dirs.clear()
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_export_config_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper(["--export_config", json_filename, "--log", "silence"])
-            assert os.path.exists(json_filename)
+            self.assertTrue(os.path.exists(json_filename))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_import_config_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             custom_config = os.path.join(tmp_dir, f"{__name__}.json")
-            shutil.copyfile(CREDSWEEPER_DIR / "secret" / "config.json", custom_config)
-            args = ["--config", custom_config, "--path", str(CREDSWEEPER_DIR), "--find-by-ext", "--log", "CRITICAL"]
+            shutil.copyfile(APP_PATH / "secret" / "config.json", custom_config)
+            args = ["--config", custom_config, "--path", str(APP_PATH), "--find-by-ext", "--log", "CRITICAL"]
             _stdout, _stderr = self._m_credsweeper(args)
-            self.assertEqual("", _stderr.decode())
-            output = _stdout.decode()
-            self.assertNotIn("CRITICAL", output)
-            self.assertIn("Time Elapsed:", output)
-            self.assertIn("Detected Credentials: 0", output)
-            self.assertEqual(2, len(output.splitlines()))
+            self.assertEqual("", _stderr)
+            self.assertNotIn("CRITICAL", _stdout)
+            self.assertIn("Time Elapsed:", _stdout)
+            self.assertIn("Detected Credentials: 0", _stdout)
+            self.assertEqual(2, len(_stdout.splitlines()))
             # add .py to find by extension
             modified_config = Util.json_load(custom_config)
             self.assertIn("find_by_ext_list", modified_config.keys())
             self.assertIsInstance(modified_config["find_by_ext_list"], list)
             modified_config["find_by_ext_list"].append(".py")
             Util.json_dump(modified_config, custom_config)
             _stdout, _stderr = self._m_credsweeper(args)
-            output = _stdout.decode()
-            self.assertEqual("", _stderr.decode())
-            self.assertNotIn("CRITICAL", output)
-            self.assertIn("Time Elapsed:", output)
-            self.assertNotIn("Detected Credentials: 0", output)
-            self.assertLess(42, len(output.splitlines()))
+            self.assertEqual("", _stderr)
+            self.assertNotIn("CRITICAL", _stdout)
+            self.assertIn("Time Elapsed:", _stdout)
+            self.assertNotIn("Detected Credentials: 0", _stdout)
+            self.assertLess(5, len(_stdout.splitlines()))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_import_config_n(self) -> None:
         # not existed file
         _stdout, _stderr = self._m_credsweeper(
             ["--config", "not_existed_file", "--path",
-             str(CREDSWEEPER_DIR), "--log", "CRITICAL"])
+             str(APP_PATH), "--log", "CRITICAL"])
         self.assertEqual(0, len(_stderr))
-        self.assertIn("CRITICAL", _stdout.decode())
+        self.assertIn("CRITICAL", _stdout)
         # wrong config
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             with open(json_filename, "w") as f:
                 f.write('{}')
             _stdout, _stderr = self._m_credsweeper(
                 ["--config", json_filename, "--path",
-                 str(CREDSWEEPER_DIR), "--log", "CRITICAL"])
+                 str(APP_PATH), "--log", "CRITICAL"])
             self.assertEqual(0, len(_stderr))
-            self.assertIn("CRITICAL", _stdout.decode())
+            self.assertIn("CRITICAL", _stdout)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_export_log_config_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             test_filename = os.path.join(tmp_dir, f"{__name__}.yaml")
             _stdout, _stderr = self._m_credsweeper(["--export_log_config", test_filename, "--log", "silence"])
-            assert os.path.exists(test_filename)
+            self.assertTrue(os.path.exists(test_filename))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_import_log_config_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             test_filename = os.path.join(tmp_dir, f"{__name__}.yaml")
             _o, _e = self._m_credsweeper(["--export_log_config", test_filename, "--log", "silence"])
@@ -432,155 +420,210 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_find_by_ext_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             # .deR will be found also!
             for f in [".pem", ".cer", ".csr", ".deR"]:
                 file_path = os.path.join(tmp_dir, f"dummy{f}")
-                assert not os.path.exists(file_path)
+                self.assertFalse(os.path.exists(file_path))
                 open(file_path, "w").write(AZ_STRING)
 
             # not of all will be found due they are empty
             for f in [".jks", ".KeY"]:
                 file_path = os.path.join(tmp_dir, f"dummy{f}")
-                assert not os.path.exists(file_path)
+                self.assertFalse(os.path.exists(file_path))
                 open(file_path, "w").close()
 
             # the directory hides all files
             ignored_dir = os.path.join(tmp_dir, "target")
             os.mkdir(ignored_dir)
             for f in [".pfx", ".p12"]:
                 file_path = os.path.join(ignored_dir, f"dummy{f}")
-                assert not os.path.exists(file_path)
+                self.assertFalse(os.path.exists(file_path))
                 open(file_path, "w").write(AZ_STRING)
 
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper(
                 ["--path", tmp_dir, "--find-by-ext", "--save-json", json_filename, "--log", "silence"])
-            assert os.path.exists(json_filename)
+            self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 4, f"{report}"
+                self.assertEqual(4, len(report), report)
                 for t in report:
-                    assert t["line_data_list"][0]["line_num"] == -1
-                    assert str(t["line_data_list"][0]["path"][-4:]) in [".pem", ".cer", ".csr", ".deR"]
+                    self.assertEqual(-1, t["line_data_list"][0]["line_num"])
+                    self.assertIn(str(t["line_data_list"][0]["path"][-4:]), [".pem", ".cer", ".csr", ".deR"])
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_find_by_ext_n(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             for f in [".pem", ".cer", ".csr", ".der", ".pfx", ".p12", ".key", ".jks"]:
                 file_path = os.path.join(tmp_dir, f"dummy{f}")
-                assert not os.path.exists(file_path)
+                self.assertFalse(os.path.exists(file_path))
                 open(file_path, "w").write(AZ_STRING)
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper(
                 ["--path", tmp_dir, "--save-json", json_filename, "--log", "silence"])
-            assert os.path.exists(json_filename)
+            self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 0
+                self.assertEqual(0, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_p(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             # depth = 3
             _stdout, _stderr = self._m_credsweeper(
                 ["--log", "silence", "--path",
-                 str(SAMPLES_DIR), "--save-json", json_filename, "--depth", "3"])
-            assert os.path.exists(json_filename)
+                 str(SAMPLES_PATH), "--save-json", json_filename, "--depth", "3"])
+            self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_3 - SAMPLES_FILTERED_BY_POST_COUNT
+                self.assertEqual(SAMPLES_POST_CRED_COUNT + SAMPLES_IN_DEEP_3 - SAMPLES_FILTERED_BY_POST_COUNT,
+                                 len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_depth_n(self) -> None:
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             # depth is not set
             _stdout, _stderr = self._m_credsweeper(
                 ["--log", "silence", "--path",
-                 str(SAMPLES_DIR), "--save-json", json_filename])
-            assert os.path.exists(json_filename)
+                 str(SAMPLES_PATH), "--save-json", json_filename])
+            self.assertTrue(os.path.exists(json_filename))
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == SAMPLES_POST_CRED_COUNT
+                self.assertEqual(SAMPLES_POST_CRED_COUNT, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_denylist_value_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
+        target_path = str(SAMPLES_PATH / "password.gradle")
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
-            denylist_filename = os.path.join(tmp_dir, f"list.txt")
+            denylist_filename = os.path.join(tmp_dir, "list.txt")
             with open(denylist_filename, "w") as f:
                 f.write("cackle!")
             _stdout, _stderr = self._m_credsweeper([
                 "--path", target_path, "--denylist", denylist_filename, "--save-json", json_filename, "--log", "silence"
             ])
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 0
+                self.assertEqual(0, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_denylist_value_n(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
+        target_path = str(SAMPLES_PATH / "password.gradle")
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
-            denylist_filename = os.path.join(tmp_dir, f"list.txt")
+            denylist_filename = os.path.join(tmp_dir, "list.txt")
             with open(denylist_filename, "w") as f:
                 f.write("abc")
             _stdout, _stderr = self._m_credsweeper([
                 "--path", target_path, "--denylist", denylist_filename, "--save-json", json_filename, "--log", "silence"
             ])
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 1
+                self.assertEqual(1, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_denylist_line_p(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
+        target_path = str(SAMPLES_PATH / "password.gradle")
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
-            denylist_filename = os.path.join(tmp_dir, f"list.txt")
+            denylist_filename = os.path.join(tmp_dir, "list.txt")
             with open(denylist_filename, "w") as f:
                 f.write('  password = "cackle!" ')
             _stdout, _stderr = self._m_credsweeper([
                 "--path", target_path, "--denylist", denylist_filename, "--save-json", json_filename, "--log", "silence"
             ])
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 0
+                self.assertEqual(0, len(report))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_denylist_line_n(self) -> None:
-        target_path = str(SAMPLES_DIR / "password")
+        target_path = str(SAMPLES_PATH / "password.gradle")
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
-            denylist_filename = os.path.join(tmp_dir, f"list.txt")
+            denylist_filename = os.path.join(tmp_dir, "list.txt")
             with open(denylist_filename, "w") as f:
                 f.write("abc")
             _stdout, _stderr = self._m_credsweeper([
                 "--path", target_path, "--denylist", denylist_filename, "--save-json", json_filename, "--log", "silence"
             ])
             with open(json_filename, "r") as json_file:
                 report = json.load(json_file)
-                assert len(report) == 1
+                self.assertEqual(1, len(report))
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+    def test_rules_ml_p(self) -> None:
+        # checks whether all rules have positive test samples with almost the same arguments during benchmark
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            json_filename = os.path.join(tmp_dir, f"{__name__}.json")
+            _stdout, _stderr = self._m_credsweeper([
+                "--log",
+                "debug",
+                "--path",
+                str(SAMPLES_PATH),
+                "--save-json",
+                json_filename,
+            ])
+            self.assertEqual(0, len(_stderr))
+            report = Util.json_load(json_filename)
+            report_set = set([i["rule"] for i in report])
+            rules = Util.yaml_load(APP_PATH / "rules" / "config.yaml")
+            rules_set = set([i["name"] for i in rules])
+            missed = {  #
+            }
+            self.assertSetEqual(rules_set.difference(missed), report_set, f"\n{_stdout}")
+            self.assertEqual(SAMPLES_POST_CRED_COUNT, len(report))
+
+            # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+    def test_rules_ml_n(self) -> None:
+        # checks whether all rules have test samples which detected without ML
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            json_filename = os.path.join(tmp_dir, f"{__name__}.json")
+            _stdout, _stderr = self._m_credsweeper([
+                "--log",
+                "debug",
+                "--path",
+                str(SAMPLES_PATH),
+                "--ml_threshold",
+                "0",
+                "--save-json",
+                json_filename,
+            ])
+            self.assertEqual(0, len(_stderr))
+            report = Util.json_load(json_filename)
+            report_set = set([i["rule"] for i in report])
+            rules = Util.yaml_load(APP_PATH / "rules" / "config.yaml")
+            rules_set = set([i["name"] for i in rules])
+            self.assertSetEqual(rules_set, report_set, f"\n{_stdout}")
+            self.assertEqual(SAMPLES_CRED_COUNT, len(report))
+
+    # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
+
+    def test_severity_p(self) -> None:
+        _stdout, _stderr = self._m_credsweeper([  #
+            "--log", "silence", "--ml_threshold", "0", "--severity", "medium", "--path",
+            str(SAMPLES_PATH)
+        ])
+        self.assertIn("severity: medium", _stdout)
+        self.assertNotIn("severity: info", _stdout)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
-    def test_rules_p(self) -> None:
-        _stdout, _stderr = self._m_credsweeper(["--log", "silence", "--ml_threshold", "0", "--path", str(SAMPLES_DIR)])
-        assert len(_stderr) == 0
-        output = _stdout.decode(errors='replace')
-        rules = Util.yaml_load(PROJECT_DIR / "credsweeper" / "rules" / "config.yaml")
-        for rule in rules:
-            rule_name = rule["name"]
-            if rule_name in ["Nonce", "Salt", "Certificate"]:
-                continue
-            self.assertIn(f"rule: {rule_name}", output)
+    def test_severity_n(self) -> None:
+        _stdout, _stderr = self._m_credsweeper([  #
+            "--log", "silence", "--ml_threshold", "0", "--severity", "critical", "--path",
+            str(SAMPLES_PATH)
+        ])
+        self.assertNotIn("severity: medium", _stdout)
```

