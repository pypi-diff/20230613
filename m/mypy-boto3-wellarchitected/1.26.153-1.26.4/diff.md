# Comparing `tmp/mypy-boto3-wellarchitected-1.26.153.tar.gz` & `tmp/mypy-boto3-wellarchitected-1.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.26.153.tar", last modified: Tue Jun 13 19:33:37 2023, max compression
+gzip compressed data, was "mypy-boto3-wellarchitected-1.26.4.tar", last modified: Mon Nov  7 20:50:37 2022, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.26.153.tar` & `mypy-boto3-wellarchitected-1.26.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:37.756408 mypy-boto3-wellarchitected-1.26.153/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-06-13 19:33:37.752407 mypy-boto3-wellarchitected-1.26.153/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:37.752407 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38027 2023-06-13 19:33:23.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37965 2023-06-13 19:33:23.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-13 19:33:24.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-06-13 19:33:23.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53029 2023-06-13 19:33:25.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52972 2023-06-13 19:33:24.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:33:37.752407 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 19:33:37.000000 mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:33:37.756408 mypy-boto3-wellarchitected-1.26.153/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-13 19:33:22.000000 mypy-boto3-wellarchitected-1.26.153/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15035 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.072346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29412 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29364 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9627 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    39740 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39695 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/LICENSE` & `mypy-boto3-wellarchitected-1.26.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/PKG-INFO` & `mypy-boto3-wellarchitected-1.26.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.153
-Summary: Type annotations for boto3.WellArchitected 1.26.153 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.4
+Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,30 +283,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileNotificationTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    QuestionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -331,199 +322,161 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    AssociateProfilesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    ProfileQuestionUpdateTypeDef,
-    CreateProfileShareInputRequestTypeDef,
     WorkloadDiscoveryConfigTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
-    DeleteProfileInputRequestTypeDef,
-    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
-    DisassociateProfilesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
-    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    WorkloadProfileTypeDef,
+    LensReviewSummaryTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
-    ListProfileNotificationsInputRequestTypeDef,
-    ProfileNotificationSummaryTypeDef,
-    ListProfileSharesInputRequestTypeDef,
-    ProfileShareSummaryTypeDef,
-    ListProfilesInputRequestTypeDef,
-    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
+    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
-    ProfileChoiceTypeDef,
-    ProfileTemplateChoiceTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
-    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
-    CreateProfileOutputTypeDef,
-    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     ImportLensOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    CreateProfileInputRequestTypeDef,
-    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
+    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    LensReviewSummaryTypeDef,
-    WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
+    ListLensReviewsOutputTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
-    ListProfileNotificationsOutputTypeDef,
-    ListProfileSharesOutputTypeDef,
-    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
-    ProfileQuestionTypeDef,
-    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
+    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
-    ProfileTypeDef,
-    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
-    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
-    GetProfileOutputTypeDef,
-    UpdateProfileOutputTypeDef,
-    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/README.md` & `mypy-boto3-wellarchitected-1.26.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,30 +252,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileNotificationTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    QuestionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -299,199 +291,161 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    AssociateProfilesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    ProfileQuestionUpdateTypeDef,
-    CreateProfileShareInputRequestTypeDef,
     WorkloadDiscoveryConfigTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
-    DeleteProfileInputRequestTypeDef,
-    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
-    DisassociateProfilesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
-    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    WorkloadProfileTypeDef,
+    LensReviewSummaryTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
-    ListProfileNotificationsInputRequestTypeDef,
-    ProfileNotificationSummaryTypeDef,
-    ListProfileSharesInputRequestTypeDef,
-    ProfileShareSummaryTypeDef,
-    ListProfilesInputRequestTypeDef,
-    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
+    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
-    ProfileChoiceTypeDef,
-    ProfileTemplateChoiceTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
-    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
-    CreateProfileOutputTypeDef,
-    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     ImportLensOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    CreateProfileInputRequestTypeDef,
-    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
+    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    LensReviewSummaryTypeDef,
-    WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
+    ListLensReviewsOutputTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
-    ListProfileNotificationsOutputTypeDef,
-    ListProfileSharesOutputTypeDef,
-    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
-    ProfileQuestionTypeDef,
-    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
+    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
-    ProfileTypeDef,
-    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
-    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
-    GetProfileOutputTypeDef,
-    UpdateProfileOutputTypeDef,
-    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/__main__.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WellArchitected 1.26.153\nVersion:         1.26.153\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.WellArchitected 1.26.4\nVersion:         1.26.4\nBuilder"
+        " version: 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.153")
+    print("1.26.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/client.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,70 +15,56 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
-    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
-    CreateProfileOutputTypeDef,
-    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
-    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
-    GetProfileOutputTypeDef,
-    GetProfileTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
     ListMilestonesOutputTypeDef,
     ListNotificationsOutputTypeDef,
-    ListProfileNotificationsOutputTypeDef,
-    ListProfileSharesOutputTypeDef,
-    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
-    ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
-    UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
@@ -126,24 +112,14 @@
         """
         Associate a lens to a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_lenses)
         """
 
-    def associate_profiles(
-        self, *, WorkloadId: str, ProfileArns: Sequence[str]
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Associate a profile with a workload.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_profiles)
-        """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#can_paginate)
         """
@@ -187,40 +163,14 @@
         """
         Create a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_milestone)
         """
 
-    def create_profile(
-        self,
-        *,
-        ProfileName: str,
-        ProfileDescription: str,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
-        ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
-    ) -> CreateProfileOutputTypeDef:
-        """
-        Create a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
-        """
-
-    def create_profile_share(
-        self, *, ProfileArn: str, SharedWith: str, ClientRequestToken: str
-    ) -> CreateProfileShareOutputTypeDef:
-        """
-        Create a profile share.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile_share)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile_share)
-        """
-
     def create_workload(
         self,
         *,
         WorkloadName: str,
         Description: str,
         Environment: WorkloadEnvironmentType,
         Lenses: Sequence[str],
@@ -232,16 +182,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...,
-        ProfileArns: Sequence[str] = ...
+        Applications: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
@@ -277,34 +226,14 @@
         """
         Delete a lens share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_lens_share)
         """
 
-    def delete_profile(
-        self, *, ProfileArn: str, ClientRequestToken: str
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Delete a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile)
-        """
-
-    def delete_profile_share(
-        self, *, ShareId: str, ProfileArn: str, ClientRequestToken: str
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Delete a profile share.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile_share)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile_share)
-        """
-
     def delete_workload(
         self, *, WorkloadId: str, ClientRequestToken: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload)
@@ -327,24 +256,14 @@
         """
         Disassociate a lens from a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_lenses)
         """
 
-    def disassociate_profiles(
-        self, *, WorkloadId: str, ProfileArns: Sequence[str]
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Disassociate a profile from a workload.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_profiles)
-        """
-
     def export_lens(self, *, LensAlias: str, LensVersion: str = ...) -> ExportLensOutputTypeDef:
         """
         Export an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.export_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#export_lens)
         """
@@ -369,29 +288,14 @@
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
 
-    def get_consolidated_report(
-        self,
-        *,
-        Format: ReportFormatType,
-        IncludeSharedResources: bool = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> GetConsolidatedReportOutputTypeDef:
-        """
-        Get a consolidated report of your workloads.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
-        """
-
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -430,30 +334,14 @@
         """
         Get a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_milestone)
         """
 
-    def get_profile(self, *, ProfileArn: str, ProfileVersion: str = ...) -> GetProfileOutputTypeDef:
-        """
-        Get profile information.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile)
-        """
-
-    def get_profile_template(self) -> GetProfileTemplateOutputTypeDef:
-        """
-        Get profile template.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile_template)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile_template)
-        """
-
     def get_workload(self, *, WorkloadId: str) -> GetWorkloadOutputTypeDef:
         """
         Get an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_workload)
         """
@@ -463,33 +351,32 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new custom lens or update an existing custom lens.
+        Import a new lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
 
     def list_answers(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        MaxResults: int = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers for a particular workload and lens.
+        List of answers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
 
     def list_check_details(
         self,
@@ -532,16 +419,15 @@
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        MaxResults: int = ...
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
@@ -551,15 +437,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews for a particular workload.
+        List lens reviews.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
 
     def list_lens_shares(
         self,
@@ -609,64 +495,22 @@
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
 
-    def list_profile_notifications(
-        self, *, WorkloadId: str = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> ListProfileNotificationsOutputTypeDef:
-        """
-        List profile notifications.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_notifications)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_notifications)
-        """
-
-    def list_profile_shares(
-        self,
-        *,
-        ProfileArn: str,
-        SharedWithPrefix: str = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...,
-        Status: ShareStatusType = ...
-    ) -> ListProfileSharesOutputTypeDef:
-        """
-        List profile shares.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
-        """
-
-    def list_profiles(
-        self,
-        *,
-        ProfileNamePrefix: str = ...,
-        ProfileOwnerType: ProfileOwnerTypeType = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListProfilesOutputTypeDef:
-        """
-        List profiles.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
-        """
-
     def list_share_invitations(
         self,
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        ProfileNamePrefix: str = ...
+        MaxResults: int = ...
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the workload invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -695,15 +539,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
 
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Paginated list of workloads.
+        List workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
 
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
@@ -737,56 +581,39 @@
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
 
     def update_global_settings(
-        self,
-        *,
-        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing and discovery integration features.
+        sharing features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
 
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review for a particular workload.
+        Update lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
 
-    def update_profile(
-        self,
-        *,
-        ProfileArn: str,
-        ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
-    ) -> UpdateProfileOutputTypeDef:
-        """
-        Update a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
-        """
-
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
     ) -> UpdateShareInvitationOutputTypeDef:
         """
         Update a workload or custom lens share invitation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_share_invitation)
@@ -831,27 +658,12 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
 
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review for a particular workload.
+        Upgrade lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
-
-    def upgrade_profile_version(
-        self,
-        *,
-        WorkloadId: str,
-        ProfileArn: str,
-        MilestoneName: str = ...,
-        ClientRequestToken: str = ...
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Upgrade a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
-        """
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/client.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -15,70 +15,56 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
-    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
     ChoiceUpdateTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
-    CreateProfileOutputTypeDef,
-    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
-    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
-    GetProfileOutputTypeDef,
-    GetProfileTemplateOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
     ListAnswersOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListLensesOutputTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListLensSharesOutputTypeDef,
     ListMilestonesOutputTypeDef,
     ListNotificationsOutputTypeDef,
-    ListProfileNotificationsOutputTypeDef,
-    ListProfileSharesOutputTypeDef,
-    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
-    ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
-    UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
@@ -121,23 +107,14 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associate a lens to a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_lenses)
         """
-    def associate_profiles(
-        self, *, WorkloadId: str, ProfileArns: Sequence[str]
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Associate a profile with a workload.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.associate_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#associate_profiles)
-        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#can_paginate)
         """
@@ -176,38 +153,14 @@
     ) -> CreateMilestoneOutputTypeDef:
         """
         Create a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_milestone)
         """
-    def create_profile(
-        self,
-        *,
-        ProfileName: str,
-        ProfileDescription: str,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef],
-        ClientRequestToken: str,
-        Tags: Mapping[str, str] = ...
-    ) -> CreateProfileOutputTypeDef:
-        """
-        Create a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile)
-        """
-    def create_profile_share(
-        self, *, ProfileArn: str, SharedWith: str, ClientRequestToken: str
-    ) -> CreateProfileShareOutputTypeDef:
-        """
-        Create a profile share.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_profile_share)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_profile_share)
-        """
     def create_workload(
         self,
         *,
         WorkloadName: str,
         Description: str,
         Environment: WorkloadEnvironmentType,
         Lenses: Sequence[str],
@@ -219,16 +172,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
         DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
-        Applications: Sequence[str] = ...,
-        ProfileArns: Sequence[str] = ...
+        Applications: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#create_workload)
         """
@@ -260,32 +212,14 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a lens share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_lens_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_lens_share)
         """
-    def delete_profile(
-        self, *, ProfileArn: str, ClientRequestToken: str
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Delete a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile)
-        """
-    def delete_profile_share(
-        self, *, ShareId: str, ProfileArn: str, ClientRequestToken: str
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Delete a profile share.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_profile_share)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#delete_profile_share)
-        """
     def delete_workload(
         self, *, WorkloadId: str, ClientRequestToken: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.delete_workload)
@@ -305,23 +239,14 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disassociate a lens from a workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_lenses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_lenses)
         """
-    def disassociate_profiles(
-        self, *, WorkloadId: str, ProfileArns: Sequence[str]
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Disassociate a profile from a workload.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.disassociate_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#disassociate_profiles)
-        """
     def export_lens(self, *, LensAlias: str, LensVersion: str = ...) -> ExportLensOutputTypeDef:
         """
         Export an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.export_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#export_lens)
         """
@@ -343,28 +268,14 @@
     ) -> GetAnswerOutputTypeDef:
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
-    def get_consolidated_report(
-        self,
-        *,
-        Format: ReportFormatType,
-        IncludeSharedResources: bool = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> GetConsolidatedReportOutputTypeDef:
-        """
-        Get a consolidated report of your workloads.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
-        """
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -398,28 +309,14 @@
     def get_milestone(self, *, WorkloadId: str, MilestoneNumber: int) -> GetMilestoneOutputTypeDef:
         """
         Get a milestone for an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_milestone)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_milestone)
         """
-    def get_profile(self, *, ProfileArn: str, ProfileVersion: str = ...) -> GetProfileOutputTypeDef:
-        """
-        Get profile information.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile)
-        """
-    def get_profile_template(self) -> GetProfileTemplateOutputTypeDef:
-        """
-        Get profile template.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_profile_template)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_profile_template)
-        """
     def get_workload(self, *, WorkloadId: str) -> GetWorkloadOutputTypeDef:
         """
         Get an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_workload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_workload)
         """
@@ -428,32 +325,31 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new custom lens or update an existing custom lens.
+        Import a new lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
     def list_answers(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        MaxResults: int = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers for a particular workload and lens.
+        List of answers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
     def list_check_details(
         self,
         *,
@@ -493,16 +389,15 @@
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        QuestionPriority: QuestionPriorityType = ...
+        MaxResults: int = ...
     ) -> ListLensReviewImprovementsOutputTypeDef:
         """
         List lens review improvements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_review_improvements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_review_improvements)
         """
@@ -511,15 +406,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews for a particular workload.
+        List lens reviews.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
     def list_lens_shares(
         self,
         *,
@@ -564,61 +459,22 @@
     ) -> ListNotificationsOutputTypeDef:
         """
         List lens notifications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_notifications)
         """
-    def list_profile_notifications(
-        self, *, WorkloadId: str = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> ListProfileNotificationsOutputTypeDef:
-        """
-        List profile notifications.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_notifications)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_notifications)
-        """
-    def list_profile_shares(
-        self,
-        *,
-        ProfileArn: str,
-        SharedWithPrefix: str = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...,
-        Status: ShareStatusType = ...
-    ) -> ListProfileSharesOutputTypeDef:
-        """
-        List profile shares.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profile_shares)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profile_shares)
-        """
-    def list_profiles(
-        self,
-        *,
-        ProfileNamePrefix: str = ...,
-        ProfileOwnerType: ProfileOwnerTypeType = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListProfilesOutputTypeDef:
-        """
-        List profiles.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_profiles)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_profiles)
-        """
     def list_share_invitations(
         self,
         *,
         WorkloadNamePrefix: str = ...,
         LensNamePrefix: str = ...,
         ShareResourceType: ShareResourceTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...,
-        ProfileNamePrefix: str = ...
+        MaxResults: int = ...
     ) -> ListShareInvitationsOutputTypeDef:
         """
         List the workload invitations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_share_invitations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_share_invitations)
         """
@@ -644,15 +500,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Paginated list of workloads.
+        List workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to the specified resource.
@@ -682,53 +538,37 @@
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
     def update_global_settings(
-        self,
-        *,
-        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing and discovery integration features.
+        sharing features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review for a particular workload.
+        Update lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
-    def update_profile(
-        self,
-        *,
-        ProfileArn: str,
-        ProfileDescription: str = ...,
-        ProfileQuestions: Sequence[ProfileQuestionUpdateTypeDef] = ...
-    ) -> UpdateProfileOutputTypeDef:
-        """
-        Update a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_profile)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_profile)
-        """
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
     ) -> UpdateShareInvitationOutputTypeDef:
         """
         Update a workload or custom lens share invitation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_share_invitation)
@@ -770,26 +610,12 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review for a particular workload.
+        Upgrade lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
-    def upgrade_profile_version(
-        self,
-        *,
-        WorkloadId: str,
-        ProfileArn: str,
-        MilestoneName: str = ...,
-        ClientRequestToken: str = ...
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Upgrade a profile.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_profile_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_profile_version)
-        """
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/literals.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,30 +23,22 @@
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
-    "DefinitionTypeType",
     "DifferenceStatusType",
-    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
-    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
-    "ProfileNotificationTypeType",
-    "ProfileOwnerTypeType",
-    "QuestionPriorityType",
-    "QuestionTypeType",
-    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
@@ -66,33 +58,25 @@
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
-DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
-DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
-MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
-ProfileNotificationTypeType = Literal["PROFILE_ANSWERS_UPDATED", "PROFILE_DELETED"]
-ProfileOwnerTypeType = Literal["SELF", "SHARED"]
-QuestionPriorityType = Literal["NONE", "PRIORITIZED"]
-QuestionTypeType = Literal["NON_PRIORITIZED", "PRIORITIZED"]
-ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
-ShareResourceTypeType = Literal["LENS", "PROFILE", "WORKLOAD"]
+ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
@@ -118,15 +102,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -136,35 +119,30 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -190,15 +168,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -243,57 +220,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -306,15 +277,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -326,35 +296,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -363,15 +326,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -382,64 +344,55 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/literals.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -22,30 +22,22 @@
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
-    "DefinitionTypeType",
     "DifferenceStatusType",
-    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
-    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
-    "ProfileNotificationTypeType",
-    "ProfileOwnerTypeType",
-    "QuestionPriorityType",
-    "QuestionTypeType",
-    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
@@ -64,33 +56,25 @@
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
-DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
-DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
-MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
-ProfileNotificationTypeType = Literal["PROFILE_ANSWERS_UPDATED", "PROFILE_DELETED"]
-ProfileOwnerTypeType = Literal["SELF", "SHARED"]
-QuestionPriorityType = Literal["NONE", "PRIORITIZED"]
-QuestionTypeType = Literal["NON_PRIORITIZED", "PRIORITIZED"]
-ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
-ShareResourceTypeType = Literal["LENS", "PROFILE", "WORKLOAD"]
+ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 WorkloadEnvironmentType = Literal["PREPRODUCTION", "PRODUCTION"]
 WorkloadImprovementStatusType = Literal[
     "COMPLETE", "IN_PROGRESS", "NOT_APPLICABLE", "NOT_STARTED", "RISK_ACKNOWLEDGED"
@@ -116,15 +100,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -134,35 +117,30 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -188,15 +166,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -241,57 +218,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -304,15 +275,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -324,35 +294,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -361,15 +324,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -380,64 +342,55 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/type_defs.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,29 +18,22 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileNotificationTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    QuestionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -57,157 +50,119 @@
 
 
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
-    "AssociateProfilesInputRequestTypeDef",
-    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "ProfileQuestionUpdateTypeDef",
-    "CreateProfileShareInputRequestTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
-    "DeleteProfileInputRequestTypeDef",
-    "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
-    "DisassociateProfilesInputRequestTypeDef",
     "ExportLensInputRequestTypeDef",
     "GetAnswerInputRequestTypeDef",
-    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
-    "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "WorkloadProfileTypeDef",
+    "LensReviewSummaryTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
     "ListCheckSummariesInputRequestTypeDef",
     "ListLensReviewImprovementsInputRequestTypeDef",
     "ListLensReviewsInputRequestTypeDef",
     "ListLensSharesInputRequestTypeDef",
     "ListLensesInputRequestTypeDef",
     "ListMilestonesInputRequestTypeDef",
     "ListNotificationsInputRequestTypeDef",
-    "ListProfileNotificationsInputRequestTypeDef",
-    "ProfileNotificationSummaryTypeDef",
-    "ListProfileSharesInputRequestTypeDef",
-    "ProfileShareSummaryTypeDef",
-    "ListProfilesInputRequestTypeDef",
-    "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
+    "WorkloadSummaryTypeDef",
     "QuestionDifferenceTypeDef",
-    "ProfileChoiceTypeDef",
-    "ProfileTemplateChoiceTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
-    "UpgradeProfileVersionInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
-    "CreateProfileOutputTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportLensOutputTypeDef",
     "ImportLensOutputTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "CreateProfileInputRequestTypeDef",
-    "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
+    "WorkloadTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
-    "LensReviewSummaryTypeDef",
-    "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
+    "ListLensReviewsOutputTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
-    "ListProfileNotificationsOutputTypeDef",
-    "ListProfileSharesOutputTypeDef",
-    "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
+    "ListWorkloadsOutputTypeDef",
+    "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
-    "ProfileQuestionTypeDef",
-    "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
-    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
-    "ListLensReviewsOutputTypeDef",
-    "ListWorkloadsOutputTypeDef",
-    "MilestoneSummaryTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
+    "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
-    "ProfileTypeDef",
-    "ProfileTemplateTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
-    "LensMetricTypeDef",
-    "ListMilestonesOutputTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
-    "GetProfileOutputTypeDef",
-    "UpdateProfileOutputTypeDef",
-    "GetProfileTemplateOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
-    "ConsolidatedReportMetricTypeDef",
-    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -240,31 +195,14 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-AssociateProfilesInputRequestTypeDef = TypedDict(
-    "AssociateProfilesInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArns": Sequence[str],
-    },
-)
-
-BestPracticeTypeDef = TypedDict(
-    "BestPracticeTypeDef",
-    {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-    },
-    total=False,
-)
-
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -377,37 +315,18 @@
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-ProfileQuestionUpdateTypeDef = TypedDict(
-    "ProfileQuestionUpdateTypeDef",
-    {
-        "QuestionId": str,
-        "SelectedChoiceIds": Sequence[str],
-    },
-    total=False,
-)
-
-CreateProfileShareInputRequestTypeDef = TypedDict(
-    "CreateProfileShareInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-        "SharedWith": str,
-        "ClientRequestToken": str,
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
@@ -432,31 +351,14 @@
     {
         "ShareId": str,
         "LensAlias": str,
         "ClientRequestToken": str,
     },
 )
 
-DeleteProfileInputRequestTypeDef = TypedDict(
-    "DeleteProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-        "ClientRequestToken": str,
-    },
-)
-
-DeleteProfileShareInputRequestTypeDef = TypedDict(
-    "DeleteProfileShareInputRequestTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ClientRequestToken": str,
-    },
-)
-
 DeleteWorkloadInputRequestTypeDef = TypedDict(
     "DeleteWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ClientRequestToken": str,
     },
 )
@@ -474,22 +376,14 @@
     "DisassociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-DisassociateProfilesInputRequestTypeDef = TypedDict(
-    "DisassociateProfilesInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArns": Sequence[str],
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -526,38 +420,14 @@
 
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
 
-_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetConsolidatedReportInputRequestTypeDef",
-    {
-        "Format": ReportFormatType,
-    },
-)
-_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetConsolidatedReportInputRequestTypeDef",
-    {
-        "IncludeSharedResources": bool,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetConsolidatedReportInputRequestTypeDef(
-    _RequiredGetConsolidatedReportInputRequestTypeDef,
-    _OptionalGetConsolidatedReportInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalGetLensInputRequestTypeDef = TypedDict(
@@ -670,35 +540,14 @@
     "GetMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
     },
 )
 
-_RequiredGetProfileInputRequestTypeDef = TypedDict(
-    "_RequiredGetProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalGetProfileInputRequestTypeDef = TypedDict(
-    "_OptionalGetProfileInputRequestTypeDef",
-    {
-        "ProfileVersion": str,
-    },
-    total=False,
-)
-
-
-class GetProfileInputRequestTypeDef(
-    _RequiredGetProfileInputRequestTypeDef, _OptionalGetProfileInputRequestTypeDef
-):
-    pass
-
-
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 
@@ -721,31 +570,35 @@
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
 
-WorkloadProfileTypeDef = TypedDict(
-    "WorkloadProfileTypeDef",
+LensReviewSummaryTypeDef = TypedDict(
+    "LensReviewSummaryTypeDef",
     {
-        "ProfileArn": str,
-        "ProfileVersion": str,
+        "LensAlias": str,
+        "LensArn": str,
+        "LensVersion": str,
+        "LensName": str,
+        "LensStatus": LensStatusType,
+        "UpdatedAt": datetime,
+        "RiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 PillarReviewSummaryTypeDef = TypedDict(
     "PillarReviewSummaryTypeDef",
     {
         "PillarId": str,
         "PillarName": str,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 LensShareSummaryTypeDef = TypedDict(
     "LensShareSummaryTypeDef",
     {
@@ -797,15 +650,14 @@
 _OptionalListAnswersInputRequestTypeDef = TypedDict(
     "_OptionalListAnswersInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
-        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
 
 class ListAnswersInputRequestTypeDef(
     _RequiredListAnswersInputRequestTypeDef, _OptionalListAnswersInputRequestTypeDef
@@ -875,15 +727,14 @@
 _OptionalListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_OptionalListLensReviewImprovementsInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
-        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
 
 class ListLensReviewImprovementsInputRequestTypeDef(
     _RequiredListLensReviewImprovementsInputRequestTypeDef,
@@ -979,107 +830,22 @@
         "WorkloadId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProfileNotificationsInputRequestTypeDef = TypedDict(
-    "ListProfileNotificationsInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ProfileNotificationSummaryTypeDef = TypedDict(
-    "ProfileNotificationSummaryTypeDef",
-    {
-        "CurrentProfileVersion": str,
-        "LatestProfileVersion": str,
-        "Type": ProfileNotificationTypeType,
-        "ProfileArn": str,
-        "ProfileName": str,
-        "WorkloadId": str,
-        "WorkloadName": str,
-    },
-    total=False,
-)
-
-_RequiredListProfileSharesInputRequestTypeDef = TypedDict(
-    "_RequiredListProfileSharesInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalListProfileSharesInputRequestTypeDef = TypedDict(
-    "_OptionalListProfileSharesInputRequestTypeDef",
-    {
-        "SharedWithPrefix": str,
-        "NextToken": str,
-        "MaxResults": int,
-        "Status": ShareStatusType,
-    },
-    total=False,
-)
-
-
-class ListProfileSharesInputRequestTypeDef(
-    _RequiredListProfileSharesInputRequestTypeDef, _OptionalListProfileSharesInputRequestTypeDef
-):
-    pass
-
-
-ProfileShareSummaryTypeDef = TypedDict(
-    "ProfileShareSummaryTypeDef",
-    {
-        "ShareId": str,
-        "SharedWith": str,
-        "Status": ShareStatusType,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
-ListProfilesInputRequestTypeDef = TypedDict(
-    "ListProfilesInputRequestTypeDef",
-    {
-        "ProfileNamePrefix": str,
-        "ProfileOwnerType": ProfileOwnerTypeType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ProfileSummaryTypeDef = TypedDict(
-    "ProfileSummaryTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "Owner": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-    },
-    total=False,
-)
-
 ListShareInvitationsInputRequestTypeDef = TypedDict(
     "ListShareInvitationsInputRequestTypeDef",
     {
         "WorkloadNamePrefix": str,
         "LensNamePrefix": str,
         "ShareResourceType": ShareResourceTypeType,
         "NextToken": str,
         "MaxResults": int,
-        "ProfileNamePrefix": str,
     },
     total=False,
 )
 
 ShareInvitationSummaryTypeDef = TypedDict(
     "ShareInvitationSummaryTypeDef",
     {
@@ -1088,16 +854,14 @@
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadName": str,
         "WorkloadId": str,
         "LensName": str,
         "LensArn": str,
-        "ProfileName": str,
-        "ProfileArn": str,
     },
     total=False,
 )
 
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
@@ -1147,53 +911,47 @@
         "WorkloadNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-QuestionDifferenceTypeDef = TypedDict(
-    "QuestionDifferenceTypeDef",
-    {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "DifferenceStatus": DifferenceStatusType,
-    },
-    total=False,
-)
-
-ProfileChoiceTypeDef = TypedDict(
-    "ProfileChoiceTypeDef",
+WorkloadSummaryTypeDef = TypedDict(
+    "WorkloadSummaryTypeDef",
     {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-        "ChoiceDescription": str,
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Owner": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[str],
+        "RiskCounts": Dict[RiskType, int],
+        "ImprovementStatus": WorkloadImprovementStatusType,
     },
     total=False,
 )
 
-ProfileTemplateChoiceTypeDef = TypedDict(
-    "ProfileTemplateChoiceTypeDef",
+QuestionDifferenceTypeDef = TypedDict(
+    "QuestionDifferenceTypeDef",
     {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-        "ChoiceDescription": str,
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "DifferenceStatus": DifferenceStatusType,
     },
     total=False,
 )
 
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
-        "ProfileArn": str,
     },
     total=False,
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
@@ -1210,15 +968,14 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
-        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -1292,57 +1049,23 @@
 
 class UpgradeLensReviewInputRequestTypeDef(
     _RequiredUpgradeLensReviewInputRequestTypeDef, _OptionalUpgradeLensReviewInputRequestTypeDef
 ):
     pass
 
 
-_RequiredUpgradeProfileVersionInputRequestTypeDef = TypedDict(
-    "_RequiredUpgradeProfileVersionInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArn": str,
-    },
-)
-_OptionalUpgradeProfileVersionInputRequestTypeDef = TypedDict(
-    "_OptionalUpgradeProfileVersionInputRequestTypeDef",
-    {
-        "MilestoneName": str,
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class UpgradeProfileVersionInputRequestTypeDef(
-    _RequiredUpgradeProfileVersionInputRequestTypeDef,
-    _OptionalUpgradeProfileVersionInputRequestTypeDef,
-):
-    pass
-
-
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
-QuestionMetricTypeDef = TypedDict(
-    "QuestionMetricTypeDef",
-    {
-        "QuestionId": str,
-        "Risk": RiskType,
-        "BestPractices": List[BestPracticeTypeDef],
-    },
-    total=False,
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1401,32 +1124,14 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkloadOutputTypeDef = TypedDict(
     "CreateWorkloadOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1487,60 +1192,14 @@
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProfileInputRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileInputRequestTypeDef",
-    {
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
-        "ClientRequestToken": str,
-    },
-)
-_OptionalCreateProfileInputRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileInputRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateProfileInputRequestTypeDef(
-    _RequiredCreateProfileInputRequestTypeDef, _OptionalCreateProfileInputRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateProfileInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalUpdateProfileInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileInputRequestTypeDef",
-    {
-        "ProfileDescription": str,
-        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateProfileInputRequestTypeDef(
-    _RequiredUpdateProfileInputRequestTypeDef, _OptionalUpdateProfileInputRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkloadInputRequestTypeDef",
     {
         "WorkloadName": str,
         "Description": str,
         "Environment": WorkloadEnvironmentType,
         "Lenses": Sequence[str],
@@ -1558,15 +1217,14 @@
         "ReviewOwner": str,
         "IndustryType": str,
         "Industry": str,
         "Notes": str,
         "Tags": Mapping[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
-        "ProfileArns": Sequence[str],
     },
     total=False,
 )
 
 
 class CreateWorkloadInputRequestTypeDef(
     _RequiredCreateWorkloadInputRequestTypeDef, _OptionalCreateWorkloadInputRequestTypeDef
@@ -1606,65 +1264,14 @@
 
 class UpdateWorkloadInputRequestTypeDef(
     _RequiredUpdateWorkloadInputRequestTypeDef, _OptionalUpdateWorkloadInputRequestTypeDef
 ):
     pass
 
 
-GetLensOutputTypeDef = TypedDict(
-    "GetLensOutputTypeDef",
-    {
-        "Lens": LensTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLensReviewReportOutputTypeDef = TypedDict(
-    "GetLensReviewReportOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LensReviewSummaryTypeDef = TypedDict(
-    "LensReviewSummaryTypeDef",
-    {
-        "LensAlias": str,
-        "LensArn": str,
-        "LensVersion": str,
-        "LensName": str,
-        "LensStatus": LensStatusType,
-        "UpdatedAt": datetime,
-        "RiskCounts": Dict[RiskType, int],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
-WorkloadSummaryTypeDef = TypedDict(
-    "WorkloadSummaryTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Owner": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[str],
-        "RiskCounts": Dict[RiskType, int],
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
         "Description": str,
@@ -1685,35 +1292,60 @@
         "PillarPriorities": List[str],
         "Lenses": List[str],
         "Owner": str,
         "ShareInvitationId": str,
         "Tags": Dict[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
+GetLensOutputTypeDef = TypedDict(
+    "GetLensOutputTypeDef",
+    {
+        "Lens": LensTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLensReviewReportOutputTypeDef = TypedDict(
+    "GetLensReviewReportOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewReport": LensReviewReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLensReviewsOutputTypeDef = TypedDict(
+    "ListLensReviewsOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
         "LensStatus": LensStatusType,
         "PillarReviewSummaries": List[PillarReviewSummaryTypeDef],
         "UpdatedAt": datetime,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
         "NextToken": str,
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
@@ -1737,41 +1369,14 @@
     {
         "Type": NotificationTypeType,
         "LensUpgradeSummary": LensUpgradeSummaryTypeDef,
     },
     total=False,
 )
 
-ListProfileNotificationsOutputTypeDef = TypedDict(
-    "ListProfileNotificationsOutputTypeDef",
-    {
-        "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProfileSharesOutputTypeDef = TypedDict(
-    "ListProfileSharesOutputTypeDef",
-    {
-        "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProfilesOutputTypeDef = TypedDict(
-    "ListProfilesOutputTypeDef",
-    {
-        "ProfileSummaries": List[ProfileSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1783,48 +1388,41 @@
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PillarDifferenceTypeDef = TypedDict(
-    "PillarDifferenceTypeDef",
+ListWorkloadsOutputTypeDef = TypedDict(
+    "ListWorkloadsOutputTypeDef",
     {
-        "PillarId": str,
-        "PillarName": str,
-        "DifferenceStatus": DifferenceStatusType,
-        "QuestionDifferences": List[QuestionDifferenceTypeDef],
+        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ProfileQuestionTypeDef = TypedDict(
-    "ProfileQuestionTypeDef",
+MilestoneSummaryTypeDef = TypedDict(
+    "MilestoneSummaryTypeDef",
     {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "QuestionDescription": str,
-        "QuestionChoices": List[ProfileChoiceTypeDef],
-        "SelectedChoiceIds": List[str],
-        "MinSelectedChoices": int,
-        "MaxSelectedChoices": int,
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-ProfileTemplateQuestionTypeDef = TypedDict(
-    "ProfileTemplateQuestionTypeDef",
+PillarDifferenceTypeDef = TypedDict(
+    "PillarDifferenceTypeDef",
     {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "QuestionDescription": str,
-        "QuestionChoices": List[ProfileTemplateChoiceTypeDef],
-        "MinSelectedChoices": int,
-        "MaxSelectedChoices": int,
+        "PillarId": str,
+        "PillarName": str,
+        "DifferenceStatus": DifferenceStatusType,
+        "QuestionDifferences": List[QuestionDifferenceTypeDef],
     },
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
@@ -1851,68 +1449,27 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
-PillarMetricTypeDef = TypedDict(
-    "PillarMetricTypeDef",
-    {
-        "PillarId": str,
-        "RiskCounts": Dict[RiskType, int],
-        "Questions": List[QuestionMetricTypeDef],
-    },
-    total=False,
-)
-
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLensReviewsOutputTypeDef = TypedDict(
-    "ListLensReviewsOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListWorkloadsOutputTypeDef = TypedDict(
-    "ListWorkloadsOutputTypeDef",
-    {
-        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MilestoneSummaryTypeDef = TypedDict(
-    "MilestoneSummaryTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "WorkloadSummary": WorkloadSummaryTypeDef,
-    },
-    total=False,
-)
-
 GetWorkloadOutputTypeDef = TypedDict(
     "GetWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1960,46 +1517,28 @@
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VersionDifferencesTypeDef = TypedDict(
-    "VersionDifferencesTypeDef",
-    {
-        "PillarDifferences": List[PillarDifferenceTypeDef],
-    },
-    total=False,
-)
-
-ProfileTypeDef = TypedDict(
-    "ProfileTypeDef",
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
     {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "ProfileQuestions": List[ProfileQuestionTypeDef],
-        "Owner": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ProfileTemplateTypeDef = TypedDict(
-    "ProfileTemplateTypeDef",
+VersionDifferencesTypeDef = TypedDict(
+    "VersionDifferencesTypeDef",
     {
-        "TemplateName": str,
-        "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
+        "PillarDifferences": List[PillarDifferenceTypeDef],
     },
     total=False,
 )
 
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
@@ -2008,15 +1547,14 @@
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
         "SelectedChoices": List[str],
         "ChoiceAnswerSummaries": List[ChoiceAnswerSummaryTypeDef],
         "IsApplicable": bool,
         "Risk": RiskType,
         "Reason": AnswerReasonType,
-        "QuestionType": QuestionTypeType,
     },
     total=False,
 )
 
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
@@ -2034,34 +1572,14 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
-LensMetricTypeDef = TypedDict(
-    "LensMetricTypeDef",
-    {
-        "LensArn": str,
-        "Pillars": List[PillarMetricTypeDef],
-        "RiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2076,38 +1594,14 @@
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetProfileOutputTypeDef = TypedDict(
-    "GetProfileOutputTypeDef",
-    {
-        "Profile": ProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProfileOutputTypeDef = TypedDict(
-    "UpdateProfileOutputTypeDef",
-    {
-        "Profile": ProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProfileTemplateOutputTypeDef = TypedDict(
-    "GetProfileTemplateOutputTypeDef",
-    {
-        "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
@@ -2135,32 +1629,7 @@
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ConsolidatedReportMetricTypeDef = TypedDict(
-    "ConsolidatedReportMetricTypeDef",
-    {
-        "MetricType": Literal["WORKLOAD"],
-        "RiskCounts": Dict[RiskType, int],
-        "WorkloadId": str,
-        "WorkloadName": str,
-        "WorkloadArn": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[LensMetricTypeDef],
-        "LensesAppliedCount": int,
-    },
-    total=False,
-)
-
-GetConsolidatedReportOutputTypeDef = TypedDict(
-    "GetConsolidatedReportOutputTypeDef",
-    {
-        "Metrics": List[ConsolidatedReportMetricTypeDef],
-        "NextToken": str,
-        "Base64String": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -18,29 +18,22 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileNotificationTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    QuestionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -56,157 +49,119 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
-    "AssociateProfilesInputRequestTypeDef",
-    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "ProfileQuestionUpdateTypeDef",
-    "CreateProfileShareInputRequestTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
-    "DeleteProfileInputRequestTypeDef",
-    "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
-    "DisassociateProfilesInputRequestTypeDef",
     "ExportLensInputRequestTypeDef",
     "GetAnswerInputRequestTypeDef",
-    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
-    "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "WorkloadProfileTypeDef",
+    "LensReviewSummaryTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
     "ListCheckSummariesInputRequestTypeDef",
     "ListLensReviewImprovementsInputRequestTypeDef",
     "ListLensReviewsInputRequestTypeDef",
     "ListLensSharesInputRequestTypeDef",
     "ListLensesInputRequestTypeDef",
     "ListMilestonesInputRequestTypeDef",
     "ListNotificationsInputRequestTypeDef",
-    "ListProfileNotificationsInputRequestTypeDef",
-    "ProfileNotificationSummaryTypeDef",
-    "ListProfileSharesInputRequestTypeDef",
-    "ProfileShareSummaryTypeDef",
-    "ListProfilesInputRequestTypeDef",
-    "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
+    "WorkloadSummaryTypeDef",
     "QuestionDifferenceTypeDef",
-    "ProfileChoiceTypeDef",
-    "ProfileTemplateChoiceTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
-    "UpgradeProfileVersionInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
-    "CreateProfileOutputTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportLensOutputTypeDef",
     "ImportLensOutputTypeDef",
     "ListCheckDetailsOutputTypeDef",
     "ListCheckSummariesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "CreateProfileInputRequestTypeDef",
-    "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
+    "WorkloadTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
-    "LensReviewSummaryTypeDef",
-    "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
+    "ListLensReviewsOutputTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
-    "ListProfileNotificationsOutputTypeDef",
-    "ListProfileSharesOutputTypeDef",
-    "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
+    "ListWorkloadsOutputTypeDef",
+    "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
-    "ProfileQuestionTypeDef",
-    "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
-    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
-    "ListLensReviewsOutputTypeDef",
-    "ListWorkloadsOutputTypeDef",
-    "MilestoneSummaryTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
+    "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
-    "ProfileTypeDef",
-    "ProfileTemplateTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
-    "LensMetricTypeDef",
-    "ListMilestonesOutputTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
-    "GetProfileOutputTypeDef",
-    "UpdateProfileOutputTypeDef",
-    "GetProfileTemplateOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
-    "ConsolidatedReportMetricTypeDef",
-    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -239,31 +194,14 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-AssociateProfilesInputRequestTypeDef = TypedDict(
-    "AssociateProfilesInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArns": Sequence[str],
-    },
-)
-
-BestPracticeTypeDef = TypedDict(
-    "BestPracticeTypeDef",
-    {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-    },
-    total=False,
-)
-
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -372,37 +310,18 @@
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-ProfileQuestionUpdateTypeDef = TypedDict(
-    "ProfileQuestionUpdateTypeDef",
-    {
-        "QuestionId": str,
-        "SelectedChoiceIds": Sequence[str],
-    },
-    total=False,
-)
-
-CreateProfileShareInputRequestTypeDef = TypedDict(
-    "CreateProfileShareInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-        "SharedWith": str,
-        "ClientRequestToken": str,
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
@@ -427,31 +346,14 @@
     {
         "ShareId": str,
         "LensAlias": str,
         "ClientRequestToken": str,
     },
 )
 
-DeleteProfileInputRequestTypeDef = TypedDict(
-    "DeleteProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-        "ClientRequestToken": str,
-    },
-)
-
-DeleteProfileShareInputRequestTypeDef = TypedDict(
-    "DeleteProfileShareInputRequestTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ClientRequestToken": str,
-    },
-)
-
 DeleteWorkloadInputRequestTypeDef = TypedDict(
     "DeleteWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ClientRequestToken": str,
     },
 )
@@ -469,22 +371,14 @@
     "DisassociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-DisassociateProfilesInputRequestTypeDef = TypedDict(
-    "DisassociateProfilesInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArns": Sequence[str],
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -517,36 +411,14 @@
 )
 
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
-_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetConsolidatedReportInputRequestTypeDef",
-    {
-        "Format": ReportFormatType,
-    },
-)
-_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetConsolidatedReportInputRequestTypeDef",
-    {
-        "IncludeSharedResources": bool,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetConsolidatedReportInputRequestTypeDef(
-    _RequiredGetConsolidatedReportInputRequestTypeDef,
-    _OptionalGetConsolidatedReportInputRequestTypeDef,
-):
-    pass
-
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalGetLensInputRequestTypeDef = TypedDict(
@@ -651,33 +523,14 @@
     "GetMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
     },
 )
 
-_RequiredGetProfileInputRequestTypeDef = TypedDict(
-    "_RequiredGetProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalGetProfileInputRequestTypeDef = TypedDict(
-    "_OptionalGetProfileInputRequestTypeDef",
-    {
-        "ProfileVersion": str,
-    },
-    total=False,
-)
-
-class GetProfileInputRequestTypeDef(
-    _RequiredGetProfileInputRequestTypeDef, _OptionalGetProfileInputRequestTypeDef
-):
-    pass
-
 GetWorkloadInputRequestTypeDef = TypedDict(
     "GetWorkloadInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 
@@ -698,31 +551,35 @@
 )
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
-WorkloadProfileTypeDef = TypedDict(
-    "WorkloadProfileTypeDef",
+LensReviewSummaryTypeDef = TypedDict(
+    "LensReviewSummaryTypeDef",
     {
-        "ProfileArn": str,
-        "ProfileVersion": str,
+        "LensAlias": str,
+        "LensArn": str,
+        "LensVersion": str,
+        "LensName": str,
+        "LensStatus": LensStatusType,
+        "UpdatedAt": datetime,
+        "RiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 PillarReviewSummaryTypeDef = TypedDict(
     "PillarReviewSummaryTypeDef",
     {
         "PillarId": str,
         "PillarName": str,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 LensShareSummaryTypeDef = TypedDict(
     "LensShareSummaryTypeDef",
     {
@@ -774,15 +631,14 @@
 _OptionalListAnswersInputRequestTypeDef = TypedDict(
     "_OptionalListAnswersInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
-        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
 class ListAnswersInputRequestTypeDef(
     _RequiredListAnswersInputRequestTypeDef, _OptionalListAnswersInputRequestTypeDef
 ):
@@ -846,15 +702,14 @@
 _OptionalListLensReviewImprovementsInputRequestTypeDef = TypedDict(
     "_OptionalListLensReviewImprovementsInputRequestTypeDef",
     {
         "PillarId": str,
         "MilestoneNumber": int,
         "NextToken": str,
         "MaxResults": int,
-        "QuestionPriority": QuestionPriorityType,
     },
     total=False,
 )
 
 class ListLensReviewImprovementsInputRequestTypeDef(
     _RequiredListLensReviewImprovementsInputRequestTypeDef,
     _OptionalListLensReviewImprovementsInputRequestTypeDef,
@@ -942,105 +797,22 @@
         "WorkloadId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProfileNotificationsInputRequestTypeDef = TypedDict(
-    "ListProfileNotificationsInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ProfileNotificationSummaryTypeDef = TypedDict(
-    "ProfileNotificationSummaryTypeDef",
-    {
-        "CurrentProfileVersion": str,
-        "LatestProfileVersion": str,
-        "Type": ProfileNotificationTypeType,
-        "ProfileArn": str,
-        "ProfileName": str,
-        "WorkloadId": str,
-        "WorkloadName": str,
-    },
-    total=False,
-)
-
-_RequiredListProfileSharesInputRequestTypeDef = TypedDict(
-    "_RequiredListProfileSharesInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalListProfileSharesInputRequestTypeDef = TypedDict(
-    "_OptionalListProfileSharesInputRequestTypeDef",
-    {
-        "SharedWithPrefix": str,
-        "NextToken": str,
-        "MaxResults": int,
-        "Status": ShareStatusType,
-    },
-    total=False,
-)
-
-class ListProfileSharesInputRequestTypeDef(
-    _RequiredListProfileSharesInputRequestTypeDef, _OptionalListProfileSharesInputRequestTypeDef
-):
-    pass
-
-ProfileShareSummaryTypeDef = TypedDict(
-    "ProfileShareSummaryTypeDef",
-    {
-        "ShareId": str,
-        "SharedWith": str,
-        "Status": ShareStatusType,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
-ListProfilesInputRequestTypeDef = TypedDict(
-    "ListProfilesInputRequestTypeDef",
-    {
-        "ProfileNamePrefix": str,
-        "ProfileOwnerType": ProfileOwnerTypeType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ProfileSummaryTypeDef = TypedDict(
-    "ProfileSummaryTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "Owner": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-    },
-    total=False,
-)
-
 ListShareInvitationsInputRequestTypeDef = TypedDict(
     "ListShareInvitationsInputRequestTypeDef",
     {
         "WorkloadNamePrefix": str,
         "LensNamePrefix": str,
         "ShareResourceType": ShareResourceTypeType,
         "NextToken": str,
         "MaxResults": int,
-        "ProfileNamePrefix": str,
     },
     total=False,
 )
 
 ShareInvitationSummaryTypeDef = TypedDict(
     "ShareInvitationSummaryTypeDef",
     {
@@ -1049,16 +821,14 @@
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadName": str,
         "WorkloadId": str,
         "LensName": str,
         "LensArn": str,
-        "ProfileName": str,
-        "ProfileArn": str,
     },
     total=False,
 )
 
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
@@ -1106,53 +876,47 @@
         "WorkloadNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-QuestionDifferenceTypeDef = TypedDict(
-    "QuestionDifferenceTypeDef",
-    {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "DifferenceStatus": DifferenceStatusType,
-    },
-    total=False,
-)
-
-ProfileChoiceTypeDef = TypedDict(
-    "ProfileChoiceTypeDef",
+WorkloadSummaryTypeDef = TypedDict(
+    "WorkloadSummaryTypeDef",
     {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-        "ChoiceDescription": str,
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Owner": str,
+        "UpdatedAt": datetime,
+        "Lenses": List[str],
+        "RiskCounts": Dict[RiskType, int],
+        "ImprovementStatus": WorkloadImprovementStatusType,
     },
     total=False,
 )
 
-ProfileTemplateChoiceTypeDef = TypedDict(
-    "ProfileTemplateChoiceTypeDef",
+QuestionDifferenceTypeDef = TypedDict(
+    "QuestionDifferenceTypeDef",
     {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-        "ChoiceDescription": str,
+        "QuestionId": str,
+        "QuestionTitle": str,
+        "DifferenceStatus": DifferenceStatusType,
     },
     total=False,
 )
 
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
-        "ProfileArn": str,
     },
     total=False,
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
@@ -1169,15 +933,14 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
-        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -1247,55 +1010,23 @@
 )
 
 class UpgradeLensReviewInputRequestTypeDef(
     _RequiredUpgradeLensReviewInputRequestTypeDef, _OptionalUpgradeLensReviewInputRequestTypeDef
 ):
     pass
 
-_RequiredUpgradeProfileVersionInputRequestTypeDef = TypedDict(
-    "_RequiredUpgradeProfileVersionInputRequestTypeDef",
-    {
-        "WorkloadId": str,
-        "ProfileArn": str,
-    },
-)
-_OptionalUpgradeProfileVersionInputRequestTypeDef = TypedDict(
-    "_OptionalUpgradeProfileVersionInputRequestTypeDef",
-    {
-        "MilestoneName": str,
-        "ClientRequestToken": str,
-    },
-    total=False,
-)
-
-class UpgradeProfileVersionInputRequestTypeDef(
-    _RequiredUpgradeProfileVersionInputRequestTypeDef,
-    _OptionalUpgradeProfileVersionInputRequestTypeDef,
-):
-    pass
-
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
-QuestionMetricTypeDef = TypedDict(
-    "QuestionMetricTypeDef",
-    {
-        "QuestionId": str,
-        "Risk": RiskType,
-        "BestPractices": List[BestPracticeTypeDef],
-    },
-    total=False,
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1352,32 +1083,14 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateWorkloadOutputTypeDef = TypedDict(
     "CreateWorkloadOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1438,56 +1151,14 @@
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProfileInputRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileInputRequestTypeDef",
-    {
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
-        "ClientRequestToken": str,
-    },
-)
-_OptionalCreateProfileInputRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileInputRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateProfileInputRequestTypeDef(
-    _RequiredCreateProfileInputRequestTypeDef, _OptionalCreateProfileInputRequestTypeDef
-):
-    pass
-
-_RequiredUpdateProfileInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateProfileInputRequestTypeDef",
-    {
-        "ProfileArn": str,
-    },
-)
-_OptionalUpdateProfileInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateProfileInputRequestTypeDef",
-    {
-        "ProfileDescription": str,
-        "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
-    },
-    total=False,
-)
-
-class UpdateProfileInputRequestTypeDef(
-    _RequiredUpdateProfileInputRequestTypeDef, _OptionalUpdateProfileInputRequestTypeDef
-):
-    pass
-
 _RequiredCreateWorkloadInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkloadInputRequestTypeDef",
     {
         "WorkloadName": str,
         "Description": str,
         "Environment": WorkloadEnvironmentType,
         "Lenses": Sequence[str],
@@ -1505,15 +1176,14 @@
         "ReviewOwner": str,
         "IndustryType": str,
         "Industry": str,
         "Notes": str,
         "Tags": Mapping[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": Sequence[str],
-        "ProfileArns": Sequence[str],
     },
     total=False,
 )
 
 class CreateWorkloadInputRequestTypeDef(
     _RequiredCreateWorkloadInputRequestTypeDef, _OptionalCreateWorkloadInputRequestTypeDef
 ):
@@ -1549,65 +1219,14 @@
 )
 
 class UpdateWorkloadInputRequestTypeDef(
     _RequiredUpdateWorkloadInputRequestTypeDef, _OptionalUpdateWorkloadInputRequestTypeDef
 ):
     pass
 
-GetLensOutputTypeDef = TypedDict(
-    "GetLensOutputTypeDef",
-    {
-        "Lens": LensTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLensReviewReportOutputTypeDef = TypedDict(
-    "GetLensReviewReportOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LensReviewSummaryTypeDef = TypedDict(
-    "LensReviewSummaryTypeDef",
-    {
-        "LensAlias": str,
-        "LensArn": str,
-        "LensVersion": str,
-        "LensName": str,
-        "LensStatus": LensStatusType,
-        "UpdatedAt": datetime,
-        "RiskCounts": Dict[RiskType, int],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
-WorkloadSummaryTypeDef = TypedDict(
-    "WorkloadSummaryTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Owner": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[str],
-        "RiskCounts": Dict[RiskType, int],
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 WorkloadTypeDef = TypedDict(
     "WorkloadTypeDef",
     {
         "WorkloadId": str,
         "WorkloadArn": str,
         "WorkloadName": str,
         "Description": str,
@@ -1628,35 +1247,60 @@
         "PillarPriorities": List[str],
         "Lenses": List[str],
         "Owner": str,
         "ShareInvitationId": str,
         "Tags": Dict[str, str],
         "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
         "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
+GetLensOutputTypeDef = TypedDict(
+    "GetLensOutputTypeDef",
+    {
+        "Lens": LensTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLensReviewReportOutputTypeDef = TypedDict(
+    "GetLensReviewReportOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewReport": LensReviewReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLensReviewsOutputTypeDef = TypedDict(
+    "ListLensReviewsOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
         "LensStatus": LensStatusType,
         "PillarReviewSummaries": List[PillarReviewSummaryTypeDef],
         "UpdatedAt": datetime,
         "Notes": str,
         "RiskCounts": Dict[RiskType, int],
         "NextToken": str,
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
@@ -1680,41 +1324,14 @@
     {
         "Type": NotificationTypeType,
         "LensUpgradeSummary": LensUpgradeSummaryTypeDef,
     },
     total=False,
 )
 
-ListProfileNotificationsOutputTypeDef = TypedDict(
-    "ListProfileNotificationsOutputTypeDef",
-    {
-        "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProfileSharesOutputTypeDef = TypedDict(
-    "ListProfileSharesOutputTypeDef",
-    {
-        "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProfilesOutputTypeDef = TypedDict(
-    "ListProfilesOutputTypeDef",
-    {
-        "ProfileSummaries": List[ProfileSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1726,48 +1343,41 @@
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PillarDifferenceTypeDef = TypedDict(
-    "PillarDifferenceTypeDef",
+ListWorkloadsOutputTypeDef = TypedDict(
+    "ListWorkloadsOutputTypeDef",
     {
-        "PillarId": str,
-        "PillarName": str,
-        "DifferenceStatus": DifferenceStatusType,
-        "QuestionDifferences": List[QuestionDifferenceTypeDef],
+        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ProfileQuestionTypeDef = TypedDict(
-    "ProfileQuestionTypeDef",
+MilestoneSummaryTypeDef = TypedDict(
+    "MilestoneSummaryTypeDef",
     {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "QuestionDescription": str,
-        "QuestionChoices": List[ProfileChoiceTypeDef],
-        "SelectedChoiceIds": List[str],
-        "MinSelectedChoices": int,
-        "MaxSelectedChoices": int,
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-ProfileTemplateQuestionTypeDef = TypedDict(
-    "ProfileTemplateQuestionTypeDef",
+PillarDifferenceTypeDef = TypedDict(
+    "PillarDifferenceTypeDef",
     {
-        "QuestionId": str,
-        "QuestionTitle": str,
-        "QuestionDescription": str,
-        "QuestionChoices": List[ProfileTemplateChoiceTypeDef],
-        "MinSelectedChoices": int,
-        "MaxSelectedChoices": int,
+        "PillarId": str,
+        "PillarName": str,
+        "DifferenceStatus": DifferenceStatusType,
+        "QuestionDifferences": List[QuestionDifferenceTypeDef],
     },
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
@@ -1794,68 +1404,27 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
-PillarMetricTypeDef = TypedDict(
-    "PillarMetricTypeDef",
-    {
-        "PillarId": str,
-        "RiskCounts": Dict[RiskType, int],
-        "Questions": List[QuestionMetricTypeDef],
-    },
-    total=False,
-)
-
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListLensReviewsOutputTypeDef = TypedDict(
-    "ListLensReviewsOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "LensReviewSummaries": List[LensReviewSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListWorkloadsOutputTypeDef = TypedDict(
-    "ListWorkloadsOutputTypeDef",
-    {
-        "WorkloadSummaries": List[WorkloadSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MilestoneSummaryTypeDef = TypedDict(
-    "MilestoneSummaryTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "WorkloadSummary": WorkloadSummaryTypeDef,
-    },
-    total=False,
-)
-
 GetWorkloadOutputTypeDef = TypedDict(
     "GetWorkloadOutputTypeDef",
     {
         "Workload": WorkloadTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1903,46 +1472,28 @@
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VersionDifferencesTypeDef = TypedDict(
-    "VersionDifferencesTypeDef",
-    {
-        "PillarDifferences": List[PillarDifferenceTypeDef],
-    },
-    total=False,
-)
-
-ProfileTypeDef = TypedDict(
-    "ProfileTypeDef",
+ListMilestonesOutputTypeDef = TypedDict(
+    "ListMilestonesOutputTypeDef",
     {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ProfileName": str,
-        "ProfileDescription": str,
-        "ProfileQuestions": List[ProfileQuestionTypeDef],
-        "Owner": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
+        "WorkloadId": str,
+        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ProfileTemplateTypeDef = TypedDict(
-    "ProfileTemplateTypeDef",
+VersionDifferencesTypeDef = TypedDict(
+    "VersionDifferencesTypeDef",
     {
-        "TemplateName": str,
-        "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
+        "PillarDifferences": List[PillarDifferenceTypeDef],
     },
     total=False,
 )
 
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
@@ -1951,15 +1502,14 @@
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
         "SelectedChoices": List[str],
         "ChoiceAnswerSummaries": List[ChoiceAnswerSummaryTypeDef],
         "IsApplicable": bool,
         "Risk": RiskType,
         "Reason": AnswerReasonType,
-        "QuestionType": QuestionTypeType,
     },
     total=False,
 )
 
 AnswerTypeDef = TypedDict(
     "AnswerTypeDef",
     {
@@ -1977,34 +1527,14 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
-LensMetricTypeDef = TypedDict(
-    "LensMetricTypeDef",
-    {
-        "LensArn": str,
-        "Pillars": List[PillarMetricTypeDef],
-        "RiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
-ListMilestonesOutputTypeDef = TypedDict(
-    "ListMilestonesOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneSummaries": List[MilestoneSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2019,38 +1549,14 @@
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetProfileOutputTypeDef = TypedDict(
-    "GetProfileOutputTypeDef",
-    {
-        "Profile": ProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProfileOutputTypeDef = TypedDict(
-    "UpdateProfileOutputTypeDef",
-    {
-        "Profile": ProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProfileTemplateOutputTypeDef = TypedDict(
-    "GetProfileTemplateOutputTypeDef",
-    {
-        "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
@@ -2078,32 +1584,7 @@
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ConsolidatedReportMetricTypeDef = TypedDict(
-    "ConsolidatedReportMetricTypeDef",
-    {
-        "MetricType": Literal["WORKLOAD"],
-        "RiskCounts": Dict[RiskType, int],
-        "WorkloadId": str,
-        "WorkloadName": str,
-        "WorkloadArn": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[LensMetricTypeDef],
-        "LensesAppliedCount": int,
-    },
-    total=False,
-)
-
-GetConsolidatedReportOutputTypeDef = TypedDict(
-    "GetConsolidatedReportOutputTypeDef",
-    {
-        "Metrics": List[ConsolidatedReportMetricTypeDef],
-        "NextToken": str,
-        "Base64String": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.153
-Summary: Type annotations for boto3.WellArchitected 1.26.153 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.4
+Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.153](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,30 +283,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ProfileNotificationTypeType,
-    ProfileOwnerTypeType,
-    QuestionPriorityType,
-    QuestionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -331,199 +322,161 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    AssociateProfilesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    ProfileQuestionUpdateTypeDef,
-    CreateProfileShareInputRequestTypeDef,
     WorkloadDiscoveryConfigTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
-    DeleteProfileInputRequestTypeDef,
-    DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
-    DisassociateProfilesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
-    GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    WorkloadProfileTypeDef,
+    LensReviewSummaryTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
     ListCheckSummariesInputRequestTypeDef,
     ListLensReviewImprovementsInputRequestTypeDef,
     ListLensReviewsInputRequestTypeDef,
     ListLensSharesInputRequestTypeDef,
     ListLensesInputRequestTypeDef,
     ListMilestonesInputRequestTypeDef,
     ListNotificationsInputRequestTypeDef,
-    ListProfileNotificationsInputRequestTypeDef,
-    ProfileNotificationSummaryTypeDef,
-    ListProfileSharesInputRequestTypeDef,
-    ProfileShareSummaryTypeDef,
-    ListProfilesInputRequestTypeDef,
-    ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
+    WorkloadSummaryTypeDef,
     QuestionDifferenceTypeDef,
-    ProfileChoiceTypeDef,
-    ProfileTemplateChoiceTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
-    UpgradeProfileVersionInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
-    CreateProfileOutputTypeDef,
-    CreateProfileShareOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     ImportLensOutputTypeDef,
     ListCheckDetailsOutputTypeDef,
     ListCheckSummariesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    CreateProfileInputRequestTypeDef,
-    UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
+    WorkloadTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
-    LensReviewSummaryTypeDef,
-    WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
+    ListLensReviewsOutputTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
-    ListProfileNotificationsOutputTypeDef,
-    ListProfileSharesOutputTypeDef,
-    ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
+    ListWorkloadsOutputTypeDef,
+    MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
-    ProfileQuestionTypeDef,
-    ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
-    ListLensReviewsOutputTypeDef,
-    ListWorkloadsOutputTypeDef,
-    MilestoneSummaryTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
+    ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
-    ProfileTypeDef,
-    ProfileTemplateTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
-    ListMilestonesOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
-    GetProfileOutputTypeDef,
-    UpdateProfileOutputTypeDef,
-    GetProfileTemplateOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.153/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.26.153/setup.py` & `mypy-boto3-wellarchitected-1.26.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """
 Setup script for mypy-boto3-wellarchitected.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.26.153",
+    version="1.26.4",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WellArchitected 1.26.153 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WellArchitected 1.26.4 service generated with"
+        " mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

