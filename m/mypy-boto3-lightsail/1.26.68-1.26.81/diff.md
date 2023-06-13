# Comparing `tmp/mypy-boto3-lightsail-1.26.68.tar.gz` & `tmp/mypy-boto3-lightsail-1.26.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.26.81.tar", last modified: Tue Feb 28 20:28:07 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.26.68.tar` & `mypy-boto3-lightsail-1.26.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.982837 mypy-boto3-lightsail-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35936 2023-02-09 20:26:49.982837 mypy-boto3-lightsail-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34441 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.982837 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   111338 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   111156 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24370 2023-02-09 20:26:29.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-02-09 20:26:29.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-02-09 20:26:29.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   142091 2023-02-09 20:26:33.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   141994 2023-02-09 20:26:31.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.982837 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35936 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-09 20:26:49.000000 mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.982837 mypy-boto3-lightsail-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-09 20:26:28.000000 mypy-boto3-lightsail-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35040 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.518319 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113914 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113728 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-02-28 20:27:49.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-02-28 20:27:49.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   146228 2023-02-28 20:27:52.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146129 2023-02-28 20:27:51.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 20:27:48.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 20:28:07.000000 mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 20:28:07.522319 mypy-boto3-lightsail-1.26.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-28 20:27:47.000000 mypy-boto3-lightsail-1.26.81/setup.py
```

### Comparing `mypy-boto3-lightsail-1.26.68/LICENSE` & `mypy-boto3-lightsail-1.26.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.68/PKG-INFO` & `mypy-boto3-lightsail-1.26.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.26.68
-Summary: Type annotations for boto3.Lightsail 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.81
+Summary: Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,14 +359,16 @@
 ```python
 from mypy_boto3_lightsail.literals import (
     AccessDirectionType,
     AccessTypeType,
     AccountLevelBpaSyncStatusType,
     AddOnTypeType,
     AlarmStateType,
+    AppCategoryType,
+    AutoMountStatusType,
     AutoSnapshotStatusType,
     BPAStatusMessageType,
     BehaviorEnumType,
     BlueprintTypeType,
     BucketMetricNameType,
     CertificateDomainValidationStatusType,
     CertificateStatusType,
@@ -377,14 +379,15 @@
     ContactProtocolType,
     ContainerServiceDeploymentStateType,
     ContainerServiceMetricNameType,
     ContainerServicePowerNameType,
     ContainerServiceProtocolType,
     ContainerServiceStateDetailCodeType,
     ContainerServiceStateType,
+    CurrencyType,
     DiskSnapshotStateType,
     DiskStateType,
     DistributionMetricNameType,
     DnsRecordCreationStateCodeType,
     ExportSnapshotRecordSourceTypeType,
     ForwardValuesType,
     GetActiveNamesPaginatorName,
@@ -436,23 +439,25 @@
     NetworkProtocolType,
     OperationStatusType,
     OperationTypeType,
     OriginProtocolPolicyEnumType,
     PortAccessTypeType,
     PortInfoSourceTypeType,
     PortStateType,
+    PricingUnitType,
     R53HostedZoneDeletionStateCodeType,
     RecordStateType,
     RegionNameType,
     RelationalDatabaseEngineType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
+    StatusType,
     StatusTypeType,
     TreatMissingDataType,
     LightsailServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -472,14 +477,15 @@
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
+    StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
@@ -514,14 +520,16 @@
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
+    CreateGUISessionAccessDetailsRequestRequestTypeDef,
+    SessionTypeDef,
     DiskMapTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
@@ -545,14 +553,15 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
@@ -565,14 +574,15 @@
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
@@ -642,16 +652,18 @@
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
+    StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
+    StopGUISessionRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopRelationalDatabaseRequestRequestTypeDef,
     TestAlarmRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBucketBundleRequestRequestTypeDef,
     UpdateDistributionBundleRequestRequestTypeDef,
     UpdateInstanceMetadataOptionsRequestRequestTypeDef,
@@ -707,17 +719,19 @@
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
+    CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
+    EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDisksRequestGetDisksPaginateTypeDef,
     GetDomainsRequestGetDomainsPaginateTypeDef,
@@ -825,16 +839,18 @@
     RebootInstanceResultTypeDef,
     RebootRelationalDatabaseResultTypeDef,
     ReleaseStaticIpResultTypeDef,
     ResetDistributionCacheResultTypeDef,
     SendContactMethodVerificationResultTypeDef,
     SetIpAddressTypeResultTypeDef,
     SetResourceAccessForBucketResultTypeDef,
+    StartGUISessionResultTypeDef,
     StartInstanceResultTypeDef,
     StartRelationalDatabaseResultTypeDef,
+    StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TestAlarmResultTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
     UpdateBucketBundleResultTypeDef,
@@ -869,14 +885,15 @@
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
     RenewalSummaryTypeDef,
+    CostEstimateTypeDef,
     GetInstanceAccessDetailsResultTypeDef,
     LoadBalancerTlsCertificateTypeDef,
     GetLoadBalancerResultTypeDef,
     GetLoadBalancersResultTypeDef,
     DomainTypeDef,
     GetRelationalDatabaseResultTypeDef,
     GetRelationalDatabasesResultTypeDef,
@@ -886,25 +903,27 @@
     CreateDistributionResultTypeDef,
     GetDistributionsResultTypeDef,
     ContainerServiceTypeDef,
     GetContainerServiceDeploymentsResultTypeDef,
     CreateContainerServiceRequestRequestTypeDef,
     ExportSnapshotRecordTypeDef,
     CertificateTypeDef,
+    ResourceBudgetEstimateTypeDef,
     GetLoadBalancerTlsCertificatesResultTypeDef,
     GetDomainResultTypeDef,
     GetDomainsResultTypeDef,
     GetInstanceResultTypeDef,
     GetInstancesResultTypeDef,
     ContainerServicesListResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
     CreateContainerServiceResultTypeDef,
     UpdateContainerServiceResultTypeDef,
     GetExportSnapshotRecordsResultTypeDef,
     CertificateSummaryTypeDef,
+    GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
 def get_structure() -> AccessKeyLastUsedTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lightsail-1.26.68/README.md` & `mypy-boto3-lightsail-1.26.81/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,14 +327,16 @@
 ```python
 from mypy_boto3_lightsail.literals import (
     AccessDirectionType,
     AccessTypeType,
     AccountLevelBpaSyncStatusType,
     AddOnTypeType,
     AlarmStateType,
+    AppCategoryType,
+    AutoMountStatusType,
     AutoSnapshotStatusType,
     BPAStatusMessageType,
     BehaviorEnumType,
     BlueprintTypeType,
     BucketMetricNameType,
     CertificateDomainValidationStatusType,
     CertificateStatusType,
@@ -345,14 +347,15 @@
     ContactProtocolType,
     ContainerServiceDeploymentStateType,
     ContainerServiceMetricNameType,
     ContainerServicePowerNameType,
     ContainerServiceProtocolType,
     ContainerServiceStateDetailCodeType,
     ContainerServiceStateType,
+    CurrencyType,
     DiskSnapshotStateType,
     DiskStateType,
     DistributionMetricNameType,
     DnsRecordCreationStateCodeType,
     ExportSnapshotRecordSourceTypeType,
     ForwardValuesType,
     GetActiveNamesPaginatorName,
@@ -404,23 +407,25 @@
     NetworkProtocolType,
     OperationStatusType,
     OperationTypeType,
     OriginProtocolPolicyEnumType,
     PortAccessTypeType,
     PortInfoSourceTypeType,
     PortStateType,
+    PricingUnitType,
     R53HostedZoneDeletionStateCodeType,
     RecordStateType,
     RegionNameType,
     RelationalDatabaseEngineType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
+    StatusType,
     StatusTypeType,
     TreatMissingDataType,
     LightsailServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -440,14 +445,15 @@
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
+    StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
@@ -482,14 +488,16 @@
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
+    CreateGUISessionAccessDetailsRequestRequestTypeDef,
+    SessionTypeDef,
     DiskMapTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
@@ -513,14 +521,15 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
@@ -533,14 +542,15 @@
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
@@ -610,16 +620,18 @@
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
+    StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
+    StopGUISessionRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopRelationalDatabaseRequestRequestTypeDef,
     TestAlarmRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBucketBundleRequestRequestTypeDef,
     UpdateDistributionBundleRequestRequestTypeDef,
     UpdateInstanceMetadataOptionsRequestRequestTypeDef,
@@ -675,17 +687,19 @@
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
+    CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
+    EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDisksRequestGetDisksPaginateTypeDef,
     GetDomainsRequestGetDomainsPaginateTypeDef,
@@ -793,16 +807,18 @@
     RebootInstanceResultTypeDef,
     RebootRelationalDatabaseResultTypeDef,
     ReleaseStaticIpResultTypeDef,
     ResetDistributionCacheResultTypeDef,
     SendContactMethodVerificationResultTypeDef,
     SetIpAddressTypeResultTypeDef,
     SetResourceAccessForBucketResultTypeDef,
+    StartGUISessionResultTypeDef,
     StartInstanceResultTypeDef,
     StartRelationalDatabaseResultTypeDef,
+    StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TestAlarmResultTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
     UpdateBucketBundleResultTypeDef,
@@ -837,14 +853,15 @@
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
     RenewalSummaryTypeDef,
+    CostEstimateTypeDef,
     GetInstanceAccessDetailsResultTypeDef,
     LoadBalancerTlsCertificateTypeDef,
     GetLoadBalancerResultTypeDef,
     GetLoadBalancersResultTypeDef,
     DomainTypeDef,
     GetRelationalDatabaseResultTypeDef,
     GetRelationalDatabasesResultTypeDef,
@@ -854,25 +871,27 @@
     CreateDistributionResultTypeDef,
     GetDistributionsResultTypeDef,
     ContainerServiceTypeDef,
     GetContainerServiceDeploymentsResultTypeDef,
     CreateContainerServiceRequestRequestTypeDef,
     ExportSnapshotRecordTypeDef,
     CertificateTypeDef,
+    ResourceBudgetEstimateTypeDef,
     GetLoadBalancerTlsCertificatesResultTypeDef,
     GetDomainResultTypeDef,
     GetDomainsResultTypeDef,
     GetInstanceResultTypeDef,
     GetInstancesResultTypeDef,
     ContainerServicesListResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
     CreateContainerServiceResultTypeDef,
     UpdateContainerServiceResultTypeDef,
     GetExportSnapshotRecordsResultTypeDef,
     CertificateSummaryTypeDef,
+    GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
 def get_structure() -> AccessKeyLastUsedTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.26.68\nVersion:         1.26.68\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.26.81\nVersion:         1.26.81\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.68")
+    print("1.26.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AddOnTypeType,
     AlarmStateType,
     BucketMetricNameType,
     CertificateStatusType,
     ComparisonOperatorType,
     ContactProtocolType,
     ContainerServiceMetricNameType,
     ContainerServicePowerNameType,
@@ -96,14 +97,15 @@
     CreateContainerServiceResultTypeDef,
     CreateDiskFromSnapshotResultTypeDef,
     CreateDiskResultTypeDef,
     CreateDiskSnapshotResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDomainEntryResultTypeDef,
     CreateDomainResultTypeDef,
+    CreateGUISessionAccessDetailsResultTypeDef,
     CreateInstancesFromSnapshotResultTypeDef,
     CreateInstanceSnapshotResultTypeDef,
     CreateInstancesResultTypeDef,
     CreateKeyPairResultTypeDef,
     CreateLoadBalancerResultTypeDef,
     CreateLoadBalancerTlsCertificateResultTypeDef,
     CreateRelationalDatabaseFromSnapshotResultTypeDef,
@@ -153,14 +155,15 @@
     GetContactMethodsResultTypeDef,
     GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesResultTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServiceDeploymentsResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetContainerServicePowersResultTypeDef,
+    GetCostEstimateResultTypeDef,
     GetDiskResultTypeDef,
     GetDiskSnapshotResultTypeDef,
     GetDiskSnapshotsResultTypeDef,
     GetDisksResultTypeDef,
     GetDistributionBundlesResultTypeDef,
     GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
@@ -216,16 +219,18 @@
     RegisterContainerImageResultTypeDef,
     RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpResultTypeDef,
     ResetDistributionCacheResultTypeDef,
     SendContactMethodVerificationResultTypeDef,
     SetIpAddressTypeResultTypeDef,
     SetResourceAccessForBucketResultTypeDef,
+    StartGUISessionResultTypeDef,
     StartInstanceResultTypeDef,
     StartRelationalDatabaseResultTypeDef,
+    StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TagTypeDef,
     TestAlarmResultTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
@@ -302,15 +307,15 @@
         network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.attach_certificate_to_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#attach_certificate_to_distribution)
         """
 
     def attach_disk(
-        self, *, diskName: str, instanceName: str, diskPath: str
+        self, *, diskName: str, instanceName: str, diskPath: str, autoMounting: bool = ...
     ) -> AttachDiskResultTypeDef:
         """
         Attaches a block storage disk to a running or stopped Lightsail instance and
         exposes it to the instance with the specified disk name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.attach_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#attach_disk)
@@ -582,14 +587,25 @@
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain_entry)
         """
 
+    def create_gui_session_access_details(
+        self, *, resourceName: str
+    ) -> CreateGUISessionAccessDetailsResultTypeDef:
+        """
+        Creates two URLs that are used to access a virtual computer’s graphical user
+        interface (GUI) session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_gui_session_access_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_gui_session_access_details)
+        """
+
     def create_instance_snapshot(
         self, *, instanceSnapshotName: str, instanceName: str, tags: Sequence[TagTypeDef] = ...
     ) -> CreateInstanceSnapshotResultTypeDef:
         """
         Creates a snapshot of a specific virtual private server, or *instance*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instance_snapshot)
@@ -980,15 +996,15 @@
         Detaches a static IP from the Amazon Lightsail instance to which it is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.detach_static_ip)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#detach_static_ip)
         """
 
     def disable_add_on(
-        self, *, addOnType: Literal["AutoSnapshot"], resourceName: str
+        self, *, addOnType: AddOnTypeType, resourceName: str
     ) -> DisableAddOnResultTypeDef:
         """
         Disables an add-on for an Amazon Lightsail resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.disable_add_on)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#disable_add_on)
         """
@@ -1057,15 +1073,19 @@
         Returns the available automatic snapshots for an instance or disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_auto_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_auto_snapshots)
         """
 
     def get_blueprints(
-        self, *, includeInactive: bool = ..., pageToken: str = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        pageToken: str = ...,
+        appCategory: Literal["LfR"] = ...
     ) -> GetBlueprintsResultTypeDef:
         """
         Returns the list of available instance images, or *blueprints*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_blueprints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_blueprints)
         """
@@ -1111,15 +1131,19 @@
         Returns information about one or more Amazon Lightsail buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_buckets)
         """
 
     def get_bundles(
-        self, *, includeInactive: bool = ..., pageToken: str = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        pageToken: str = ...,
+        appCategory: Literal["LfR"] = ...
     ) -> GetBundlesResultTypeDef:
         """
         Returns the bundles that you can apply to an Amazon Lightsail instance when you
         create it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bundles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_bundles)
@@ -1242,14 +1266,24 @@
         Returns information about one or more of your Amazon Lightsail container
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_services)
         """
 
+    def get_cost_estimate(
+        self, *, resourceName: str, startTime: Union[datetime, str], endTime: Union[datetime, str]
+    ) -> GetCostEstimateResultTypeDef:
+        """
+        Retrieves information about the cost estimate for a specified resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_cost_estimate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_cost_estimate)
+        """
+
     def get_disk(self, *, diskName: str) -> GetDiskResultTypeDef:
         """
         Returns information about a specific block storage disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_disk)
         """
@@ -1859,14 +1893,23 @@
         Sets the Amazon Lightsail resources that can access the specified Lightsail
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.set_resource_access_for_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#set_resource_access_for_bucket)
         """
 
+    def start_gui_session(self, *, resourceName: str) -> StartGUISessionResultTypeDef:
+        """
+        Initiates a graphical user interface (GUI) session that’s used to access a
+        virtual computer’s operating system and application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_gui_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_gui_session)
+        """
+
     def start_instance(self, *, instanceName: str) -> StartInstanceResultTypeDef:
         """
         Starts a specific Amazon Lightsail instance from a stopped state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_instance)
         """
@@ -1877,14 +1920,23 @@
         """
         Starts a specific database from a stopped state in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_relational_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_relational_database)
         """
 
+    def stop_gui_session(self, *, resourceName: str) -> StopGUISessionResultTypeDef:
+        """
+        Terminates a web-based NICE DCV session that’s used to access a virtual
+        computer’s operating system or application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.stop_gui_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#stop_gui_session)
+        """
+
     def stop_instance(self, *, instanceName: str, force: bool = ...) -> StopInstanceResultTypeDef:
         """
         Stops a specific Amazon Lightsail instance that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.stop_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#stop_instance)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    AddOnTypeType,
     AlarmStateType,
     BucketMetricNameType,
     CertificateStatusType,
     ComparisonOperatorType,
     ContactProtocolType,
     ContainerServiceMetricNameType,
     ContainerServicePowerNameType,
@@ -96,14 +97,15 @@
     CreateContainerServiceResultTypeDef,
     CreateDiskFromSnapshotResultTypeDef,
     CreateDiskResultTypeDef,
     CreateDiskSnapshotResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDomainEntryResultTypeDef,
     CreateDomainResultTypeDef,
+    CreateGUISessionAccessDetailsResultTypeDef,
     CreateInstancesFromSnapshotResultTypeDef,
     CreateInstanceSnapshotResultTypeDef,
     CreateInstancesResultTypeDef,
     CreateKeyPairResultTypeDef,
     CreateLoadBalancerResultTypeDef,
     CreateLoadBalancerTlsCertificateResultTypeDef,
     CreateRelationalDatabaseFromSnapshotResultTypeDef,
@@ -153,14 +155,15 @@
     GetContactMethodsResultTypeDef,
     GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesResultTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServiceDeploymentsResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetContainerServicePowersResultTypeDef,
+    GetCostEstimateResultTypeDef,
     GetDiskResultTypeDef,
     GetDiskSnapshotResultTypeDef,
     GetDiskSnapshotsResultTypeDef,
     GetDisksResultTypeDef,
     GetDistributionBundlesResultTypeDef,
     GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
@@ -216,16 +219,18 @@
     RegisterContainerImageResultTypeDef,
     RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpResultTypeDef,
     ResetDistributionCacheResultTypeDef,
     SendContactMethodVerificationResultTypeDef,
     SetIpAddressTypeResultTypeDef,
     SetResourceAccessForBucketResultTypeDef,
+    StartGUISessionResultTypeDef,
     StartInstanceResultTypeDef,
     StartRelationalDatabaseResultTypeDef,
+    StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TagTypeDef,
     TestAlarmResultTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
@@ -295,15 +300,15 @@
         Attaches an SSL/TLS certificate to your Amazon Lightsail content delivery
         network (CDN) distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.attach_certificate_to_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#attach_certificate_to_distribution)
         """
     def attach_disk(
-        self, *, diskName: str, instanceName: str, diskPath: str
+        self, *, diskName: str, instanceName: str, diskPath: str, autoMounting: bool = ...
     ) -> AttachDiskResultTypeDef:
         """
         Attaches a block storage disk to a running or stopped Lightsail instance and
         exposes it to the instance with the specified disk name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.attach_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#attach_disk)
@@ -553,14 +558,24 @@
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_domain_entry)
         """
+    def create_gui_session_access_details(
+        self, *, resourceName: str
+    ) -> CreateGUISessionAccessDetailsResultTypeDef:
+        """
+        Creates two URLs that are used to access a virtual computer’s graphical user
+        interface (GUI) session.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_gui_session_access_details)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#create_gui_session_access_details)
+        """
     def create_instance_snapshot(
         self, *, instanceSnapshotName: str, instanceName: str, tags: Sequence[TagTypeDef] = ...
     ) -> CreateInstanceSnapshotResultTypeDef:
         """
         Creates a snapshot of a specific virtual private server, or *instance*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_instance_snapshot)
@@ -917,15 +932,15 @@
         """
         Detaches a static IP from the Amazon Lightsail instance to which it is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.detach_static_ip)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#detach_static_ip)
         """
     def disable_add_on(
-        self, *, addOnType: Literal["AutoSnapshot"], resourceName: str
+        self, *, addOnType: AddOnTypeType, resourceName: str
     ) -> DisableAddOnResultTypeDef:
         """
         Disables an add-on for an Amazon Lightsail resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.disable_add_on)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#disable_add_on)
         """
@@ -986,15 +1001,19 @@
         """
         Returns the available automatic snapshots for an instance or disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_auto_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_auto_snapshots)
         """
     def get_blueprints(
-        self, *, includeInactive: bool = ..., pageToken: str = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        pageToken: str = ...,
+        appCategory: Literal["LfR"] = ...
     ) -> GetBlueprintsResultTypeDef:
         """
         Returns the list of available instance images, or *blueprints*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_blueprints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_blueprints)
         """
@@ -1035,15 +1054,19 @@
         """
         Returns information about one or more Amazon Lightsail buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_buckets)
         """
     def get_bundles(
-        self, *, includeInactive: bool = ..., pageToken: str = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        pageToken: str = ...,
+        appCategory: Literal["LfR"] = ...
     ) -> GetBundlesResultTypeDef:
         """
         Returns the bundles that you can apply to an Amazon Lightsail instance when you
         create it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_bundles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_bundles)
@@ -1155,14 +1178,23 @@
         """
         Returns information about one or more of your Amazon Lightsail container
         services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_container_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_container_services)
         """
+    def get_cost_estimate(
+        self, *, resourceName: str, startTime: Union[datetime, str], endTime: Union[datetime, str]
+    ) -> GetCostEstimateResultTypeDef:
+        """
+        Retrieves information about the cost estimate for a specified resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_cost_estimate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_cost_estimate)
+        """
     def get_disk(self, *, diskName: str) -> GetDiskResultTypeDef:
         """
         Returns information about a specific block storage disk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.get_disk)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#get_disk)
         """
@@ -1714,14 +1746,22 @@
         """
         Sets the Amazon Lightsail resources that can access the specified Lightsail
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.set_resource_access_for_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#set_resource_access_for_bucket)
         """
+    def start_gui_session(self, *, resourceName: str) -> StartGUISessionResultTypeDef:
+        """
+        Initiates a graphical user interface (GUI) session that’s used to access a
+        virtual computer’s operating system and application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_gui_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_gui_session)
+        """
     def start_instance(self, *, instanceName: str) -> StartInstanceResultTypeDef:
         """
         Starts a specific Amazon Lightsail instance from a stopped state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_instance)
         """
@@ -1730,14 +1770,22 @@
     ) -> StartRelationalDatabaseResultTypeDef:
         """
         Starts a specific database from a stopped state in Amazon Lightsail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.start_relational_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#start_relational_database)
         """
+    def stop_gui_session(self, *, resourceName: str) -> StopGUISessionResultTypeDef:
+        """
+        Terminates a web-based NICE DCV session that’s used to access a virtual
+        computer’s operating system or application.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.stop_gui_session)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#stop_gui_session)
+        """
     def stop_instance(self, *, instanceName: str, force: bool = ...) -> StopInstanceResultTypeDef:
         """
         Stops a specific Amazon Lightsail instance that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.stop_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/client/#stop_instance)
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 __all__ = (
     "AccessDirectionType",
     "AccessTypeType",
     "AccountLevelBpaSyncStatusType",
     "AddOnTypeType",
     "AlarmStateType",
+    "AppCategoryType",
+    "AutoMountStatusType",
     "AutoSnapshotStatusType",
     "BPAStatusMessageType",
     "BehaviorEnumType",
     "BlueprintTypeType",
     "BucketMetricNameType",
     "CertificateDomainValidationStatusType",
     "CertificateStatusType",
@@ -39,14 +41,15 @@
     "ContactProtocolType",
     "ContainerServiceDeploymentStateType",
     "ContainerServiceMetricNameType",
     "ContainerServicePowerNameType",
     "ContainerServiceProtocolType",
     "ContainerServiceStateDetailCodeType",
     "ContainerServiceStateType",
+    "CurrencyType",
     "DiskSnapshotStateType",
     "DiskStateType",
     "DistributionMetricNameType",
     "DnsRecordCreationStateCodeType",
     "ExportSnapshotRecordSourceTypeType",
     "ForwardValuesType",
     "GetActiveNamesPaginatorName",
@@ -98,38 +101,42 @@
     "NetworkProtocolType",
     "OperationStatusType",
     "OperationTypeType",
     "OriginProtocolPolicyEnumType",
     "PortAccessTypeType",
     "PortInfoSourceTypeType",
     "PortStateType",
+    "PricingUnitType",
     "R53HostedZoneDeletionStateCodeType",
     "RecordStateType",
     "RegionNameType",
     "RelationalDatabaseEngineType",
     "RelationalDatabaseMetricNameType",
     "RelationalDatabasePasswordVersionType",
     "RenewalStatusType",
     "ResourceBucketAccessType",
     "ResourceTypeType",
+    "StatusType",
     "StatusTypeType",
     "TreatMissingDataType",
     "LightsailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AccessDirectionType = Literal["inbound", "outbound"]
 AccessTypeType = Literal["private", "public"]
 AccountLevelBpaSyncStatusType = Literal["Defaulted", "Failed", "InSync", "NeverSynced"]
-AddOnTypeType = Literal["AutoSnapshot"]
+AddOnTypeType = Literal["AutoSnapshot", "StopInstanceOnIdle"]
 AlarmStateType = Literal["ALARM", "INSUFFICIENT_DATA", "OK"]
+AppCategoryType = Literal["LfR"]
+AutoMountStatusType = Literal["Failed", "Mounted", "NotMounted", "Pending"]
 AutoSnapshotStatusType = Literal["Failed", "InProgress", "NotFound", "Success"]
 BPAStatusMessageType = Literal[
     "DEFAULTED_FOR_SLR_MISSING", "DEFAULTED_FOR_SLR_MISSING_ON_HOLD", "SYNC_ON_HOLD", "Unknown"
 ]
 BehaviorEnumType = Literal["cache", "dont-cache"]
 BlueprintTypeType = Literal["app", "os"]
 BucketMetricNameType = Literal["BucketSizeBytes", "NumberOfObjects"]
@@ -167,14 +174,15 @@
     "PROVISIONING_CERTIFICATE",
     "PROVISIONING_SERVICE",
     "UNKNOWN_ERROR",
 ]
 ContainerServiceStateType = Literal[
     "DELETING", "DEPLOYING", "DISABLED", "PENDING", "READY", "RUNNING", "UPDATING"
 ]
+CurrencyType = Literal["USD"]
 DiskSnapshotStateType = Literal["completed", "error", "pending", "unknown"]
 DiskStateType = Literal["available", "error", "in-use", "pending", "unknown"]
 DistributionMetricNameType = Literal[
     "BytesDownloaded",
     "BytesUploaded",
     "Http4xxErrorRate",
     "Http5xxErrorRate",
@@ -435,16 +443,18 @@
     "RebootRelationalDatabase",
     "RegisterContainerImage",
     "ReleaseStaticIp",
     "ResetDistributionCache",
     "SendContactMethodVerification",
     "SetIpAddressType",
     "SetResourceAccessForBucket",
+    "StartGUISession",
     "StartInstance",
     "StartRelationalDatabase",
+    "StopGUISession",
     "StopInstance",
     "StopRelationalDatabase",
     "TestAlarm",
     "UpdateBucket",
     "UpdateBucketBundle",
     "UpdateContainerService",
     "UpdateDistribution",
@@ -455,14 +465,15 @@
     "UpdateRelationalDatabase",
     "UpdateRelationalDatabaseParameters",
 ]
 OriginProtocolPolicyEnumType = Literal["http-only", "https-only"]
 PortAccessTypeType = Literal["Private", "Public"]
 PortInfoSourceTypeType = Literal["CLOSED", "DEFAULT", "INSTANCE", "NONE"]
 PortStateType = Literal["closed", "open"]
+PricingUnitType = Literal["Bundles", "GB", "GB-Mo", "Hrs", "Queries"]
 R53HostedZoneDeletionStateCodeType = Literal["FAILED", "PENDING", "STARTED", "SUCCEEDED"]
 RecordStateType = Literal["Failed", "Started", "Succeeded"]
 RegionNameType = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
@@ -508,14 +519,26 @@
     "LoadBalancer",
     "LoadBalancerTlsCertificate",
     "PeeredVpc",
     "RelationalDatabase",
     "RelationalDatabaseSnapshot",
     "StaticIp",
 ]
+StatusType = Literal[
+    "failedInstanceCreation",
+    "failedStartingGUISession",
+    "failedStoppingGUISession",
+    "notStarted",
+    "settingUpInstance",
+    "startExpired",
+    "started",
+    "starting",
+    "stopped",
+    "stopping",
+]
 StatusTypeType = Literal["Active", "Inactive"]
 TreatMissingDataType = Literal["breaching", "ignore", "missing", "notBreaching"]
 LightsailServiceName = Literal["lightsail"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -659,14 +682,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -835,14 +859,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 __all__ = (
     "AccessDirectionType",
     "AccessTypeType",
     "AccountLevelBpaSyncStatusType",
     "AddOnTypeType",
     "AlarmStateType",
+    "AppCategoryType",
+    "AutoMountStatusType",
     "AutoSnapshotStatusType",
     "BPAStatusMessageType",
     "BehaviorEnumType",
     "BlueprintTypeType",
     "BucketMetricNameType",
     "CertificateDomainValidationStatusType",
     "CertificateStatusType",
@@ -38,14 +40,15 @@
     "ContactProtocolType",
     "ContainerServiceDeploymentStateType",
     "ContainerServiceMetricNameType",
     "ContainerServicePowerNameType",
     "ContainerServiceProtocolType",
     "ContainerServiceStateDetailCodeType",
     "ContainerServiceStateType",
+    "CurrencyType",
     "DiskSnapshotStateType",
     "DiskStateType",
     "DistributionMetricNameType",
     "DnsRecordCreationStateCodeType",
     "ExportSnapshotRecordSourceTypeType",
     "ForwardValuesType",
     "GetActiveNamesPaginatorName",
@@ -97,37 +100,41 @@
     "NetworkProtocolType",
     "OperationStatusType",
     "OperationTypeType",
     "OriginProtocolPolicyEnumType",
     "PortAccessTypeType",
     "PortInfoSourceTypeType",
     "PortStateType",
+    "PricingUnitType",
     "R53HostedZoneDeletionStateCodeType",
     "RecordStateType",
     "RegionNameType",
     "RelationalDatabaseEngineType",
     "RelationalDatabaseMetricNameType",
     "RelationalDatabasePasswordVersionType",
     "RenewalStatusType",
     "ResourceBucketAccessType",
     "ResourceTypeType",
+    "StatusType",
     "StatusTypeType",
     "TreatMissingDataType",
     "LightsailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccessDirectionType = Literal["inbound", "outbound"]
 AccessTypeType = Literal["private", "public"]
 AccountLevelBpaSyncStatusType = Literal["Defaulted", "Failed", "InSync", "NeverSynced"]
-AddOnTypeType = Literal["AutoSnapshot"]
+AddOnTypeType = Literal["AutoSnapshot", "StopInstanceOnIdle"]
 AlarmStateType = Literal["ALARM", "INSUFFICIENT_DATA", "OK"]
+AppCategoryType = Literal["LfR"]
+AutoMountStatusType = Literal["Failed", "Mounted", "NotMounted", "Pending"]
 AutoSnapshotStatusType = Literal["Failed", "InProgress", "NotFound", "Success"]
 BPAStatusMessageType = Literal[
     "DEFAULTED_FOR_SLR_MISSING", "DEFAULTED_FOR_SLR_MISSING_ON_HOLD", "SYNC_ON_HOLD", "Unknown"
 ]
 BehaviorEnumType = Literal["cache", "dont-cache"]
 BlueprintTypeType = Literal["app", "os"]
 BucketMetricNameType = Literal["BucketSizeBytes", "NumberOfObjects"]
@@ -165,14 +172,15 @@
     "PROVISIONING_CERTIFICATE",
     "PROVISIONING_SERVICE",
     "UNKNOWN_ERROR",
 ]
 ContainerServiceStateType = Literal[
     "DELETING", "DEPLOYING", "DISABLED", "PENDING", "READY", "RUNNING", "UPDATING"
 ]
+CurrencyType = Literal["USD"]
 DiskSnapshotStateType = Literal["completed", "error", "pending", "unknown"]
 DiskStateType = Literal["available", "error", "in-use", "pending", "unknown"]
 DistributionMetricNameType = Literal[
     "BytesDownloaded",
     "BytesUploaded",
     "Http4xxErrorRate",
     "Http5xxErrorRate",
@@ -433,16 +441,18 @@
     "RebootRelationalDatabase",
     "RegisterContainerImage",
     "ReleaseStaticIp",
     "ResetDistributionCache",
     "SendContactMethodVerification",
     "SetIpAddressType",
     "SetResourceAccessForBucket",
+    "StartGUISession",
     "StartInstance",
     "StartRelationalDatabase",
+    "StopGUISession",
     "StopInstance",
     "StopRelationalDatabase",
     "TestAlarm",
     "UpdateBucket",
     "UpdateBucketBundle",
     "UpdateContainerService",
     "UpdateDistribution",
@@ -453,14 +463,15 @@
     "UpdateRelationalDatabase",
     "UpdateRelationalDatabaseParameters",
 ]
 OriginProtocolPolicyEnumType = Literal["http-only", "https-only"]
 PortAccessTypeType = Literal["Private", "Public"]
 PortInfoSourceTypeType = Literal["CLOSED", "DEFAULT", "INSTANCE", "NONE"]
 PortStateType = Literal["closed", "open"]
+PricingUnitType = Literal["Bundles", "GB", "GB-Mo", "Hrs", "Queries"]
 R53HostedZoneDeletionStateCodeType = Literal["FAILED", "PENDING", "STARTED", "SUCCEEDED"]
 RecordStateType = Literal["Failed", "Started", "Succeeded"]
 RegionNameType = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
@@ -506,14 +517,26 @@
     "LoadBalancer",
     "LoadBalancerTlsCertificate",
     "PeeredVpc",
     "RelationalDatabase",
     "RelationalDatabaseSnapshot",
     "StaticIp",
 ]
+StatusType = Literal[
+    "failedInstanceCreation",
+    "failedStartingGUISession",
+    "failedStoppingGUISession",
+    "notStarted",
+    "settingUpInstance",
+    "startExpired",
+    "started",
+    "starting",
+    "stopped",
+    "stopping",
+]
 StatusTypeType = Literal["Active", "Inactive"]
 TreatMissingDataType = Literal["breaching", "ignore", "missing", "notBreaching"]
 LightsailServiceName = Literal["lightsail"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -657,14 +680,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -833,14 +857,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     get_relational_database_events_paginator: GetRelationalDatabaseEventsPaginator = client.get_paginator("get_relational_database_events")
     get_relational_database_parameters_paginator: GetRelationalDatabaseParametersPaginator = client.get_paginator("get_relational_database_parameters")
     get_relational_database_snapshots_paginator: GetRelationalDatabaseSnapshotsPaginator = client.get_paginator("get_relational_database_snapshots")
     get_relational_databases_paginator: GetRelationalDatabasesPaginator = client.get_paginator("get_relational_databases")
     get_static_ips_paginator: GetStaticIpsPaginator = client.get_paginator("get_static_ips")
     ```
 """
+import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     GetActiveNamesResultTypeDef,
     GetBlueprintsResultTypeDef,
@@ -81,14 +82,20 @@
     GetRelationalDatabaseParametersResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
     GetRelationalDatabasesResultTypeDef,
     GetStaticIpsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = (
     "GetActiveNamesPaginator",
     "GetBlueprintsPaginator",
     "GetBundlesPaginator",
     "GetCloudFormationStackRecordsPaginator",
     "GetDiskSnapshotsPaginator",
     "GetDisksPaginator",
@@ -137,30 +144,38 @@
 class GetBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        appCategory: Literal["LfR"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 
 class GetBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        appCategory: Literal["LfR"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     get_relational_database_events_paginator: GetRelationalDatabaseEventsPaginator = client.get_paginator("get_relational_database_events")
     get_relational_database_parameters_paginator: GetRelationalDatabaseParametersPaginator = client.get_paginator("get_relational_database_parameters")
     get_relational_database_snapshots_paginator: GetRelationalDatabaseSnapshotsPaginator = client.get_paginator("get_relational_database_snapshots")
     get_relational_databases_paginator: GetRelationalDatabasesPaginator = client.get_paginator("get_relational_databases")
     get_static_ips_paginator: GetStaticIpsPaginator = client.get_paginator("get_static_ips")
     ```
 """
+import sys
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     GetActiveNamesResultTypeDef,
     GetBlueprintsResultTypeDef,
@@ -81,14 +82,19 @@
     GetRelationalDatabaseParametersResultTypeDef,
     GetRelationalDatabaseSnapshotsResultTypeDef,
     GetRelationalDatabasesResultTypeDef,
     GetStaticIpsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = (
     "GetActiveNamesPaginator",
     "GetBlueprintsPaginator",
     "GetBundlesPaginator",
     "GetCloudFormationStackRecordsPaginator",
     "GetDiskSnapshotsPaginator",
     "GetDisksPaginator",
@@ -133,29 +139,37 @@
 class GetBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        appCategory: Literal["LfR"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 class GetBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        includeInactive: bool = ...,
+        appCategory: Literal["LfR"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
 
 class GetCloudFormationStackRecordsPaginator(Paginator):
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessDirectionType,
     AccessTypeType,
     AccountLevelBpaSyncStatusType,
+    AddOnTypeType,
     AlarmStateType,
+    AutoMountStatusType,
     AutoSnapshotStatusType,
     BehaviorEnumType,
     BlueprintTypeType,
     BPAStatusMessageType,
     BucketMetricNameType,
     CertificateDomainValidationStatusType,
     CertificateStatusType,
@@ -71,22 +73,24 @@
     NetworkProtocolType,
     OperationStatusType,
     OperationTypeType,
     OriginProtocolPolicyEnumType,
     PortAccessTypeType,
     PortInfoSourceTypeType,
     PortStateType,
+    PricingUnitType,
     R53HostedZoneDeletionStateCodeType,
     RecordStateType,
     RegionNameType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
+    StatusType,
     StatusTypeType,
     TreatMissingDataType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -98,14 +102,15 @@
 
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
+    "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
@@ -140,14 +145,16 @@
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
+    "CreateGUISessionAccessDetailsRequestRequestTypeDef",
+    "SessionTypeDef",
     "DiskMapTypeDef",
     "DeleteAlarmRequestRequestTypeDef",
     "DeleteAutoSnapshotRequestRequestTypeDef",
     "DeleteBucketAccessKeyRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteContactMethodRequestRequestTypeDef",
@@ -171,14 +178,15 @@
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "ResourceRecordTypeDef",
+    "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
@@ -191,14 +199,15 @@
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
+    "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
@@ -268,16 +277,18 @@
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
+    "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
+    "StopGUISessionRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopRelationalDatabaseRequestRequestTypeDef",
     "TestAlarmRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBucketBundleRequestRequestTypeDef",
     "UpdateDistributionBundleRequestRequestTypeDef",
     "UpdateInstanceMetadataOptionsRequestRequestTypeDef",
@@ -333,17 +344,19 @@
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
+    "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
+    "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDomainsRequestGetDomainsPaginateTypeDef",
@@ -451,16 +464,18 @@
     "RebootInstanceResultTypeDef",
     "RebootRelationalDatabaseResultTypeDef",
     "ReleaseStaticIpResultTypeDef",
     "ResetDistributionCacheResultTypeDef",
     "SendContactMethodVerificationResultTypeDef",
     "SetIpAddressTypeResultTypeDef",
     "SetResourceAccessForBucketResultTypeDef",
+    "StartGUISessionResultTypeDef",
     "StartInstanceResultTypeDef",
     "StartRelationalDatabaseResultTypeDef",
+    "StopGUISessionResultTypeDef",
     "StopInstanceResultTypeDef",
     "StopRelationalDatabaseResultTypeDef",
     "TagResourceResultTypeDef",
     "TestAlarmResultTypeDef",
     "UnpeerVpcResultTypeDef",
     "UntagResourceResultTypeDef",
     "UpdateBucketBundleResultTypeDef",
@@ -495,14 +510,15 @@
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
     "RenewalSummaryTypeDef",
+    "CostEstimateTypeDef",
     "GetInstanceAccessDetailsResultTypeDef",
     "LoadBalancerTlsCertificateTypeDef",
     "GetLoadBalancerResultTypeDef",
     "GetLoadBalancersResultTypeDef",
     "DomainTypeDef",
     "GetRelationalDatabaseResultTypeDef",
     "GetRelationalDatabasesResultTypeDef",
@@ -512,25 +528,27 @@
     "CreateDistributionResultTypeDef",
     "GetDistributionsResultTypeDef",
     "ContainerServiceTypeDef",
     "GetContainerServiceDeploymentsResultTypeDef",
     "CreateContainerServiceRequestRequestTypeDef",
     "ExportSnapshotRecordTypeDef",
     "CertificateTypeDef",
+    "ResourceBudgetEstimateTypeDef",
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     "GetDomainResultTypeDef",
     "GetDomainsResultTypeDef",
     "GetInstanceResultTypeDef",
     "GetInstancesResultTypeDef",
     "ContainerServicesListResultTypeDef",
     "CreateContainerServiceDeploymentResultTypeDef",
     "CreateContainerServiceResultTypeDef",
     "UpdateContainerServiceResultTypeDef",
     "GetExportSnapshotRecordsResultTypeDef",
     "CertificateSummaryTypeDef",
+    "GetCostEstimateResultTypeDef",
     "CreateCertificateResultTypeDef",
     "GetCertificatesResultTypeDef",
 )
 
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
@@ -565,21 +583,32 @@
     "AutoSnapshotAddOnRequestTypeDef",
     {
         "snapshotTimeOfDay": str,
     },
     total=False,
 )
 
+StopInstanceOnIdleRequestTypeDef = TypedDict(
+    "StopInstanceOnIdleRequestTypeDef",
+    {
+        "threshold": str,
+        "duration": str,
+    },
+    total=False,
+)
+
 AddOnTypeDef = TypedDict(
     "AddOnTypeDef",
     {
         "name": str,
         "status": str,
         "snapshotTimeOfDay": str,
         "nextSnapshotTimeOfDay": str,
+        "threshold": str,
+        "duration": str,
     },
     total=False,
 )
 
 MonitoredResourceInfoTypeDef = TypedDict(
     "MonitoredResourceInfoTypeDef",
     {
@@ -621,22 +650,36 @@
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
 
-AttachDiskRequestRequestTypeDef = TypedDict(
-    "AttachDiskRequestRequestTypeDef",
+_RequiredAttachDiskRequestRequestTypeDef = TypedDict(
+    "_RequiredAttachDiskRequestRequestTypeDef",
     {
         "diskName": str,
         "instanceName": str,
         "diskPath": str,
     },
 )
+_OptionalAttachDiskRequestRequestTypeDef = TypedDict(
+    "_OptionalAttachDiskRequestRequestTypeDef",
+    {
+        "autoMounting": bool,
+    },
+    total=False,
+)
+
+
+class AttachDiskRequestRequestTypeDef(
+    _RequiredAttachDiskRequestRequestTypeDef, _OptionalAttachDiskRequestRequestTypeDef
+):
+    pass
+
 
 AttachInstancesToLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instanceNames": Sequence[str],
     },
@@ -687,14 +730,15 @@
         "isActive": bool,
         "minPower": int,
         "version": str,
         "versionCode": str,
         "productUrl": str,
         "licenseUrl": str,
         "platform": InstancePlatformType,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
@@ -767,14 +811,15 @@
         "instanceType": str,
         "isActive": bool,
         "name": str,
         "power": int,
         "ramSizeInGb": float,
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
+        "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
@@ -1025,14 +1070,31 @@
         "isAlias": bool,
         "type": str,
         "options": Mapping[str, str],
     },
     total=False,
 )
 
+CreateGUISessionAccessDetailsRequestRequestTypeDef = TypedDict(
+    "CreateGUISessionAccessDetailsRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
+SessionTypeDef = TypedDict(
+    "SessionTypeDef",
+    {
+        "name": str,
+        "url": str,
+        "isPrimary": bool,
+    },
+    total=False,
+)
+
 DiskMapTypeDef = TypedDict(
     "DiskMapTypeDef",
     {
         "originalDiskPath": str,
         "newDiskName": str,
     },
     total=False,
@@ -1298,15 +1360,15 @@
         "staticIpName": str,
     },
 )
 
 DisableAddOnRequestRequestTypeDef = TypedDict(
     "DisableAddOnRequestRequestTypeDef",
     {
-        "addOnType": Literal["AutoSnapshot"],
+        "addOnType": AddOnTypeType,
         "resourceName": str,
     },
 )
 
 DiskInfoTypeDef = TypedDict(
     "DiskInfoTypeDef",
     {
@@ -1353,14 +1415,23 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "start": datetime,
+        "end": datetime,
+    },
+    total=False,
+)
+
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
@@ -1400,14 +1471,15 @@
 )
 
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 GetBucketAccessKeysRequestRequestTypeDef = TypedDict(
     "GetBucketAccessKeysRequestRequestTypeDef",
     {
@@ -1461,14 +1533,15 @@
 )
 
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 GetCertificatesRequestRequestTypeDef = TypedDict(
     "GetCertificatesRequestRequestTypeDef",
     {
@@ -1550,14 +1623,23 @@
     "GetContainerServicesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
 
+GetCostEstimateRequestRequestTypeDef = TypedDict(
+    "GetCostEstimateRequestRequestTypeDef",
+    {
+        "resourceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+
 GetDiskRequestRequestTypeDef = TypedDict(
     "GetDiskRequestRequestTypeDef",
     {
         "diskName": str,
     },
 )
 
@@ -2357,28 +2439,42 @@
     {
         "resourceName": str,
         "bucketName": str,
         "access": ResourceBucketAccessType,
     },
 )
 
+StartGUISessionRequestRequestTypeDef = TypedDict(
+    "StartGUISessionRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
 StartRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "StartRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
+StopGUISessionRequestRequestTypeDef = TypedDict(
+    "StopGUISessionRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
 _RequiredStopInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredStopInstanceRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 _OptionalStopInstanceRequestRequestTypeDef = TypedDict(
@@ -2540,21 +2636,22 @@
     },
     total=False,
 )
 
 _RequiredAddOnRequestTypeDef = TypedDict(
     "_RequiredAddOnRequestTypeDef",
     {
-        "addOnType": Literal["AutoSnapshot"],
+        "addOnType": AddOnTypeType,
     },
 )
 _OptionalAddOnRequestTypeDef = TypedDict(
     "_OptionalAddOnRequestTypeDef",
     {
         "autoSnapshotAddOnRequest": AutoSnapshotAddOnRequestTypeDef,
+        "stopInstanceOnIdleRequest": StopInstanceOnIdleRequestTypeDef,
     },
     total=False,
 )
 
 
 class AddOnRequestTypeDef(_RequiredAddOnRequestTypeDef, _OptionalAddOnRequestTypeDef):
     pass
@@ -3097,14 +3194,15 @@
         "iops": int,
         "path": str,
         "state": DiskStateType,
         "attachedTo": str,
         "isAttached": bool,
         "attachmentState": str,
         "gbInUse": int,
+        "autoMountStatus": AutoMountStatusType,
     },
     total=False,
 )
 
 KeyPairTypeDef = TypedDict(
     "KeyPairTypeDef",
     {
@@ -3341,14 +3439,26 @@
     "UpdateDomainEntryRequestRequestTypeDef",
     {
         "domainName": str,
         "domainEntry": DomainEntryTypeDef,
     },
 )
 
+CreateGUISessionAccessDetailsResultTypeDef = TypedDict(
+    "CreateGUISessionAccessDetailsResultTypeDef",
+    {
+        "resourceName": str,
+        "status": StatusType,
+        "percentageComplete": int,
+        "failureReason": str,
+        "sessions": List[SessionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
         "fromBlueprintId": str,
         "fromDiskInfo": List[DiskInfoTypeDef],
     },
@@ -3370,35 +3480,49 @@
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
     },
     total=False,
 )
 
+EstimateByTimeTypeDef = TypedDict(
+    "EstimateByTimeTypeDef",
+    {
+        "usageCost": float,
+        "pricingUnit": PricingUnitType,
+        "unit": float,
+        "currency": Literal["USD"],
+        "timePeriod": TimePeriodTypeDef,
+    },
+    total=False,
+)
+
 GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     {
         "includeInactive": bool,
+        "appCategory": Literal["LfR"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     {
         "includeInactive": bool,
+        "appCategory": Literal["LfR"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
@@ -4486,14 +4610,22 @@
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartGUISessionResultTypeDef = TypedDict(
+    "StartGUISessionResultTypeDef",
+    {
+        "operations": List[OperationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4502,14 +4634,22 @@
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StopGUISessionResultTypeDef = TypedDict(
+    "StopGUISessionResultTypeDef",
+    {
+        "operations": List[OperationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4975,14 +5115,23 @@
         "renewalStatus": RenewalStatusType,
         "renewalStatusReason": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+CostEstimateTypeDef = TypedDict(
+    "CostEstimateTypeDef",
+    {
+        "usageType": str,
+        "resultsByTime": List[EstimateByTimeTypeDef],
+    },
+    total=False,
+)
+
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5233,14 +5382,26 @@
         "revocationReason": str,
         "tags": List[TagTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
+ResourceBudgetEstimateTypeDef = TypedDict(
+    "ResourceBudgetEstimateTypeDef",
+    {
+        "resourceName": str,
+        "resourceType": ResourceTypeType,
+        "costEstimates": List[CostEstimateTypeDef],
+        "startTime": datetime,
+        "endTime": datetime,
+    },
+    total=False,
+)
+
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5328,14 +5489,22 @@
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+GetCostEstimateResultTypeDef = TypedDict(
+    "GetCostEstimateResultTypeDef",
+    {
+        "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessDirectionType,
     AccessTypeType,
     AccountLevelBpaSyncStatusType,
+    AddOnTypeType,
     AlarmStateType,
+    AutoMountStatusType,
     AutoSnapshotStatusType,
     BehaviorEnumType,
     BlueprintTypeType,
     BPAStatusMessageType,
     BucketMetricNameType,
     CertificateDomainValidationStatusType,
     CertificateStatusType,
@@ -71,22 +73,24 @@
     NetworkProtocolType,
     OperationStatusType,
     OperationTypeType,
     OriginProtocolPolicyEnumType,
     PortAccessTypeType,
     PortInfoSourceTypeType,
     PortStateType,
+    PricingUnitType,
     R53HostedZoneDeletionStateCodeType,
     RecordStateType,
     RegionNameType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
+    StatusType,
     StatusTypeType,
     TreatMissingDataType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -97,14 +101,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
+    "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
@@ -139,14 +144,16 @@
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
+    "CreateGUISessionAccessDetailsRequestRequestTypeDef",
+    "SessionTypeDef",
     "DiskMapTypeDef",
     "DeleteAlarmRequestRequestTypeDef",
     "DeleteAutoSnapshotRequestRequestTypeDef",
     "DeleteBucketAccessKeyRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteContactMethodRequestRequestTypeDef",
@@ -170,14 +177,15 @@
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "ResourceRecordTypeDef",
+    "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
@@ -190,14 +198,15 @@
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
+    "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
@@ -267,16 +276,18 @@
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
+    "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
+    "StopGUISessionRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopRelationalDatabaseRequestRequestTypeDef",
     "TestAlarmRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBucketBundleRequestRequestTypeDef",
     "UpdateDistributionBundleRequestRequestTypeDef",
     "UpdateInstanceMetadataOptionsRequestRequestTypeDef",
@@ -332,17 +343,19 @@
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
+    "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
+    "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDomainsRequestGetDomainsPaginateTypeDef",
@@ -450,16 +463,18 @@
     "RebootInstanceResultTypeDef",
     "RebootRelationalDatabaseResultTypeDef",
     "ReleaseStaticIpResultTypeDef",
     "ResetDistributionCacheResultTypeDef",
     "SendContactMethodVerificationResultTypeDef",
     "SetIpAddressTypeResultTypeDef",
     "SetResourceAccessForBucketResultTypeDef",
+    "StartGUISessionResultTypeDef",
     "StartInstanceResultTypeDef",
     "StartRelationalDatabaseResultTypeDef",
+    "StopGUISessionResultTypeDef",
     "StopInstanceResultTypeDef",
     "StopRelationalDatabaseResultTypeDef",
     "TagResourceResultTypeDef",
     "TestAlarmResultTypeDef",
     "UnpeerVpcResultTypeDef",
     "UntagResourceResultTypeDef",
     "UpdateBucketBundleResultTypeDef",
@@ -494,14 +509,15 @@
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
     "RenewalSummaryTypeDef",
+    "CostEstimateTypeDef",
     "GetInstanceAccessDetailsResultTypeDef",
     "LoadBalancerTlsCertificateTypeDef",
     "GetLoadBalancerResultTypeDef",
     "GetLoadBalancersResultTypeDef",
     "DomainTypeDef",
     "GetRelationalDatabaseResultTypeDef",
     "GetRelationalDatabasesResultTypeDef",
@@ -511,25 +527,27 @@
     "CreateDistributionResultTypeDef",
     "GetDistributionsResultTypeDef",
     "ContainerServiceTypeDef",
     "GetContainerServiceDeploymentsResultTypeDef",
     "CreateContainerServiceRequestRequestTypeDef",
     "ExportSnapshotRecordTypeDef",
     "CertificateTypeDef",
+    "ResourceBudgetEstimateTypeDef",
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     "GetDomainResultTypeDef",
     "GetDomainsResultTypeDef",
     "GetInstanceResultTypeDef",
     "GetInstancesResultTypeDef",
     "ContainerServicesListResultTypeDef",
     "CreateContainerServiceDeploymentResultTypeDef",
     "CreateContainerServiceResultTypeDef",
     "UpdateContainerServiceResultTypeDef",
     "GetExportSnapshotRecordsResultTypeDef",
     "CertificateSummaryTypeDef",
+    "GetCostEstimateResultTypeDef",
     "CreateCertificateResultTypeDef",
     "GetCertificatesResultTypeDef",
 )
 
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
@@ -564,21 +582,32 @@
     "AutoSnapshotAddOnRequestTypeDef",
     {
         "snapshotTimeOfDay": str,
     },
     total=False,
 )
 
+StopInstanceOnIdleRequestTypeDef = TypedDict(
+    "StopInstanceOnIdleRequestTypeDef",
+    {
+        "threshold": str,
+        "duration": str,
+    },
+    total=False,
+)
+
 AddOnTypeDef = TypedDict(
     "AddOnTypeDef",
     {
         "name": str,
         "status": str,
         "snapshotTimeOfDay": str,
         "nextSnapshotTimeOfDay": str,
+        "threshold": str,
+        "duration": str,
     },
     total=False,
 )
 
 MonitoredResourceInfoTypeDef = TypedDict(
     "MonitoredResourceInfoTypeDef",
     {
@@ -620,22 +649,34 @@
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
 
-AttachDiskRequestRequestTypeDef = TypedDict(
-    "AttachDiskRequestRequestTypeDef",
+_RequiredAttachDiskRequestRequestTypeDef = TypedDict(
+    "_RequiredAttachDiskRequestRequestTypeDef",
     {
         "diskName": str,
         "instanceName": str,
         "diskPath": str,
     },
 )
+_OptionalAttachDiskRequestRequestTypeDef = TypedDict(
+    "_OptionalAttachDiskRequestRequestTypeDef",
+    {
+        "autoMounting": bool,
+    },
+    total=False,
+)
+
+class AttachDiskRequestRequestTypeDef(
+    _RequiredAttachDiskRequestRequestTypeDef, _OptionalAttachDiskRequestRequestTypeDef
+):
+    pass
 
 AttachInstancesToLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     {
         "loadBalancerName": str,
         "instanceNames": Sequence[str],
     },
@@ -686,14 +727,15 @@
         "isActive": bool,
         "minPower": int,
         "version": str,
         "versionCode": str,
         "productUrl": str,
         "licenseUrl": str,
         "platform": InstancePlatformType,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
@@ -764,14 +806,15 @@
         "instanceType": str,
         "isActive": bool,
         "name": str,
         "power": int,
         "ramSizeInGb": float,
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
+        "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
@@ -1018,14 +1061,31 @@
         "isAlias": bool,
         "type": str,
         "options": Mapping[str, str],
     },
     total=False,
 )
 
+CreateGUISessionAccessDetailsRequestRequestTypeDef = TypedDict(
+    "CreateGUISessionAccessDetailsRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
+SessionTypeDef = TypedDict(
+    "SessionTypeDef",
+    {
+        "name": str,
+        "url": str,
+        "isPrimary": bool,
+    },
+    total=False,
+)
+
 DiskMapTypeDef = TypedDict(
     "DiskMapTypeDef",
     {
         "originalDiskPath": str,
         "newDiskName": str,
     },
     total=False,
@@ -1279,15 +1339,15 @@
         "staticIpName": str,
     },
 )
 
 DisableAddOnRequestRequestTypeDef = TypedDict(
     "DisableAddOnRequestRequestTypeDef",
     {
-        "addOnType": Literal["AutoSnapshot"],
+        "addOnType": AddOnTypeType,
         "resourceName": str,
     },
 )
 
 DiskInfoTypeDef = TypedDict(
     "DiskInfoTypeDef",
     {
@@ -1334,14 +1394,23 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "start": datetime,
+        "end": datetime,
+    },
+    total=False,
+)
+
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
@@ -1381,14 +1450,15 @@
 )
 
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 GetBucketAccessKeysRequestRequestTypeDef = TypedDict(
     "GetBucketAccessKeysRequestRequestTypeDef",
     {
@@ -1442,14 +1512,15 @@
 )
 
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
+        "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
 GetCertificatesRequestRequestTypeDef = TypedDict(
     "GetCertificatesRequestRequestTypeDef",
     {
@@ -1529,14 +1600,23 @@
     "GetContainerServicesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
 
+GetCostEstimateRequestRequestTypeDef = TypedDict(
+    "GetCostEstimateRequestRequestTypeDef",
+    {
+        "resourceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+
 GetDiskRequestRequestTypeDef = TypedDict(
     "GetDiskRequestRequestTypeDef",
     {
         "diskName": str,
     },
 )
 
@@ -2322,28 +2402,42 @@
     {
         "resourceName": str,
         "bucketName": str,
         "access": ResourceBucketAccessType,
     },
 )
 
+StartGUISessionRequestRequestTypeDef = TypedDict(
+    "StartGUISessionRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 
 StartRelationalDatabaseRequestRequestTypeDef = TypedDict(
     "StartRelationalDatabaseRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
+StopGUISessionRequestRequestTypeDef = TypedDict(
+    "StopGUISessionRequestRequestTypeDef",
+    {
+        "resourceName": str,
+    },
+)
+
 _RequiredStopInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredStopInstanceRequestRequestTypeDef",
     {
         "instanceName": str,
     },
 )
 _OptionalStopInstanceRequestRequestTypeDef = TypedDict(
@@ -2495,21 +2589,22 @@
     },
     total=False,
 )
 
 _RequiredAddOnRequestTypeDef = TypedDict(
     "_RequiredAddOnRequestTypeDef",
     {
-        "addOnType": Literal["AutoSnapshot"],
+        "addOnType": AddOnTypeType,
     },
 )
 _OptionalAddOnRequestTypeDef = TypedDict(
     "_OptionalAddOnRequestTypeDef",
     {
         "autoSnapshotAddOnRequest": AutoSnapshotAddOnRequestTypeDef,
+        "stopInstanceOnIdleRequest": StopInstanceOnIdleRequestTypeDef,
     },
     total=False,
 )
 
 class AddOnRequestTypeDef(_RequiredAddOnRequestTypeDef, _OptionalAddOnRequestTypeDef):
     pass
 
@@ -3026,14 +3121,15 @@
         "iops": int,
         "path": str,
         "state": DiskStateType,
         "attachedTo": str,
         "isAttached": bool,
         "attachmentState": str,
         "gbInUse": int,
+        "autoMountStatus": AutoMountStatusType,
     },
     total=False,
 )
 
 KeyPairTypeDef = TypedDict(
     "KeyPairTypeDef",
     {
@@ -3266,14 +3362,26 @@
     "UpdateDomainEntryRequestRequestTypeDef",
     {
         "domainName": str,
         "domainEntry": DomainEntryTypeDef,
     },
 )
 
+CreateGUISessionAccessDetailsResultTypeDef = TypedDict(
+    "CreateGUISessionAccessDetailsResultTypeDef",
+    {
+        "resourceName": str,
+        "status": StatusType,
+        "percentageComplete": int,
+        "failureReason": str,
+        "sessions": List[SessionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
         "fromBlueprintId": str,
         "fromDiskInfo": List[DiskInfoTypeDef],
     },
@@ -3295,35 +3403,49 @@
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
     },
     total=False,
 )
 
+EstimateByTimeTypeDef = TypedDict(
+    "EstimateByTimeTypeDef",
+    {
+        "usageCost": float,
+        "pricingUnit": PricingUnitType,
+        "unit": float,
+        "currency": Literal["USD"],
+        "timePeriod": TimePeriodTypeDef,
+    },
+    total=False,
+)
+
 GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     {
         "includeInactive": bool,
+        "appCategory": Literal["LfR"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     {
         "includeInactive": bool,
+        "appCategory": Literal["LfR"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
@@ -4399,14 +4521,22 @@
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartGUISessionResultTypeDef = TypedDict(
+    "StartGUISessionResultTypeDef",
+    {
+        "operations": List[OperationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4415,14 +4545,22 @@
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StopGUISessionResultTypeDef = TypedDict(
+    "StopGUISessionResultTypeDef",
+    {
+        "operations": List[OperationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4880,14 +5018,23 @@
         "renewalStatus": RenewalStatusType,
         "renewalStatusReason": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
+CostEstimateTypeDef = TypedDict(
+    "CostEstimateTypeDef",
+    {
+        "usageType": str,
+        "resultsByTime": List[EstimateByTimeTypeDef],
+    },
+    total=False,
+)
+
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5136,14 +5283,26 @@
         "revocationReason": str,
         "tags": List[TagTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
+ResourceBudgetEstimateTypeDef = TypedDict(
+    "ResourceBudgetEstimateTypeDef",
+    {
+        "resourceName": str,
+        "resourceType": ResourceTypeType,
+        "costEstimates": List[CostEstimateTypeDef],
+        "startTime": datetime,
+        "endTime": datetime,
+    },
+    total=False,
+)
+
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5231,14 +5390,22 @@
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+GetCostEstimateResultTypeDef = TypedDict(
+    "GetCostEstimateResultTypeDef",
+    {
+        "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.26.68
-Summary: Type annotations for boto3.Lightsail 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.81
+Summary: Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lightsail?color=blue)](https://pypistats.org/packages/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.26.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,14 +359,16 @@
 ```python
 from mypy_boto3_lightsail.literals import (
     AccessDirectionType,
     AccessTypeType,
     AccountLevelBpaSyncStatusType,
     AddOnTypeType,
     AlarmStateType,
+    AppCategoryType,
+    AutoMountStatusType,
     AutoSnapshotStatusType,
     BPAStatusMessageType,
     BehaviorEnumType,
     BlueprintTypeType,
     BucketMetricNameType,
     CertificateDomainValidationStatusType,
     CertificateStatusType,
@@ -377,14 +379,15 @@
     ContactProtocolType,
     ContainerServiceDeploymentStateType,
     ContainerServiceMetricNameType,
     ContainerServicePowerNameType,
     ContainerServiceProtocolType,
     ContainerServiceStateDetailCodeType,
     ContainerServiceStateType,
+    CurrencyType,
     DiskSnapshotStateType,
     DiskStateType,
     DistributionMetricNameType,
     DnsRecordCreationStateCodeType,
     ExportSnapshotRecordSourceTypeType,
     ForwardValuesType,
     GetActiveNamesPaginatorName,
@@ -436,23 +439,25 @@
     NetworkProtocolType,
     OperationStatusType,
     OperationTypeType,
     OriginProtocolPolicyEnumType,
     PortAccessTypeType,
     PortInfoSourceTypeType,
     PortStateType,
+    PricingUnitType,
     R53HostedZoneDeletionStateCodeType,
     RecordStateType,
     RegionNameType,
     RelationalDatabaseEngineType,
     RelationalDatabaseMetricNameType,
     RelationalDatabasePasswordVersionType,
     RenewalStatusType,
     ResourceBucketAccessType,
     ResourceTypeType,
+    StatusType,
     StatusTypeType,
     TreatMissingDataType,
     LightsailServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
@@ -472,14 +477,15 @@
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
+    StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
@@ -514,14 +520,16 @@
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
+    CreateGUISessionAccessDetailsRequestRequestTypeDef,
+    SessionTypeDef,
     DiskMapTypeDef,
     DeleteAlarmRequestRequestTypeDef,
     DeleteAutoSnapshotRequestRequestTypeDef,
     DeleteBucketAccessKeyRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteContactMethodRequestRequestTypeDef,
@@ -545,14 +553,15 @@
     DetachStaticIpRequestRequestTypeDef,
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     ResourceRecordTypeDef,
+    TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
@@ -565,14 +574,15 @@
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
+    GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
@@ -642,16 +652,18 @@
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
+    StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
+    StopGUISessionRequestRequestTypeDef,
     StopInstanceRequestRequestTypeDef,
     StopRelationalDatabaseRequestRequestTypeDef,
     TestAlarmRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBucketBundleRequestRequestTypeDef,
     UpdateDistributionBundleRequestRequestTypeDef,
     UpdateInstanceMetadataOptionsRequestRequestTypeDef,
@@ -707,17 +719,19 @@
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
+    CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
+    EstimateByTimeTypeDef,
     GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
     GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBundlesRequestGetBundlesPaginateTypeDef,
     GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDisksRequestGetDisksPaginateTypeDef,
     GetDomainsRequestGetDomainsPaginateTypeDef,
@@ -825,16 +839,18 @@
     RebootInstanceResultTypeDef,
     RebootRelationalDatabaseResultTypeDef,
     ReleaseStaticIpResultTypeDef,
     ResetDistributionCacheResultTypeDef,
     SendContactMethodVerificationResultTypeDef,
     SetIpAddressTypeResultTypeDef,
     SetResourceAccessForBucketResultTypeDef,
+    StartGUISessionResultTypeDef,
     StartInstanceResultTypeDef,
     StartRelationalDatabaseResultTypeDef,
+    StopGUISessionResultTypeDef,
     StopInstanceResultTypeDef,
     StopRelationalDatabaseResultTypeDef,
     TagResourceResultTypeDef,
     TestAlarmResultTypeDef,
     UnpeerVpcResultTypeDef,
     UntagResourceResultTypeDef,
     UpdateBucketBundleResultTypeDef,
@@ -869,14 +885,15 @@
     GetCloudFormationStackRecordsResultTypeDef,
     UpdateContainerServiceRequestRequestTypeDef,
     ContainerServiceDeploymentTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     CreateContainerServiceDeploymentRequestRequestTypeDef,
     ExportSnapshotRecordSourceInfoTypeDef,
     RenewalSummaryTypeDef,
+    CostEstimateTypeDef,
     GetInstanceAccessDetailsResultTypeDef,
     LoadBalancerTlsCertificateTypeDef,
     GetLoadBalancerResultTypeDef,
     GetLoadBalancersResultTypeDef,
     DomainTypeDef,
     GetRelationalDatabaseResultTypeDef,
     GetRelationalDatabasesResultTypeDef,
@@ -886,25 +903,27 @@
     CreateDistributionResultTypeDef,
     GetDistributionsResultTypeDef,
     ContainerServiceTypeDef,
     GetContainerServiceDeploymentsResultTypeDef,
     CreateContainerServiceRequestRequestTypeDef,
     ExportSnapshotRecordTypeDef,
     CertificateTypeDef,
+    ResourceBudgetEstimateTypeDef,
     GetLoadBalancerTlsCertificatesResultTypeDef,
     GetDomainResultTypeDef,
     GetDomainsResultTypeDef,
     GetInstanceResultTypeDef,
     GetInstancesResultTypeDef,
     ContainerServicesListResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
     CreateContainerServiceResultTypeDef,
     UpdateContainerServiceResultTypeDef,
     GetExportSnapshotRecordsResultTypeDef,
     CertificateSummaryTypeDef,
+    GetCostEstimateResultTypeDef,
     CreateCertificateResultTypeDef,
     GetCertificatesResultTypeDef,
 )
 
 
 def get_structure() -> AccessKeyLastUsedTypeDef:
     return {...}
```

### Comparing `mypy-boto3-lightsail-1.26.68/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.26.81/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.26.68/setup.py` & `mypy-boto3-lightsail-1.26.81/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.26.68",
+    version="1.26.81",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lightsail 1.26.68 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Lightsail 1.26.81 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

