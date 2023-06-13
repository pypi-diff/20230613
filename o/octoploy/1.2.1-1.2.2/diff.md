# Comparing `tmp/octoploy-1.2.1.tar.gz` & `tmp/octoploy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoploy-1.2.1.tar", last modified: Mon Jun 12 13:17:16 2023, max compression
+gzip compressed data, was "octoploy-1.2.2.tar", last modified: Tue Jun 13 08:03:30 2023, max compression
```

## Comparing `octoploy-1.2.1.tar` & `octoploy-1.2.2.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 13:17:04.000000 octoploy-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-12 13:17:16.505139 octoploy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-12 13:17:04.000000 octoploy-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/Oc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/backup/BackupGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/BaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/DeploymentActionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/DynamicConfigMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/YmlConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/AppDeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/DeploymentBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/K8sObjectDeployer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/BaseObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/SecretObj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/octoploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/processing/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/DataPreProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/DecryptionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/K8sObjectMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/NamespaceProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/TreeWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/ValueLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/YmlTemplateProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/state/StateTracking.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.501139 octoploy-1.2.1/octoploy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Cert.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/DictUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/Yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/YmlWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/octoploy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.497139 octoploy-1.2.1/octoploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 13:17:16.000000 octoploy-1.2.1/octoploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 13:17:16.505139 octoploy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-12 13:17:04.000000 octoploy-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/AppDeploymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/DictUtilsTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/OcObjectMergeTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/StateTrackingTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/TestUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/YmlTempalteProcessorTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/config/AppConfigTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/processing/ValueLoaderTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:16.505139 octoploy-1.2.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/EncryptionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/YmlWriterTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:17:04.000000 octoploy-1.2.1/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:03:17.000000 octoploy-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-13 08:03:30.419119 octoploy-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-13 08:03:17.000000 octoploy-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/Oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/backup/BackupGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/BaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/DeploymentActionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/DynamicConfigMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/YmlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/AppDeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/DeploymentBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/K8sObjectDeployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/BaseObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/SecretObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/octoploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DataDiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DataPreProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DecryptionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/K8sObjectMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/NamespaceProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/TreeWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/ValueLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/YmlTemplateProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/state/StateTracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/octoploy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/DictUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/YmlWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 08:03:30.419119 octoploy-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-13 08:03:17.000000 octoploy-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/AppDeploymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/DictUtilsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/OcObjectMergeTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/StateTrackingTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/YmlTempalteProcessorTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/config/AppConfigTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/processing/ValueLoaderTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/EncryptionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/YmlWriterTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/__init__.py
```

### Comparing `octoploy-1.2.1/LICENSE` & `octoploy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/PKG-INFO` & `octoploy-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.1/README.md` & `octoploy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/api/Model.py` & `octoploy-1.2.2/octoploy/api/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,16 @@
         pass
 
 
 class ItemDescription:
     def __init__(self, data):
         self.data = data
 
-    def get_annotation(self, key: str) -> str:
-        item = self.data.get('metadata', {}).get('annotations', {}).get(key)
-        return item
+    def get_annotation(self, key: str) -> Optional[str]:
+        return self.data.get('metadata', {}).get('annotations', {}).get(key)
 
 
 class PodData:
     def __init__(self):
         self.name = ''
         self.ready = False
         self.version = 0
```

### Comparing `octoploy-1.2.1/octoploy/api/Oc.py` & `octoploy-1.2.2/octoploy/api/Oc.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,20 +92,20 @@
         """
         raise NotImplemented
 
     @abstractmethod
     def switch_context(self, context: str):
         """
         Changes the configuration context
-        :param context: Context
+        :param context: Context which should be used
         """
         raise NotImplemented
 
     @abstractmethod
-    def annotate(self, name: str, key: str, value: str, namespace: Optional[str] = None):
+    def annotate(self, name: str, key: str, value: Optional[str], namespace: Optional[str] = None):
         """
         Add / updates the annotation at the given item
         :param name: Name
         :param key: Annotation key
         :param value: Annotation value
         :param namespace: Namespace
         """
@@ -189,15 +189,20 @@
         proc_args = ['exec', pod_name, '--namespace', namespace, '--', cmd]
         proc_args.extend(args)
         self._exec(proc_args, print_out=True)
 
     def switch_context(self, context: str):
         raise NotImplemented('Not available for openshift')
 
-    def annotate(self, name: str, key: str, value: str, namespace: Optional[str] = None):
+    def annotate(self, name: str, key: str, value: Optional[str], namespace: Optional[str] = None):
+        if value is None:
+            # Remove the annotation
+            self._exec(['annotate', name, key + '-'], namespace=namespace)
+            return
+
         self._exec(['annotate', '--overwrite=true', name, key + '=' + value], namespace=namespace)
 
     def delete(self, name: str, namespace: str):
         try:
             self._exec(['delete', name], namespace=namespace)
         except Exception as e:
             # Yes, we all know this is bad...
@@ -235,15 +240,15 @@
         if platform.system() == 'Windows':
             return 'oc.exe'
         return 'oc'
 
 
 class K8(Oc):
     def rollout(self, name: str, namespace: Optional[str] = None):
-        self._exec(['rollout', 'restart', 'deployments', name], namespace=namespace)
+        self._exec(['rollout', 'restart', name], namespace=namespace)
 
     def tag(self, source: str, dest: str, namespace: Optional[str] = None):
         raise NotImplemented('Not available for k8')
 
     def switch_context(self, context: str):
         self._exec(['config', 'use-context', context])
```

### Comparing `octoploy-1.2.1/octoploy/backup/BackupGenerator.py` & `octoploy-1.2.2/octoploy/backup/BackupGenerator.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/config/AppConfig.py` & `octoploy-1.2.2/octoploy/config/AppConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/config/BaseConfig.py` & `octoploy-1.2.2/octoploy/config/BaseConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/config/Config.py` & `octoploy-1.2.2/octoploy/config/Config.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/config/DeploymentActionConfig.py` & `octoploy-1.2.2/octoploy/config/DeploymentActionConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/config/DynamicConfigMap.py` & `octoploy-1.2.2/octoploy/config/DynamicConfigMap.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/deploy/AppDeploy.py` & `octoploy-1.2.2/octoploy/deploy/AppDeploy.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/deploy/DeploymentBundle.py` & `octoploy-1.2.2/octoploy/deploy/DeploymentBundle.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/deploy/K8sObjectDeployer.py` & `octoploy-1.2.2/octoploy/deploy/K8sObjectDeployer.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,62 +44,65 @@
         item_path = k8s_object.get_fqn()
         namespace = k8s_object.namespace
 
         current_object = self._api.get(item_path, namespace=namespace)
         if current_object is None:
             self._log_create(item_path)
 
-        current_hash = None
+        state_hash = None
+        old_state_hash = None
         if current_object is not None:
+            old_state_hash = current_object.get_annotation(self.HASH_ANNOTATION)
             obj_state = self._state.get_state(self._app_config.get_name(), k8s_object)
             if obj_state is not None and obj_state.hash != '':
-                current_hash = obj_state.hash
+                state_hash = obj_state.hash
             else:  # Fallback to old hash location
-                current_hash = current_object.get_annotation(self.HASH_ANNOTATION)
+                state_hash = old_state_hash
 
-        if current_object is not None and current_hash is None:
+        if current_object is not None and state_hash is None:
             # Item has not been deployed with octoploy, but it does already exist
             self.log.warning(f'{item_path} has no state annotation, assuming no change required')
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             return
 
-        if current_hash == hash_val:
+        if state_hash == hash_val:
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             self.log.debug(f"{item_path} hasn't changed")
             return
 
         if current_object is not None:
             self._log_update(item_path)
 
         if self._mode.plan:
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             return
 
+        if old_state_hash is not None:
+            # Migrate to new state format by removing the old one
+            self._api.annotate(k8s_object.get_fqn(), self.HASH_ANNOTATION, None, namespace=k8s_object.namespace)
         self._api.apply(k8s_object.as_string(), namespace=namespace)
         self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
 
         if k8s_object.is_kind('ConfigMap'):
             self._reload_config()
 
     def delete_abandoned_objects(self):
         """
         Deletes all objects which are not anymore included in the
         current app config
         """
         abandoned = self._state.get_not_visited(self._app_config.get_name())
         for item in abandoned:
             namespace = item.namespace
-            if namespace is None:
-                namespace = self._root_config.get_namespace_name()
-            item_path = item.kind + '/' + item.name
-            self._log_delete(item_path)
+
+            self._log_delete(item.fqn)
             if self._mode.plan:
                 continue
 
-            self._api.delete(item_path, namespace=namespace)
+            self._api.delete(item.fqn, namespace=namespace)
             self._state.remove(item)
 
     def _reload_config(self):
         """
         Tries to reload the configuration for the app
         """
         reload_actions = self._app_config.get_reload_actions()
```

### Comparing `octoploy-1.2.1/octoploy/k8s/BaseObj.py` & `octoploy-1.2.2/octoploy/k8s/BaseObj.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/octoploy.py` & `octoploy-1.2.2/octoploy/octoploy.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/DataPreProcessor.py` & `octoploy-1.2.2/octoploy/processing/DataPreProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/DecryptionProcessor.py` & `octoploy-1.2.2/octoploy/processing/DecryptionProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/K8sObjectMerge.py` & `octoploy-1.2.2/octoploy/processing/K8sObjectMerge.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/NamespaceProcessor.py` & `octoploy-1.2.2/octoploy/processing/NamespaceProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/TreeWalker.py` & `octoploy-1.2.2/octoploy/processing/TreeWalker.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/ValueLoader.py` & `octoploy-1.2.2/octoploy/processing/ValueLoader.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/processing/YmlTemplateProcessor.py` & `octoploy-1.2.2/octoploy/processing/YmlTemplateProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/state/StateTracking.py` & `octoploy-1.2.2/octoploy/state/StateTracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,56 +7,63 @@
 from octoploy.api.Oc import K8sApi
 from octoploy.k8s.BaseObj import BaseObj
 from octoploy.utils.Log import Log
 from octoploy.utils.YmlWriter import YmlWriter
 
 
 class ObjectState:
+    fqn: str
+    """
+    Fully qualified name of the object in the format
+    kind.group/name
+    """
+
+    visited: bool
+    """
+    Transient flag to indicate if the object has been visited by octoploy
+    """
+
     def __init__(self):
-        self.context = ''
-        self.name = ''
-        self.kind = ''
+        self.context: str = ''
+        self.namespace: str = ''
+
+        self.fqn = ''
+
         self.hash = ''
-        self.namespace: Optional[str] = None
         self.visited = False
-        """
-        Transient flag to indicate if the object has been visited by octoploy
-        """
 
     def update_from_key(self, key: str):
-        segments = key.split('/')
-        count = len(segments)
-        if count > 0:
-            self.context = segments[0]
-        if count > 1:
-            self.namespace = segments[1]
-        if count > 2:
-            self.kind = segments[2]
-        if count > 3:
-            self.name = segments[3]
+        segments = key.split('/', 2)
+        if len(segments) < 3:
+            raise ValueError(f'Invalid key, must be 3 segments long {key}')
+
+        self.context = segments[0]
+        self.namespace = segments[1]
+        self.fqn = segments[2]
 
     def parse(self, data: Dict[str, str]) -> ObjectState:
-        self.context = data['context']
-        self.namespace = data['namespace']
-        self.kind = data['kind']
-        self.name = data['name']
+        self.context = data.get('context')
+        self.namespace = data.get('namespace')
+        self.fqn = data.get('fqn')
+        if self.context is None or self.namespace is None or self.fqn is None:
+            raise ValueError(f'Corrupt octoploy state, could not parse {data}')
+
         self.hash = data.get('hash', '')
         return self
 
     def to_dict(self) -> Dict[str, str]:
         return {
-            'name': self.name,
-            'hash': self.hash,
-            'kind': self.kind,
             'context': self.context,
             'namespace': self.namespace,
+            'fqn': self.fqn,
+            'hash': self.hash,
         }
 
     def get_key(self) -> str:
-        return f'{self.context}/{self.namespace}/{self.kind}/{self.name}'
+        return f'{self.context}/{self.namespace}/{self.fqn}'
 
 
 class StateTracking(Log):
     """
     Stores the objects that have been deployed with octoploy.
     This allows octoploy to detect renamed / deleted objects.
     """
@@ -154,19 +161,14 @@
         existing_state.visited = True
 
     def remove(self, object_state: ObjectState):
         del self._state[object_state.get_key()]
 
     @staticmethod
     def _k8s_to_state(context_name: str, k8s_object: BaseObj) -> ObjectState:
-        api_version = k8s_object.api_version
-        kind = k8s_object.kind
-        name = k8s_object.name
-
+        # At this point we always have a namespace set for the object
         state = ObjectState()
-        state.namespace = k8s_object.namespace
         state.context = context_name
-        state.api_version = api_version
-        state.kind = kind
-        state.name = name
+        state.namespace = k8s_object.namespace
+        state.fqn = k8s_object.get_fqn()
         state.visited = True
         return state
```

### Comparing `octoploy-1.2.1/octoploy/utils/Cert.py` & `octoploy-1.2.2/octoploy/utils/Cert.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/utils/DictUtils.py` & `octoploy-1.2.2/octoploy/utils/DictUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/utils/Encryption.py` & `octoploy-1.2.2/octoploy/utils/Encryption.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/utils/Log.py` & `octoploy-1.2.2/octoploy/utils/Log.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy/utils/YmlWriter.py` & `octoploy-1.2.2/octoploy/utils/YmlWriter.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/octoploy.egg-info/PKG-INFO` & `octoploy-1.2.2/octoploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.1/octoploy.egg-info/SOURCES.txt` & `octoploy-1.2.2/octoploy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 octoploy/deploy/AppDeploy.py
 octoploy/deploy/DeploymentBundle.py
 octoploy/deploy/K8sObjectDeployer.py
 octoploy/deploy/__init__.py
 octoploy/k8s/BaseObj.py
 octoploy/k8s/SecretObj.py
 octoploy/k8s/__init__.py
+octoploy/processing/DataDiff.py
 octoploy/processing/DataPreProcessor.py
 octoploy/processing/DecryptionProcessor.py
 octoploy/processing/K8sObjectMerge.py
 octoploy/processing/NamespaceProcessor.py
 octoploy/processing/TreeWalker.py
 octoploy/processing/ValueLoader.py
 octoploy/processing/YmlTemplateProcessor.py
```

### Comparing `octoploy-1.2.1/setup.py` & `octoploy-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/AppDeploymentTest.py` & `octoploy-1.2.2/tests/AppDeploymentTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/DictUtilsTest.py` & `octoploy-1.2.2/tests/DictUtilsTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/OcObjectMergeTest.py` & `octoploy-1.2.2/tests/OcObjectMergeTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/StateTrackingTest.py` & `octoploy-1.2.2/tests/StateTrackingTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,84 +29,103 @@
             return self._dummy_api
 
         prj_config = RootConfig.load(os.path.join(self._base_path, config_dir))
         prj_config.get_state()._k8s_api = self._dummy_api
         prj_config.create_api = get_dummy_api
         return prj_config
 
-    def test_move(self):
-        state = StateTracking(None)
-        data = state._state
-
+    def _create_state_data(self):
+        data = {}
         obj = ObjectState()
-        obj.update_from_key('a/b/c/d')
+        obj.update_from_key('a/b/c.d/12')
+        data['a'] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
-        self.assertEqual('c', obj.kind)
-        self.assertEqual('d', obj.name)
-        data['a'] = obj
+        self.assertEqual('c.d/12', obj.fqn)
 
         obj = ObjectState()
         obj.update_from_key('a/b/c')
+        data['b'] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
-        self.assertEqual('c', obj.kind)
-        obj.name = 'name'
-        data['b'] = obj
+        self.assertEqual('c', obj.fqn)
 
         obj = ObjectState()
-        obj.update_from_key('a/b')
+        obj.update_from_key('a/b/Deployment/name')
+        data['c'] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
-        obj.kind = 'Deployment'
-        obj.name = 'name'
-        data['c'] = obj
+        return data
 
-        obj = ObjectState()
-        obj.update_from_key('a')
-        self.assertEqual('a', obj.context)
-        obj.namespace = 'unittest'
-        obj.kind = 'Deployment'
-        obj.name = 'name'
-        data['d'] = obj
-        init_state = dict(data)
+    def test_move(self):
+        state = StateTracking(None)
+        data = state._state
+        data.update(self._create_state_data())
 
-        state.move('a/b/c/d', '1/2/3/4')
+        self.assertEqual('a', data['a'].context)
+        self.assertEqual('b', data['a'].namespace)
+        self.assertEqual('c.d/12', data['a'].fqn)
+
+        self.assertEqual('a', data['b'].context)
+        self.assertEqual('b', data['b'].namespace)
+        self.assertEqual('c', data['b'].fqn)
+
+        self.assertEqual('a', data['c'].context)
+        self.assertEqual('b', data['c'].namespace)
+
+        state.move('a/b/c.d/12', '1/2/3/4')
         self.assertEqual('1', data['a'].context)
         self.assertEqual('2', data['a'].namespace)
-        self.assertEqual('3', data['a'].kind)
-        self.assertEqual('4', data['a'].name)
-        state.move('1/2/3/4', 'a/b/c/d')
+        self.assertEqual('3/4', data['a'].fqn)
+        data = state._state = self._create_state_data()
 
-        state.move('a/b/c', '1/2/3')
+        state.move('a/b', '1/2')
         self.assertEqual('1', data['a'].context)
         self.assertEqual('2', data['a'].namespace)
-        self.assertEqual('3', data['a'].kind)
-        self.assertEqual('d', data['a'].name)
+        self.assertEqual('c.d/12', data['a'].fqn)
 
         self.assertEqual('1', data['b'].context)
         self.assertEqual('2', data['b'].namespace)
-        self.assertEqual('3', data['b'].kind)
-        self.assertEqual('name', data['b'].name)
-        state.move('1/2/3', 'a/b/c')
+        self.assertEqual('c', data['b'].fqn)
+        data = state._state = self._create_state_data()
 
     def test_create_new(self):
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '', error=Exception('NotFound'))
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], '{}')
 
         octoploy.octoploy._run_app_deploy('app_deploy_test', 'app', self._mode)
 
         self.assertEqual(4, len(self._dummy_api.commands))
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([{"context": "ABC",
                                 "hash": "e2e4634c5cd31a1b58da917e8b181b28",
-                                "kind": "Deployment",
-                                "name": "ABC",
+                                "fqn": "Deployment/ABC",
+                                "namespace": "oc-project",
+                                }], state_update.stdin)
+
+    def test_duplicate_kinds(self):
+        self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '', error=Exception('NotFound'))
+        self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], '{}')
+
+        octoploy.octoploy._run_app_deploy('app_deploy_test_duplicate_kinds', 'app', self._mode)
+
+        self.assertEqual(4, len(self._dummy_api.commands))
+        self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
+        state_update = self._dummy_api.commands[-1]
+        self.assertEqual(['apply', '-f', '-'], state_update.args)
+        self.assertStateEqual([{"context": "app",
+                                "hash": "aa859898df4ff9412857e720beeabfba",
+                                "fqn": "ProviderConfig.kubernetes.crossplane.io/default",
+                                "namespace": "oc-project",
+                                },
+                               {"context": "app",
+                                "hash": "8652aee0d35b000096f2a263c6e3eb77",
+                                "fqn": "ProviderConfig.grafana.crossplane.io/default",
                                 "namespace": "oc-project",
                                 }], state_update.stdin)
 
     def test_deploy_all_then_app(self):
         """
         Deploys an entire folder, then a single app and makes
         sure the other objects don't get removed again from k8s
@@ -120,46 +139,39 @@
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
 
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([
             {"context": "ABC",
              "hash": "e2e4634c5cd31a1b58da917e8b181b28",
-             "kind": "Deployment",
-             "name": "ABC",
+             "fqn": "Deployment/ABC",
              "namespace": "oc-project"},
             {"context": "entity-compare-api",
              "hash": "644921ab79abf165d8fb8304913ff1c7",
-             "kind": "Deployment",
-             "name": "8080",
+             "fqn": "Deployment/8080",
              "namespace": "oc-project"},
             {"context": "favorite-api",
              "hash": "3005876d55a8c9af38a58a4227a377fc",
-             "kind": "Deployment",
-             "name": "8081",
+             "fqn": "Deployment/8081",
              "namespace": "oc-project"},
             {"context": "cm-types",
              "hash": "1f4d778af0ea594402e656fd6139c584",
-             "kind": "ConfigMap",
-             "name": "config",
+             "fqn": "ConfigMap/config",
              "namespace": "oc-project"},
             {"context": "ABC2",
              "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
-             "kind": "Secret",
-             "name": "secret",
+             "fqn": "Secret/secret",
              "namespace": "oc-project"},
             {"context": "ABC2",
              "hash": "178859f1aa21598384610f352d314ae6",
-             "kind": "Secret",
-             "name": "plain-secret",
+             "fqn": "Secret/plain-secret",
              "namespace": "oc-project"},
             {"context": "var-append",
              "hash": "24d921e38f585e26cdc247d8fddc260e",
-             "kind": "ConfigMap",
-             "name": "config",
+             "fqn": "ConfigMap/config",
              "namespace": "oc-project"},
         ], state_update.stdin)
 
         # Now deploy a single app
         current_state = yaml.safe_load(state_update.stdin)
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], json.dumps(current_state))
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '{}')
@@ -183,46 +195,39 @@
         self.assertEqual(14, len(self._dummy_api.commands))
         self.assertEqual(['get', 'ConfigMap/octoploy-state', '-o', 'json'], self._dummy_api.commands[0].args)
 
         state_update = self._dummy_api.commands[-1]
         self.assertEqual(['apply', '-f', '-'], state_update.args)
         self.assertStateEqual([{"context": "ABC",
                                 "hash": "e2e4634c5cd31a1b58da917e8b181b28",
-                                "kind": "Deployment",
-                                "name": "ABC",
+                                "fqn": "Deployment/ABC",
                                 "namespace": "oc-project"},
                                {"context": "entity-compare-api",
                                 "hash": "644921ab79abf165d8fb8304913ff1c7",
-                                "kind": "Deployment",
-                                "name": "8080",
+                                "fqn": "Deployment/8080",
                                 "namespace": "oc-project"},
                                {"context": "favorite-api",
                                 "hash": "3005876d55a8c9af38a58a4227a377fc",
-                                "kind": "Deployment",
-                                "name": "8081",
+                                "fqn": "Deployment/8081",
                                 "namespace": "oc-project"},
                                {"context": "cm-types",
                                 "hash": "1f4d778af0ea594402e656fd6139c584",
-                                "kind": "ConfigMap",
-                                "name": "config",
+                                "fqn": "ConfigMap/config",
                                 "namespace": "oc-project"},
                                {"context": "ABC2",
                                 "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
-                                "kind": "Secret",
-                                "name": "secret",
+                                "fqn": "Secret/secret",
                                 "namespace": "oc-project"},
                                {"context": "var-append",
                                 "hash": "24d921e38f585e26cdc247d8fddc260e",
-                                "kind": "ConfigMap",
-                                "name": "config",
+                                "fqn": "ConfigMap/config",
                                 "namespace": "oc-project"},
                                {"context": "ABC2",
                                 "hash": "178859f1aa21598384610f352d314ae6",
-                                "kind": "Secret",
-                                "name": "plain-secret",
+                                "fqn": "Secret/plain-secret",
                                 "namespace": "oc-project"},
                                ], state_update.stdin)
         # Now deploy a single app
         current_state = yaml.safe_load(state_update.stdin)
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], json.dumps(current_state))
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '{}')
         self._dummy_api.respond(['get', 'Deployment/8080', '-o', 'json'], '{}')
@@ -241,17 +246,17 @@
         self.assertEqual(current_state, new_state)
 
     def test_removed_in_repo(self):
         self._dummy_api.respond(['get', 'DeploymentConfig/ABC', '-o', 'json'], '', error=Exception('NotFound'))
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], '''{
   "apiVersion": "v1",
   "data": {
-    "state": "[{\\"apiVersion\\": \\"v1\\", \\"context\\": \\"ABC\\", \\"kind\\": \\"DeploymentConfig\\", \\"name\\": \\"ABC\\", \\"namespace\\": \\"oc-project\\"}]"
+    "state": "[{\\"context\\": \\"ABC\\", \\"fqn\\": \\"DeploymentConfig/ABC\\", \\"namespace\\": \\"oc-project\\"}]"
   },
-  "kind": "ConfigMap",
+  "fqn": "ConfigMap",
   "metadata": {
     "name": "octoploy-state"
   }
 }''')
 
         octoploy.octoploy._run_app_deploy('app_deploy_test_empty', 'app', self._mode)
```

### Comparing `octoploy-1.2.1/tests/TestUtils.py` & `octoploy-1.2.2/tests/TestUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/YmlTempalteProcessorTest.py` & `octoploy-1.2.2/tests/YmlTempalteProcessorTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/processing/ValueLoaderTest.py` & `octoploy-1.2.2/tests/processing/ValueLoaderTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.1/tests/utils/EncryptionTest.py` & `octoploy-1.2.2/tests/utils/EncryptionTest.py`

 * *Files identical despite different names*

