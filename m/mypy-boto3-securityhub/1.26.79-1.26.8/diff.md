# Comparing `tmp/mypy-boto3-securityhub-1.26.79.tar.gz` & `tmp/mypy-boto3-securityhub-1.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
```

## Comparing `mypy-boto3-securityhub-1.26.79.tar` & `mypy-boto3-securityhub-1.26.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.749199 mypy-boto3-securityhub-1.26.79/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47462 2023-02-24 21:22:49.737199 mypy-boto3-securityhub-1.26.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45959 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.733199 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47092 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47010 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-02-24 21:22:23.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-02-24 21:22:23.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-02-24 21:22:23.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   253451 2023-02-24 21:22:31.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   253392 2023-02-24 21:22:27.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47462 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-24 21:22:49.000000 mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.749199 mypy-boto3-securityhub-1.26.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-24 21:22:22.000000 mypy-boto3-securityhub-1.26.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-securityhub-1.26.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    42413 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    40962 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41843 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41768 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12058 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    14452 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14438 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)   219409 2022-11-11 21:07:43.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)   219366 2022-11-11 21:07:41.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:39.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    42413 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-11 21:07:53.000000 mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.070122 mypy-boto3-securityhub-1.26.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-11-11 21:07:38.000000 mypy-boto3-securityhub-1.26.8/setup.py
```

### Comparing `mypy-boto3-securityhub-1.26.79/LICENSE` & `mypy-boto3-securityhub-1.26.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.26.79/PKG-INFO` & `mypy-boto3-securityhub-1.26.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.26.79
-Summary: Type annotations for boto3.SecurityHub 1.26.79 service generated with mypy-boto3-builder 7.12.4
+Version: 1.26.8
+Summary: Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
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
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,16 +290,14 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -325,38 +322,30 @@
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
-list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
-    client.get_paginator("list_security_control_definitions")
-)
-list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
-    client.get_paginator("list_standards_control_associations")
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
-    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
     GetEnabledStandardsPaginatorName,
@@ -364,32 +353,28 @@
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
-    ListSecurityControlDefinitionsPaginatorName,
-    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
-    RegionAvailabilityStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
-    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -421,15 +406,14 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardTypeDef,
     AvailabilityZoneTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
@@ -478,42 +462,14 @@
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
@@ -669,15 +625,14 @@
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
@@ -700,31 +655,22 @@
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
-    BatchGetSecurityControlsRequestRequestTypeDef,
-    SecurityControlTypeDef,
-    UnprocessedSecurityControlTypeDef,
-    StandardsControlAssociationIdTypeDef,
-    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     NoteUpdateTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
@@ -739,14 +685,15 @@
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
     DescribeStandardsRequestRequestTypeDef,
+    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
@@ -765,18 +712,14 @@
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestRequestTypeDef,
-    SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestRequestTypeDef,
-    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
@@ -785,15 +728,14 @@
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
-    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
@@ -820,19 +762,14 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -874,30 +811,26 @@
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
-    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeHubResponseTypeDef,
@@ -906,21 +839,16 @@
     GetFindingAggregatorResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
-    BatchGetSecurityControlsResponseTypeDef,
-    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
-    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
@@ -932,52 +860,47 @@
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
-    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
-    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
@@ -999,45 +922,35 @@
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
-    AwsWafv2ActionAllowDetailsTypeDef,
-    AwsWafv2RulesActionCaptchaDetailsTypeDef,
-    AwsWafv2RulesActionCountDetailsTypeDef,
-    AwsWafv2ActionBlockDetailsTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
-    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
-    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
-    AwsWafv2RulesActionDetailsTypeDef,
-    AwsWafv2WebAclActionDetailsTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -1047,23 +960,20 @@
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
-    AwsWafv2RulesDetailsTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
-    AwsWafv2RuleGroupDetailsTypeDef,
-    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.26.79/README.md` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,60 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-securityhub
+Version: 1.26.8
+Summary: Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,16 +290,14 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -293,38 +322,30 @@
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
-list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
-    client.get_paginator("list_security_control_definitions")
-)
-list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
-    client.get_paginator("list_standards_control_associations")
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
-    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
     GetEnabledStandardsPaginatorName,
@@ -332,32 +353,28 @@
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
-    ListSecurityControlDefinitionsPaginatorName,
-    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
-    RegionAvailabilityStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
-    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -389,15 +406,14 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardTypeDef,
     AvailabilityZoneTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
@@ -446,42 +462,14 @@
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
@@ -637,15 +625,14 @@
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
@@ -668,31 +655,22 @@
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
-    BatchGetSecurityControlsRequestRequestTypeDef,
-    SecurityControlTypeDef,
-    UnprocessedSecurityControlTypeDef,
-    StandardsControlAssociationIdTypeDef,
-    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     NoteUpdateTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
@@ -707,14 +685,15 @@
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
     DescribeStandardsRequestRequestTypeDef,
+    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
@@ -733,18 +712,14 @@
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestRequestTypeDef,
-    SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestRequestTypeDef,
-    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
@@ -753,15 +728,14 @@
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
-    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
@@ -788,19 +762,14 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -842,30 +811,26 @@
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
-    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeHubResponseTypeDef,
@@ -874,21 +839,16 @@
     GetFindingAggregatorResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
-    BatchGetSecurityControlsResponseTypeDef,
-    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
-    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
@@ -900,52 +860,47 @@
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
-    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
-    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
@@ -967,45 +922,35 @@
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
-    AwsWafv2ActionAllowDetailsTypeDef,
-    AwsWafv2RulesActionCaptchaDetailsTypeDef,
-    AwsWafv2RulesActionCountDetailsTypeDef,
-    AwsWafv2ActionBlockDetailsTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
-    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
-    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
-    AwsWafv2RulesActionDetailsTypeDef,
-    AwsWafv2WebAclActionDetailsTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -1015,23 +960,20 @@
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
-    AwsWafv2RulesDetailsTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
-    AwsWafv2RuleGroupDetailsTypeDef,
-    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,14 @@
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
-        ListSecurityControlDefinitionsPaginator,
-        ListStandardsControlAssociationsPaginator,
         SecurityHubClient,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
@@ -35,16 +33,14 @@
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
-    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
-    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from .client import SecurityHubClient
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
@@ -53,32 +49,27 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 
 Client = SecurityHubClient
 
-
 __all__ = (
     "Client",
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsControlsPaginator",
     "DescribeStandardsPaginator",
     "GetEnabledStandardsPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
-    "ListSecurityControlDefinitionsPaginator",
-    "ListStandardsControlAssociationsPaginator",
     "SecurityHubClient",
 )
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,14 @@
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
-        ListSecurityControlDefinitionsPaginator,
-        ListStandardsControlAssociationsPaginator,
         SecurityHubClient,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
@@ -35,16 +33,14 @@
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
-    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
-    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from .client import SecurityHubClient
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
     DescribeStandardsControlsPaginator,
@@ -53,31 +49,28 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 
 Client = SecurityHubClient
 
+
 __all__ = (
     "Client",
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
     "DescribeStandardsControlsPaginator",
     "DescribeStandardsPaginator",
     "GetEnabledStandardsPaginator",
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
-    "ListSecurityControlDefinitionsPaginator",
-    "ListStandardsControlAssociationsPaginator",
     "SecurityHubClient",
 )
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.26.79\nVersion:         1.26.79\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.26.8\nVersion:         1.26.8\nBuilder version:"
+        " 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.79")
+    print("1.26.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     RecordStateType,
     VerificationStateType,
 )
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
@@ -34,29 +33,24 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     AwsSecurityFindingTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
-    BatchGetSecurityControlsResponseTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateFindingsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
@@ -80,23 +74,19 @@
     GetMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
-    StandardsControlAssociationIdTypeDef,
-    StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -178,41 +168,19 @@
         """
         Enables the standards specified by the provided `StandardsArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_enable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_enable_standards)
         """
 
-    def batch_get_security_controls(
-        self, *, SecurityControlIds: Sequence[str]
-    ) -> BatchGetSecurityControlsResponseTypeDef:
-        """
-        Provides details about a batch of security controls for the current Amazon Web
-        Services account and Amazon Web Services Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_security_controls)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_security_controls)
-        """
-
-    def batch_get_standards_control_associations(
-        self, *, StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef]
-    ) -> BatchGetStandardsControlAssociationsResponseTypeDef:
-        """
-        For a batch of security controls and standards, identifies whether each control
-        is currently enabled or disabled in a standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
-        """
-
     def batch_import_findings(
         self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
-        Imports security findings generated by a finding provider into Security Hub.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
 
     def batch_update_findings(
         self,
@@ -225,34 +193,20 @@
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
         RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
-        Used by Security Hub customers to update information about their investigation
-        into a finding.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_findings)
         """
 
-    def batch_update_standards_control_associations(
-        self,
-        *,
-        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
-    ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
-        """
-        For a batch of security controls and standards, this operation updates the
-        enablement status of a control in a standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_standards_control_associations)
-        """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#can_paginate)
         """
@@ -481,19 +435,15 @@
         Designates the Security Hub administrator account for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_organization_admin_account)
         """
 
     def enable_security_hub(
-        self,
-        *,
-        Tags: Mapping[str, str] = ...,
-        EnableDefaultStandards: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        self, *, Tags: Mapping[str, str] = ..., EnableDefaultStandards: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_security_hub)
@@ -551,15 +501,15 @@
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
-        Returns a list of findings that match the specified criteria.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_findings)
         """
 
     def get_insight_results(self, *, InsightArn: str) -> GetInsightResultsResponseTypeDef:
         """
@@ -664,35 +614,14 @@
         """
         Lists the Security Hub administrator accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_organization_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_organization_admin_accounts)
         """
 
-    def list_security_control_definitions(
-        self, *, StandardsArn: str = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityControlDefinitionsResponseTypeDef:
-        """
-        Lists all of the security controls that apply to a specified standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_security_control_definitions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_security_control_definitions)
-        """
-
-    def list_standards_control_associations(
-        self, *, SecurityControlId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListStandardsControlAssociationsResponseTypeDef:
-        """
-        Specifies whether a control is currently enabled or disabled in each enabled
-        standard in the calling account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_standards_control_associations)
-        """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_tags_for_resource)
         """
@@ -769,18 +698,15 @@
         Used to update the configuration related to Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
 
     def update_security_hub_configuration(
-        self,
-        *,
-        AutoEnableControls: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        self, *, AutoEnableControls: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_hub_configuration)
         """
@@ -897,25 +823,7 @@
     def get_paginator(
         self, operation_name: Literal["list_organization_admin_accounts"]
     ) -> ListOrganizationAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
-
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_security_control_definitions"]
-    ) -> ListSecurityControlDefinitionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
-        """
-
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_standards_control_associations"]
-    ) -> ListStandardsControlAssociationsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
-        """
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoEnableStandardsType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     RecordStateType,
     VerificationStateType,
 )
 from .paginator import (
     DescribeActionTargetsPaginator,
     DescribeProductsPaginator,
@@ -34,29 +33,24 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 from .type_defs import (
     AccountDetailsTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
     AwsSecurityFindingTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
-    BatchGetSecurityControlsResponseTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateFindingsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
@@ -80,23 +74,19 @@
     GetMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     SortCriterionTypeDef,
-    StandardsControlAssociationIdTypeDef,
-    StandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionRequestTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     WorkflowUpdateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -169,39 +159,19 @@
     ) -> BatchEnableStandardsResponseTypeDef:
         """
         Enables the standards specified by the provided `StandardsArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_enable_standards)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_enable_standards)
         """
-    def batch_get_security_controls(
-        self, *, SecurityControlIds: Sequence[str]
-    ) -> BatchGetSecurityControlsResponseTypeDef:
-        """
-        Provides details about a batch of security controls for the current Amazon Web
-        Services account and Amazon Web Services Region.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_security_controls)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_security_controls)
-        """
-    def batch_get_standards_control_associations(
-        self, *, StandardsControlAssociationIds: Sequence[StandardsControlAssociationIdTypeDef]
-    ) -> BatchGetStandardsControlAssociationsResponseTypeDef:
-        """
-        For a batch of security controls and standards, identifies whether each control
-        is currently enabled or disabled in a standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_get_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_get_standards_control_associations)
-        """
     def batch_import_findings(
         self, *, Findings: Sequence[AwsSecurityFindingTypeDef]
     ) -> BatchImportFindingsResponseTypeDef:
         """
-        Imports security findings generated by a finding provider into Security Hub.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_import_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_import_findings)
         """
     def batch_update_findings(
         self,
         *,
@@ -213,32 +183,19 @@
         Criticality: int = ...,
         Types: Sequence[str] = ...,
         UserDefinedFields: Mapping[str, str] = ...,
         Workflow: WorkflowUpdateTypeDef = ...,
         RelatedFindings: Sequence[RelatedFindingTypeDef] = ...
     ) -> BatchUpdateFindingsResponseTypeDef:
         """
-        Used by Security Hub customers to update information about their investigation
-        into a finding.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_findings)
         """
-    def batch_update_standards_control_associations(
-        self,
-        *,
-        StandardsControlAssociationUpdates: Sequence[StandardsControlAssociationUpdateTypeDef]
-    ) -> BatchUpdateStandardsControlAssociationsResponseTypeDef:
-        """
-        For a batch of security controls and standards, this operation updates the
-        enablement status of a control in a standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.batch_update_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#batch_update_standards_control_associations)
-        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#can_paginate)
         """
@@ -441,19 +398,15 @@
         """
         Designates the Security Hub administrator account for an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_organization_admin_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_organization_admin_account)
         """
     def enable_security_hub(
-        self,
-        *,
-        Tags: Mapping[str, str] = ...,
-        EnableDefaultStandards: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        self, *, Tags: Mapping[str, str] = ..., EnableDefaultStandards: bool = ...
     ) -> Dict[str, Any]:
         """
         Enables Security Hub for your account in the current Region or the Region you
         specify in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.enable_security_hub)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#enable_security_hub)
@@ -506,15 +459,15 @@
         *,
         Filters: AwsSecurityFindingFiltersTypeDef = ...,
         SortCriteria: Sequence[SortCriterionTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetFindingsResponseTypeDef:
         """
-        Returns a list of findings that match the specified criteria.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_findings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_findings)
         """
     def get_insight_results(self, *, InsightArn: str) -> GetInsightResultsResponseTypeDef:
         """
         Lists the results of the Security Hub insight specified by the insight ARN.
@@ -607,33 +560,14 @@
     ) -> ListOrganizationAdminAccountsResponseTypeDef:
         """
         Lists the Security Hub administrator accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_organization_admin_accounts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_organization_admin_accounts)
         """
-    def list_security_control_definitions(
-        self, *, StandardsArn: str = ..., NextToken: str = ..., MaxResults: int = ...
-    ) -> ListSecurityControlDefinitionsResponseTypeDef:
-        """
-        Lists all of the security controls that apply to a specified standard.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_security_control_definitions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_security_control_definitions)
-        """
-    def list_standards_control_associations(
-        self, *, SecurityControlId: str, NextToken: str = ..., MaxResults: int = ...
-    ) -> ListStandardsControlAssociationsResponseTypeDef:
-        """
-        Specifies whether a control is currently enabled or disabled in each enabled
-        standard in the calling account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_standards_control_associations)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_standards_control_associations)
-        """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#list_tags_for_resource)
         """
@@ -702,18 +636,15 @@
         """
         Used to update the configuration related to Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_organization_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_organization_configuration)
         """
     def update_security_hub_configuration(
-        self,
-        *,
-        AutoEnableControls: bool = ...,
-        ControlFindingGenerator: ControlFindingGeneratorType = ...
+        self, *, AutoEnableControls: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates configuration options for Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.update_security_hub_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#update_security_hub_configuration)
         """
@@ -817,23 +748,7 @@
     def get_paginator(
         self, operation_name: Literal["list_organization_admin_accounts"]
     ) -> ListOrganizationAdminAccountsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
         """
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_security_control_definitions"]
-    ) -> ListSecurityControlDefinitionsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
-        """
-    @overload
-    def get_paginator(
-        self, operation_name: Literal["list_standards_control_associations"]
-    ) -> ListStandardsControlAssociationsPaginator:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Client.get_paginator)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/client/#get_paginator)
-        """
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,20 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdminStatusType",
-    "AssociationStatusType",
     "AutoEnableStandardsType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
     "ComplianceStatusType",
-    "ControlFindingGeneratorType",
     "ControlStatusType",
     "DateRangeUnitType",
     "DescribeActionTargetsPaginatorName",
     "DescribeProductsPaginatorName",
     "DescribeStandardsControlsPaginatorName",
     "DescribeStandardsPaginatorName",
     "GetEnabledStandardsPaginatorName",
@@ -38,51 +35,44 @@
     "GetInsightsPaginatorName",
     "IntegrationTypeType",
     "ListEnabledProductsForImportPaginatorName",
     "ListFindingAggregatorsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
-    "ListSecurityControlDefinitionsPaginatorName",
-    "ListStandardsControlAssociationsPaginatorName",
     "MalwareStateType",
     "MalwareTypeType",
     "MapFilterComparisonType",
     "NetworkDirectionType",
     "PartitionType",
     "RecordStateType",
-    "RegionAvailabilityStatusType",
     "SeverityLabelType",
     "SeverityRatingType",
     "SortOrderType",
     "StandardsStatusType",
     "StatusReasonCodeType",
     "StringFilterComparisonType",
     "ThreatIntelIndicatorCategoryType",
     "ThreatIntelIndicatorTypeType",
-    "UnprocessedErrorCodeType",
     "VerificationStateType",
     "VulnerabilityFixAvailableType",
     "WorkflowStateType",
     "WorkflowStatusType",
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
-AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
-ControlFindingGeneratorType = Literal["SECURITY_CONTROL", "STANDARD_CONTROL"]
 ControlStatusType = Literal["DISABLED", "ENABLED"]
 DateRangeUnitType = Literal["DAYS"]
 DescribeActionTargetsPaginatorName = Literal["describe_action_targets"]
 DescribeProductsPaginatorName = Literal["describe_products"]
 DescribeStandardsControlsPaginatorName = Literal["describe_standards_controls"]
 DescribeStandardsPaginatorName = Literal["describe_standards"]
 GetEnabledStandardsPaginatorName = Literal["get_enabled_standards"]
@@ -94,16 +84,14 @@
     "UPDATE_FINDINGS_IN_SECURITY_HUB",
 ]
 ListEnabledProductsForImportPaginatorName = Literal["list_enabled_products_for_import"]
 ListFindingAggregatorsPaginatorName = Literal["list_finding_aggregators"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
-ListSecurityControlDefinitionsPaginatorName = Literal["list_security_control_definitions"]
-ListStandardsControlAssociationsPaginatorName = Literal["list_standards_control_associations"]
 MalwareStateType = Literal["OBSERVED", "REMOVAL_FAILED", "REMOVED"]
 MalwareTypeType = Literal[
     "ADWARE",
     "BLENDED_THREAT",
     "BOTNET_AGENT",
     "COIN_MINER",
     "EXPLOIT_KIT",
@@ -118,15 +106,14 @@
     "VIRUS",
     "WORM",
 ]
 MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
-RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
 StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
 ThreatIntelIndicatorCategoryType = Literal[
@@ -141,15 +128,14 @@
     "HASH_SHA512",
     "IPV4_ADDRESS",
     "IPV6_ADDRESS",
     "MUTEX",
     "PROCESS",
     "URL",
 ]
-UnprocessedErrorCodeType = Literal["ACCESS_DENIED", "INVALID_INPUT", "LIMIT_EXCEEDED", "NOT_FOUND"]
 VerificationStateType = Literal["BENIGN_POSITIVE", "FALSE_POSITIVE", "TRUE_POSITIVE", "UNKNOWN"]
 VulnerabilityFixAvailableType = Literal["NO", "PARTIAL", "YES"]
 WorkflowStateType = Literal["ASSIGNED", "DEFERRED", "IN_PROGRESS", "NEW", "RESOLVED"]
 WorkflowStatusType = Literal["NEW", "NOTIFIED", "RESOLVED", "SUPPRESSED"]
 SecurityHubServiceName = Literal["securityhub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -171,15 +157,14 @@
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
@@ -189,31 +174,27 @@
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
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -242,15 +223,14 @@
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
@@ -298,15 +278,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -317,33 +296,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -375,32 +351,28 @@
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
     "outposts",
     "panorama",
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
@@ -428,58 +400,52 @@
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
     "scheduler",
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
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -514,16 +480,14 @@
     "get_findings",
     "get_insights",
     "list_enabled_products_for_import",
     "list_finding_aggregators",
     "list_invitations",
     "list_members",
     "list_organization_admin_accounts",
-    "list_security_control_definitions",
-    "list_standards_control_associations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -534,15 +498,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdminStatusType",
-    "AssociationStatusType",
     "AutoEnableStandardsType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
     "ComplianceStatusType",
-    "ControlFindingGeneratorType",
     "ControlStatusType",
     "DateRangeUnitType",
     "DescribeActionTargetsPaginatorName",
     "DescribeProductsPaginatorName",
     "DescribeStandardsControlsPaginatorName",
     "DescribeStandardsPaginatorName",
     "GetEnabledStandardsPaginatorName",
@@ -37,50 +36,45 @@
     "GetInsightsPaginatorName",
     "IntegrationTypeType",
     "ListEnabledProductsForImportPaginatorName",
     "ListFindingAggregatorsPaginatorName",
     "ListInvitationsPaginatorName",
     "ListMembersPaginatorName",
     "ListOrganizationAdminAccountsPaginatorName",
-    "ListSecurityControlDefinitionsPaginatorName",
-    "ListStandardsControlAssociationsPaginatorName",
     "MalwareStateType",
     "MalwareTypeType",
     "MapFilterComparisonType",
     "NetworkDirectionType",
     "PartitionType",
     "RecordStateType",
-    "RegionAvailabilityStatusType",
     "SeverityLabelType",
     "SeverityRatingType",
     "SortOrderType",
     "StandardsStatusType",
     "StatusReasonCodeType",
     "StringFilterComparisonType",
     "ThreatIntelIndicatorCategoryType",
     "ThreatIntelIndicatorTypeType",
-    "UnprocessedErrorCodeType",
     "VerificationStateType",
     "VulnerabilityFixAvailableType",
     "WorkflowStateType",
     "WorkflowStatusType",
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
-AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
-ControlFindingGeneratorType = Literal["SECURITY_CONTROL", "STANDARD_CONTROL"]
 ControlStatusType = Literal["DISABLED", "ENABLED"]
 DateRangeUnitType = Literal["DAYS"]
 DescribeActionTargetsPaginatorName = Literal["describe_action_targets"]
 DescribeProductsPaginatorName = Literal["describe_products"]
 DescribeStandardsControlsPaginatorName = Literal["describe_standards_controls"]
 DescribeStandardsPaginatorName = Literal["describe_standards"]
 GetEnabledStandardsPaginatorName = Literal["get_enabled_standards"]
@@ -92,16 +86,14 @@
     "UPDATE_FINDINGS_IN_SECURITY_HUB",
 ]
 ListEnabledProductsForImportPaginatorName = Literal["list_enabled_products_for_import"]
 ListFindingAggregatorsPaginatorName = Literal["list_finding_aggregators"]
 ListInvitationsPaginatorName = Literal["list_invitations"]
 ListMembersPaginatorName = Literal["list_members"]
 ListOrganizationAdminAccountsPaginatorName = Literal["list_organization_admin_accounts"]
-ListSecurityControlDefinitionsPaginatorName = Literal["list_security_control_definitions"]
-ListStandardsControlAssociationsPaginatorName = Literal["list_standards_control_associations"]
 MalwareStateType = Literal["OBSERVED", "REMOVAL_FAILED", "REMOVED"]
 MalwareTypeType = Literal[
     "ADWARE",
     "BLENDED_THREAT",
     "BOTNET_AGENT",
     "COIN_MINER",
     "EXPLOIT_KIT",
@@ -116,15 +108,14 @@
     "VIRUS",
     "WORM",
 ]
 MapFilterComparisonType = Literal["EQUALS", "NOT_EQUALS"]
 NetworkDirectionType = Literal["IN", "OUT"]
 PartitionType = Literal["aws", "aws-cn", "aws-us-gov"]
 RecordStateType = Literal["ACTIVE", "ARCHIVED"]
-RegionAvailabilityStatusType = Literal["AVAILABLE", "UNAVAILABLE"]
 SeverityLabelType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM"]
 SeverityRatingType = Literal["CRITICAL", "HIGH", "LOW", "MEDIUM"]
 SortOrderType = Literal["asc", "desc"]
 StandardsStatusType = Literal["DELETING", "FAILED", "INCOMPLETE", "PENDING", "READY"]
 StatusReasonCodeType = Literal["INTERNAL_ERROR", "NO_AVAILABLE_CONFIGURATION_RECORDER"]
 StringFilterComparisonType = Literal["EQUALS", "NOT_EQUALS", "PREFIX", "PREFIX_NOT_EQUALS"]
 ThreatIntelIndicatorCategoryType = Literal[
@@ -139,15 +130,14 @@
     "HASH_SHA512",
     "IPV4_ADDRESS",
     "IPV6_ADDRESS",
     "MUTEX",
     "PROCESS",
     "URL",
 ]
-UnprocessedErrorCodeType = Literal["ACCESS_DENIED", "INVALID_INPUT", "LIMIT_EXCEEDED", "NOT_FOUND"]
 VerificationStateType = Literal["BENIGN_POSITIVE", "FALSE_POSITIVE", "TRUE_POSITIVE", "UNKNOWN"]
 VulnerabilityFixAvailableType = Literal["NO", "PARTIAL", "YES"]
 WorkflowStateType = Literal["ASSIGNED", "DEFERRED", "IN_PROGRESS", "NEW", "RESOLVED"]
 WorkflowStatusType = Literal["NEW", "NOTIFIED", "RESOLVED", "SUPPRESSED"]
 SecurityHubServiceName = Literal["securityhub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -169,15 +159,14 @@
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
@@ -187,31 +176,27 @@
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
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -240,15 +225,14 @@
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
@@ -296,15 +280,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
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
@@ -315,33 +298,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -373,32 +353,28 @@
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
     "outposts",
     "panorama",
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
@@ -426,58 +402,52 @@
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
     "scheduler",
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
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -512,16 +482,14 @@
     "get_findings",
     "get_insights",
     "list_enabled_products_for_import",
     "list_finding_aggregators",
     "list_invitations",
     "list_members",
     "list_organization_admin_accounts",
-    "list_security_control_definitions",
-    "list_standards_control_associations",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
@@ -532,15 +500,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,14 @@
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
-        ListSecurityControlDefinitionsPaginator,
-        ListStandardsControlAssociationsPaginator,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
@@ -37,16 +35,14 @@
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
-    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
-    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
@@ -59,16 +55,14 @@
     GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
@@ -78,16 +72,14 @@
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
-    "ListSecurityControlDefinitionsPaginator",
-    "ListStandardsControlAssociationsPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -281,37 +273,7 @@
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
-
-
-class ListSecurityControlDefinitionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
-    """
-
-    def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
-        """
-
-
-class ListStandardsControlAssociationsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
-    """
-
-    def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
-        """
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,14 @@
         GetFindingsPaginator,
         GetInsightsPaginator,
         ListEnabledProductsForImportPaginator,
         ListFindingAggregatorsPaginator,
         ListInvitationsPaginator,
         ListMembersPaginator,
         ListOrganizationAdminAccountsPaginator,
-        ListSecurityControlDefinitionsPaginator,
-        ListStandardsControlAssociationsPaginator,
     )
 
     session = Session()
     client: SecurityHubClient = session.client("securityhub")
 
     describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
     describe_products_paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
@@ -37,16 +35,14 @@
     get_findings_paginator: GetFindingsPaginator = client.get_paginator("get_findings")
     get_insights_paginator: GetInsightsPaginator = client.get_paginator("get_insights")
     list_enabled_products_for_import_paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
     list_finding_aggregators_paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
     list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
     list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
     list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
-    list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = client.get_paginator("list_security_control_definitions")
-    list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = client.get_paginator("list_standards_control_associations")
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
@@ -59,16 +55,14 @@
     GetFindingsResponseTypeDef,
     GetInsightsResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     PaginatorConfigTypeDef,
     SortCriterionTypeDef,
 )
 
 __all__ = (
     "DescribeActionTargetsPaginator",
     "DescribeProductsPaginator",
@@ -78,16 +72,14 @@
     "GetFindingsPaginator",
     "GetInsightsPaginator",
     "ListEnabledProductsForImportPaginator",
     "ListFindingAggregatorsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
-    "ListSecurityControlDefinitionsPaginator",
-    "ListStandardsControlAssociationsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
@@ -267,35 +259,7 @@
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listorganizationadminaccountspaginator)
         """
-
-class ListSecurityControlDefinitionsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
-    """
-
-    def paginate(
-        self, *, StandardsArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListSecurityControlDefinitionsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListSecurityControlDefinitions.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#listsecuritycontroldefinitionspaginator)
-        """
-
-class ListStandardsControlAssociationsPaginator(Paginator):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations)
-    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
-    """
-
-    def paginate(
-        self, *, SecurityControlId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListStandardsControlAssociationsResponseTypeDef]:
-        """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListStandardsControlAssociations.paginate)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/paginators/#liststandardscontrolassociationspaginator)
-        """
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,38 +13,34 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
-    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     IntegrationTypeType,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
-    RegionAvailabilityStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
-    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
 )
 
 if sys.version_info >= (3, 9):
@@ -68,15 +64,14 @@
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
-    "AssociatedStandardTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationTypeDef",
@@ -125,42 +120,14 @@
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
@@ -316,15 +283,14 @@
     "AwsS3BucketLoggingConfigurationTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
@@ -347,31 +313,22 @@
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
-    "AwsWafv2CustomHttpHeaderTypeDef",
-    "AwsWafv2VisibilityConfigDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StandardsSubscriptionRequestTypeDef",
-    "BatchGetSecurityControlsRequestRequestTypeDef",
-    "SecurityControlTypeDef",
-    "UnprocessedSecurityControlTypeDef",
-    "StandardsControlAssociationIdTypeDef",
-    "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "NoteUpdateTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
-    "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
     "ResultTypeDef",
@@ -386,14 +343,15 @@
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
+    "StandardTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
@@ -412,18 +370,14 @@
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListSecurityControlDefinitionsRequestRequestTypeDef",
-    "SecurityControlDefinitionTypeDef",
-    "ListStandardsControlAssociationsRequestRequestTypeDef",
-    "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
     "RecommendationTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
@@ -432,15 +386,14 @@
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
-    "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
@@ -467,19 +420,14 @@
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
@@ -521,30 +469,26 @@
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
-    "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    "AwsWafv2CustomResponseDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
     "DeleteInsightResponseTypeDef",
     "DescribeActionTargetsResponseTypeDef",
     "DescribeHubResponseTypeDef",
@@ -553,21 +497,16 @@
     "GetFindingAggregatorResponseTypeDef",
     "GetInvitationsCountResponseTypeDef",
     "ListEnabledProductsForImportResponseTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateFindingAggregatorResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
-    "BatchGetSecurityControlsResponseTypeDef",
-    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
-    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
-    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
@@ -579,52 +518,47 @@
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
+    "DescribeStandardsResponseTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
-    "ListSecurityControlDefinitionsResponseTypeDef",
-    "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesTypeDef",
-    "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
-    "AwsEc2LaunchTemplateDataDetailsTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
@@ -646,45 +580,35 @@
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsTypeDef",
-    "AwsWafv2ActionAllowDetailsTypeDef",
-    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
-    "AwsWafv2RulesActionCountDetailsTypeDef",
-    "AwsWafv2ActionBlockDetailsTypeDef",
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
-    "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
-    "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
-    "AwsWafv2RulesActionDetailsTypeDef",
-    "AwsWafv2WebAclActionDetailsTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentTypeDef",
@@ -694,23 +618,20 @@
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
-    "AwsWafv2RulesDetailsTypeDef",
     "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
-    "AwsWafv2RuleGroupDetailsTypeDef",
-    "AwsWafv2WebAclDetailsTypeDef",
     "ClassificationResultTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
     "AwsS3BucketDetailsTypeDef",
     "DataClassificationDetailsTypeDef",
     "RuleGroupDetailsTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
@@ -852,22 +773,14 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
-AssociatedStandardTypeDef = TypedDict(
-    "AssociatedStandardTypeDef",
-    {
-        "StandardsId": str,
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
@@ -1437,275 +1350,14 @@
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "SnapshotId": str,
-        "Throughput": int,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    {
-        "CapacityReservationId": str,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    {
-        "CoreCount": int,
-        "ThreadsPerCore": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    {
-        "CpuCredits": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
-    {
-        "Count": int,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
-    {
-        "Configured": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
-    {
-        "AutoRecovery": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpTokens": str,
-        "HttpPutResponseHopLimit": int,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPlacementDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
-    {
-        "Affinity": str,
-        "AvailabilityZone": str,
-        "GroupName": str,
-        "HostId": str,
-        "HostResourceGroupArn": str,
-        "PartitionNumber": int,
-        "SpreadDomain": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    {
-        "EnableResourceNameDnsAAAARecord": bool,
-        "EnableResourceNameDnsARecord": bool,
-        "HostnameType": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "InstanceInterruptionBehavior": str,
-        "MaxPrice": str,
-        "SpotInstanceType": str,
-        "ValidUntil": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
-    {
-        "Ipv4Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
-    {
-        "Ipv6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
-    {
-        "Ipv6Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
-    {
-        "Primary": bool,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
@@ -3323,22 +2975,14 @@
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
-    {
-        "MinimumInstanceMetadataServiceVersion": str,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
@@ -3652,41 +3296,14 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
-    "AwsWafv2CustomHttpHeaderTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
-    "AwsWafv2VisibilityConfigDetailsTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-        "SampledRequestsEnabled": bool,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-    total=False,
-)
-
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
@@ -3728,94 +3345,14 @@
 
 class StandardsSubscriptionRequestTypeDef(
     _RequiredStandardsSubscriptionRequestTypeDef, _OptionalStandardsSubscriptionRequestTypeDef
 ):
     pass
 
 
-BatchGetSecurityControlsRequestRequestTypeDef = TypedDict(
-    "BatchGetSecurityControlsRequestRequestTypeDef",
-    {
-        "SecurityControlIds": Sequence[str],
-    },
-)
-
-SecurityControlTypeDef = TypedDict(
-    "SecurityControlTypeDef",
-    {
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "Title": str,
-        "Description": str,
-        "RemediationUrl": str,
-        "SeverityRating": SeverityRatingType,
-        "SecurityControlStatus": ControlStatusType,
-    },
-)
-
-_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
-    "_RequiredUnprocessedSecurityControlTypeDef",
-    {
-        "SecurityControlId": str,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
-    "_OptionalUnprocessedSecurityControlTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-
-class UnprocessedSecurityControlTypeDef(
-    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
-):
-    pass
-
-
-StandardsControlAssociationIdTypeDef = TypedDict(
-    "StandardsControlAssociationIdTypeDef",
-    {
-        "SecurityControlId": str,
-        "StandardsArn": str,
-    },
-)
-
-_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationDetailTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationDetailTypeDef",
-    {
-        "RelatedRequirements": List[str],
-        "UpdatedAt": datetime,
-        "UpdatedReason": str,
-        "StandardsControlTitle": str,
-        "StandardsControlDescription": str,
-        "StandardsControlArns": List[str],
-    },
-    total=False,
-)
-
-
-class StandardsControlAssociationDetailTypeDef(
-    _RequiredStandardsControlAssociationDetailTypeDef,
-    _OptionalStandardsControlAssociationDetailTypeDef,
-):
-    pass
-
-
 ImportFindingsErrorTypeDef = TypedDict(
     "ImportFindingsErrorTypeDef",
     {
         "Id": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -3843,38 +3380,14 @@
     "WorkflowUpdateTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-_RequiredStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationUpdateTypeDef",
-    {
-        "UpdatedReason": str,
-    },
-    total=False,
-)
-
-
-class StandardsControlAssociationUpdateTypeDef(
-    _RequiredStandardsControlAssociationUpdateTypeDef,
-    _OptionalStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
-
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
@@ -4119,14 +3632,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+StandardTypeDef = TypedDict(
+    "StandardTypeDef",
+    {
+        "StandardsArn": str,
+        "Name": str,
+        "Description": str,
+        "EnabledByDefault": bool,
+    },
+    total=False,
+)
+
 DisableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "DisableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductSubscriptionArn": str,
     },
 )
 
@@ -4159,15 +3683,14 @@
 )
 
 EnableSecurityHubRequestRequestTypeDef = TypedDict(
     "EnableSecurityHubRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
@@ -4345,88 +3868,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestRequestTypeDef",
-    {
-        "StandardsArn": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-SecurityControlDefinitionTypeDef = TypedDict(
-    "SecurityControlDefinitionTypeDef",
-    {
-        "SecurityControlId": str,
-        "Title": str,
-        "Description": str,
-        "RemediationUrl": str,
-        "SeverityRating": SeverityRatingType,
-        "CurrentRegionAvailability": RegionAvailabilityStatusType,
-    },
-)
-
-_RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListStandardsControlAssociationsRequestRequestTypeDef(
-    _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
-    _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationSummaryTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationSummaryTypeDef",
-    {
-        "RelatedRequirements": List[str],
-        "UpdatedAt": datetime,
-        "UpdatedReason": str,
-        "StandardsControlTitle": str,
-        "StandardsControlDescription": str,
-    },
-    total=False,
-)
-
-
-class StandardsControlAssociationSummaryTypeDef(
-    _RequiredStandardsControlAssociationSummaryTypeDef,
-    _OptionalStandardsControlAssociationSummaryTypeDef,
-):
-    pass
-
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -4566,25 +4015,14 @@
         "Epoch": str,
         "Release": str,
         "Architecture": str,
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
-        "SourceLayerHash": str,
-        "SourceLayerArn": str,
-    },
-    total=False,
-)
-
-StandardsManagedByTypeDef = TypedDict(
-    "StandardsManagedByTypeDef",
-    {
-        "Company": str,
-        "Product": str,
     },
     total=False,
 )
 
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
@@ -4684,15 +4122,14 @@
     pass
 
 
 UpdateSecurityHubConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     {
         "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 _RequiredUpdateStandardsControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStandardsControlRequestRequestTypeDef",
     {
@@ -5084,117 +4521,14 @@
         "NetworkInterfaces": Sequence[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-        "NoDevice": str,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    {
-        "CapacityReservationPreference": str,
-        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    {
-        "MarketType": str,
-        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    {
-        "AcceleratorCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
-        ),
-        "AcceleratorManufacturers": Sequence[str],
-        "AcceleratorNames": Sequence[str],
-        "AcceleratorTotalMemoryMiB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
-        ),
-        "AcceleratorTypes": Sequence[str],
-        "BareMetal": str,
-        "BaselineEbsBandwidthMbps": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
-        ),
-        "BurstablePerformance": str,
-        "CpuManufacturers": Sequence[str],
-        "ExcludedInstanceTypes": Sequence[str],
-        "InstanceGenerations": Sequence[str],
-        "LocalStorage": str,
-        "LocalStorageTypes": Sequence[str],
-        "MemoryGiBPerVCpu": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
-        ),
-        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
-        "NetworkInterfaceCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
-        ),
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "RequireHibernateSupport": bool,
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "TotalLocalStorageGB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
-        ),
-        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
-    {
-        "AssociateCarrierIpAddress": bool,
-        "AssociatePublicIpAddress": bool,
-        "DeleteOnTermination": bool,
-        "Description": str,
-        "DeviceIndex": int,
-        "Groups": Sequence[str],
-        "InterfaceType": str,
-        "Ipv4PrefixCount": int,
-        "Ipv4Prefixes": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef
-        ],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
-        ],
-        "Ipv6PrefixCount": int,
-        "Ipv6Prefixes": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef
-        ],
-        "NetworkCardIndex": int,
-        "NetworkInterfaceId": str,
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
-        ],
-        "SecondaryPrivateIpAddressCount": int,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
@@ -5338,17 +4672,15 @@
     total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
-        "LogConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
-        ),
+        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
         "Logging": str,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -5360,17 +4692,15 @@
     },
     total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
-        "DeploymentCircuitBreaker": (
-            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
-        ),
+        "DeploymentCircuitBreaker": AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
@@ -5380,17 +4710,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
-        "Capabilities": (
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
-        ),
+        "Capabilities": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
         "Devices": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef
         ],
         "InitProcessEnabled": bool,
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
@@ -5424,17 +4752,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
-        "AuthorizationConfig": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
-        ),
+        "AuthorizationConfig": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
@@ -5492,17 +4818,15 @@
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
         "InstanceType": str,
-        "ZoneAwarenessConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
-        ),
+        "ZoneAwarenessConfig": AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
@@ -5682,17 +5006,15 @@
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": (
-            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef
-        ),
+        "ZoneAwarenessConfig": AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
@@ -5873,43 +5195,14 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceDetailsTypeDef",
-    {
-        "AcceleratorTypes": Sequence[str],
-        "AdditionalCodeRepositories": Sequence[str],
-        "DefaultCodeRepository": str,
-        "DirectInternetAccess": str,
-        "FailureReason": str,
-        "InstanceMetadataServiceConfiguration": (
-            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
-        ),
-        "InstanceType": str,
-        "KmsKeyId": str,
-        "NetworkInterfaceId": str,
-        "NotebookInstanceArn": str,
-        "NotebookInstanceLifecycleConfigName": str,
-        "NotebookInstanceName": str,
-        "NotebookInstanceStatus": str,
-        "PlatformIdentifier": str,
-        "RoleArn": str,
-        "RootAccess": str,
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "Url": str,
-        "VolumeSizeInGB": int,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -6047,40 +5340,14 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    {
-        "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseCode": int,
-        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
-    {
-        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
-    },
-    total=False,
-)
-
 CreateActionTargetResponseTypeDef = TypedDict(
     "CreateActionTargetResponseTypeDef",
     {
         "ActionTargetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6131,15 +5398,14 @@
 
 DescribeHubResponseTypeDef = TypedDict(
     "DescribeHubResponseTypeDef",
     {
         "HubArn": str,
         "SubscribedAt": str,
         "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
@@ -6217,53 +5483,14 @@
 BatchEnableStandardsRequestRequestTypeDef = TypedDict(
     "BatchEnableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
     },
 )
 
-BatchGetSecurityControlsResponseTypeDef = TypedDict(
-    "BatchGetSecurityControlsResponseTypeDef",
-    {
-        "SecurityControls": List[SecurityControlTypeDef],
-        "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
-    },
-)
-
-_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-
-class UnprocessedStandardsControlAssociationTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationTypeDef,
-):
-    pass
-
-
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6296,52 +5523,20 @@
 class BatchUpdateFindingsRequestRequestTypeDef(
     _RequiredBatchUpdateFindingsRequestRequestTypeDef,
     _OptionalBatchUpdateFindingsRequestRequestTypeDef,
 ):
     pass
 
 
-BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
-    },
-)
-
-_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-
-class UnprocessedStandardsControlAssociationUpdateTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
-
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
-        "SecurityControlId": str,
-        "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
@@ -6509,45 +5704,14 @@
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    {
-        "StandardsArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
-    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-):
-    pass
-
-
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6558,14 +5722,23 @@
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeStandardsResponseTypeDef = TypedDict(
+    "DescribeStandardsResponseTypeDef",
+    {
+        "Standards": List[StandardTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
         "FilePaths": Sequence[FilePathsTypeDef],
@@ -6642,32 +5815,14 @@
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 
-ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsResponseTypeDef",
-    {
-        "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "ListStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
@@ -6740,26 +5895,14 @@
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
 )
 
-StandardTypeDef = TypedDict(
-    "StandardTypeDef",
-    {
-        "StandardsArn": str,
-        "Name": str,
-        "Description": str,
-        "EnabledByDefault": bool,
-        "StandardsManagedBy": StandardsManagedByTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -6849,20 +5992,16 @@
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
-        "InstancesDistribution": (
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
-        ),
-        "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
-        ),
+        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
+        "LaunchTemplate": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -6965,59 +6104,14 @@
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataDetailsTypeDef",
-    {
-        "BlockDeviceMappingSet": Sequence[
-            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
-        ],
-        "CapacityReservationSpecification": (
-            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
-        ),
-        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-        "DisableApiStop": bool,
-        "DisableApiTermination": bool,
-        "EbsOptimized": bool,
-        "ElasticGpuSpecificationSet": Sequence[
-            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
-        ],
-        "ElasticInferenceAcceleratorSet": Sequence[
-            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
-        ],
-        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
-        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
-        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
-        "ImageId": str,
-        "InstanceInitiatedShutdownBehavior": str,
-        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
-        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
-        "InstanceType": str,
-        "KernelId": str,
-        "KeyName": str,
-        "LicenseSet": Sequence[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
-        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
-        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
-        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
-        "NetworkInterfaceSet": Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef],
-        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
-        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-        "RamDiskId": str,
-        "SecurityGroupIdSet": Sequence[str],
-        "SecurityGroupSet": Sequence[str],
-        "UserData": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
@@ -7069,17 +6163,15 @@
     },
     total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
-        "ExecuteCommandConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
-        ),
+        "ExecuteCommandConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
@@ -7123,17 +6215,15 @@
         "EntryPoint": Sequence[str],
         "Environment": Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
         "ExtraHosts": Sequence[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
-        "FirelensConfiguration": (
-            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef
-        ),
+        "FirelensConfiguration": AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
         "Links": Sequence[str],
         "LinuxParameters": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
         "LogConfiguration": AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
@@ -7143,17 +6233,15 @@
         "Name": str,
         "PortMappings": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef
         ],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
-        "RepositoryCredentials": (
-            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
-        ),
+        "RepositoryCredentials": AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
         "ResourceRequirements": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
         "Secrets": Sequence[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": Sequence[
@@ -7166,17 +6254,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
-        "DockerVolumeConfiguration": (
-            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
-        ),
+        "DockerVolumeConfiguration": AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
@@ -7231,17 +6317,15 @@
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Mapping[str, str],
         "ElasticsearchVersion": str,
-        "ElasticsearchClusterConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
-        ),
+        "ElasticsearchClusterConfig": AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
         "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
@@ -7321,33 +6405,29 @@
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigTypeDef,
         "Version": str,
-        "Architectures": Sequence[str],
-        "PackageType": str,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
         "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
-        "NodeToNodeEncryptionOptions": (
-            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
-        ),
+        "NodeToNodeEncryptionOptions": AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
         "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
         "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
         "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
@@ -7517,63 +6597,14 @@
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
-AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
-    "AwsWafv2ActionAllowDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2RulesActionCaptchaDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionCountDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsTypeDef",
-    {
-        "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
-    },
-    total=False,
-)
-
-BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
-        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    {
-        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -7664,16 +6695,14 @@
         "FindingProviderFieldsCriticality": Sequence[NumberFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsId": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsProductArn": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityLabel": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityOriginal": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsTypes": Sequence[StringFilterTypeDef],
         "Sample": Sequence[BooleanFilterTypeDef],
-        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
-        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
@@ -7709,23 +6738,14 @@
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
-DescribeStandardsResponseTypeDef = TypedDict(
-    "DescribeStandardsResponseTypeDef",
-    {
-        "Standards": List[StandardTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7772,17 +6792,15 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
         "AvailabilityZones": Sequence[
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
-        "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
-        ),
+        "LaunchTemplate": AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
@@ -7864,26 +6882,14 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDetailsTypeDef",
-    {
-        "LaunchTemplateName": str,
-        "Id": str,
-        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
-        "DefaultVersionNumber": int,
-        "LatestVersionNumber": int,
-    },
-    total=False,
-)
-
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -7999,34 +7005,14 @@
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2RulesActionDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionDetailsTypeDef",
-    {
-        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
-        "Block": AwsWafv2ActionBlockDetailsTypeDef,
-        "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
-        "Count": AwsWafv2RulesActionCountDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclActionDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclActionDetailsTypeDef",
-    {
-        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
-        "Block": AwsWafv2ActionBlockDetailsTypeDef,
-    },
-    total=False,
-)
-
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -8208,17 +7194,15 @@
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
-        "AbortIncompleteMultipartUpload": (
-            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
-        ),
+        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": Sequence[
@@ -8237,26 +7221,14 @@
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
-AwsWafv2RulesDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesDetailsTypeDef",
-    {
-        "Action": AwsWafv2RulesActionDetailsTypeDef,
-        "Name": str,
-        "OverrideAction": str,
-        "Priority": int,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8310,46 +7282,14 @@
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
-AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
-    "AwsWafv2RuleGroupDetailsTypeDef",
-    {
-        "Capacity": int,
-        "Description": str,
-        "Id": str,
-        "Name": str,
-        "Arn": str,
-        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
-        "Scope": str,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclDetailsTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "ManagedbyFirewallManager": bool,
-        "Id": str,
-        "Capacity": int,
-        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
-        "DefaultAction": AwsWafv2WebAclActionDetailsTypeDef,
-        "Description": str,
-        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
@@ -8373,17 +7313,15 @@
 
 RuleGroupSourceTypeDef = TypedDict(
     "RuleGroupSourceTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsTypeDef,
         "RulesString": str,
         "StatefulRules": Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef],
-        "StatelessRulesAndCustomActions": (
-            RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
-        ),
+        "StatelessRulesAndCustomActions": RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -8513,18 +7451,14 @@
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsTypeDef,
         "AwsWafRule": AwsWafRuleDetailsTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsTypeDef,
         "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
-        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsTypeDef,
-        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsTypeDef,
-        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsTypeDef,
-        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -13,38 +13,34 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdminStatusType,
-    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     IntegrationTypeType,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
-    RegionAvailabilityStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
-    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
 )
 
 if sys.version_info >= (3, 9):
@@ -67,15 +63,14 @@
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
     "DnsRequestActionTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
-    "AssociatedStandardTypeDef",
     "AvailabilityZoneTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationTypeDef",
@@ -124,42 +119,14 @@
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     "AwsEc2EipDetailsTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
@@ -315,15 +282,14 @@
     "AwsS3BucketLoggingConfigurationTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     "AwsS3ObjectDetailsTypeDef",
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
@@ -346,31 +312,22 @@
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
-    "AwsWafv2CustomHttpHeaderTypeDef",
-    "AwsWafv2VisibilityConfigDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StandardsSubscriptionRequestTypeDef",
-    "BatchGetSecurityControlsRequestRequestTypeDef",
-    "SecurityControlTypeDef",
-    "UnprocessedSecurityControlTypeDef",
-    "StandardsControlAssociationIdTypeDef",
-    "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "NoteUpdateTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
-    "StandardsControlAssociationUpdateTypeDef",
     "CellTypeDef",
     "ClassificationStatusTypeDef",
     "StatusReasonTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
     "ResultTypeDef",
@@ -385,14 +342,15 @@
     "DescribeActionTargetsRequestRequestTypeDef",
     "DescribeHubRequestRequestTypeDef",
     "DescribeProductsRequestRequestTypeDef",
     "ProductTypeDef",
     "DescribeStandardsControlsRequestRequestTypeDef",
     "StandardsControlTypeDef",
     "DescribeStandardsRequestRequestTypeDef",
+    "StandardTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
     "FilePathsTypeDef",
@@ -411,18 +369,14 @@
     "InsightResultValueTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "ListEnabledProductsForImportRequestRequestTypeDef",
     "ListFindingAggregatorsRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListSecurityControlDefinitionsRequestRequestTypeDef",
-    "SecurityControlDefinitionTypeDef",
-    "ListStandardsControlAssociationsRequestRequestTypeDef",
-    "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PortRangeTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
     "RecommendationTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
@@ -431,15 +385,14 @@
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     "SoftwarePackageTypeDef",
-    "StandardsManagedByTypeDef",
     "StandardsStatusReasonTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
@@ -466,19 +419,14 @@
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
     "AwsEc2VolumeDetailsTypeDef",
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
@@ -520,30 +468,26 @@
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
-    "AwsSageMakerNotebookInstanceDetailsTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
     "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "AwsSnsTopicDetailsTypeDef",
     "AwsSsmPatchTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleTypeDef",
-    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    "AwsWafv2CustomResponseDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
     "DeleteInsightResponseTypeDef",
     "DescribeActionTargetsResponseTypeDef",
     "DescribeHubResponseTypeDef",
@@ -552,21 +496,16 @@
     "GetFindingAggregatorResponseTypeDef",
     "GetInvitationsCountResponseTypeDef",
     "ListEnabledProductsForImportResponseTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateFindingAggregatorResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
-    "BatchGetSecurityControlsResponseTypeDef",
-    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
-    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
-    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
@@ -578,52 +517,47 @@
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetInsightsRequestGetInsightsPaginateTypeDef",
     "ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef",
     "ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef",
     "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListMembersRequestListMembersPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    "ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
     "DescribeProductsResponseTypeDef",
     "DescribeStandardsControlsResponseTypeDef",
+    "DescribeStandardsResponseTypeDef",
     "ThreatTypeDef",
     "ListFindingAggregatorsResponseTypeDef",
     "FindingProviderFieldsTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
-    "ListSecurityControlDefinitionsResponseTypeDef",
-    "ListStandardsControlAssociationsResponseTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
     "PageTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesTypeDef",
-    "StandardTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     "AwsCloudFrontDistributionOriginItemTypeDef",
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     "AwsCodeBuildProjectDetailsTypeDef",
     "AwsDynamoDbTableReplicaTypeDef",
-    "AwsEc2LaunchTemplateDataDetailsTypeDef",
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
@@ -645,45 +579,35 @@
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsTypeDef",
-    "AwsWafv2ActionAllowDetailsTypeDef",
-    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
-    "AwsWafv2RulesActionCountDetailsTypeDef",
-    "AwsWafv2ActionBlockDetailsTypeDef",
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
-    "DescribeStandardsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
     "AwsCloudFrontDistributionOriginsTypeDef",
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     "AwsDynamoDbTableDetailsTypeDef",
-    "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
-    "AwsWafv2RulesActionDetailsTypeDef",
-    "AwsWafv2WebAclActionDetailsTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "InsightTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentTypeDef",
@@ -693,23 +617,20 @@
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     "RuleGroupSourceCustomActionsDetailsTypeDef",
     "ActionTypeDef",
     "AwsBackupBackupPlanDetailsTypeDef",
     "AwsCloudFrontDistributionDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
-    "AwsWafv2RulesDetailsTypeDef",
     "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
-    "AwsWafv2RuleGroupDetailsTypeDef",
-    "AwsWafv2WebAclDetailsTypeDef",
     "ClassificationResultTypeDef",
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     "RuleGroupSourceTypeDef",
     "AwsS3BucketDetailsTypeDef",
     "DataClassificationDetailsTypeDef",
     "RuleGroupDetailsTypeDef",
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
@@ -849,22 +770,14 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
-AssociatedStandardTypeDef = TypedDict(
-    "AssociatedStandardTypeDef",
-    {
-        "StandardsId": str,
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
@@ -1434,275 +1347,14 @@
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "SnapshotId": str,
-        "Throughput": int,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    {
-        "CapacityReservationId": str,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    {
-        "CoreCount": int,
-        "ThreadsPerCore": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    {
-        "CpuCredits": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
-    {
-        "Count": int,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
-    {
-        "Configured": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
-    {
-        "AutoRecovery": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpTokens": str,
-        "HttpPutResponseHopLimit": int,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPlacementDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
-    {
-        "Affinity": str,
-        "AvailabilityZone": str,
-        "GroupName": str,
-        "HostId": str,
-        "HostResourceGroupArn": str,
-        "PartitionNumber": int,
-        "SpreadDomain": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    {
-        "EnableResourceNameDnsAAAARecord": bool,
-        "EnableResourceNameDnsARecord": bool,
-        "HostnameType": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "InstanceInterruptionBehavior": str,
-        "MaxPrice": str,
-        "SpotInstanceType": str,
-        "ValidUntil": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
-    {
-        "Ipv4Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
-    {
-        "Ipv6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
-    {
-        "Ipv6Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
-    {
-        "Primary": bool,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
@@ -3320,22 +2972,14 @@
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
-    {
-        "MinimumInstanceMetadataServiceVersion": str,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
@@ -3645,41 +3289,14 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
-    "AwsWafv2CustomHttpHeaderTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
-    "AwsWafv2VisibilityConfigDetailsTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-        "SampledRequestsEnabled": bool,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-    total=False,
-)
-
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
@@ -3719,90 +3336,14 @@
 )
 
 class StandardsSubscriptionRequestTypeDef(
     _RequiredStandardsSubscriptionRequestTypeDef, _OptionalStandardsSubscriptionRequestTypeDef
 ):
     pass
 
-BatchGetSecurityControlsRequestRequestTypeDef = TypedDict(
-    "BatchGetSecurityControlsRequestRequestTypeDef",
-    {
-        "SecurityControlIds": Sequence[str],
-    },
-)
-
-SecurityControlTypeDef = TypedDict(
-    "SecurityControlTypeDef",
-    {
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "Title": str,
-        "Description": str,
-        "RemediationUrl": str,
-        "SeverityRating": SeverityRatingType,
-        "SecurityControlStatus": ControlStatusType,
-    },
-)
-
-_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
-    "_RequiredUnprocessedSecurityControlTypeDef",
-    {
-        "SecurityControlId": str,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
-    "_OptionalUnprocessedSecurityControlTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-class UnprocessedSecurityControlTypeDef(
-    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
-):
-    pass
-
-StandardsControlAssociationIdTypeDef = TypedDict(
-    "StandardsControlAssociationIdTypeDef",
-    {
-        "SecurityControlId": str,
-        "StandardsArn": str,
-    },
-)
-
-_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationDetailTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationDetailTypeDef",
-    {
-        "RelatedRequirements": List[str],
-        "UpdatedAt": datetime,
-        "UpdatedReason": str,
-        "StandardsControlTitle": str,
-        "StandardsControlDescription": str,
-        "StandardsControlArns": List[str],
-    },
-    total=False,
-)
-
-class StandardsControlAssociationDetailTypeDef(
-    _RequiredStandardsControlAssociationDetailTypeDef,
-    _OptionalStandardsControlAssociationDetailTypeDef,
-):
-    pass
-
 ImportFindingsErrorTypeDef = TypedDict(
     "ImportFindingsErrorTypeDef",
     {
         "Id": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -3830,36 +3371,14 @@
     "WorkflowUpdateTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-_RequiredStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationUpdateTypeDef",
-    {
-        "UpdatedReason": str,
-    },
-    total=False,
-)
-
-class StandardsControlAssociationUpdateTypeDef(
-    _RequiredStandardsControlAssociationUpdateTypeDef,
-    _OptionalStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
@@ -4096,14 +3615,25 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+StandardTypeDef = TypedDict(
+    "StandardTypeDef",
+    {
+        "StandardsArn": str,
+        "Name": str,
+        "Description": str,
+        "EnabledByDefault": bool,
+    },
+    total=False,
+)
+
 DisableImportFindingsForProductRequestRequestTypeDef = TypedDict(
     "DisableImportFindingsForProductRequestRequestTypeDef",
     {
         "ProductSubscriptionArn": str,
     },
 )
 
@@ -4136,15 +3666,14 @@
 )
 
 EnableSecurityHubRequestRequestTypeDef = TypedDict(
     "EnableSecurityHubRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
@@ -4322,84 +3851,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestRequestTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestRequestTypeDef",
-    {
-        "StandardsArn": str,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-SecurityControlDefinitionTypeDef = TypedDict(
-    "SecurityControlDefinitionTypeDef",
-    {
-        "SecurityControlId": str,
-        "Title": str,
-        "Description": str,
-        "RemediationUrl": str,
-        "SeverityRating": SeverityRatingType,
-        "CurrentRegionAvailability": RegionAvailabilityStatusType,
-    },
-)
-
-_RequiredListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListStandardsControlAssociationsRequestRequestTypeDef(
-    _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
-    _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationSummaryTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "SecurityControlArn": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationSummaryTypeDef",
-    {
-        "RelatedRequirements": List[str],
-        "UpdatedAt": datetime,
-        "UpdatedReason": str,
-        "StandardsControlTitle": str,
-        "StandardsControlDescription": str,
-    },
-    total=False,
-)
-
-class StandardsControlAssociationSummaryTypeDef(
-    _RequiredStandardsControlAssociationSummaryTypeDef,
-    _OptionalStandardsControlAssociationSummaryTypeDef,
-):
-    pass
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -4539,25 +3998,14 @@
         "Epoch": str,
         "Release": str,
         "Architecture": str,
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
-        "SourceLayerHash": str,
-        "SourceLayerArn": str,
-    },
-    total=False,
-)
-
-StandardsManagedByTypeDef = TypedDict(
-    "StandardsManagedByTypeDef",
-    {
-        "Company": str,
-        "Product": str,
     },
     total=False,
 )
 
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
@@ -4651,15 +4099,14 @@
 ):
     pass
 
 UpdateSecurityHubConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     {
         "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
 _RequiredUpdateStandardsControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStandardsControlRequestRequestTypeDef",
     {
@@ -5047,117 +4494,14 @@
         "NetworkInterfaces": Sequence[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-        "NoDevice": str,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    {
-        "CapacityReservationPreference": str,
-        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
-    {
-        "MarketType": str,
-        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
-    {
-        "AcceleratorCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
-        ),
-        "AcceleratorManufacturers": Sequence[str],
-        "AcceleratorNames": Sequence[str],
-        "AcceleratorTotalMemoryMiB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
-        ),
-        "AcceleratorTypes": Sequence[str],
-        "BareMetal": str,
-        "BaselineEbsBandwidthMbps": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
-        ),
-        "BurstablePerformance": str,
-        "CpuManufacturers": Sequence[str],
-        "ExcludedInstanceTypes": Sequence[str],
-        "InstanceGenerations": Sequence[str],
-        "LocalStorage": str,
-        "LocalStorageTypes": Sequence[str],
-        "MemoryGiBPerVCpu": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
-        ),
-        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
-        "NetworkInterfaceCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
-        ),
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "RequireHibernateSupport": bool,
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "TotalLocalStorageGB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
-        ),
-        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
-    {
-        "AssociateCarrierIpAddress": bool,
-        "AssociatePublicIpAddress": bool,
-        "DeleteOnTermination": bool,
-        "Description": str,
-        "DeviceIndex": int,
-        "Groups": Sequence[str],
-        "InterfaceType": str,
-        "Ipv4PrefixCount": int,
-        "Ipv4Prefixes": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef
-        ],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
-        ],
-        "Ipv6PrefixCount": int,
-        "Ipv6Prefixes": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef
-        ],
-        "NetworkCardIndex": int,
-        "NetworkInterfaceId": str,
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
-        ],
-        "SecondaryPrivateIpAddressCount": int,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
@@ -5301,17 +4645,15 @@
     total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
-        "LogConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
-        ),
+        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
         "Logging": str,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -5323,17 +4665,15 @@
     },
     total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
-        "DeploymentCircuitBreaker": (
-            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
-        ),
+        "DeploymentCircuitBreaker": AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
     total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
@@ -5343,17 +4683,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
-        "Capabilities": (
-            AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
-        ),
+        "Capabilities": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
         "Devices": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef
         ],
         "InitProcessEnabled": bool,
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
@@ -5387,17 +4725,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
-        "AuthorizationConfig": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
-        ),
+        "AuthorizationConfig": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
@@ -5455,17 +4791,15 @@
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
         "InstanceType": str,
-        "ZoneAwarenessConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
-        ),
+        "ZoneAwarenessConfig": AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
@@ -5645,17 +4979,15 @@
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": (
-            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef
-        ),
+        "ZoneAwarenessConfig": AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
@@ -5836,43 +5168,14 @@
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceDetailsTypeDef",
-    {
-        "AcceleratorTypes": Sequence[str],
-        "AdditionalCodeRepositories": Sequence[str],
-        "DefaultCodeRepository": str,
-        "DirectInternetAccess": str,
-        "FailureReason": str,
-        "InstanceMetadataServiceConfiguration": (
-            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
-        ),
-        "InstanceType": str,
-        "KmsKeyId": str,
-        "NetworkInterfaceId": str,
-        "NotebookInstanceArn": str,
-        "NotebookInstanceLifecycleConfigName": str,
-        "NotebookInstanceName": str,
-        "NotebookInstanceStatus": str,
-        "PlatformIdentifier": str,
-        "RoleArn": str,
-        "RootAccess": str,
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "Url": str,
-        "VolumeSizeInGB": int,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -6010,40 +5313,14 @@
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomRequestHandlingDetailsTypeDef",
-    {
-        "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseCode": int,
-        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
-    {
-        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
-    },
-    total=False,
-)
-
 CreateActionTargetResponseTypeDef = TypedDict(
     "CreateActionTargetResponseTypeDef",
     {
         "ActionTargetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6094,15 +5371,14 @@
 
 DescribeHubResponseTypeDef = TypedDict(
     "DescribeHubResponseTypeDef",
     {
         "HubArn": str,
         "SubscribedAt": str,
         "AutoEnableControls": bool,
-        "ControlFindingGenerator": ControlFindingGeneratorType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
@@ -6180,51 +5456,14 @@
 BatchEnableStandardsRequestRequestTypeDef = TypedDict(
     "BatchEnableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionRequests": Sequence[StandardsSubscriptionRequestTypeDef],
     },
 )
 
-BatchGetSecurityControlsResponseTypeDef = TypedDict(
-    "BatchGetSecurityControlsResponseTypeDef",
-    {
-        "SecurityControls": List[SecurityControlTypeDef],
-        "UnprocessedIds": List[UnprocessedSecurityControlTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
-    },
-)
-
-_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-class UnprocessedStandardsControlAssociationTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationTypeDef,
-):
-    pass
-
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -6255,50 +5494,20 @@
 
 class BatchUpdateFindingsRequestRequestTypeDef(
     _RequiredBatchUpdateFindingsRequestRequestTypeDef,
     _OptionalBatchUpdateFindingsRequestRequestTypeDef,
 ):
     pass
 
-BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
-    {
-        "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
-    },
-)
-
-_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-class UnprocessedStandardsControlAssociationUpdateTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
         "StatusReasons": Sequence[StatusReasonTypeDef],
-        "SecurityControlId": str,
-        "AssociatedStandards": Sequence[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
@@ -6464,43 +5673,14 @@
     "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef",
-    {
-        "StandardsArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "SecurityControlId": str,
-    },
-)
-_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef(
-    _RequiredListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-    _OptionalListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
-):
-    pass
-
 DescribeProductsResponseTypeDef = TypedDict(
     "DescribeProductsResponseTypeDef",
     {
         "Products": List[ProductTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6511,14 +5691,23 @@
     {
         "Controls": List[StandardsControlTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeStandardsResponseTypeDef = TypedDict(
+    "DescribeStandardsResponseTypeDef",
+    {
+        "Standards": List[StandardTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
         "FilePaths": Sequence[FilePathsTypeDef],
@@ -6595,32 +5784,14 @@
     {
         "InsightArn": str,
         "GroupByAttribute": str,
         "ResultValues": List[InsightResultValueTypeDef],
     },
 )
 
-ListSecurityControlDefinitionsResponseTypeDef = TypedDict(
-    "ListSecurityControlDefinitionsResponseTypeDef",
-    {
-        "SecurityControlDefinitions": List[SecurityControlDefinitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "ListStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
     },
     total=False,
@@ -6693,26 +5864,14 @@
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
     },
     total=False,
 )
 
-StandardTypeDef = TypedDict(
-    "StandardTypeDef",
-    {
-        "StandardsArn": str,
-        "Name": str,
-        "Description": str,
-        "EnabledByDefault": bool,
-        "StandardsManagedBy": StandardsManagedByTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -6798,20 +5957,16 @@
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
-        "InstancesDistribution": (
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
-        ),
-        "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef
-        ),
+        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
+        "LaunchTemplate": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -6914,59 +6069,14 @@
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataDetailsTypeDef",
-    {
-        "BlockDeviceMappingSet": Sequence[
-            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
-        ],
-        "CapacityReservationSpecification": (
-            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
-        ),
-        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-        "DisableApiStop": bool,
-        "DisableApiTermination": bool,
-        "EbsOptimized": bool,
-        "ElasticGpuSpecificationSet": Sequence[
-            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
-        ],
-        "ElasticInferenceAcceleratorSet": Sequence[
-            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
-        ],
-        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
-        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
-        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
-        "ImageId": str,
-        "InstanceInitiatedShutdownBehavior": str,
-        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
-        "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
-        "InstanceType": str,
-        "KernelId": str,
-        "KeyName": str,
-        "LicenseSet": Sequence[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
-        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
-        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
-        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
-        "NetworkInterfaceSet": Sequence[AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef],
-        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
-        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-        "RamDiskId": str,
-        "SecurityGroupIdSet": Sequence[str],
-        "SecurityGroupSet": Sequence[str],
-        "UserData": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
@@ -7018,17 +6128,15 @@
     },
     total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
-        "ExecuteCommandConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
-        ),
+        "ExecuteCommandConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
@@ -7072,17 +6180,15 @@
         "EntryPoint": Sequence[str],
         "Environment": Sequence[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
         "ExtraHosts": Sequence[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
-        "FirelensConfiguration": (
-            AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef
-        ),
+        "FirelensConfiguration": AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
         "Links": Sequence[str],
         "LinuxParameters": AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
         "LogConfiguration": AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
@@ -7092,17 +6198,15 @@
         "Name": str,
         "PortMappings": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef
         ],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
-        "RepositoryCredentials": (
-            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
-        ),
+        "RepositoryCredentials": AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
         "ResourceRequirements": Sequence[
             AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
         "Secrets": Sequence[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": Sequence[
@@ -7115,17 +6219,15 @@
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
-        "DockerVolumeConfiguration": (
-            AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
-        ),
+        "DockerVolumeConfiguration": AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
         "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
@@ -7180,17 +6282,15 @@
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Mapping[str, str],
         "ElasticsearchVersion": str,
-        "ElasticsearchClusterConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
-        ),
+        "ElasticsearchClusterConfig": AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
         "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
         "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsTypeDef,
     },
     total=False,
@@ -7270,33 +6370,29 @@
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigTypeDef,
         "Version": str,
-        "Architectures": Sequence[str],
-        "PackageType": str,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
         "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
-        "NodeToNodeEncryptionOptions": (
-            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
-        ),
+        "NodeToNodeEncryptionOptions": AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
         "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
         "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
         "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Mapping[str, str],
         "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
@@ -7466,63 +6562,14 @@
         "DefaultAction": str,
         "Rules": Sequence[AwsWafWebAclRuleTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
-AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
-    "AwsWafv2ActionAllowDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2RulesActionCaptchaDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionCaptchaDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2RulesActionCountDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionCountDetailsTypeDef",
-    {
-        "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsTypeDef",
-    {
-        "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
-    },
-    total=False,
-)
-
-BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
-        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    {
-        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -7613,16 +6660,14 @@
         "FindingProviderFieldsCriticality": Sequence[NumberFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsId": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsRelatedFindingsProductArn": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityLabel": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsSeverityOriginal": Sequence[StringFilterTypeDef],
         "FindingProviderFieldsTypes": Sequence[StringFilterTypeDef],
         "Sample": Sequence[BooleanFilterTypeDef],
-        "ComplianceSecurityControlId": Sequence[StringFilterTypeDef],
-        "ComplianceAssociatedStandardsId": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
 GetInsightResultsResponseTypeDef = TypedDict(
     "GetInsightResultsResponseTypeDef",
     {
@@ -7658,23 +6703,14 @@
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     },
     total=False,
 )
 
-DescribeStandardsResponseTypeDef = TypedDict(
-    "DescribeStandardsResponseTypeDef",
-    {
-        "Standards": List[StandardTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7721,17 +6757,15 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
         "AvailabilityZones": Sequence[
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
-        "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
-        ),
+        "LaunchTemplate": AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
@@ -7813,26 +6847,14 @@
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDetailsTypeDef",
-    {
-        "LaunchTemplateName": str,
-        "Id": str,
-        "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsTypeDef,
-        "DefaultVersionNumber": int,
-        "LatestVersionNumber": int,
-    },
-    total=False,
-)
-
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": Sequence[str],
         "ClusterSettings": Sequence[AwsEcsClusterClusterSettingsDetailsTypeDef],
@@ -7948,34 +6970,14 @@
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
         "Destination": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2RulesActionDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesActionDetailsTypeDef",
-    {
-        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
-        "Block": AwsWafv2ActionBlockDetailsTypeDef,
-        "Captcha": AwsWafv2RulesActionCaptchaDetailsTypeDef,
-        "Count": AwsWafv2RulesActionCountDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclActionDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclActionDetailsTypeDef",
-    {
-        "Allow": AwsWafv2ActionAllowDetailsTypeDef,
-        "Block": AwsWafv2ActionBlockDetailsTypeDef,
-    },
-    total=False,
-)
-
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -8153,17 +7155,15 @@
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
-        "AbortIncompleteMultipartUpload": (
-            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
-        ),
+        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": Sequence[
@@ -8182,26 +7182,14 @@
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
     total=False,
 )
 
-AwsWafv2RulesDetailsTypeDef = TypedDict(
-    "AwsWafv2RulesDetailsTypeDef",
-    {
-        "Action": AwsWafv2RulesActionDetailsTypeDef,
-        "Name": str,
-        "OverrideAction": str,
-        "Priority": int,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -8255,46 +7243,14 @@
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
     total=False,
 )
 
-AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
-    "AwsWafv2RuleGroupDetailsTypeDef",
-    {
-        "Capacity": int,
-        "Description": str,
-        "Id": str,
-        "Name": str,
-        "Arn": str,
-        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
-        "Scope": str,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
-AwsWafv2WebAclDetailsTypeDef = TypedDict(
-    "AwsWafv2WebAclDetailsTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "ManagedbyFirewallManager": bool,
-        "Id": str,
-        "Capacity": int,
-        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
-        "DefaultAction": AwsWafv2WebAclActionDetailsTypeDef,
-        "Description": str,
-        "Rules": Sequence[AwsWafv2RulesDetailsTypeDef],
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
-    },
-    total=False,
-)
-
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusTypeDef,
@@ -8318,17 +7274,15 @@
 
 RuleGroupSourceTypeDef = TypedDict(
     "RuleGroupSourceTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsTypeDef,
         "RulesString": str,
         "StatefulRules": Sequence[RuleGroupSourceStatefulRulesDetailsTypeDef],
-        "StatelessRulesAndCustomActions": (
-            RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef
-        ),
+        "StatelessRulesAndCustomActions": RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -8458,18 +7412,14 @@
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsTypeDef,
         "AwsWafRule": AwsWafRuleDetailsTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsTypeDef,
         "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
-        "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsTypeDef,
-        "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsTypeDef,
-        "AwsWafv2WebAcl": AwsWafv2WebAclDetailsTypeDef,
-        "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.26.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-securityhub
-Version: 1.26.79
-Summary: Type annotations for boto3.SecurityHub 1.26.79 service generated with mypy-boto3-builder 7.12.4
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,16 +259,14 @@
     GetFindingsPaginator,
     GetInsightsPaginator,
     ListEnabledProductsForImportPaginator,
     ListFindingAggregatorsPaginator,
     ListInvitationsPaginator,
     ListMembersPaginator,
     ListOrganizationAdminAccountsPaginator,
-    ListSecurityControlDefinitionsPaginator,
-    ListStandardsControlAssociationsPaginator,
 )
 
 client: SecurityHubClient = Session().client("securityhub")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 describe_action_targets_paginator: DescribeActionTargetsPaginator = client.get_paginator(
@@ -325,38 +291,30 @@
     "list_finding_aggregators"
 )
 list_invitations_paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
 list_members_paginator: ListMembersPaginator = client.get_paginator("list_members")
 list_organization_admin_accounts_paginator: ListOrganizationAdminAccountsPaginator = (
     client.get_paginator("list_organization_admin_accounts")
 )
-list_security_control_definitions_paginator: ListSecurityControlDefinitionsPaginator = (
-    client.get_paginator("list_security_control_definitions")
-)
-list_standards_control_associations_paginator: ListStandardsControlAssociationsPaginator = (
-    client.get_paginator("list_standards_control_associations")
-)
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_securityhub.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_securityhub.literals import (
     AdminStatusType,
-    AssociationStatusType,
     AutoEnableStandardsType,
     AwsIamAccessKeyStatusType,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
     ComplianceStatusType,
-    ControlFindingGeneratorType,
     ControlStatusType,
     DateRangeUnitType,
     DescribeActionTargetsPaginatorName,
     DescribeProductsPaginatorName,
     DescribeStandardsControlsPaginatorName,
     DescribeStandardsPaginatorName,
     GetEnabledStandardsPaginatorName,
@@ -364,32 +322,28 @@
     GetInsightsPaginatorName,
     IntegrationTypeType,
     ListEnabledProductsForImportPaginatorName,
     ListFindingAggregatorsPaginatorName,
     ListInvitationsPaginatorName,
     ListMembersPaginatorName,
     ListOrganizationAdminAccountsPaginatorName,
-    ListSecurityControlDefinitionsPaginatorName,
-    ListStandardsControlAssociationsPaginatorName,
     MalwareStateType,
     MalwareTypeType,
     MapFilterComparisonType,
     NetworkDirectionType,
     PartitionType,
     RecordStateType,
-    RegionAvailabilityStatusType,
     SeverityLabelType,
     SeverityRatingType,
     SortOrderType,
     StandardsStatusType,
     StatusReasonCodeType,
     StringFilterComparisonType,
     ThreatIntelIndicatorCategoryType,
     ThreatIntelIndicatorTypeType,
-    UnprocessedErrorCodeType,
     VerificationStateType,
     VulnerabilityFixAvailableType,
     WorkflowStateType,
     WorkflowStatusType,
     SecurityHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -421,15 +375,14 @@
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
     DnsRequestActionTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardTypeDef,
     AvailabilityZoneTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationTypeDef,
@@ -478,42 +431,14 @@
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     AwsEc2EipDetailsTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
@@ -669,15 +594,14 @@
     AwsS3BucketLoggingConfigurationTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
@@ -700,31 +624,22 @@
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StandardsSubscriptionRequestTypeDef,
-    BatchGetSecurityControlsRequestRequestTypeDef,
-    SecurityControlTypeDef,
-    UnprocessedSecurityControlTypeDef,
-    StandardsControlAssociationIdTypeDef,
-    StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     NoteUpdateTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    StandardsControlAssociationUpdateTypeDef,
     CellTypeDef,
     ClassificationStatusTypeDef,
     StatusReasonTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
@@ -739,14 +654,15 @@
     DescribeActionTargetsRequestRequestTypeDef,
     DescribeHubRequestRequestTypeDef,
     DescribeProductsRequestRequestTypeDef,
     ProductTypeDef,
     DescribeStandardsControlsRequestRequestTypeDef,
     StandardsControlTypeDef,
     DescribeStandardsRequestRequestTypeDef,
+    StandardTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
     FilePathsTypeDef,
@@ -765,18 +681,14 @@
     InsightResultValueTypeDef,
     InviteMembersRequestRequestTypeDef,
     ListEnabledProductsForImportRequestRequestTypeDef,
     ListFindingAggregatorsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListSecurityControlDefinitionsRequestRequestTypeDef,
-    SecurityControlDefinitionTypeDef,
-    ListStandardsControlAssociationsRequestRequestTypeDef,
-    StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PortRangeTypeDef,
     RangeTypeDef,
     RecordTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
@@ -785,15 +697,14 @@
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
     SoftwarePackageTypeDef,
-    StandardsManagedByTypeDef,
     StandardsStatusReasonTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
@@ -820,19 +731,14 @@
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsTypeDef,
     AwsEc2VolumeDetailsTypeDef,
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
@@ -874,30 +780,26 @@
     AwsRdsDbSecurityGroupDetailsTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
-    AwsSageMakerNotebookInstanceDetailsTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
     BatchUpdateFindingsUnprocessedFindingTypeDef,
     AwsSnsTopicDetailsTypeDef,
     AwsSsmPatchTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleTypeDef,
-    AwsWafv2CustomRequestHandlingDetailsTypeDef,
-    AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
     DescribeActionTargetsResponseTypeDef,
     DescribeHubResponseTypeDef,
@@ -906,21 +808,16 @@
     GetFindingAggregatorResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
     ListEnabledProductsForImportResponseTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
-    BatchGetSecurityControlsResponseTypeDef,
-    BatchGetStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
-    BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
@@ -932,52 +829,47 @@
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetInsightsRequestGetInsightsPaginateTypeDef,
     ListEnabledProductsForImportRequestListEnabledProductsForImportPaginateTypeDef,
     ListFindingAggregatorsRequestListFindingAggregatorsPaginateTypeDef,
     ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListMembersRequestListMembersPaginateTypeDef,
     ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
-    ListSecurityControlDefinitionsRequestListSecurityControlDefinitionsPaginateTypeDef,
-    ListStandardsControlAssociationsRequestListStandardsControlAssociationsPaginateTypeDef,
     DescribeProductsResponseTypeDef,
     DescribeStandardsControlsResponseTypeDef,
+    DescribeStandardsResponseTypeDef,
     ThreatTypeDef,
     ListFindingAggregatorsResponseTypeDef,
     FindingProviderFieldsTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
-    ListSecurityControlDefinitionsResponseTypeDef,
-    ListStandardsControlAssociationsResponseTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
     PageTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesTypeDef,
-    StandardTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
     AwsCertificateManagerCertificateRenewalSummaryTypeDef,
     AwsCloudFrontDistributionOriginItemTypeDef,
     AwsCloudFrontDistributionOriginGroupTypeDef,
     AwsCodeBuildProjectDetailsTypeDef,
     AwsDynamoDbTableReplicaTypeDef,
-    AwsEc2LaunchTemplateDataDetailsTypeDef,
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
@@ -999,45 +891,35 @@
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsTypeDef,
-    AwsWafv2ActionAllowDetailsTypeDef,
-    AwsWafv2RulesActionCaptchaDetailsTypeDef,
-    AwsWafv2RulesActionCountDetailsTypeDef,
-    AwsWafv2ActionBlockDetailsTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
-    DescribeStandardsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
     AwsCloudFrontDistributionOriginsTypeDef,
     AwsCloudFrontDistributionOriginGroupsTypeDef,
     AwsDynamoDbTableDetailsTypeDef,
-    AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
-    AwsWafv2RulesActionDetailsTypeDef,
-    AwsWafv2WebAclActionDetailsTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     InsightTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentTypeDef,
@@ -1047,23 +929,20 @@
     FirewallPolicyStatelessCustomActionsDetailsTypeDef,
     RuleGroupSourceCustomActionsDetailsTypeDef,
     ActionTypeDef,
     AwsBackupBackupPlanDetailsTypeDef,
     AwsCloudFrontDistributionDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
-    AwsWafv2RulesDetailsTypeDef,
     GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef,
-    AwsWafv2RuleGroupDetailsTypeDef,
-    AwsWafv2WebAclDetailsTypeDef,
     ClassificationResultTypeDef,
     AwsNetworkFirewallFirewallPolicyDetailsTypeDef,
     RuleGroupSourceTypeDef,
     AwsS3BucketDetailsTypeDef,
     DataClassificationDetailsTypeDef,
     RuleGroupDetailsTypeDef,
     AwsNetworkFirewallRuleGroupDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.26.79/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.26.8/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.26.79/setup.py` & `mypy-boto3-securityhub-1.26.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.26.79",
+    version="1.26.8",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.26.79 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.SecurityHub 1.26.8 service generated with mypy-boto3-builder"
+        " 7.11.10"
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
     keywords="boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_securityhub": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_securityhub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

