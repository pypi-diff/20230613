# Comparing `tmp/doccano_client-1.2.7.tar.gz` & `tmp/doccano_client-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doccano_client-1.2.7.tar", max compression
+gzip compressed data, was "doccano_client-1.2.8.tar", max compression
```

## Comparing `doccano_client-1.2.7.tar` & `doccano_client-1.2.8.tar`

### file list

```diff
@@ -1,130 +1,129 @@
--rw-r--r--   0        0        0     1071 2023-02-09 17:55:01.996619 doccano_client-1.2.7/LICENSE
--rw-r--r--   0        0        0     1389 2023-02-09 17:55:01.996619 doccano_client-1.2.7/README.md
--rw-r--r--   0        0        0       77 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/__init__.py
--rw-r--r--   0        0        0     1708 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/README.md
--rw-r--r--   0        0        0       63 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/__init__.py
--rw-r--r--   0        0        0     1766 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/client.py
--rw-r--r--   0        0        0     1682 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/__init__.py
--rw-r--r--   0        0        0     2199 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/annotation.py
--rw-r--r--   0        0        0     3193 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/category.py
--rw-r--r--   0        0        0     3787 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/category_type.py
--rw-r--r--   0        0        0     3746 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/comment.py
--rw-r--r--   0        0        0     6232 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/example.py
--rw-r--r--   0        0        0     7524 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/label.py
--rw-r--r--   0        0        0     3106 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/member.py
--rw-r--r--   0        0        0     6779 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/project.py
--rw-r--r--   0        0        0     3184 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/relation.py
--rw-r--r--   0        0        0     3787 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/relation_type.py
--rw-r--r--   0        0        0     2937 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/span.py
--rw-r--r--   0        0        0     3463 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/span_type.py
--rw-r--r--   0        0        0     2936 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/controllers/text.py
--rw-r--r--   0        0        0      956 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/__init__.py
--rw-r--r--   0        0        0      732 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/annotations.py
--rw-r--r--   0        0        0      251 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/category.py
--rw-r--r--   0        0        0      606 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/category_type.py
--rw-r--r--   0        0        0      164 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/comments.py
--rw-r--r--   0        0        0      521 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/examples.py
--rw-r--r--   0        0        0      560 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/labels.py
--rw-r--r--   0        0        0      175 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/members.py
--rw-r--r--   0        0        0     2178 2023-02-09 17:55:01.996619 doccano_client-1.2.7/doccano_client/beta/models/projects.py
--rw-r--r--   0        0        0      276 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/models/relation.py
--rw-r--r--   0        0        0      606 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/models/relation_type.py
--rw-r--r--   0        0        0      283 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/models/span.py
--rw-r--r--   0        0        0      598 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/models/span_type.py
--rw-r--r--   0        0        0      230 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/models/text.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/py.typed
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/__init__.py
--rw-r--r--   0        0        0     1147 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/__init__.py
--rw-r--r--   0        0        0      227 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/__init__.py
--rw-r--r--   0        0        0     1281 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/annotations.py
--rw-r--r--   0        0        0      430 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/bad.py
--rw-r--r--   0        0        0     1069 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/categories.py
--rw-r--r--   0        0        0     1574 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/category_types.py
--rw-r--r--   0        0        0     1062 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/comments.py
--rw-r--r--   0        0        0     3717 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/examples.py
--rw-r--r--   0        0        0     1450 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/labels.py
--rw-r--r--   0        0        0     1308 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/members.py
--rw-r--r--   0        0        0    10221 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/projects.py
--rw-r--r--   0        0        0     1574 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/relation_types.py
--rw-r--r--   0        0        0     1183 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/relations.py
--rw-r--r--   0        0        0     1512 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/span_types.py
--rw-r--r--   0        0        0     1184 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/spans.py
--rw-r--r--   0        0        0     1038 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/texts.py
--rw-r--r--   0        0        0     2594 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_annotation.py.unused.bak
--rw-r--r--   0        0        0     1817 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_category.py
--rw-r--r--   0        0        0     4410 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_category_type.py
--rw-r--r--   0        0        0     4276 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_comment.py
--rw-r--r--   0        0        0     4768 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_example.py
--rw-r--r--   0        0        0     9088 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_label.py.unused.bak
--rw-r--r--   0        0        0     3744 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_member.py
--rw-r--r--   0        0        0     5057 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_project.py
--rw-r--r--   0        0        0     1795 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_relation.py
--rw-r--r--   0        0        0     4410 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_relation_type.py
--rw-r--r--   0        0        0     1673 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_span.py
--rw-r--r--   0        0        0     4010 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_span_type.py
--rw-r--r--   0        0        0     1661 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_text.py
--rw-r--r--   0        0        0     2640 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/test_client.py
--rw-r--r--   0        0        0     3722 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/test_full_integration_tests.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/utils/__init__.py
--rw-r--r--   0        0        0      935 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/tests/utils/test_response.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/utils/__init__.py
--rw-r--r--   0        0        0      638 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/beta/utils/response.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/__init__.py
--rw-r--r--   0        0        0      824 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/languages.py
--rw-r--r--   0        0        0     4095 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/manager.py
--rw-r--r--   0        0        0     5294 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/models.py
--rw-r--r--   0        0        0     4012 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/preparation.py
--rw-r--r--   0        0        0      954 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/strategies.py
--rw-r--r--   0        0        0     1360 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/active_learning/trainer.py
--rw-r--r--   0        0        0     5304 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/commands.py
--rw-r--r--   0        0        0      549 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/entity.py
--rw-r--r--   0        0        0      958 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/estimators.py
--rw-r--r--   0        0        0     3419 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/cli/usecases.py
--rw-r--r--   0        0        0    53125 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/client.py
--rw-r--r--   0        0        0      531 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/__init__.py
--rw-r--r--   0        0        0      228 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/comment.py
--rw-r--r--   0        0        0       94 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/data_download.py
--rw-r--r--   0        0        0      688 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/data_upload.py
--rw-r--r--   0        0        0      392 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/example.py
--rw-r--r--   0        0        0     1401 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/label.py
--rw-r--r--   0        0        0     1946 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/label_type.py
--rw-r--r--   0        0        0      266 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/member.py
--rw-r--r--   0        0        0      431 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/metrics.py
--rw-r--r--   0        0        0     2955 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/project.py
--rw-r--r--   0        0        0       82 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/role.py
--rw-r--r--   0        0        0      185 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/task_status.py
--rw-r--r--   0        0        0      128 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/user.py
--rw-r--r--   0        0        0      835 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/models/user_details.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/__init__.py
--rw-r--r--   0        0        0     5326 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/base.py
--rw-r--r--   0        0        0     3710 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/comment.py
--rw-r--r--   0        0        0     3129 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/data_download.py
--rw-r--r--   0        0        0     2604 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/data_upload.py
--rw-r--r--   0        0        0     4414 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/example.py
--rw-r--r--   0        0        0     4336 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/label.py
--rw-r--r--   0        0        0     5207 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/label_type.py
--rw-r--r--   0        0        0     3351 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/member.py
--rw-r--r--   0        0        0     3404 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/metrics.py
--rw-r--r--   0        0        0     2227 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/project.py
--rw-r--r--   0        0        0     1044 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/role.py
--rw-r--r--   0        0        0     1294 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/task_status.py
--rw-r--r--   0        0        0     1883 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/user.py
--rw-r--r--   0        0        0     1792 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/repositories/user_details.py
--rw-r--r--   0        0        0     1111 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/services/label_type.py
--rw-r--r--   0        0        0        0 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/__init__.py
--rw-r--r--   0        0        0     2756 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/comment.py
--rw-r--r--   0        0        0     1681 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/data_download.py
--rw-r--r--   0        0        0     1879 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/data_upload.py
--rw-r--r--   0        0        0     4061 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/example.py
--rw-r--r--   0        0        0    19920 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/label.py
--rw-r--r--   0        0        0     4437 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/label_type.py
--rw-r--r--   0        0        0     3060 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/member.py
--rw-r--r--   0        0        0     6051 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/project.py
--rw-r--r--   0        0        0      419 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/role.py
--rw-r--r--   0        0        0     2253 2023-02-09 17:55:02.000619 doccano_client-1.2.7/doccano_client/usecase/user_details.py
--rw-r--r--   0        0        0     2461 2023-02-09 17:55:02.004619 doccano_client-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 doccano_client-1.2.7/setup.py
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 doccano_client-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 02:25:26.955544 doccano_client-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1389 2023-06-13 02:25:26.955544 doccano_client-1.2.8/README.md
+-rw-r--r--   0        0        0       77 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/README.md
+-rw-r--r--   0        0        0       63 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/__init__.py
+-rw-r--r--   0        0        0     1766 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/client.py
+-rw-r--r--   0        0        0     1682 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/__init__.py
+-rw-r--r--   0        0        0     2199 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/annotation.py
+-rw-r--r--   0        0        0     3193 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/category.py
+-rw-r--r--   0        0        0     3787 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/category_type.py
+-rw-r--r--   0        0        0     3746 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/comment.py
+-rw-r--r--   0        0        0     6232 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/example.py
+-rw-r--r--   0        0        0     7524 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/label.py
+-rw-r--r--   0        0        0     3106 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/member.py
+-rw-r--r--   0        0        0     6779 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/project.py
+-rw-r--r--   0        0        0     3184 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/relation.py
+-rw-r--r--   0        0        0     3787 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/relation_type.py
+-rw-r--r--   0        0        0     2937 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/span.py
+-rw-r--r--   0        0        0     3463 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/span_type.py
+-rw-r--r--   0        0        0     2936 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/controllers/text.py
+-rw-r--r--   0        0        0      956 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/__init__.py
+-rw-r--r--   0        0        0      732 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/annotations.py
+-rw-r--r--   0        0        0      251 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/category.py
+-rw-r--r--   0        0        0      606 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/category_type.py
+-rw-r--r--   0        0        0      164 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/comments.py
+-rw-r--r--   0        0        0      521 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/examples.py
+-rw-r--r--   0        0        0      560 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/labels.py
+-rw-r--r--   0        0        0      175 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/members.py
+-rw-r--r--   0        0        0     2178 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/projects.py
+-rw-r--r--   0        0        0      276 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/relation.py
+-rw-r--r--   0        0        0      606 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/relation_type.py
+-rw-r--r--   0        0        0      283 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/span.py
+-rw-r--r--   0        0        0      598 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/span_type.py
+-rw-r--r--   0        0        0      230 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/models/text.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/py.typed
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/__init__.py
+-rw-r--r--   0        0        0     1281 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/annotations.py
+-rw-r--r--   0        0        0      430 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/bad.py
+-rw-r--r--   0        0        0     1069 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/categories.py
+-rw-r--r--   0        0        0     1574 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/category_types.py
+-rw-r--r--   0        0        0     1062 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/comments.py
+-rw-r--r--   0        0        0     3717 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/examples.py
+-rw-r--r--   0        0        0     1450 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/labels.py
+-rw-r--r--   0        0        0     1308 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/members.py
+-rw-r--r--   0        0        0    10221 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/projects.py
+-rw-r--r--   0        0        0     1574 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/relation_types.py
+-rw-r--r--   0        0        0     1183 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/relations.py
+-rw-r--r--   0        0        0     1512 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/span_types.py
+-rw-r--r--   0        0        0     1184 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/spans.py
+-rw-r--r--   0        0        0     1038 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/texts.py
+-rw-r--r--   0        0        0     2594 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_annotation.py.unused.bak
+-rw-r--r--   0        0        0     1817 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_category.py
+-rw-r--r--   0        0        0     4410 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_category_type.py
+-rw-r--r--   0        0        0     4276 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_comment.py
+-rw-r--r--   0        0        0     4768 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_example.py
+-rw-r--r--   0        0        0     9088 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_label.py.unused.bak
+-rw-r--r--   0        0        0     3744 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_member.py
+-rw-r--r--   0        0        0     5057 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_project.py
+-rw-r--r--   0        0        0     1795 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_relation.py
+-rw-r--r--   0        0        0     4410 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_relation_type.py
+-rw-r--r--   0        0        0     1673 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_span.py
+-rw-r--r--   0        0        0     4010 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_span_type.py
+-rw-r--r--   0        0        0     1661 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_text.py
+-rw-r--r--   0        0        0     2640 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/test_client.py
+-rw-r--r--   0        0        0     3722 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/test_full_integration_tests.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/utils/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/tests/utils/test_response.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/utils/__init__.py
+-rw-r--r--   0        0        0      638 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/beta/utils/response.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/__init__.py
+-rw-r--r--   0        0        0      824 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/languages.py
+-rw-r--r--   0        0        0     4095 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/manager.py
+-rw-r--r--   0        0        0     5294 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/models.py
+-rw-r--r--   0        0        0     4012 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/preparation.py
+-rw-r--r--   0        0        0      954 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/strategies.py
+-rw-r--r--   0        0        0     1360 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/active_learning/trainer.py
+-rw-r--r--   0        0        0     5304 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/commands.py
+-rw-r--r--   0        0        0      549 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/entity.py
+-rw-r--r--   0        0        0      958 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/estimators.py
+-rw-r--r--   0        0        0     3419 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/cli/usecases.py
+-rw-r--r--   0        0        0    53125 2023-06-13 02:25:26.955544 doccano_client-1.2.8/doccano_client/client.py
+-rw-r--r--   0        0        0      531 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/__init__.py
+-rw-r--r--   0        0        0      228 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/comment.py
+-rw-r--r--   0        0        0       94 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/data_download.py
+-rw-r--r--   0        0        0      688 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/data_upload.py
+-rw-r--r--   0        0        0      392 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/example.py
+-rw-r--r--   0        0        0     1401 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/label.py
+-rw-r--r--   0        0        0     1946 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/label_type.py
+-rw-r--r--   0        0        0      266 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/member.py
+-rw-r--r--   0        0        0      431 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/metrics.py
+-rw-r--r--   0        0        0     2955 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/project.py
+-rw-r--r--   0        0        0       82 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/role.py
+-rw-r--r--   0        0        0      185 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/task_status.py
+-rw-r--r--   0        0        0      128 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/user.py
+-rw-r--r--   0        0        0      835 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/models/user_details.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/__init__.py
+-rw-r--r--   0        0        0     5326 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/base.py
+-rw-r--r--   0        0        0     3710 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/comment.py
+-rw-r--r--   0        0        0     3129 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/data_download.py
+-rw-r--r--   0        0        0     2604 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/data_upload.py
+-rw-r--r--   0        0        0     4414 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/example.py
+-rw-r--r--   0        0        0     4336 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/label.py
+-rw-r--r--   0        0        0     5207 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/label_type.py
+-rw-r--r--   0        0        0     3351 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/member.py
+-rw-r--r--   0        0        0     3404 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/metrics.py
+-rw-r--r--   0        0        0     3131 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/project.py
+-rw-r--r--   0        0        0     1044 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/role.py
+-rw-r--r--   0        0        0     1294 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/task_status.py
+-rw-r--r--   0        0        0     1883 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/user.py
+-rw-r--r--   0        0        0     1792 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/repositories/user_details.py
+-rw-r--r--   0        0        0     1111 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/services/label_type.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/__init__.py
+-rw-r--r--   0        0        0     2756 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/comment.py
+-rw-r--r--   0        0        0     1681 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/data_download.py
+-rw-r--r--   0        0        0     1879 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/data_upload.py
+-rw-r--r--   0        0        0     4061 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/example.py
+-rw-r--r--   0        0        0    19920 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/label.py
+-rw-r--r--   0        0        0     4437 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/label_type.py
+-rw-r--r--   0        0        0     3060 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/member.py
+-rw-r--r--   0        0        0     6051 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/project.py
+-rw-r--r--   0        0        0      419 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/role.py
+-rw-r--r--   0        0        0     2253 2023-06-13 02:25:26.959544 doccano_client-1.2.8/doccano_client/usecase/user_details.py
+-rw-r--r--   0        0        0     2461 2023-06-13 02:25:26.959544 doccano_client-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 doccano_client-1.2.8/PKG-INFO
```

### Comparing `doccano_client-1.2.7/LICENSE` & `doccano_client-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/README.md` & `doccano_client-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/README.md` & `doccano_client-1.2.8/doccano_client/beta/README.md`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/client.py` & `doccano_client-1.2.8/doccano_client/beta/client.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/__init__.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/annotation.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/annotation.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/category.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/category.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/category_type.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/category_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/comment.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/comment.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/example.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/example.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/label.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/label.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/member.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/member.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/project.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/project.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/relation.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/relation.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/relation_type.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/relation_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/span.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/span.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/span_type.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/span_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/controllers/text.py` & `doccano_client-1.2.8/doccano_client/beta/controllers/text.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/__init__.py` & `doccano_client-1.2.8/doccano_client/beta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/annotations.py` & `doccano_client-1.2.8/doccano_client/beta/models/annotations.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/category_type.py` & `doccano_client-1.2.8/doccano_client/beta/models/category_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/examples.py` & `doccano_client-1.2.8/doccano_client/beta/models/examples.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/labels.py` & `doccano_client-1.2.8/doccano_client/beta/models/labels.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/projects.py` & `doccano_client-1.2.8/doccano_client/beta/models/projects.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/relation_type.py` & `doccano_client-1.2.8/doccano_client/beta/models/relation_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/models/span_type.py` & `doccano_client-1.2.8/doccano_client/beta/models/span_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/conftest.py` & `doccano_client-1.2.8/doccano_client/beta/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/annotations.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/annotations.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/categories.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/categories.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/category_types.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/category_types.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/comments.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/comments.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/examples.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/examples.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/labels.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/labels.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/members.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/members.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/projects.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/projects.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/relation_types.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/relation_types.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/relations.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/relations.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/span_types.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/span_types.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/spans.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/spans.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/mock_api_responses/texts.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/mock_api_responses/texts.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_annotation.py.unused.bak` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_annotation.py.unused.bak`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_category.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_category.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_category_type.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_category_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_comment.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_comment.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_example.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_example.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_label.py.unused.bak` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_label.py.unused.bak`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_member.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_member.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_project.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_project.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_relation.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_relation.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_relation_type.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_relation_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_span.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_span.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_span_type.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_span_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/controllers/test_text.py` & `doccano_client-1.2.8/doccano_client/beta/tests/controllers/test_text.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/test_client.py` & `doccano_client-1.2.8/doccano_client/beta/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/test_full_integration_tests.py` & `doccano_client-1.2.8/doccano_client/beta/tests/test_full_integration_tests.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/tests/utils/test_response.py` & `doccano_client-1.2.8/doccano_client/beta/tests/utils/test_response.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/beta/utils/response.py` & `doccano_client-1.2.8/doccano_client/beta/utils/response.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/languages.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/languages.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/manager.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/manager.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/models.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/models.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/preparation.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/preparation.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/strategies.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/strategies.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/active_learning/trainer.py` & `doccano_client-1.2.8/doccano_client/cli/active_learning/trainer.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/commands.py` & `doccano_client-1.2.8/doccano_client/cli/commands.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/entity.py` & `doccano_client-1.2.8/doccano_client/cli/entity.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/estimators.py` & `doccano_client-1.2.8/doccano_client/cli/estimators.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/cli/usecases.py` & `doccano_client-1.2.8/doccano_client/cli/usecases.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/client.py` & `doccano_client-1.2.8/doccano_client/client.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/exceptions.py` & `doccano_client-1.2.8/doccano_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/models/data_upload.py` & `doccano_client-1.2.8/doccano_client/models/data_upload.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/models/label.py` & `doccano_client-1.2.8/doccano_client/models/label.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/models/label_type.py` & `doccano_client-1.2.8/doccano_client/models/label_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/models/project.py` & `doccano_client-1.2.8/doccano_client/models/project.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/models/user_details.py` & `doccano_client-1.2.8/doccano_client/models/user_details.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/base.py` & `doccano_client-1.2.8/doccano_client/repositories/base.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/comment.py` & `doccano_client-1.2.8/doccano_client/repositories/comment.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/data_download.py` & `doccano_client-1.2.8/doccano_client/repositories/data_download.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/data_upload.py` & `doccano_client-1.2.8/doccano_client/repositories/data_upload.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/example.py` & `doccano_client-1.2.8/doccano_client/repositories/example.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/label.py` & `doccano_client-1.2.8/doccano_client/repositories/label.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/label_type.py` & `doccano_client-1.2.8/doccano_client/repositories/label_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/member.py` & `doccano_client-1.2.8/doccano_client/repositories/member.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/metrics.py` & `doccano_client-1.2.8/doccano_client/repositories/metrics.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/project.py` & `doccano_client-1.2.8/doccano_client/repositories/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 from __future__ import annotations
 
-from typing import Iterator
+from typing import Any, Dict, Iterator
 
 from doccano_client.models.project import Project
 from doccano_client.repositories.base import BaseRepository
 
 
 class ProjectRepository:
     """Repository for interacting with the Doccano project API"""
 
     def __init__(self, client: BaseRepository):
         self._client = client
 
+    def _to_domain(self, response: Dict[str, Any]) -> Project:
+        """Convert a response to a domain object
+
+        Args:
+            response (Dict[str, Any]): The response to convert
+
+        Returns:
+            Project: The converted project
+        """
+        response["tags"] = [tag["text"] for tag in response.get("tags", [])]
+        return Project.parse_obj(response)
+
+    def _to_persistent(self, project: Project) -> Dict[str, Any]:
+        """Convert a domain object to a persistent object
+
+        Args:
+            project (Project): The project to convert
+
+        Returns:
+            Dict[str, Any]: The converted project
+        """
+        project_dict = project.dict()
+        project_dict["tags"] = [{"text": tag} for tag in project_dict["tags"]]
+        return project_dict
+
     def find_by_id(self, project_id: int) -> Project:
         """Find a project by id
 
         Args:
             project_id (int): The id of the project to find
 
         Returns:
             Project: The found project
         """
         response = self._client.get(f"projects/{project_id}")
-        return Project.parse_obj(response.json())
+        return self._to_domain(response.json())
 
     def list(self) -> Iterator[Project]:
         """Return all projects in which you are a member
 
         Yields:
             Project: The next project.
         """
         response = self._client.get("projects")
 
         while True:
             projects = response.json()
             for project in projects["results"]:
-                yield Project.parse_obj(project)
+                yield self._to_domain(project)
 
             if projects["next"] is None:
                 break
             else:
                 response = self._client.get(projects["next"])
 
     def create(self, project: Project) -> Project:
@@ -47,29 +72,32 @@
 
         Args:
             project (Project): The project to create
 
         Returns:
             Project: The created project
         """
-        response = self._client.post("projects", json=project.dict(exclude={"id"}))
-        return Project.parse_obj(response.json())
+        payload = self._to_persistent(project)
+        payload.pop("id", None)
+        response = self._client.post("projects", json=payload)
+        return self._to_domain(response.json())
 
     def update(self, project: Project) -> Project:
         """Update a project
 
         Args:
             project (Project): The project to update
 
         Returns:
             Project: The updated project
         """
         resource = f"projects/{project.id}"
-        response = self._client.put(resource, json=project.dict())
-        return Project.parse_obj(response.json())
+        payload = self._to_persistent(project)
+        response = self._client.put(resource, json=payload)
+        return self._to_domain(response.json())
 
     def delete(self, project: Project | int):
         """Delete a project
 
         Args:
             project (Project | int): The project to delete
         """
```

### Comparing `doccano_client-1.2.7/doccano_client/repositories/role.py` & `doccano_client-1.2.8/doccano_client/repositories/role.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/task_status.py` & `doccano_client-1.2.8/doccano_client/repositories/task_status.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/user.py` & `doccano_client-1.2.8/doccano_client/repositories/user.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/repositories/user_details.py` & `doccano_client-1.2.8/doccano_client/repositories/user_details.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/services/label_type.py` & `doccano_client-1.2.8/doccano_client/services/label_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/comment.py` & `doccano_client-1.2.8/doccano_client/usecase/comment.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/data_download.py` & `doccano_client-1.2.8/doccano_client/usecase/data_download.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/data_upload.py` & `doccano_client-1.2.8/doccano_client/usecase/data_upload.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/example.py` & `doccano_client-1.2.8/doccano_client/usecase/example.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/label.py` & `doccano_client-1.2.8/doccano_client/usecase/label.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/label_type.py` & `doccano_client-1.2.8/doccano_client/usecase/label_type.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/member.py` & `doccano_client-1.2.8/doccano_client/usecase/member.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/project.py` & `doccano_client-1.2.8/doccano_client/usecase/project.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/doccano_client/usecase/user_details.py` & `doccano_client-1.2.8/doccano_client/usecase/user_details.py`

 * *Files identical despite different names*

### Comparing `doccano_client-1.2.7/pyproject.toml` & `doccano_client-1.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doccano-client"
-version = "1.2.7"
+version = "1.2.8"
 description = "A simple client for doccano API."
 authors = ["Hironsan <hiroki.nakayama.py@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/doccano/doccano-client"
 repository = "https://github.com/doccano/doccano-client"
 classifiers = [
```

### Comparing `doccano_client-1.2.7/PKG-INFO` & `doccano_client-1.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: doccano-client
-Version: 1.2.7
+Version: 1.2.8
 Summary: A simple client for doccano API.
 Home-page: https://github.com/doccano/doccano-client
 License: MIT
 Author: Hironsan
 Author-email: hiroki.nakayama.py@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Provides-Extra: al
 Provides-Extra: spacy
 Provides-Extra: whisper
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0) ; extra == "whisper"
 Requires-Dist: pandas (>=1.5.1,<2.0.0) ; extra == "al"
```

