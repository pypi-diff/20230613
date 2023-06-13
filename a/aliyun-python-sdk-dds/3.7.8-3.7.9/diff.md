# Comparing `tmp/aliyun-python-sdk-dds-3.7.8.tar.gz` & `tmp/aliyun-python-sdk-dds-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dds-3.7.8.tar", last modified: Fri Mar 17 02:39:47 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dds-3.7.9.tar", last modified: Fri Mar 31 13:52:15 2023, max compression
```

## Comparing `aliyun-python-sdk-dds-3.7.8.tar` & `aliyun-python-sdk-dds-3.7.9.tar`

### file list

```diff
@@ -1,107 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6026 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/AllocateNodePrivateNetworkAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/AllocatePublicNetworkAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CheckCloudResourceAuthorizedRequest.py
--rw-r--r--   0 root         (0) root         (0)     3102 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CheckRecoveryConditionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateNodeBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     4411 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     7807 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateShardingDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DeleteDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2612 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DeleteNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditLogFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4050 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAvailableEngineVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAvailableResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupDBsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2268 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3336 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceEncryptionKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3342 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceTDEInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancesOverviewRequest.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeErrorLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2877 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2286 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeKernelReleaseNotesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeMongoDBLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParameterModificationHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParameterTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     3651 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribePriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2650 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRenewalPriceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeReplicaSetRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2268 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRoleZoneInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRunningLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeShardingNetworkAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3744 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeUserEncryptionKeyListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DestroyInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3848 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/EvaluateResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/MigrateAvailableZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     2604 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/MigrateToOtherZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2614 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAuditLogFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3118 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAuditPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3961 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     2706 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2471 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2790 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetworkTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     4324 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     2660 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyInstanceAutoRenewalAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyInstanceVpcAuthModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyNodeSpecBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyNodeSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifySecurityGroupConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ReleaseNodePrivateNetworkAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ReleasePublicNetworkAddressRequest.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RenewDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RestartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RestoreDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/SwitchDBInstanceHARequest.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TransformInstanceChargeTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TransformToPrePaidRequest.py
--rw-r--r--   0 root         (0) root         (0)     2931 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UpgradeDBInstanceEngineVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UpgradeDBInstanceKernelVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-03-17 02:39:47.000000 aliyun-python-sdk-dds-3.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6533 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/AllocateNodePrivateNetworkAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/AllocatePublicNetworkAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CheckCloudResourceAuthorizedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CheckRecoveryConditionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8181 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateGlobalSecurityIPGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateNodeBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateShardingDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DeleteDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DeleteGlobalSecurityIPGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DeleteNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditLogFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4050 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAvailableEngineVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupDBsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3336 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceEncryptionKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceTDEInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancesOverviewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeErrorLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeGlobalSecurityIPGroupRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeGlobalSecurityIPGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeKernelReleaseNotesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeMongoDBLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParameterModificationHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParameterTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribePriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRenewalPriceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeReplicaSetRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRoleZoneInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRunningLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeShardingNetworkAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3744 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeUserEncryptionKeyListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DestroyInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/EvaluateResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/MigrateAvailableZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2604 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/MigrateToOtherZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAuditLogFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAuditPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3275 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetworkTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceTDERequest.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyInstanceAutoRenewalAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyInstanceVpcAuthModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyNodeSpecBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyNodeSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifySecurityGroupConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ReleaseNodePrivateNetworkAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ReleasePublicNetworkAddressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RenewDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RestartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RestoreDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/SwitchDBInstanceHARequest.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TransformInstanceChargeTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TransformToPrePaidRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UpgradeDBInstanceEngineVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UpgradeDBInstanceKernelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-03-31 13:52:15.000000 aliyun-python-sdk-dds-3.7.9/setup.py
```

### Comparing `aliyun-python-sdk-dds-3.7.8/LICENSE` & `aliyun-python-sdk-dds-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/PKG-INFO` & `aliyun-python-sdk-dds-3.7.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dds
-Version: 3.7.8
+Version: 3.7.9
 Summary: The dds module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dds
```

### Comparing `aliyun-python-sdk-dds-3.7.8/README.rst` & `aliyun-python-sdk-dds-3.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/PKG-INFO` & `aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dds
-Version: 3.7.8
+Version: 3.7.9
 Summary: The dds module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dds
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyun_python_sdk_dds.egg-info/SOURCES.txt` & `aliyun-python-sdk-dds-3.7.9/aliyun_python_sdk_dds.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 aliyunsdkdds/request/__init__.py
 aliyunsdkdds/request/v20151201/AllocateNodePrivateNetworkAddressRequest.py
 aliyunsdkdds/request/v20151201/AllocatePublicNetworkAddressRequest.py
 aliyunsdkdds/request/v20151201/CheckCloudResourceAuthorizedRequest.py
 aliyunsdkdds/request/v20151201/CheckRecoveryConditionRequest.py
 aliyunsdkdds/request/v20151201/CreateBackupRequest.py
 aliyunsdkdds/request/v20151201/CreateDBInstanceRequest.py
+aliyunsdkdds/request/v20151201/CreateGlobalSecurityIPGroupRequest.py
 aliyunsdkdds/request/v20151201/CreateNodeBatchRequest.py
 aliyunsdkdds/request/v20151201/CreateNodeRequest.py
 aliyunsdkdds/request/v20151201/CreateShardingDBInstanceRequest.py
 aliyunsdkdds/request/v20151201/DeleteDBInstanceRequest.py
+aliyunsdkdds/request/v20151201/DeleteGlobalSecurityIPGroupRequest.py
 aliyunsdkdds/request/v20151201/DeleteNodeRequest.py
 aliyunsdkdds/request/v20151201/DescribeAccountsRequest.py
 aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskCountRequest.py
 aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskTypeRequest.py
 aliyunsdkdds/request/v20151201/DescribeAuditLogFilterRequest.py
 aliyunsdkdds/request/v20151201/DescribeAuditPolicyRequest.py
 aliyunsdkdds/request/v20151201/DescribeAuditRecordsRequest.py
@@ -37,14 +39,16 @@
 aliyunsdkdds/request/v20151201/DescribeDBInstanceMonitorRequest.py
 aliyunsdkdds/request/v20151201/DescribeDBInstancePerformanceRequest.py
 aliyunsdkdds/request/v20151201/DescribeDBInstanceSSLRequest.py
 aliyunsdkdds/request/v20151201/DescribeDBInstanceTDEInfoRequest.py
 aliyunsdkdds/request/v20151201/DescribeDBInstancesOverviewRequest.py
 aliyunsdkdds/request/v20151201/DescribeDBInstancesRequest.py
 aliyunsdkdds/request/v20151201/DescribeErrorLogRecordsRequest.py
+aliyunsdkdds/request/v20151201/DescribeGlobalSecurityIPGroupRelationRequest.py
+aliyunsdkdds/request/v20151201/DescribeGlobalSecurityIPGroupRequest.py
 aliyunsdkdds/request/v20151201/DescribeInstanceAutoRenewalAttributeRequest.py
 aliyunsdkdds/request/v20151201/DescribeKernelReleaseNotesRequest.py
 aliyunsdkdds/request/v20151201/DescribeMongoDBLogConfigRequest.py
 aliyunsdkdds/request/v20151201/DescribeParameterModificationHistoryRequest.py
 aliyunsdkdds/request/v20151201/DescribeParameterTemplatesRequest.py
 aliyunsdkdds/request/v20151201/DescribeParametersRequest.py
 aliyunsdkdds/request/v20151201/DescribePriceRequest.py
@@ -73,14 +77,17 @@
 aliyunsdkdds/request/v20151201/ModifyDBInstanceMaintainTimeRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceMonitorRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceNetExpireTimeRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceNetworkTypeRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceSSLRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceSpecRequest.py
 aliyunsdkdds/request/v20151201/ModifyDBInstanceTDERequest.py
+aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupNameRequest.py
+aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupRelationRequest.py
+aliyunsdkdds/request/v20151201/ModifyGlobalSecurityIPGroupRequest.py
 aliyunsdkdds/request/v20151201/ModifyInstanceAutoRenewalAttributeRequest.py
 aliyunsdkdds/request/v20151201/ModifyInstanceVpcAuthModeRequest.py
 aliyunsdkdds/request/v20151201/ModifyNodeSpecBatchRequest.py
 aliyunsdkdds/request/v20151201/ModifyNodeSpecRequest.py
 aliyunsdkdds/request/v20151201/ModifyParametersRequest.py
 aliyunsdkdds/request/v20151201/ModifyResourceGroupRequest.py
 aliyunsdkdds/request/v20151201/ModifySecurityGroupConfigurationRequest.py
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/AllocateNodePrivateNetworkAddressRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/AllocateNodePrivateNetworkAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/AllocatePublicNetworkAddressRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/AllocatePublicNetworkAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CheckCloudResourceAuthorizedRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CheckCloudResourceAuthorizedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CheckRecoveryConditionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CheckRecoveryConditionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateBackupRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateDBInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
 	def get_DBInstanceDescription(self): # String
 		return self.get_query_params().get('DBInstanceDescription')
 
 	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
 		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
+	def get_GlobalSecurityGroupIds(self): # String
+		return self.get_query_params().get('GlobalSecurityGroupIds')
+
+	def set_GlobalSecurityGroupIds(self, GlobalSecurityGroupIds):  # String
+		self.add_query_param('GlobalSecurityGroupIds', GlobalSecurityGroupIds)
 	def get_BusinessInfo(self): # String
 		return self.get_query_params().get('BusinessInfo')
 
 	def set_BusinessInfo(self, BusinessInfo):  # String
 		self.add_query_param('BusinessInfo', BusinessInfo)
 	def get_Period(self): # Integer
 		return self.get_query_params().get('Period')
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateNodeBatchRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateNodeBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateNodeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/CreateShardingDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/CreateShardingDBInstanceRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,19 @@
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
 	def get_DBInstanceDescription(self): # String
 		return self.get_query_params().get('DBInstanceDescription')
 
 	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
 		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
+	def get_GlobalSecurityGroupIds(self): # String
+		return self.get_query_params().get('GlobalSecurityGroupIds')
+
+	def set_GlobalSecurityGroupIds(self, GlobalSecurityGroupIds):  # String
+		self.add_query_param('GlobalSecurityGroupIds', GlobalSecurityGroupIds)
 	def get_Period(self): # Integer
 		return self.get_query_params().get('Period')
 
 	def set_Period(self, Period):  # Integer
 		self.add_query_param('Period', Period)
 	def get_ConfigServers(self): # RepeatList
 		return self.get_query_params().get('ConfigServer')
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DeleteDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DeleteDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DeleteNodeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DeleteNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAccountsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskCountRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskTypeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeActiveOperationTaskTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditLogFilterRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditLogFilterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditPolicyRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAuditRecordsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAuditRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAvailableEngineVersionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAvailableEngineVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeAvailableResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupDBsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupDBsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeBackupsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceAttributeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceEncryptionKeyRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceEncryptionKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceMonitorRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancePerformanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceSSLRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstanceTDEInfoRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstanceTDEInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancesOverviewRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancesOverviewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeDBInstancesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeErrorLogRecordsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeErrorLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeInstanceAutoRenewalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeKernelReleaseNotesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeKernelReleaseNotesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeMongoDBLogConfigRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeMongoDBLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParameterModificationHistoryRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParameterModificationHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParameterTemplatesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParameterTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeParametersRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribePriceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRegionsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRenewalPriceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRenewalPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeReplicaSetRoleRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeReplicaSetRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRoleZoneInfoRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRoleZoneInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeRunningLogRecordsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeRunningLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSecurityIpsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeShardingNetworkAddressRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeShardingNetworkAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeTagsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DescribeUserEncryptionKeyListRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DescribeUserEncryptionKeyListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/DestroyInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/DestroyInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/EvaluateResourceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/EvaluateResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ListTagResourcesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/MigrateAvailableZoneRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/MigrateAvailableZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/MigrateToOtherZoneRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/MigrateToOtherZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAuditLogFilterRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAuditLogFilterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyAuditPolicyRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyAuditPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceConnectionStringRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceConnectionStringRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_NewPort(self): # Integer
+		return self.get_query_params().get('NewPort')
+
+	def set_NewPort(self, NewPort):  # Integer
+		self.add_query_param('NewPort', NewPort)
 	def get_NewConnectionString(self): # String
 		return self.get_query_params().get('NewConnectionString')
 
 	def set_NewConnectionString(self, NewConnectionString):  # String
 		self.add_query_param('NewConnectionString', NewConnectionString)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceDescriptionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceMaintainTimeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceMonitorRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetExpireTimeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetExpireTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetworkTypeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceNetworkTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceSSLRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceSpecRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyDBInstanceTDERequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyDBInstanceTDERequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyInstanceAutoRenewalAttributeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyInstanceAutoRenewalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyInstanceVpcAuthModeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyInstanceVpcAuthModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyNodeSpecBatchRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyNodeSpecBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyNodeSpecRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyNodeSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyParametersRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifyResourceGroupRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifyResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifySecurityGroupConfigurationRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifySecurityGroupConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ReleaseNodePrivateNetworkAddressRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ReleaseNodePrivateNetworkAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ReleasePublicNetworkAddressRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ReleasePublicNetworkAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RenewDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RenewDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/SwitchDBInstanceHARequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,50 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ResetAccountPasswordRequest(RpcRequest):
+class SwitchDBInstanceHARequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'ResetAccountPassword','dds')
+		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'SwitchDBInstanceHA','dds')
 		self.set_method('POST')
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
+	def get_SwitchMode(self): # Integer
+		return self.get_query_params().get('SwitchMode')
 
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
+	def set_SwitchMode(self, SwitchMode):  # Integer
+		self.add_query_param('SwitchMode', SwitchMode)
+	def get_RoleIds(self): # String
+		return self.get_query_params().get('RoleIds')
+
+	def set_RoleIds(self, RoleIds):  # String
+		self.add_query_param('RoleIds', RoleIds)
 	def get_SecurityToken(self): # String
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_NodeId(self): # String
+		return self.get_query_params().get('NodeId')
+
+	def set_NodeId(self, NodeId):  # String
+		self.add_query_param('NodeId', NodeId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
@@ -56,12 +66,7 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_AccountPassword(self): # String
-		return self.get_query_params().get('AccountPassword')
-
-	def set_AccountPassword(self, AccountPassword):  # String
-		self.add_query_param('AccountPassword', AccountPassword)
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RestartDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RestartDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/RestoreDBInstanceRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/RestoreDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/SwitchDBInstanceHARequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TransformToPrePaidRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,50 +15,50 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class SwitchDBInstanceHARequest(RpcRequest):
+class TransformToPrePaidRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'SwitchDBInstanceHA','dds')
+		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'TransformToPrePaid','dds')
 		self.set_method('POST')
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_SwitchMode(self): # Integer
-		return self.get_query_params().get('SwitchMode')
+	def get_CouponNo(self): # String
+		return self.get_query_params().get('CouponNo')
 
-	def set_SwitchMode(self, SwitchMode):  # Integer
-		self.add_query_param('SwitchMode', SwitchMode)
-	def get_RoleIds(self): # String
-		return self.get_query_params().get('RoleIds')
-
-	def set_RoleIds(self, RoleIds):  # String
-		self.add_query_param('RoleIds', RoleIds)
+	def set_CouponNo(self, CouponNo):  # String
+		self.add_query_param('CouponNo', CouponNo)
 	def get_SecurityToken(self): # String
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
+	def get_BusinessInfo(self): # String
+		return self.get_query_params().get('BusinessInfo')
 
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_NodeId(self): # String
-		return self.get_query_params().get('NodeId')
+	def set_BusinessInfo(self, BusinessInfo):  # String
+		self.add_query_param('BusinessInfo', BusinessInfo)
+	def get_Period(self): # Long
+		return self.get_query_params().get('Period')
+
+	def set_Period(self, Period):  # Long
+		self.add_query_param('Period', Period)
+	def get_AutoPay(self): # Boolean
+		return self.get_query_params().get('AutoPay')
 
-	def set_NodeId(self, NodeId):  # String
-		self.add_query_param('NodeId', NodeId)
+	def set_AutoPay(self, AutoPay):  # Boolean
+		self.add_query_param('AutoPay', AutoPay)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
@@ -66,7 +66,17 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_AutoRenew(self): # String
+		return self.get_query_params().get('AutoRenew')
+
+	def set_AutoRenew(self, AutoRenew):  # String
+		self.add_query_param('AutoRenew', AutoRenew)
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TagResourcesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TransformInstanceChargeTypeRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/TransformInstanceChargeTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/TransformToPrePaidRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/ResetAccountPasswordRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,50 +15,40 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class TransformToPrePaidRequest(RpcRequest):
+class ResetAccountPasswordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'TransformToPrePaid','dds')
+		RpcRequest.__init__(self, 'Dds', '2015-12-01', 'ResetAccountPassword','dds')
 		self.set_method('POST')
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_CouponNo(self): # String
-		return self.get_query_params().get('CouponNo')
+	def get_AccountName(self): # String
+		return self.get_query_params().get('AccountName')
 
-	def set_CouponNo(self, CouponNo):  # String
-		self.add_query_param('CouponNo', CouponNo)
+	def set_AccountName(self, AccountName):  # String
+		self.add_query_param('AccountName', AccountName)
 	def get_SecurityToken(self): # String
 		return self.get_query_params().get('SecurityToken')
 
 	def set_SecurityToken(self, SecurityToken):  # String
 		self.add_query_param('SecurityToken', SecurityToken)
-	def get_BusinessInfo(self): # String
-		return self.get_query_params().get('BusinessInfo')
+	def get_DBInstanceId(self): # String
+		return self.get_query_params().get('DBInstanceId')
 
-	def set_BusinessInfo(self, BusinessInfo):  # String
-		self.add_query_param('BusinessInfo', BusinessInfo)
-	def get_Period(self): # Long
-		return self.get_query_params().get('Period')
-
-	def set_Period(self, Period):  # Long
-		self.add_query_param('Period', Period)
-	def get_AutoPay(self): # Boolean
-		return self.get_query_params().get('AutoPay')
-
-	def set_AutoPay(self, AutoPay):  # Boolean
-		self.add_query_param('AutoPay', AutoPay)
+	def set_DBInstanceId(self, DBInstanceId):  # String
+		self.add_query_param('DBInstanceId', DBInstanceId)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
@@ -66,17 +56,17 @@
 	def set_OwnerAccount(self, OwnerAccount):  # String
 		self.add_query_param('OwnerAccount', OwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_AccountPassword(self): # String
+		return self.get_query_params().get('AccountPassword')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
-	def get_AutoRenew(self): # String
-		return self.get_query_params().get('AutoRenew')
+	def set_AccountPassword(self, AccountPassword):  # String
+		self.add_query_param('AccountPassword', AccountPassword)
+	def get_CharacterType(self): # String
+		return self.get_query_params().get('CharacterType')
 
-	def set_AutoRenew(self, AutoRenew):  # String
-		self.add_query_param('AutoRenew', AutoRenew)
+	def set_CharacterType(self, CharacterType):  # String
+		self.add_query_param('CharacterType', CharacterType)
```

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UntagResourcesRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UpgradeDBInstanceEngineVersionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UpgradeDBInstanceEngineVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/aliyunsdkdds/request/v20151201/UpgradeDBInstanceKernelVersionRequest.py` & `aliyun-python-sdk-dds-3.7.9/aliyunsdkdds/request/v20151201/UpgradeDBInstanceKernelVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dds-3.7.8/setup.py` & `aliyun-python-sdk-dds-3.7.9/setup.py`

 * *Files identical despite different names*

