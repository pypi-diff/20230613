# Comparing `tmp/iambic_core-0.8.1.tar.gz` & `tmp/iambic_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.8.1.tar", max compression
+gzip compressed data, was "iambic_core-0.9.1.tar", max compression
```

## Comparing `iambic_core-0.8.1.tar` & `iambic_core-0.9.1.tar`

### file list

```diff
@@ -1,163 +1,162 @@
--rw-r--r--   0        0        0    11356 2023-05-30 20:48:04.299115 iambic_core-0.8.1/LICENSE.md
--rw-r--r--   0        0        0    15630 2023-05-30 20:48:04.299115 iambic_core-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/templates.py
--rw-r--r--   0        0        0     3312 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/utils.py
--rw-r--r--   0        0        0    77625 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/logger.py
--rw-r--r--   0        0        0    24977 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5516 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/parser.py
--rw-r--r--   0        0        0    48021 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    31220 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    14289 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-30 20:48:04.335115 iambic_core-0.8.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2728 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2712 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     2102 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    17407 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    39352 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    18144 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13681 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15896 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    18077 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10706 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21757 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24521 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    21076 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22644 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     5650 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35636 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    30301 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
--rw-r--r--   0        0        0      101 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
--rw-r--r--   0        0        0    18860 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
--rw-r--r--   0        0        0    11040 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
--rw-r--r--   0        0        0    19286 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
--rw-r--r--   0        0        0     1291 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.339115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     3009 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10209 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    14003 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8798 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14801 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5237 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1359 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9327 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11442 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-30 20:48:04.343115 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2685 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1290 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9587 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      994 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      173 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-30 20:48:04.347116 iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     2312 2023-05-30 20:48:04.347116 iambic_core-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    18129 1970-01-01 00:00:00.000000 iambic_core-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-13 13:55:31.171837 iambic_core-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0    15630 2023-06-13 13:55:31.171837 iambic_core-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    19724 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0     3312 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    79176 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15943 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4845 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1844 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    25633 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5515 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    48281 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    33010 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    14434 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2728 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2712 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     2102 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    17407 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    39712 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    18144 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13681 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15896 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    18077 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10706 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21757 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24602 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    21076 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22644 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     5842 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35636 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    30301 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
+-rw-r--r--   0        0        0    18860 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
+-rw-r--r--   0        0        0    11040 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
+-rw-r--r--   0        0        0    19286 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
+-rw-r--r--   0        0        0     1291 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     3009 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10209 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    14003 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3820 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2283 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     2033 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8798 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3783 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0     1128 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    34737 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    12212 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     2015 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5383 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14801 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5437 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1359 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7860 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3029 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3177 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9327 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3176 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11442 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3606 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2502 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2890 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1290 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3495 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4293 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      994 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      173 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     2263 2023-06-13 13:55:31.215837 iambic_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    17598 1970-01-01 00:00:00.000000 iambic_core-0.9.1/PKG-INFO
```

### Comparing `iambic_core-0.8.1/LICENSE.md` & `iambic_core-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/README.md` & `iambic_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/config/dynamic_config.py` & `iambic_core-0.9.1/iambic/config/dynamic_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from pydantic import create_model as create_pydantic_model
 
 import iambic.plugins.v0_1_0.github
 from iambic.core.context import ctx
 from iambic.core.exceptions import MultipleSecretsNotAcceptedException
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.core.logger import log
-from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
+from iambic.core.models import (
+    BaseTemplate,
+    ConfigMixin,
+    ExecutionMessage,
+    TemplateChangeDetails,
+)
 from iambic.core.utils import sort_dict, yaml
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION, aws, azure_ad, google_workspace, okta
 
 CURRENT_IAMBIC_VERSION = "1"
 
 
 class CoreConfig(BaseModel):
@@ -90,15 +95,15 @@
 class ExtendsConfig(BaseModel):
     key: ExtendsConfigKey
     value: str
     assume_role_arn: Optional[str]
     external_id: Optional[str]
 
 
-class Config(BaseTemplate):
+class Config(ConfigMixin, BaseTemplate):
     template_type: str = "NOQ::Core::Config"
     version: str = Field(
         description="Do not change! The version of iambic this repo is compatible with.",
     )
     plugins: Optional[list[PluginDefinition]] = Field(
         default=[
             PluginDefinition(
@@ -151,17 +156,25 @@
         return getattr(self, plugin.config_name)
 
     def set_config_plugin(self, plugin: ProviderPlugin, config: BaseModel):
         setattr(self, plugin.config_name, config)
 
     @property
     def configured_plugins(self):
-        return [
-            plugin for plugin in self.plugin_instances if self.get_config_plugin(plugin)
-        ]
+        plugin_instances = getattr(self, "plugin_instances", [])
+
+        return [plugin for plugin in plugin_instances if self.get_config_plugin(plugin)]
+
+    @property
+    def templates(self):
+        templates = []
+        for plugin in self.configured_plugins:
+            templates.extend([template for template in plugin.templates])
+
+        return templates
 
     async def set_config_secrets(self):
         if self.extends:
             if len(self.extends) > 1:
                 raise MultipleSecretsNotAcceptedException()
 
             extend = self.extends[0]
@@ -282,36 +295,24 @@
         elif not ctx.execute:
             log.info("Finished scanning for changes.")
         else:
             log.info("No changes found.")
 
         return template_changes
 
-    async def run_detect_changes(
-        self, repo_dir: str, run_import_as_fallback: bool = False
-    ) -> Union[str, None]:
+    async def run_detect_changes(self, repo_dir: str) -> Union[str, None]:
         change_str_list = await asyncio.gather(
             *[
                 plugin.async_detect_changes_callable(
                     self.get_config_plugin(plugin), repo_dir
                 )
                 for plugin in self.configured_plugins
                 if plugin.async_detect_changes_callable
             ]
         )
-        if run_import_as_fallback:
-            await asyncio.gather(
-                *[
-                    plugin.async_import_callable(
-                        self.get_config_plugin(plugin), repo_dir
-                    )
-                    for plugin in self.configured_plugins
-                    if not plugin.async_detect_changes_callable
-                ]
-            )
 
         if change_str_list := [
             change_str for change_str in change_str_list if change_str
         ]:
             return "\n".join(change_str_list)
 
     async def run_discover_upstream_config_changes(
@@ -466,16 +467,14 @@
 async def process_config(
     base_config: Config,
     config_path,
     config_dict,
     configure_plugins: bool = True,
     approved_plugins_only: bool = False,
 ) -> Config:
-    from iambic.config.templates import TEMPLATES
-
     if approved_plugins_only:
         default_plugins = [
             plugin.location for plugin in Config.__fields__["plugins"].default
         ]
         base_config.plugins = [
             plugin
             for plugin in base_config.plugins
@@ -495,21 +494,14 @@
     )
 
     if configure_plugins:
         log.info("Setting config metadata...")
         await config.configure_plugins()
         log.info("Plugins loaded successfully...")
 
-    TEMPLATES.set_templates(
-        list(
-            itertools.chain.from_iterable(
-                [plugin.templates for plugin in config.plugin_instances]
-            )
-        )
-    )
     return config
 
 
 async def init_plugins(config_path: str):
     """
     Download plugins and install plugin dependencies
     """
```

### Comparing `iambic_core-0.8.1/iambic/config/utils.py` & `iambic_core-0.9.1/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/config/wizard.py` & `iambic_core-0.9.1/iambic/config/wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -612,17 +612,30 @@
                 )
                 continue
 
             self.profile_name = profile_name
             with contextlib.suppress(
                 ClientError, NoCredentialsError, FileNotFoundError
             ):
-                self.autodetected_org_settings = self.boto3_session.client(
+                org_client = self.boto3_session.client(
                     "organizations", region_name=self.aws_default_region
-                ).describe_organization()["Organization"]
+                )
+                self.autodetected_org_settings = org_client.describe_organization()[
+                    "Organization"
+                ]
+                self._has_cf_permissions = (
+                    "member.org.stacksets.cloudformation.amazonaws.com"
+                    in [
+                        p["ServicePrincipal"]
+                        for p in org_client.list_aws_service_access_for_organization()[
+                            "EnabledServicePrincipals"
+                        ]
+                    ]
+                )
+
             break
 
     def get_boto3_session_for_account(self, account_id: str, region_name: str = None):
         # This need to follow standard credentials provider chain
         if not region_name:
             region_name = self.aws_default_region
 
@@ -691,15 +704,19 @@
             exe_message = ExecutionMessage(
                 execution_id=str(uuid.uuid4()),
                 command=Command.APPLY,
                 provider_type="aws",
             )
             sub_config = self.config.aws.copy()
             sub_config.accounts = accounts
-            await aws_apply(exe_message, sub_config, load_templates(templates))
+            await aws_apply(
+                exe_message,
+                sub_config,
+                load_templates(templates, sub_config.template_map),
+            )
             ctx.command = current_command
 
         await self.run_import_aws_resources()
 
     async def sync_config_aws_org(self, run_config_discovery: bool = True):
         if not self.config.aws:
             self.config.aws = AWSConfig()
@@ -1075,17 +1092,24 @@
             if questionary.confirm("Would you like to use this identity?").ask():
                 self.caller_identity = default_caller_identity
                 # If we are going to use the default_caller_identity,
                 # we need to set teh autodetected_org_settings to
                 with contextlib.suppress(
                     ClientError, NoCredentialsError, FileNotFoundError
                 ):
-                    self.autodetected_org_settings = self.boto3_session.client(
-                        "organizations"
-                    ).describe_organization()["Organization"]
+                    org_client = self.boto3_session.client("organizations")
+                    self.autodetected_org_settings = org_client.describe_organization()[
+                        "Organization"
+                    ]
+                    self._has_cf_permissions = "member.org.stacksets.cloudformation.amazonaws.com" in [
+                        p["ServicePrincipal"]
+                        for p in org_client.list_aws_service_access_for_organization()[
+                            "EnabledServicePrincipals"
+                        ]
+                    ]
             else:
                 self.set_boto3_session()
         else:
             self.set_boto3_session()
 
         asyncio.run(self.sync_config_aws_org())
 
@@ -1267,20 +1291,32 @@
             if questionary.confirm("Exit?").unsafe_ask():
                 log.info("Exiting...")
                 sys.exit(0)
 
         asyncio.run(self.sync_config_aws_org())
 
     def configuration_wizard_aws_organizations(self):
-        # Currently only 1 org per config is supported.
-        click.echo(
-            "\nIf you would like to use AWS Organizations, the IAMbic hub account you configured must be the same "
-            "AWS account as your AWS Organization."
-        )
-        if questionary.confirm("Is this the case?").unsafe_ask():
+        def maybe_prompt():
+            if (
+                self.autodetected_org_settings
+                and self.hub_account_id
+                == self.autodetected_org_settings["MasterAccountId"]
+            ):
+                # https://github.com/noqdev/iambic/issues/405
+                # no need to prompt because we succeed in detecting organization and hub_account_id matches the org management account
+                return True
+            else:
+                # Currently only 1 org per config is supported.
+                click.echo(
+                    "\nIf you would like to use AWS Organizations, the IAMbic hub account you configured must be the same "
+                    "AWS account as your AWS Organization."
+                )
+                return questionary.confirm("Is this the case?").unsafe_ask()
+
+        if maybe_prompt():
             if self.config.aws and self.config.aws.organizations:
                 self.configuration_wizard_aws_organizations_edit()
             else:
                 self.configuration_wizard_aws_organizations_add()
 
     def configuration_wizard_aws(self):
         self.setup_aws_configuration()
@@ -1879,15 +1915,17 @@
         # cloudtrail is not cross-region, so we need to use us-east-1
         # sqs_arn = f"arn:aws:sqs:{self.aws_default_region}:{hub_account_id}:IAMbicChangeDetectionQueue{IAMBIC_CHANGE_DETECTION_SUFFIX}"
         sqs_arn = f"arn:aws:sqs:us-east-1:{hub_account_id}:IAMbicChangeDetectionQueue{IAMBIC_CHANGE_DETECTION_SUFFIX}"
 
         if not self.existing_role_template_map:
             log.info("Loading AWS role templates...")
             self.existing_role_template_map = asyncio.run(
-                get_existing_template_map(self.repo_dir, AWS_IAM_ROLE_TEMPLATE_TYPE)
+                get_existing_template_map(
+                    self.repo_dir, AWS_IAM_ROLE_TEMPLATE_TYPE, self.config.template_map
+                )
             )
 
         role_template: AwsIamRoleTemplate = self.existing_role_template_map.get(
             role_name
         )
 
         self.config.aws.sqs_cloudtrail_changes_queues = [sqs_arn]
```

### Comparing `iambic_core-0.8.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.9.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/core/exceptions.py` & `iambic_core-0.9.1/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/core/git.py` & `iambic_core-0.9.1/iambic/core/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import os
 import re
 from io import StringIO
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Type
 
 from deepdiff import DeepDiff
 from git import Repo
 from git.exc import GitCommandError
 from pydantic import BaseModel as PydanticBaseModel
 
-from iambic.config.templates import TEMPLATES
 from iambic.core.logger import log
+from iambic.core.models import BaseTemplate
 from iambic.core.parser import load_templates
 from iambic.core.utils import NOQ_TEMPLATE_REGEX, file_regex_search, yaml
 
 if TYPE_CHECKING:
     from iambic.config.dynamic_config import Config
 
 
@@ -74,14 +74,15 @@
     if default_branch == "":
         default_branch = "main"
     return default_branch
 
 
 async def retrieve_git_changes(
     repo_dir: str,
+    template_map: dict[str, Type[BaseTemplate]],
     allow_dirty: bool = False,
     from_sha=None,
     to_sha=None,
 ) -> dict[str, list[GitDiff]]:
     repo = Repo(repo_dir)
     if repo.is_dirty():
         log.error(
@@ -162,20 +163,25 @@
                         template_dict,
                         main_template_dict,
                         ignore_order=True,
                         report_repetition=True,
                     ):
                         continue  # Just renamed but no file changes
 
-                    template_cls = TEMPLATES.template_map[
-                        main_template_dict["template_type"]
-                    ]
+                    if not (
+                        template_cls := _get_template_map(
+                            template_map, main_template_dict
+                        )
+                    ):
+                        continue
+
                     main_template = template_cls(
                         file_path=deleted_file.path, **main_template_dict
                     )
+                    main_template.is_memory_only = True
                     template = template_cls(file_path=path, **template_dict)
                     if main_template.resource_id != template.resource_id:
                         files["deleted_files"].append(deleted_file)
                         files["new_files"].append(GitDiff(path=path))
                         continue
 
             file = GitDiff(
@@ -183,62 +189,68 @@
                 content=file_obj.a_blob.data_stream.read().decode("utf-8"),
             )
             files["modified_files"].append(file)
 
     return files
 
 
-def create_templates_for_deleted_files(deleted_files: list[GitDiff]) -> list:
+def create_templates_for_deleted_files(
+    deleted_files: list[GitDiff], template_map: dict[str, Type[BaseTemplate]]
+) -> list:
     """
     Create a class instance of the deleted file content with its template type
     If it wasn't deleted, set it to deleted
     Add that instance to templates
     """
     templates = []
     for git_diff in deleted_files:
         template_dict = yaml.load(StringIO(git_diff.content))
-        template_cls = TEMPLATES.template_map[template_dict["template_type"]]
+        if not (template_cls := _get_template_map(template_map, template_dict)):
+            continue
+
         template = template_cls(file_path=git_diff.path, **template_dict)
+        template.is_memory_only = True
         if template.deleted is True:
             continue
         template.deleted = True
         log.info("Template marked as deleted", file_path=git_diff.path)
         templates.append(template)
 
     return templates
 
 
 def create_templates_for_modified_files(
-    config: Config, modified_files: list[GitDiff]
+    config: Config,
+    modified_files: list[GitDiff],
 ) -> list:
     """
     Create a class instance of the original file content and the new file content with its template type
     Check for aws_accounts that were removed from included_accounts or added to excluded_accounts
     Update the template to be applied to delete the role from the aws_accounts that hit on the above statement
     """
     templates = []
     for git_diff in modified_files:
         main_template_dict = yaml.load(StringIO(git_diff.content))
         template_type_string = main_template_dict["template_type"]
-        template_cls = TEMPLATES.template_map.get(template_type_string, None)
+        template_cls = config.template_map.get(template_type_string, None)
 
         if template_cls is None:
             # well the case is the previous version is an unknown config type now.
             # this is typically the config file
             log_params = {"template_type": template_type_string}
             log.warning(
                 "template_type is not registered among template_map", **log_params
             )
             continue
 
         main_template = template_cls(file_path=git_diff.path, **main_template_dict)
 
         # template_dict = yaml.load(open(git_diff.path))
         # template = template_cls(file_path=git_diff.path, **template_dict)
-        template = load_templates([git_diff.path])[0]
+        template = load_templates([git_diff.path], config.template_map)[0]
 
         # EN-1634 dealing with providers that have no concept of multi-accounts
         # a hack to just ignore template that does not have included_accounts attribute
         if getattr(main_template, "included_accounts", None) is None:
             templates.append(template)
             # The rest of the account inclusion/exclusion logic does not apply
             # plugin that does not have concept of included_accounts
@@ -372,7 +384,20 @@
 
         if deleted_included_accounts and template.deleted is not True:
             template.deleted = True
 
         templates.append(template)
 
     return templates
+
+
+def _get_template_map(
+    template_map: dict[str, Type[BaseTemplate]],
+    main_template_dict: dict,
+) -> Type[BaseTemplate] | None:
+    template_cls = template_map.get(main_template_dict.get("template_type", "N/A"))
+    if not template_cls:
+        log.error(
+            f"Template type not found: {main_template_dict.get('template_type', 'N/A')}"
+        )
+
+    return template_cls
```

### Comparing `iambic_core-0.8.1/iambic/core/iambic_enum.py` & `iambic_core-0.9.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/core/iambic_plugin.py` & `iambic_core-0.9.1/iambic/core/iambic_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Any, Optional
+from typing import Any, Optional, Type
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Field
 
 from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
 
 
@@ -90,8 +90,17 @@
     async_discover_upstream_config_changes_callable: Optional[Any] = Field(
         description="(OPTIONAL) The function that called to discover upstream config changes."
         "An example of this would be a new account being added to an AWS Organization,"
         "or a change to AWS account's name or tags."
         "This function must accept the params: (exe_message: ExecutionMessage, config: ProviderConfig, repo_dir: str, remote_worker: Worker = None)",
         hidden_from_schema=True,
     )
-    templates: list = Field(description="The list of templates used for this provider.")
+    templates: list[Type[BaseTemplate]] = Field(
+        description="The list of templates used for this provider."
+    )
+
+    @property
+    def template_map(self) -> dict[str, Type[BaseTemplate]]:
+        return {
+            template.__fields__["template_type"].default: template
+            for template in self.templates
+        }
```

### Comparing `iambic_core-0.8.1/iambic/core/logger.py` & `iambic_core-0.9.1/iambic/core/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,37 +23,41 @@
             value = "\n  ".join(str(json.dumps(value, indent=2)).split("\n"))
 
         return_dict[key] = value
 
     return return_dict
 
 
-LOG_LEVEL = os.getenv("LOG_LEVEL", "INFO")
-logging.basicConfig(level=LOG_LEVEL)
-structlog.configure(
-    processors=[
-        pretty_log,
-        structlog.processors.add_log_level,
-        structlog.processors.StackInfoRenderer(),
-        structlog.dev.set_exc_info,
-        structlog.processors.TimeStamper("%Y/%m/%d %H:%M:%S", utc=False),
-        structlog.dev.ConsoleRenderer(),
-    ],
-    wrapper_class=structlog.make_filtering_bound_logger(
-        logging.getLevelName(LOG_LEVEL)
-    ),
-    context_class=dict,
-    logger_factory=structlog.PrintLoggerFactory(),
-    cache_logger_on_first_use=False,
-)
-log = structlog.get_logger("NoqForm")
-
-if LOG_LEVEL == "DEBUG":
-    boto3.set_stream_logger("", "DEBUG")
-else:
-    default_logging_levels = {
-        "boto3": "CRITICAL",
-        "boto": "CRITICAL",
-        "botocore": "CRITICAL",
-    }
-    for logger, level in default_logging_levels.items():
-        logging.getLogger(logger).setLevel(level)
+def configure_logger(logger_name, log_level):
+    structlog.configure(
+        processors=[
+            pretty_log,
+            structlog.processors.add_log_level,
+            structlog.processors.StackInfoRenderer(),
+            structlog.dev.set_exc_info,
+            structlog.processors.TimeStamper("%Y/%m/%d %H:%M:%S", utc=False),
+            structlog.dev.ConsoleRenderer(),
+        ],
+        wrapper_class=structlog.make_filtering_bound_logger(
+            logging.getLevelName(log_level)
+        ),
+        context_class=dict,
+        logger_factory=structlog.PrintLoggerFactory(),
+        cache_logger_on_first_use=False,
+    )
+    log = structlog.get_logger(logger_name)
+
+    if log_level == "DEBUG":
+        boto3.set_stream_logger("", "DEBUG")
+    else:
+        default_logging_levels = {
+            "boto3": "CRITICAL",
+            "boto": "CRITICAL",
+            "botocore": "CRITICAL",
+        }
+        for logger, level in default_logging_levels.items():
+            logging.getLogger(logger).setLevel(level)
+
+    return log
+
+
+log = configure_logger("iambic", os.getenv("LOG_LEVEL", "INFO"))
```

### Comparing `iambic_core-0.8.1/iambic/core/models.py` & `iambic_core-0.9.1/iambic/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
     Set,
+    Type,
     Union,
     get_args,
     get_origin,
 )
 
 import aiofiles
 import dateparser
@@ -489,14 +490,19 @@
     template_type: str
     file_path: Union[str, Path] = Field(..., hidden_from_schema=True)
     owner: Optional[str]
     iambic_managed: Optional[IambicManaged] = Field(
         IambicManaged.UNDEFINED,
         description="Controls the directionality of Iambic changes",
     )
+    is_memory_only: Optional[bool] = Field(
+        False,
+        description="if true, it's in-memory only used for clean up operation",
+        hidden_from_schema=True,
+    )
 
     def dict(
         self,
         *,
         include: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
         exclude: Optional[Union["AbstractSetIntStr", "MappingIntStrAny"]] = None,
         by_alias: bool = False,
@@ -547,14 +553,17 @@
         as_yaml = self.get_body(exclude_none, exclude_unset, exclude_defaults)
         os.makedirs(os.path.dirname(os.path.expanduser(self.file_path)), exist_ok=True)
         with open(self.file_path, "w") as f:
             f.write(as_yaml)
 
     def delete(self):
         log.info("Deleting template file", file_path=self.file_path)
+        if self.is_memory_only:
+            log.info("template file is in-memory-only", file_path=self.file_path)
+            return
         try:
             repo = Repo(self.file_path, search_parent_directories=True)
             # why force=True? Expire could have modified the local contents
             # without force=True, git rm would not be able to remove the file
             repo.index.remove(
                 [
                     str(self.file_path)
@@ -724,7 +733,20 @@
 
         return response
 
 
 class ExecutionResponse(ExecutionMessage):
     status: ExecutionStatus
     errors: Optional[list[str]]
+
+
+class ConfigMixin:
+    @property
+    def templates(self) -> list[Type[BaseTemplate]]:
+        raise NotImplementedError
+
+    @property
+    def template_map(self) -> dict[str, Type[BaseTemplate]]:
+        return {
+            template.__fields__["template_type"].default: template
+            for template in self.templates
+        }
```

### Comparing `iambic_core-0.8.1/iambic/core/noq_json.py` & `iambic_core-0.9.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/core/parser.py` & `iambic_core-0.9.1/iambic/core/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import json
 import os
 import sys
 import time
 import traceback
 from functools import partial
-from typing import Union
+from typing import Type, Union
 
 from pydantic import ValidationError
 from ruamel.yaml.scanner import ScannerError
 
-from iambic.config.templates import TEMPLATES
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate
 from iambic.core.utils import transform_comments, yaml
 
 # we must avoid import multiprocessing pool in the module loading time
 if os.environ.get("AWS_LAMBDA_FUNCTION_NAME", False):
     from multiprocessing import cpu_count
@@ -90,14 +89,15 @@
         )
         if raise_validation_err:
             raise ValueError(f"{template_path} template has validation error.") from err
 
 
 def load_templates(
     template_paths: list[str],
+    template_map: dict[str, Type[BaseTemplate]],
     raise_validation_err: bool = True,
     use_multiprocessing=True,
 ) -> list[BaseTemplate]:
     templates = []
     template_dicts = None
 
     if use_multiprocessing:
@@ -117,15 +117,15 @@
         ]
 
     for template_dict in template_dicts:
         if not template_dict:
             continue
 
         try:
-            template_cls = TEMPLATES.template_map[template_dict["template_type"]]
+            template_cls = template_map[template_dict["template_type"]]
             template_cls.update_forward_refs()
             templates.append(template_cls(**template_dict))
         except KeyError:
             log.critical(
                 "Invalid template type",
                 file_path=template_dict["file_path"],
                 template_type=template_dict["template_type"],
```

### Comparing `iambic_core-0.8.1/iambic/core/template_generation.py` & `iambic_core-0.9.1/iambic/core/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Union
+from typing import Type, Union
 
 import xxhash
 
 from iambic.core import noq_json as json
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import AccessModelMixin, BaseModel, BaseTemplate, ProviderChild
@@ -17,26 +17,31 @@
     get_provider_value,
     is_regex_match,
     sanitize_string,
 )
 
 
 async def get_existing_template_map(
-    repo_dir: str, template_type: str, nested: bool = False
+    repo_dir: str,
+    template_type: str,
+    template_map: dict[str, Type[BaseTemplate]],
+    nested: bool = False,
 ) -> dict:
     """Used to keep track of existing templates on import
 
      Write to the existing file before creating a new one.
 
     :param repo_dir:
     :param template_type:
     :param nested: If true, will return a map of {template_type: {resource_id: template}}
     :return: {resource_id: template}
     """
-    templates = load_templates(await gather_templates(repo_dir, template_type))
+    templates = load_templates(
+        await gather_templates(repo_dir, template_type), template_map
+    )
     if not nested:
         return {template.resource_id: template for template in templates}
 
     response = defaultdict(dict)
     for template in templates:
         response[template.template_type][template.resource_id] = template
     return response
@@ -966,15 +971,19 @@
         """
         new_model = [new_model]
 
     for key in field_names:
         new_value = getattr(new_model, key)
         value_as_list = isinstance(new_value, list)
         existing_value = getattr(existing_model, key)
-        if isinstance(existing_value, list):
+        if key in iambic_fields:
+            # not something we want to merge because
+            # this is metadata only, not in the cloud-side
+            continue
+        elif isinstance(existing_value, list):
             if len(existing_value) > 0:
                 inner_element = existing_value[0]
 
                 if isinstance(inner_element, AccessModelMixin):
                     """
                     If the field is a list of objects that inherit from the AccessModelMixin:
                     Attempt to resolve the matching model between the 2 lists
```

### Comparing `iambic_core-0.8.1/iambic/core/utils.py` & `iambic_core-0.9.1/iambic/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from datetime import date, datetime, timezone
 from io import StringIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Coroutine, Optional, Union
 from urllib.parse import unquote_plus
 
 import aiofiles
+import jwt
 from asgiref.sync import sync_to_async
 from ruamel.yaml import YAML
 
 from iambic.core import noq_json as json
 from iambic.core.aio_utils import gather_limit
 from iambic.core.exceptions import RateLimitException
 from iambic.core.iambic_enum import IambicManaged
@@ -828,7 +829,64 @@
         data = yaml.load(input_string)
         # Convert keys from snake_case to PascalCase
         converted_data = normalize_dict_keys(data, pascalcase)
         # Convert to JSON
         output = json.dumps(converted_data, indent=2)
 
     return output
+
+
+def jws_encode_with_past_time(payload, private_key, algorithm, valid_period_in_minutes):
+    """
+    How to use?
+
+    # Generate a new ECDSA private key
+    from cryptography.hazmat.primitives.asymmetric import ec
+    private_key = ec.generate_private_key(ec.SECP256R1())  # This is equivalent to the ES256 algorithm
+    public_key = private_key.public_key()
+
+    # or load from PEM
+    from cryptography.hazmat.primitives import serialization
+    loaded_private_key = serialization.load_pem_private_key(
+        allowed_bot_approver_pub_key_string.encode("utf-8")
+    )
+
+    # payload
+    payload = {
+        "repo": "example.com/iambic-templates",
+        "pr": 1,
+        "signee": [
+            "user1@example.org",
+            "user2@example.org",
+        ]
+    }
+    algorithm = "ES256"
+    valid_period_in_minutes = 15
+    encoded_jwt = jws_encode_with_past_time(payload, private_pem, algorithm, valid_period_in_minutes)
+    """
+    import datetime as _datetime
+
+    reference_time = _datetime.datetime.now() + _datetime.timedelta(
+        minutes=valid_period_in_minutes
+    )
+    payload["exp"] = int(reference_time.timestamp())
+
+    encoded_jwt = jwt.encode(payload, private_key, algorithm=algorithm)
+    return encoded_jwt
+
+
+def decode_with_reference_time(encoded_jwt, public_key, algorithms, reference_time):
+    import datetime as _datetime
+
+    payload = jwt.decode(
+        encoded_jwt, public_key, algorithms=algorithms, options={"verify_exp": False}
+    )
+    exp = payload.get("exp")
+
+    if exp is not None:
+        exp = _datetime.datetime.fromtimestamp(exp)
+        if reference_time > exp:
+            raise jwt.exceptions.ExpiredSignatureError(
+                f"Signature has expired: ref: {reference_time} exp: {exp}"
+            )
+
+    return payload
```

### Comparing `iambic_core-0.8.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.9.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.9.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.9.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.9.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/github/utils.py` & `iambic_core-0.9.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/lambda/app.py` & `iambic_core-0.9.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/main.py` & `iambic_core-0.9.1/iambic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,21 +248,25 @@
         execution_id=str(uuid.uuid4()), command=Command.APPLY
     )
     if not templates:
         if not enforced_only:
             log.error("Please pass in specific templates to apply.")
             return template_changes
         templates = asyncio.run(gather_templates(repo_dir))
-    templates = load_templates(templates)
+    templates = load_templates(templates, config.template_map)  # type: ignore
     if enforced_only:
         templates = [t for t in templates if t.iambic_managed == IambicManaged.ENFORCED]
     if not templates:
         log.info("No templates found")
         return template_changes
-    asyncio.run(flag_expired_resources([template.file_path for template in templates]))
+    asyncio.run(
+        flag_expired_resources(
+            [template.file_path for template in templates], config.template_map
+        )
+    )
     template_changes = asyncio.run(config.run_apply(exe_message, templates))
     output_proposed_changes(template_changes, output_path=output_path)
 
     screen_render_resource_changes(template_changes)
 
     if ctx.eval_only and template_changes and click.confirm("Proceed?"):
         ctx.eval_only = False
@@ -358,15 +362,15 @@
     config = asyncio.run(load_config(config_path))
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.APPLY
     )
     asyncio.run(flag_expired_resources(templates))
     ctx.eval_only = True
     template_changes = asyncio.run(
-        config.run_apply(exe_message, load_templates(templates))
+        config.run_apply(exe_message, load_templates(templates, config.template_map))
     )
     output_proposed_changes(template_changes)
     screen_render_resource_changes(template_changes)
 
 
 @cli.command()
 @click.option(
@@ -423,20 +427,20 @@
     type=click.Path(exists=True),
     default=os.getenv("IAMBIC_REPO_DIR"),
     help="The repo directory containing the templates. Example: ~/iambic-templates",
 )
 def lint(templates: list[str], repo_dir: str):
     ctx.eval_only = True
     config_path = asyncio.run(resolve_config_template_path(repo_dir))
-    asyncio.run(load_config(config_path, configure_plugins=False))
+    config = asyncio.run(load_config(config_path, configure_plugins=False))
 
     if not templates:
         templates = asyncio.run(gather_templates(repo_dir))
 
-    templates = load_templates(templates, False)
+    templates = load_templates(templates, config.template_map, False)
     log.info("Formatting templates.")
     for template in templates:
         template.write()
 
 
 @cli.command(name="init")
 @click.option(
```

### Comparing `iambic_core-0.8.1/iambic/output/__init__.py` & `iambic_core-0.9.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/filters.py` & `iambic_core-0.9.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/models.py` & `iambic_core-0.9.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.9.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.9.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.9.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/output/text.py` & `iambic_core-0.9.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/README.md` & `iambic_core-0.9.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,15 @@
 
     if not exe_message.metadata or exe_message.metadata["service"] == "identity_center":
         identity_center_template_map = None
         if not remote_worker or exe_message.metadata:
             identity_center_template_map = await get_existing_template_map(
                 repo_dir=base_output_dir,
                 template_type="AWS::IdentityCenter.*",
+                template_map=config.template_map,
                 nested=True,
             )
 
         tasks.append(
             import_identity_center_resources(
                 exe_message,
                 config,
@@ -422,14 +423,15 @@
     if not exe_message.metadata or exe_message.metadata["service"] == "iam":
         iam_template_map = None
 
         if not remote_worker or exe_message.metadata:
             iam_template_map = await get_existing_template_map(
                 repo_dir=base_output_dir,
                 template_type="AWS::IAM.*",
+                template_map=config.template_map,
                 nested=True,
             )
 
         tasks.append(
             import_service_resources(
                 exe_message,
                 config,
@@ -466,14 +468,15 @@
     tasks = []
     if not config.organizations:
         return tasks
     exe_messages = await config.get_command_by_organization_account(exe_message)
     scp_template_map = await get_existing_template_map(
         repo_dir=base_output_dir,
         template_type=AWS_SCP_POLICY_TEMPLATE,
+        template_map=config.template_map,
         nested=True,
     )
 
     for exe_msg in exe_messages:
         aws_account_map: dict[str, AWSAccount] = await get_organizations_account_map(
             exe_msg, config
         )
@@ -707,28 +710,31 @@
         or group_messages
         or managed_policy_messages
         or scp_messages
     ):
         iam_template_map = await get_existing_template_map(
             repo_dir=repo_dir,
             template_type="AWS::IAM.*",
+            template_map=config.template_map,
             nested=True,
         )
 
     if permission_set_messages:
         identity_center_template_map = await get_existing_template_map(
             repo_dir=repo_dir,
             template_type="AWS::IdentityCenter.*",
+            template_map=config.template_map,
             nested=True,
         )
 
     if scp_messages:
         scp_template_map = await get_existing_template_map(
             repo_dir=repo_dir,
             template_type=AWS_SCP_POLICY_TEMPLATE,
+            template_map=config.template_map,
             nested=True,
         )
 
     if role_messages:
         collect_tasks.append(
             collect_aws_roles(exe_message, config, iam_template_map, role_messages)
         )
@@ -929,15 +935,20 @@
             "Applying templates to provision identities to the discovered account(s).",
         )
         templates = await gather_templates(repo_dir, "AWS.*")
         sub_message = exe_message.copy()
         sub_message.command = Command.APPLY
         sub_config = config.copy()
         sub_config.accounts = accounts_to_apply
-        await apply(exe_message, sub_config, load_templates(templates), remote_worker)
+        await apply(
+            exe_message,
+            sub_config,
+            load_templates(templates, config.template_map),
+            remote_worker,
+        )
 
     return run_import
 
 
 async def discover_aws_account_attribute_changes(
     config: AWSConfig,
     config_account_idx_map: dict[str, int],
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         if include_policies:
             current_role["ManagedPolicies"] = await get_role_managed_policies(
                 role_name, iam_client
             )
             current_role["InlinePolicies"] = await get_role_inline_policies(
                 role_name, iam_client, as_dict=False
             )
+
+        if not current_role.get("Tags"):
+            current_role["Tags"] = []
+
     except iam_client.exceptions.NoSuchEntityException:
         current_role = {}
 
     return current_role
 
 
 async def get_role_across_accounts(
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,48 @@
 
 import asyncio
 from typing import Optional
 
 from pydantic import BaseModel, Field, validator
 
 from iambic.core.iambic_plugin import ProviderPlugin
-from iambic.core.models import ExecutionMessage
+from iambic.core.models import ConfigMixin, ExecutionMessage
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.aws.handlers import (
     apply,
     aws_account_update_and_discovery,
     decode_aws_secret,
     detect_changes,
     import_aws_resources,
     load,
 )
-from iambic.plugins.v0_1_0.aws.iam.group.models import AwsIamGroupTemplate
-from iambic.plugins.v0_1_0.aws.iam.policy.models import AwsIamManagedPolicyTemplate
-from iambic.plugins.v0_1_0.aws.iam.role.models import AwsIamRoleTemplate
-from iambic.plugins.v0_1_0.aws.iam.user.models import AwsIamUserTemplate
-from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
-    AwsIdentityCenterPermissionSetTemplate,
-)
 from iambic.plugins.v0_1_0.aws.models import AWSAccount, AWSOrganization
-from iambic.plugins.v0_1_0.aws.organizations.scp.models import AwsScpPolicyTemplate
 
 
-class AWSConfig(BaseModel):
+def get_aws_templates():
+    from iambic.plugins.v0_1_0.aws.iam.group.models import AwsIamGroupTemplate
+    from iambic.plugins.v0_1_0.aws.iam.policy.models import AwsIamManagedPolicyTemplate
+    from iambic.plugins.v0_1_0.aws.iam.role.models import AwsIamRoleTemplate
+    from iambic.plugins.v0_1_0.aws.iam.user.models import AwsIamUserTemplate
+    from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
+        AwsIdentityCenterPermissionSetTemplate,
+    )
+    from iambic.plugins.v0_1_0.aws.organizations.scp.models import AwsScpPolicyTemplate
+
+    return [
+        AwsIdentityCenterPermissionSetTemplate,
+        AwsIamGroupTemplate,
+        AwsIamRoleTemplate,
+        AwsIamUserTemplate,
+        AwsIamManagedPolicyTemplate,
+        AwsScpPolicyTemplate,
+    ]
+
+
+class AWSConfig(ConfigMixin, BaseModel):
     organizations: list[AWSOrganization] = Field(
         [], description="A list of AWS Organizations to be managed by iambic"
     )
     accounts: list[AWSAccount] = Field(
         [], description="A list of AWS Accounts to be managed by iambic"
     )
     min_accounts_required_for_wildcard_included_accounts: int = Field(
@@ -79,14 +91,18 @@
         else:
             return [
                 account.hub_role_arn
                 for account in self.accounts
                 if account.hub_role_arn
             ][0]
 
+    @property
+    def templates(self):
+        return get_aws_templates()
+
     async def set_identity_center_details(self, account_id: str = None):
         if self.accounts:
             if account_id:
                 account = next(
                     account
                     for account in self.accounts
                     if account.account_id == account_id
@@ -141,16 +157,9 @@
     provider_config=AWSConfig,
     async_apply_callable=apply,
     async_import_callable=import_aws_resources,
     async_load_callable=load,
     async_decode_secret_callable=decode_aws_secret,
     async_detect_changes_callable=detect_changes,
     async_discover_upstream_config_changes_callable=aws_account_update_and_discovery,
-    templates=[
-        AwsIdentityCenterPermissionSetTemplate,
-        AwsIamGroupTemplate,
-        AwsIamRoleTemplate,
-        AwsIamUserTemplate,
-        AwsIamManagedPolicyTemplate,
-        AwsScpPolicyTemplate,
-    ],
+    templates=get_aws_templates(),
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,25 @@
         "Finished retrieving Azure AD groups.",
         azure_org=exe_message.provider_id,
         group_count=len(groups),
     )
 
 
 async def generate_group_templates(
-    exe_message: ExecutionMessage, output_dir: str, detect_messages: list = None
+    config: AzureADConfig,
+    exe_message: ExecutionMessage,
+    output_dir: str,
+    detect_messages: list = None,
 ):
     """Create the templates for all collected groups in the domain"""
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, AZURE_AD_GROUP_TEMPLATE_TYPE
+        base_path,
+        AZURE_AD_GROUP_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Azure AD group templates.")
 
     groups = await exe_message.get_sub_exe_files(
         *get_resource_dir_args(), "templates", file_name_and_extension="**.yaml"
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,11 +62,11 @@
                 log.warning(
                     "The remote worker definition must be defined in the config to run remote execution."
                 )
             await asyncio.gather(*collector_tasks)
 
     if base_runner:
         generator_tasks = [
-            generate_group_templates(exe_message, base_output_dir),
-            generate_user_templates(exe_message, base_output_dir),
+            generate_group_templates(config, exe_message, base_output_dir),
+            generate_user_templates(config, exe_message, base_output_dir),
         ]
         await asyncio.gather(*generator_tasks)
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from __future__ import annotations
 
 from pydantic import BaseModel, Field, validator
 
 from iambic.core.iambic_plugin import ProviderPlugin
+from iambic.core.models import ConfigMixin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
-from iambic.plugins.v0_1_0.azure_ad.group.models import (
-    AzureActiveDirectoryGroupTemplate,
-)
 from iambic.plugins.v0_1_0.azure_ad.handlers import import_azure_ad_resources, load
 from iambic.plugins.v0_1_0.azure_ad.models import AzureADOrganization
-from iambic.plugins.v0_1_0.azure_ad.user.models import AzureActiveDirectoryUserTemplate
 
 
-class AzureADConfig(BaseModel):
+def get_azure_ad_templates():
+    from iambic.plugins.v0_1_0.azure_ad.group.models import (
+        AzureActiveDirectoryGroupTemplate,
+    )
+    from iambic.plugins.v0_1_0.azure_ad.user.models import (
+        AzureActiveDirectoryUserTemplate,
+    )
+
+    return [AzureActiveDirectoryGroupTemplate, AzureActiveDirectoryUserTemplate]
+
+
+class AzureADConfig(ConfigMixin, BaseModel):
     organizations: list[AzureADOrganization] = Field(
         description="A list of Azure Active Directory organizations."
     )
 
     @validator(
         "organizations", allow_reuse=True
     )  # the need of allow_reuse is possibly related to how we handle inheritance
@@ -33,17 +41,21 @@
 
     def get_organization(self, idp_name: str) -> AzureADOrganization:
         for o in self.organizations:
             if o.idp_name == idp_name:
                 return o
         raise Exception(f"Could not find organization for IDP {idp_name}")
 
+    @property
+    def templates(self):
+        return get_azure_ad_templates()
+
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="azure_ad",
     version=PLUGIN_VERSION,
     provider_config=AzureADConfig,
     async_import_callable=import_azure_ad_resources,
     async_load_callable=load,
     requires_secret=True,
-    templates=[AzureActiveDirectoryGroupTemplate, AzureActiveDirectoryUserTemplate],
+    templates=get_azure_ad_templates(),
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,25 @@
         "Finished retrieving Azure AD users.",
         azure_org=exe_message.provider_id,
         user_count=len(users),
     )
 
 
 async def generate_user_templates(
-    exe_message: ExecutionMessage, output_dir: str, detect_messages: list = None
+    config: AzureADConfig,
+    exe_message: ExecutionMessage,
+    output_dir: str,
+    detect_messages: list = None,
 ):
     """Create the templates for all collected users in the domain"""
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, AZURE_AD_USER_TEMPLATE_TYPE
+        base_path,
+        AZURE_AD_USER_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Azure AD user templates.")
 
     users = await exe_message.get_sub_exe_files(
         *get_resource_dir_args(), "templates", file_name_and_extension="**.yaml"
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from __future__ import annotations
 
 from pydantic import BaseModel
 
 from iambic.core.iambic_plugin import ProviderPlugin
+from iambic.core.models import ConfigMixin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.example.handlers import import_example_resources, load
-from iambic.plugins.v0_1_0.example.local_database.models import (
-    ExampleLocalDatabaseTemplate,
-)
-from iambic.plugins.v0_1_0.example.local_file.models import (
-    ExampleLocalFileMultiAccountTemplate,
-    ExampleLocalFileTemplate,
-)
 
 
-class ExampleConfig(BaseModel):
-    pass
+def get_example_templates():
+    from iambic.plugins.v0_1_0.example.local_database.models import (
+        ExampleLocalDatabaseTemplate,
+    )
+    from iambic.plugins.v0_1_0.example.local_file.models import (
+        ExampleLocalFileMultiAccountTemplate,
+        ExampleLocalFileTemplate,
+    )
+
+    return [
+        ExampleLocalFileTemplate,
+        ExampleLocalFileMultiAccountTemplate,
+        ExampleLocalDatabaseTemplate,
+    ]
+
+
+class ExampleConfig(ConfigMixin, BaseModel):
+    @property
+    def templates(self):
+        return get_example_templates()
 
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="example",
     version=PLUGIN_VERSION,
     provider_config=ExampleConfig,
     requires_secret=True,
     async_import_callable=import_example_resources,
     async_load_callable=load,
-    templates=[
-        ExampleLocalFileTemplate,
-        ExampleLocalFileMultiAccountTemplate,
-        ExampleLocalDatabaseTemplate,
-    ],
+    templates=get_example_templates(),
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 import traceback
 import uuid
 from enum import Enum
 from typing import Any, Callable
 from urllib.parse import urlparse
 
 import github
+from cryptography.hazmat.primitives import serialization
 from github.PullRequest import PullRequest
 
 import iambic.output.markdown
 from iambic.config.dynamic_config import load_config
 from iambic.config.utils import resolve_config_template_path
 from iambic.core.context import ctx
 from iambic.core.git import Repo, clone_git_repo, get_remote_default_branch
 from iambic.core.iambic_enum import Command
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage, TemplateChangeDetails
-from iambic.core.utils import yaml
+from iambic.core.utils import decode_with_reference_time, yaml
 from iambic.main import run_apply, run_detect, run_expire, run_git_apply, run_git_plan
+from iambic.plugins.v0_1_0.github.iambic_plugin import GithubConfig
 
 iambic_app = __import__("iambic.lambda.app", globals(), locals(), [], 0)
 lambda_run_handler = getattr(iambic_app, "lambda").app.run_handler
 
 
 MERGEABLE_STATE_CLEAN = "clean"
 MERGEABLE_STATE_BLOCKED = "blocked"
@@ -68,14 +70,15 @@
 
 class HandleIssueCommentReturnCode(Enum):
     UNDEFINED = 1
     NO_MATCHING_BODY = 2
     MERGEABLE_STATE_NOT_CLEAN = 3
     MERGED = 4
     PLANNED = 5
+    APPROVED = 6
 
 
 # context is a dictionary structure published by Github Action
 # https://docs.github.com/en/actions/learn-github-actions/contexts#github-context
 def run_handler(context: dict[str, Any]):
     github_token: str = context["token"]
     event_name: str = context["event_name"]
@@ -289,17 +292,21 @@
     return session_name
 
 
 def handle_issue_comment(
     github_client: github.Github, context: dict[str, Any]
 ) -> HandleIssueCommentReturnCode:
     comment_body = context["event"]["comment"]["body"]
+    comment_user_login = context["event"]["comment"]["user"]["login"]
     log_params = {"COMMENT_DISPATCH_MAP_KEYS": COMMENT_DISPATCH_MAP.keys()}
     log.info("COMMENT_DISPATCH_MAP keys", **log_params)
-    if comment_body not in COMMENT_DISPATCH_MAP:
+
+    command_lookup = comment_body.split("\n")[0]
+
+    if command_lookup not in COMMENT_DISPATCH_MAP:
         log_params = {"comment_body": comment_body}
         log.error("handle_issue_comment: no op", **log_params)
         return HandleIssueCommentReturnCode.NO_MATCHING_BODY
 
     github_token = context["token"]
     # repo_name is already in the format {repo_owner}/{repo_short_name}
     repo_name = context["repository"]
@@ -309,37 +316,41 @@
     # repository_url_token
     templates_repo = github_client.get_repo(repo_name)
     pull_request = templates_repo.get_pull(pull_number)
     pull_request_branch_name = pull_request.head.ref
     log_params = {"pull_request_branch_name": pull_request_branch_name}
     log.info("PR remote branch name", **log_params)
 
-    comment_func: Callable = COMMENT_DISPATCH_MAP[comment_body]
+    comment_func: Callable = COMMENT_DISPATCH_MAP[command_lookup]
     return comment_func(
         context,
         github_client,
         templates_repo,
         pull_request,
         repo_name,
         pull_number,
         pull_request_branch_name,
         repo_url,
+        comment_user_login=comment_user_login,
+        comment=comment_body,
     )
 
 
 def handle_iambic_git_apply(
     context: dict[str, Any],
     github_client: github.Github,
     templates_repo: github.Repo,
     pull_request: PullRequest,
     repo_name: str,
     pull_number: str,
     pull_request_branch_name: str,
     repo_url: str,
     proposed_changes_path: str = None,
+    comment_user_login: str = None,
+    comment: str = None,
 ):
     if pull_request.mergeable_state != MERGEABLE_STATE_CLEAN:
         # TODO log error and also make a comment to PR
         pull_request.create_issue_comment(
             "Mergable state is {0}. This probably means that the necessary approvals have not been granted for the request.".format(
                 pull_request.mergeable_state
             )
@@ -484,14 +495,16 @@
     templates_repo: github.Repo,
     pull_request: PullRequest,
     repo_name: str,
     pull_number: str,
     pull_request_branch_name: str,
     repo_url: str,
     proposed_changes_path: str = None,
+    comment_user_login: str = None,
+    comment: str = None,
 ):
     session_name = get_session_name(repo_name, pull_number)
     os.environ["IAMBIC_SESSION_NAME"] = session_name
 
     try:
         repo_dir = get_lambda_repo_path()
         prepare_local_repo(repo_url, repo_dir, pull_request_branch_name)
@@ -523,14 +536,90 @@
             "exception during plan is {0} \n ```{1}```".format(
                 pull_request.mergeable_state, captured_traceback
             )
         )
         raise e
 
 
+def handle_iambic_approve(
+    context: dict[str, Any],
+    github_client: github.Github,
+    templates_repo: github.Repo,
+    pull_request: PullRequest,
+    repo_name: str,
+    pull_number: str,
+    pull_request_branch_name: str,
+    repo_url: str,
+    proposed_changes_path: str = None,
+    comment_user_login: str = None,
+    comment: str = None,
+):
+    session_name = get_session_name(repo_name, pull_number)
+    os.environ["IAMBIC_SESSION_NAME"] = session_name
+
+    try:
+        repo_dir = get_lambda_repo_path()
+        _ = prepare_local_repo_for_new_commits(repo_url, repo_dir, "detect")
+        config_path = asyncio.run(resolve_config_template_path(repo_dir))
+        # it's important to load the config from main branch
+        # we want to guard against a requester directly changing the approver
+        # knowledge in the config of the iambic-template repository
+        main_config = asyncio.run(load_config(config_path))
+        github_main_config: GithubConfig = main_config.github
+        allowed_bot_approvers = github_main_config.allowed_bot_approvers
+        matching_approvers = [
+            approver
+            for approver in allowed_bot_approvers
+            if approver.login == comment_user_login
+        ]
+
+        if len(matching_approvers) != 1:
+            pull_request.create_issue_comment(
+                f"`{comment_user_login}` is not configured to approve PR via iambic"
+            )
+            return HandleIssueCommentReturnCode.UNDEFINED
+
+        allowed_bot_approver = matching_approvers[0]
+        allowed_bot_approver_pub_key_string = allowed_bot_approver.es256_pub_key
+        loaded_public_key = serialization.load_pem_public_key(
+            allowed_bot_approver_pub_key_string.encode("utf-8")
+        )
+        encoded_jwt = comment.split("\n")[-1]
+        encoded_jwt = encoded_jwt.replace("<!--", "", 1).replace("-->", "", 1)
+        decoded = decode_with_reference_time(
+            encoded_jwt, loaded_public_key, "ES256", datetime.datetime.now()
+        )
+
+        if not (
+            decoded["repo"] == repo_name
+            and decoded["pr"] == pull_number
+            and len(decoded["signee"]) > 0
+        ):
+            raise Exception(f"Claim does not match the pull-request: {decoded}")
+
+        pull_request.create_review(
+            event="APPROVE",
+            body=f"""react to `approve` from `{comment_user_login}` with payload:
+```json
+{json.dumps(decoded)}
+```""",
+        )
+        return HandleIssueCommentReturnCode.APPROVED
+
+    except (Exception, SystemExit) as e:
+        captured_traceback = traceback.format_exc()
+        log.error("fault", exception=captured_traceback)
+        pull_request.create_issue_comment(
+            "exception during plan is {0} \n ```{1}```".format(
+                pull_request.mergeable_state, captured_traceback
+            )
+        )
+        raise e
+
+
 def github_app_workflow_wrapper(workflow_func: Callable, ux_op_name: str) -> Callable:
     def wrapped_workflow_func(
         github_client: github.Github,
         templates_repo: github.Repo,
         repo_name: str,
         repo_url: str,
         default_branch: str,
@@ -812,14 +901,15 @@
 
 
 COMMENT_DISPATCH_MAP: dict[str, Callable] = {
     "iambic git-apply": handle_iambic_git_apply,
     "iambic git-plan": handle_iambic_git_plan,
     "iambic apply": handle_iambic_git_apply,
     "iambic plan": handle_iambic_git_plan,
+    "iambic approve": handle_iambic_approve,
 }
 
 if __name__ == "__main__":
     github_context_json_str = os.environ.get("GITHUB_CONTEXT")
     github_override_token = os.environ.get("GH_OVERRIDE_TOKEN")
     iambic_integration_str = os.environ.get("IAMBIC_CLOUD_IMPORT_CMD")
     iambic_commit_email = os.environ.get("IAMBIC_COMMIT_EMAIL")
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from iambic.plugins.v0_1_0.github.github import (
     HandleIssueCommentReturnCode,
     _handle_detect_changes_from_eventbridge,
     _handle_enforce,
     _handle_expire,
     _handle_import,
     github_app_workflow_wrapper,
+    handle_iambic_approve,
     handle_iambic_git_apply,
     handle_iambic_git_plan,
     iambic_app,
 )
 
 # FIXME Lambda execution time is at most 15 minutes, and the Github installation token is at most
 # 10 min validation period.
@@ -220,24 +221,31 @@
     if action != "created":
         return
 
     comment_body = webhook_payload["comment"]["body"]
     comment_user_login = webhook_payload["comment"]["user"]["login"]
     log_params = {"COMMENT_DISPATCH_MAP_KEYS": COMMENT_DISPATCH_MAP.keys()}
     log.info("COMMENT_DISPATCH_MAP keys", **log_params)
-    if comment_body not in COMMENT_DISPATCH_MAP:
-        log_params = {"comment_body": comment_body}
+
+    command_lookup = comment_body.split("\n")[0].strip()
+
+    if command_lookup not in COMMENT_DISPATCH_MAP:
+        log_params = {
+            "command_lookup": command_lookup,
+            "comment_body": comment_body,
+        }
         log.error("handle_issue_comment: no op", **log_params)
         return HandleIssueCommentReturnCode.NO_MATCHING_BODY
 
-    # FIXME: Need to find a mechanism to avoid infinite loop
-    # the following is a very crude one
     if comment_user_login.endswith("[bot]"):
-        # return early
-        return HandleIssueCommentReturnCode.UNDEFINED
+        if command_lookup != "iambic approve":
+            # return early unless it's the approve attempt
+            # the approve handler require to walk the full config
+            # to determine.
+            return HandleIssueCommentReturnCode.UNDEFINED
 
     repo_name = webhook_payload["repository"]["full_name"]
     pull_number = webhook_payload["issue"]["number"]
     # repository_url_token
     templates_repo = github_client.get_repo(repo_name)
     pull_request = templates_repo.get_pull(pull_number)
 
@@ -247,25 +255,27 @@
     # repository_url_token
     templates_repo = github_client.get_repo(repo_name)
     pull_request = templates_repo.get_pull(pull_number)
     pull_request_branch_name = pull_request.head.ref
     log_params = {"pull_request_branch_name": pull_request_branch_name}
     log.info("PR remote branch name", **log_params)
 
-    comment_func: Callable = COMMENT_DISPATCH_MAP[comment_body]
+    comment_func: Callable = COMMENT_DISPATCH_MAP[command_lookup]
     return comment_func(
         None,
         github_client,
         templates_repo,
         pull_request,
         repo_name,
         pull_number,
         pull_request_branch_name,
         repo_url,
         proposed_changes_path=getattr(iambic_app, "lambda").app.PLAN_OUTPUT_PATH,
+        comment_user_login=comment_user_login,
+        comment=comment_body,
     )
 
 
 def handle_workflow_run(
     github_token: str, github_client: github.Github, webhook_payload: dict[str, Any]
 ) -> None:
     action = webhook_payload["action"]
@@ -305,14 +315,15 @@
 
 
 COMMENT_DISPATCH_MAP: dict[str, Callable] = {
     "iambic git-apply": handle_iambic_git_apply,
     "iambic git-plan": handle_iambic_git_plan,
     "iambic apply": handle_iambic_git_apply,
     "iambic plan": handle_iambic_git_plan,
+    "iambic approve": handle_iambic_approve,
 }
 
 WORKFLOW_DISPATCH_MAP: dict[str, Callable] = {
     ".github/workflows/iambic-enforce.yml": github_app_workflow_wrapper(
         _handle_enforce, "enforce"
     ),
     ".github/workflows/iambic-expire.yml": github_app_workflow_wrapper(
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 from __future__ import annotations
 
+from typing import Optional
+
 from pydantic import BaseModel, Field
 
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.github.handlers import import_github_resources, load
 
+DEFAULT_ALLOWED_BOT_APPROVER = None
+
+
+class GithubBotApprover(BaseModel):
+    login: str = Field(
+        ...,
+        description="login for allowed bot approver",
+    )
+    es256_pub_key: str = Field(
+        ...,
+        description="ES256 Pub Key for allowed bot approver",
+    )
+
 
 class GithubConfig(BaseModel):
     commit_message_user_name: str = Field(
         default="Iambic Automation", description="Commit message user name"
     )
     commit_message_user_email: str = Field(
         default="iambic-automation@iambic.org", description="Commit message user email"
@@ -26,14 +41,18 @@
         default="Periodic Expiration",
         description="Commit message to use during changes through expire operations",
     )
     commit_message_for_git_apply: str = Field(
         default="Replace relative time with absolute time",
         description="Commit message to use during changes through git-apply",
     )
+    allowed_bot_approvers: Optional[list[GithubBotApprover]] = Field(
+        default=[],
+        description="list of allowed bot approver",
+    )
 
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="github",
     version=PLUGIN_VERSION,
     provider_config=GithubConfig,
     requires_secret=False,
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,17 @@
     detect_messages: list = None,
 ):
     """List all groups in the domain, along with members and
     settings"""
 
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, GOOGLE_GROUP_TEMPLATE_TYPE
+        base_path,
+        GOOGLE_GROUP_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Google group templates.")
 
     for workspace in config.workspaces:
         for subject in workspace.subjects:
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 import os
 import typing
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import googleapiclient.discovery
 from google.oauth2 import service_account
 from pydantic import BaseModel, Field, SecretStr, validator
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
-from iambic.core.models import Variable
+from iambic.core.models import ConfigMixin, Variable
 from iambic.core.utils import aio_wrapper
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
-from iambic.plugins.v0_1_0.google_workspace.group.models import (
-    GoogleWorkspaceGroupTemplate,
-)
 from iambic.plugins.v0_1_0.google_workspace.handlers import (
     import_google_resources,
     load,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
-    MappingIntStrAny = typing.Mapping[int | str, Any]
-    AbstractSetIntStr = typing.AbstractSet[int | str]
+    MappingIntStrAny = typing.Mapping[Union[int, str], Any]
+    AbstractSetIntStr = typing.AbstractSet[Union[int, str]]
 
 
 class GoogleSubject(BaseModel):
     domain: str
     service_account: str
 
 
@@ -118,15 +115,25 @@
             credentials=admin_delegated_credentials,
             cache_discovery=cache_discovery,
             thread_sensitive=True,
         )
         return self._service_connection_map[key]
 
 
-class GoogleWorkspaceConfig(BaseModel):
+def get_google_templates():
+    from iambic.plugins.v0_1_0.google_workspace.group.models import (
+        GoogleWorkspaceGroupTemplate,
+    )
+
+    return [
+        GoogleWorkspaceGroupTemplate,
+    ]
+
+
+class GoogleWorkspaceConfig(ConfigMixin, BaseModel):
     workspaces: list[GoogleProject]
 
     @validator(
         "workspaces", allow_reuse=True
     )  # the need of allow_reuse is possibly related to how we handle inheritance
     def validate_google_workspaces(cls, workspaces: list[GoogleProject]):
         project_id_set = set()
@@ -141,19 +148,21 @@
 
     def get_workspace(self, project_id: str) -> GoogleProject:
         for w in self.workspaces:
             if w.project_id == project_id:
                 return w
         raise Exception(f"Could not find workspace for project_id {project_id}")
 
+    @property
+    def templates(self):
+        return get_google_templates()
+
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="google_workspace",
     version=PLUGIN_VERSION,
     provider_config=GoogleWorkspaceConfig,
     requires_secret=True,
     async_import_callable=import_google_resources,
     async_load_callable=load,
-    templates=[
-        GoogleWorkspaceGroupTemplate,
-    ],
+    templates=get_google_templates(),
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import copy
 import os
 import tempfile
 import unittest
-
-from mock import AsyncMock, MagicMock
+from unittest.mock import AsyncMock, MagicMock
 
 from iambic.core.context import ctx
 from iambic.core.models import ProposedChangeType, TemplateChangeDetails
 from iambic.plugins.v0_1_0.google_workspace.iambic_plugin import (
     GoogleProject,
     GoogleWorkspaceConfig,
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import unittest.mock
+from unittest.mock import AsyncMock
 
 import pytest
-from mock import AsyncMock
 from pydantic import SecretStr
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.models import Command, ExecutionMessage
 from iambic.plugins.v0_1_0.google_workspace.handlers import import_google_resources
 from iambic.plugins.v0_1_0.google_workspace.iambic_plugin import (
     GoogleProject,
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+from unittest.mock import MagicMock, patch
+
 import pytest
 from googleapiclient.errors import UnknownApiNameOrVersion
-from mock import MagicMock, patch
 
 from iambic.plugins.v0_1_0.google_workspace.iambic_plugin import (
     GoogleProject,
     GoogleSubject,
     SecretStr,
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,20 +59,25 @@
         "Finished retrieving Okta apps.",
         okta_org=exe_message.provider_id,
         app_count=len(apps),
     )
 
 
 async def generate_app_templates(
-    exe_message: ExecutionMessage, output_dir: str, detect_messages: list = None
+    config: OktaConfig,
+    exe_message: ExecutionMessage,
+    output_dir: str,
+    detect_messages: list = None,
 ):
     """List all apps in the domain, along with members and settings"""
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, OKTA_APP_TEMPLATE_TYPE
+        base_path,
+        OKTA_APP_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Okta app templates.")
 
     apps = await exe_message.get_sub_exe_files(
         *get_resource_dir_args(), "templates", file_name_and_extension="**.yaml"
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,25 @@
         "Finished retrieving Okta groups.",
         okta_org=exe_message.provider_id,
         group_count=len(groups),
     )
 
 
 async def generate_group_templates(
-    exe_message: ExecutionMessage, output_dir: str, detect_messages: list = None
+    config: OktaConfig,
+    exe_message: ExecutionMessage,
+    output_dir: str,
+    detect_messages: list = None,
 ):
     """List all groups in the domain, along with members and settings"""
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, OKTA_GROUP_TEMPLATE_TYPE
+        base_path,
+        OKTA_GROUP_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Okta group templates.")
 
     groups = await exe_message.get_sub_exe_files(
         *get_resource_dir_args(), "templates", file_name_and_extension="**.yaml"
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,12 +67,12 @@
                 log.warning(
                     "The remote worker definition must be defined in the config to run remote execution."
                 )
             await asyncio.gather(*collector_tasks)
 
     if base_runner:
         generator_tasks = [
-            generate_app_templates(exe_message, base_output_dir),
-            generate_group_templates(exe_message, base_output_dir),
-            generate_user_templates(exe_message, base_output_dir),
+            generate_app_templates(config, exe_message, base_output_dir),
+            generate_group_templates(config, exe_message, base_output_dir),
+            generate_user_templates(config, exe_message, base_output_dir),
         ]
         await asyncio.gather(*generator_tasks)
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,29 @@
 from typing import Any, Optional
 
 from okta.client import Client as OktaClient
 from pydantic import BaseModel, Extra, Field, SecretStr, validator
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
+from iambic.core.models import ConfigMixin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
-from iambic.plugins.v0_1_0.okta.app.models import OktaAppTemplate
-from iambic.plugins.v0_1_0.okta.group.models import OktaGroupTemplate
 from iambic.plugins.v0_1_0.okta.handlers import import_okta_resources, load
-from iambic.plugins.v0_1_0.okta.user.models import OktaUserTemplate
+
+
+def get_okta_templates():
+    from iambic.plugins.v0_1_0.okta.app.models import OktaAppTemplate
+    from iambic.plugins.v0_1_0.okta.group.models import OktaGroupTemplate
+    from iambic.plugins.v0_1_0.okta.user.models import OktaUserTemplate
+
+    return [
+        OktaAppTemplate,
+        OktaGroupTemplate,
+        OktaUserTemplate,
+    ]
 
 
 class OktaOrganization(BaseModel):
     idp_name: str
     org_url: str
     api_token: SecretStr
     request_timeout: int = 60
@@ -38,15 +48,15 @@
                     "requestTimeout": self.request_timeout,
                     "rateLimit": {"maxRetries": 0},
                 }
             )
         return self.client
 
 
-class OktaConfig(BaseModel):
+class OktaConfig(ConfigMixin, BaseModel):
     organizations: list[OktaOrganization] = Field(
         description="A list of Okta organizations."
     )
 
     @validator(
         "organizations", allow_reuse=True
     )  # the need of allow_reuse is possibly related to how we handle inheritance
@@ -63,21 +73,21 @@
 
     def get_organization(self, idp_name: str) -> OktaOrganization:
         for o in self.organizations:
             if o.idp_name == idp_name:
                 return o
         raise Exception(f"Could not find organization for IDP {idp_name}")
 
+    @property
+    def templates(self):
+        return get_okta_templates()
+
 
 IAMBIC_PLUGIN = ProviderPlugin(
     config_name="okta",
     version=PLUGIN_VERSION,
     provider_config=OktaConfig,
     requires_secret=True,
     async_import_callable=import_okta_resources,
     async_load_callable=load,
-    templates=[
-        OktaAppTemplate,
-        OktaGroupTemplate,
-        OktaUserTemplate,
-    ],
+    templates=get_okta_templates(),
 )
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,25 @@
         "Finished retrieving Okta users.",
         okta_org=exe_message.provider_id,
         user_count=len(users),
     )
 
 
 async def generate_user_templates(
-    exe_message: ExecutionMessage, output_dir: str, detect_messages: list = None
+    config: OktaConfig,
+    exe_message: ExecutionMessage,
+    output_dir: str,
+    detect_messages: list = None,
 ):
     """List all users in the domain, along with members and settings"""
     base_path = os.path.expanduser(output_dir)
     existing_template_map = await get_existing_template_map(
-        base_path, OKTA_USER_TEMPLATE_TYPE
+        base_path,
+        OKTA_USER_TEMPLATE_TYPE,
+        config.template_map,
     )
     all_resource_ids = set()
 
     log.info("Updating and creating Okta user templates.")
 
     users = await exe_message.get_sub_exe_files(
         *get_resource_dir_args(), "templates", file_name_and_extension="**.yaml"
```

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.9.1/iambic/request_handler/expire_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
 import asyncio
+from typing import Type
 
 from iambic.core.logger import log
+from iambic.core.models import BaseTemplate
 from iambic.core.parser import load_templates
 from iambic.core.utils import remove_expired_resources
 
 
-async def flag_expired_resources(template_paths: list[str]):
+async def flag_expired_resources(
+    template_paths: list[str],
+    template_map: dict[str, Type[BaseTemplate]],
+):
     # Warning: The dynamic config must be loaded before this is called.
     #   This is done using iambic.config.dynamic_config.load_config(config_path)
     log.info("Scanning for expired resources")
     templates = await asyncio.gather(
         *[
             remove_expired_resources(
                 template, template.resource_type, template.resource_id
             )
-            for template in load_templates(template_paths)
+            for template in load_templates(template_paths, template_map)
         ]
     )
 
     for template in templates:
         template.write(exclude_none=True, exclude_unset=True, exclude_defaults=True)
 
     log.info("Expired resource scan complete.")
```

### Comparing `iambic_core-0.8.1/iambic/request_handler/git_apply.py` & `iambic_core-0.9.1/iambic/request_handler/git_apply.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,57 +41,66 @@
     :param from_sha:
     :param to_sha:
     :return:
     """
 
     config = await load_config(config_path)
     file_changes = await retrieve_git_changes(
-        repo_dir, allow_dirty=allow_dirty, from_sha=from_sha, to_sha=to_sha
+        repo_dir,
+        config.template_map,
+        allow_dirty=allow_dirty,
+        from_sha=from_sha,
+        to_sha=to_sha,
     )
     if (
         not file_changes["new_files"]
         and not file_changes["modified_files"]
         and not file_changes["deleted_files"]
     ):
         log.info("No changes found.")
         return []
 
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.APPLY
     )
     new_templates = load_templates(
-        [git_diff.path for git_diff in file_changes["new_files"]]
+        [git_diff.path for git_diff in file_changes["new_files"]],
+        config.template_map,
     )
 
     deleted_templates = create_templates_for_deleted_files(
-        file_changes["deleted_files"]
+        file_changes["deleted_files"],
+        config.template_map,
     )
 
     modified_templates_doubles = create_templates_for_modified_files(
-        config, file_changes["modified_files"]
+        config,
+        file_changes["modified_files"],
     )
 
     # You can only flag expired resources on new/modified-templates
     await flag_expired_resources(
         [
             template.file_path
             for template in itertools.chain(new_templates, modified_templates_doubles)
             if os.path.exists(template.file_path)
-        ]
+        ],
+        config.template_map,
     )
 
     template_changes = await config.run_apply(
         exe_message,
         itertools.chain(new_templates, deleted_templates, modified_templates_doubles),
     )
 
     # note modified_templates_exist_in_repo has different entries from create_templates_for_modified_files because
     # create_templates_for_modified_files actually has two template instance per a single modified file
     modified_templates_exist_in_repo = load_templates(
-        [git_diff.path for git_diff in file_changes["modified_files"]]
+        [git_diff.path for git_diff in file_changes["modified_files"]],
+        config.template_map,
     )
     commit_deleted_templates(
         repo_dir, modified_templates_exist_in_repo, template_changes
     )
 
     return template_changes
```

### Comparing `iambic_core-0.8.1/iambic/request_handler/git_plan.py` & `iambic_core-0.9.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.8.1/pyproject.toml` & `iambic_core-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.8.1"
+version = "0.9.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
 
@@ -32,58 +32,56 @@
 click = "^8.1.3"
 "ruamel.yaml" = "^0.17.21"
 asgiref = "^3.6.0"
 structlog = "^22.3.0"
 pydantic = "^1.10.6"
 deepdiff = "^6.3.0"
 Jinja2 = "^3.1.2"
-black = "^23.1.0"
-isort = "^5.12.0"
-flake8 = "^6.0.0"
-pytest = "^7.2.2"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.2.1"
-pytest-rerunfailures = "^11.1.2"
-pre-commit = "^3.2.0"
 ujson = "^5.7.0"
 aiofiles = "^23.1.0"
 xxhash = "^3.2.0"
 slack-bolt = "^1.16.4"
 google-api-python-client = "^2.81.0"
 google-auth = "^2.16.2"
-jsonschema2md2 = "^0.6.0"
 GitPython = "^3.1.31"
 PyGithub = "==1.57" # Since 1.58, PyGithub does not work with Lambda. See https://github.com/PyGithub/PyGithub/issues/2430
 pydantic-factories = "^1.17.2"
 okta = "^2.9.2"
 asyncache = "^0.3.1"
 dateparser = "^1.1.7"
-pytest-mock = "^3.10.0"
 questionary = "^1.10.0"
 types-dateparser = "^1.1.4.5"
-cryptography = "^39.0.1"
+cryptography = "^41.0.1"
 aws-error-utils = "^2.7.0"
-types-mock = "^5.0.0.5"
 rich = "^13.3.2"
 dictdiffer = "^0.9.0"
 msal = "^1.21.0"
 aiohttp = "^3.8.4"
 pyopenssl = "^23.0.0"
 stringcase = "^1.2.0"
 tomlkit = "^0.11.8"
 typing-extensions = "^4.6.1"
 tenacity = "^8.2.2"
 
 [tool.poetry.scripts]
 iambic = "iambic.main:cli"
 
 [tool.poetry.group.dev.dependencies]
+black = "^23.1.0"
+flake8 = "^6.0.0"
+isort = "^5.12.0"
+jsonschema2md2 = "^0.6.0"
+pre-commit = "^3.2.0"
+pycryptodome = "^3.17"
+pytest = "^7.2.2"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.0.0"
+pytest-mock = "^3.10.0"
+pytest-xdist = "^3.2.1"
+pytest-rerunfailures = "^11.1.2"
+types-mock = "^5.0.0.5"
 types-cachetools = "^5.3.0.4"
 types-pyyaml = "^6.0.12.8"
 types-aiofiles = "^23.1.0.0"
 types-ujson = "^5.7.0.1"
-mock = "^5.0.1"
-pytest-mock-generator = "^1.2.0"
-pycryptodome = "^3.17"
 moto = {extras = ["all"], version = "^4.1.5"}
 dateparser = "^1.1.7"
```

### Comparing `iambic_core-0.8.1/PKG-INFO` & `iambic_core-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.8.1
+Version: 0.9.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,48 +15,36 @@
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyGithub (==1.57)
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asgiref (>=3.6.0,<4.0.0)
 Requires-Dist: asyncache (>=0.3.1,<0.4.0)
 Requires-Dist: aws-error-utils (>=2.7.0,<3.0.0)
-Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: boto3 (>=1.26.95,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cryptography (>=39.0.1,<40.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: dateparser (>=1.1.7,<2.0.0)
 Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
-Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: google-api-python-client (>=2.81.0,<3.0.0)
 Requires-Dist: google-auth (>=2.16.2,<3.0.0)
-Requires-Dist: isort (>=5.12.0,<6.0.0)
-Requires-Dist: jsonschema2md2 (>=0.6.0,<0.7.0)
 Requires-Dist: msal (>=1.21.0,<2.0.0)
 Requires-Dist: okta (>=2.9.2,<3.0.0)
-Requires-Dist: pre-commit (>=3.2.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pydantic-factories (>=1.17.2,<2.0.0)
 Requires-Dist: pyopenssl (>=23.0.0,<24.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
-Requires-Dist: pytest-rerunfailures (>=11.1.2,<12.0.0)
-Requires-Dist: pytest-xdist (>=3.2.1,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: slack-bolt (>=1.16.4,<2.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: types-dateparser (>=1.1.4.5,<2.0.0.0)
-Requires-Dist: types-mock (>=5.0.0.5,<6.0.0.0)
 Requires-Dist: typing-extensions (>=4.6.1,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 [![noqdev - iambic](https://img.shields.io/static/v1?label=noqdev&message=iambic&color=blue&logo=github)](https://github.com/noqdev/iambic "Go to GitHub repo")
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
```

